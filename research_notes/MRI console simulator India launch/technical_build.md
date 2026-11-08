# Technical blueprint: building and running a production-grade web-based MRI console simulator (as of Nov 2026)

Research method note: these notes come from web search results only (about 35 queries). Direct page fetches were blocked in this session for `corsmed.com` and `www.ncbi.nlm.nih.gov`, and the session's web-search budget ran out before the last few planned queries (India DPDP Rules timeline, FSL/POSSUM licence, Lars Hanson's JS Bloch simulator). Where a claim depends on a search-result summary rather than a page I read in full, it is still cited to the original URL, but the report writer should treat exact numbers as "verify before publishing". Dates are given for each item so stale ones can be spotted.

---

## 1. Image-generation approaches and trade-offs (analytic vs Bloch/k-space vs pre-computed qMRI vs AI), and how published educational simulators do it

### Takeaway
For an interactive, browser-delivered radiographer console, the evidence points to the approach most open educational simulators use: a fast signal model run on per-voxel tissue property maps (T1/T2/PD), computed on the student's device, with artifacts added by manipulating k-space (FFT) after the image is made. Full Bloch/k-space simulation (KomaMRI, JEMRIS, MRiLab, coreMRI and Corsmed's engine) gives the most realism, but it needs GPU servers and per-user compute. AI contrast synthesis is a research tool for producing the tissue maps, not a real-time engine.

### Cited Findings

**Full Bloch / k-space simulators (research grade)**
- KomaMRI.jl (Castillo-Passi et al., *MRM* 2023; 90(1):329–342, DOI 10.1002/mrm.29635) is written in Julia and solves the Bloch equations with CPU and GPU parallelisation. Its inputs are scanner parameters, a phantom and a Pulseq-compatible sequence, and it writes raw data in ISMRMRD format. It was formerly called MRIsim.jl. — [ANID record](https://investigadores.anid.cl//en/public_search/work?id=727334); [arXiv 2301.02702](https://arxiv.org/pdf/2301.02702)
- KomaMRI was validated against JEMRIS (mean absolute differences below 0.1%) and showed better GPU performance than MRiLab. The developers say it "targets researchers and students, offering an easy-to-use GUI". — [arXiv 2301.02702](https://arxiv.org/pdf/2301.02702); [Aminer abstract](https://aminer.org/pub/63bcd73090e50fcafdef97e3/komamri-jl-an-open-source-framework-for-general-mri-simulations-with-gpu)
- GPU-JEMRIS (a GPU extension of JEMRIS, which needs CUDA) reports speed-ups of about 2–5× in double precision and 4–19× in single precision. — [ISMRM 2023 #2410](https://archive.ismrm.org/2023/2410.html)
- PhoenixMR is a CUDA C/C++ GPU MRI simulator that its authors report as three orders of magnitude faster than a widely used simulator. — [PhoenixMR record](https://bvbvf1.bib-bvb.de/vufind/PrimoRecord/cdi_proquest_miscellaneous_3086066165)
- An earlier GPU MRI physics simulator (2013) found that "almost three orders of magnitude speedup" was possible with a single 448-core video card. — [PMC3559401](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3559401/)
- MRiLab is described as an open-source, GPU-accelerated simulator (2017). A comparison table marks it as not cross-platform. — [PMC10952765 (KomaMRI paper)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10952765/)
- MRSeqStudio (arXiv 2512.00011, Oct 2025; later *J Med Syst* vol. 50, 2026) is a free, open-source web platform. A browser front-end handles sequence design and calls KomaMRI on the server through a REST API. It exports JSON/Pulseq. It was validated against mtrk and gammaSTAR for GRE and bSSFP sequences with high SSIM. The authors note that the GPU JEMRIS extension "does not seem to be competitive with KomaMRI". — [arXiv 2512.00011](https://arxiv.org/html/2512.00011v1); [J Med Syst 2026](https://link.springer.com/article/10.1007/s10916-026-02394-1)
- I found no WebGPU-based Bloch simulator in the search results. Published browser tools either compute server-side on CUDA, or use simpler models client-side. — [search summary of coreMRI / Virtual Scanner / PhoenixMR results](https://joss.theoj.org/papers/10.21105/joss.01637.pdf)

**Commercial cloud Bloch approach (Corsmed / coreMRI lineage)**
- Corsmed says its simulator recreates pulse sequences and proton responses by solving the Bloch equations, uses GPU parallel processing, and returns images "up to 10X faster than real scanners". These are vendor claims. — [Corsmed: How does Corsmed's MRI simulator work](https://corsmed.com/about-mri-simulators/how-does-corsmeds-mri-simulator-work)
- coreMRI (Xanthis & Aletras, *PLOS ONE* 2019) runs on Amazon Web Services GPU instances and is reachable from any web browser. In an 8-GPU configuration it was up to 63× faster than a single GPU, cutting "hour-long simulations down to a couple of minutes". — [PMC6524794](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6524794/); [ISMRM 2017 #3825](https://archive.ismrm.org/2017/3825.html)
- The coreMRI paper lists Christos Xanthis as co-founder, board member and CEO of corsMED AB. — [PMC6524794 PDF](https://rcastoragev2.blob.core.windows.net/e028a28f0db75727b15a8a8e716eb295/PMC6524794.pdf)
- **IP note:** US 12,260,951 B2, "Method for simulation of a magnetic resonance scanner", is assigned to Corsmed AB (inventors Xanthis and Aletras). It was granted on 2025-03-25 with priority from 2020-06-10. Claim 1 covers importing a pulse-sequence calculation model, setting input data and performing slice selection *in a web interface* of a web-based MRI simulator. A related patent, US 12,326,484 B2 ("Method directed to MR imaging simulation"), also turned up; I did not confirm its assignee. — [USPTO Gazette](https://patentsgazette.uspto.gov/week12/OG/html/1532-4/US12260951-20250325.html); [Google Patents US12260951](https://patents.google.com/patent/US12260951); [Google Patents US12326484](https://patents.google.com/patent/US12326484)

**Open educational simulators and their engines**
- *Virtual Scanner* (Columbia imr-framework; *JOSS* 2019, 4(43):1637) is a browser-based, vendor-neutral "end-to-end hybrid MR simulator/console" built on Pulseq/PyPulseq. Its virtual experiments use a discrete-event approach based on the Bloch equations. It runs in the browser after launching a local Flask server, and it is licensed under AGPL. The repository's last recorded push was August 2023. — [JOSS paper](https://joss.theoj.org/papers/10.21105/joss.01637.pdf); [PyPI](https://pypi.org/project/virtual-scanner); [ecosyste.ms](https://science.ecosyste.ms/projects/2381)
- *SpinSight* (ISMRM 2025 #1968) is written in Python as a web-browser dashboard, with digital phantoms drawn as 2D vector graphics. It shows acquisition parameters, pulse sequence, k-space and image together "with low latency". It is GPL-licensed. — [ISMRM 2025 #1968](https://archive.ismrm.org/2025/1968.html); [GitHub](https://github.com/bretglun/spinsight); [PyPI](https://pypi.org/project/spinsight/)
- *SimMRI / VirtMRI* (Tönnes et al., Heidelberg–Mannheim; ISMRM 2023 #2396; *J Med Syst* 2023) does all computation in the browser. The server only delivers static files, which the authors say makes it "well suited for large student groups". It supports ¹H and ²³Na sequences, noise, voxel-count changes and compressed-sensing reconstruction, and it is open source on GitHub. — [ISMRM 2023 #2396](https://archive.ismrm.org/2023/2396.html); [J Med Syst 2023 (VirtMRI)](https://link.springer.com/article/10.1007/s10916-023-02004-4)
- The Valladolid simulator (Treceño-Fernández et al., *J Med Syst* 2020, 44:9) uses a client–server architecture. The client imitates a real scanner console; the server stores the anatomical models and runs most of the simulation. — [UVa record](https://lpi.tel.uva.es/node/841); [BVS/MEDLINE](https://pesquisa.bvsalud.org/bvsms/resource/pt/mdl-31792618)
- *eduMRIsim* (TU Eindhoven; ISMRM 2025 #1958) is written in Python to mimic a clinical scanner UI. — [ISMRM 2025 #1958](https://archive.ismrm.org/2025/1958.html); [TU/e project](https://boost.tue.nl/projects/educational-magnetic-resonance-imaging-simulator-edumrisim)
- A web-based MRI simulator with a knowledge-based AI assistant (Burhanuddin et al.) uses Node.js, JavaScript and MongoDB. The assistant uses rule-based reasoning plus domain ontologies to suggest parameters, artifact reduction and protocols. (Weak source: a LinkedIn listing; journal not confirmed.) — [LinkedIn listing](https://my.linkedin.com/in/normala-ibrahim-400a9362)

**Pre-computed quantitative maps / synthetic MRI**
- Synthetic MRI acquires multi-delay multi-echo data (MDME or 3D-QALAS) and turns it into R1, R2 and PD maps, with T1 and T2 as their inverses. From those maps it can generate contrast-weighted images with arbitrary TR, TE and TI: spin echo uses TE/TR, and inversion-recovery types (FLAIR, STIR, PSIR) add TI. — [Synthetic MRI (Wikipedia)](https://EN.wikipedia.com/wiki/Synthetic_MRI); [SyntheticMR white paper](https://www.syntheticmr.com/wp/custom/uploads/2018/05/SyntheticMR-White-Paper.pdf)
- SyMRI accepts MDME data from GE, Philips and Siemens and Philips 3D-QALAS data. Users can change the default TE/TR/TI, and the vendor reports processing in about 8 seconds. — [Siemens Healthineers Academy: SyMRI](https://academy.siemens-healthineers.com/_/en-us/theory-application-symri/); [SyntheticMR PDF](https://syntheticmr.com/wp/custom/uploads/2021/08/Synthesized-Magnetic-Resonance-Imaging-and-SyMRI.pdf)
- 3T reference relaxation times for cartilage, muscle, white and grey matter come from Stanisz et al., *MRM* 2005; 54(3):507–512. They found 3T T2 values similar to 1.5T. A 2017 review notes a wide spread of reported values. — [Stanisz 2005 record](https://www.scilit.net/publications/99103192bf65b0f1130777d04b94c22a); [Bojorquez 2017 review](https://www.pubmed.gov/27594531/)
- The IT'IS Foundation keeps a tissue-property database with referenced T1/T2 values (V5.0). — [IT'IS T1–T2 references V5.0](https://itis.swiss/assets/Downloads/TissueDb/V5-0/References_T1-T2_Properties_database_V5.0.pdf)

**AI / deep-learning contrast synthesis**
- A physics-informed GAN maps a 5-minute scan to effective quantitative parameter maps, then feeds them into a signal model to synthesise four standard contrasts. It generalised to three sequences not seen in training. — [arXiv 2305.12570](https://arxiv.org/pdf/2305.12570)
- SyMTIC estimates T1 and PD maps from routine T1w, T2w and FLAIR images, then computes multi-TI images at arbitrary inversion times. — [arXiv 2506.04173](https://arxiv.org/html/2506.04173v1)
- A parameter-embedding network builds TR/TE/TI into a physics-driven network that produces T1, T2 and PD maps from T1w/T2w/FLAIR. — [arXiv 2508.08123](https://arxiv.org/pdf/2508.08123v1)
- Virtue et al. synthesise contrast-weighted images directly from MR fingerprinting data. — [Virtue et al. PDF](https://users.ece.utexas.edu/~jtamir/files/papers/virtue-machinelearning.pdf)

**Artifact injection on images (k-space manipulation)**
- TorchIO (Pérez-García et al., 2020) has transforms that simulate MRI artifacts by working in k-space: ghosting along the phase-encode direction (from pulsatile flow or cardiac/respiratory motion), spikes (herringbone/corduroy stripes), motion, and field-inhomogeneity intensity artifacts. — [TorchIO RandomGhosting docs](https://docs.torchio.org/transforms/augmentation/RandomGhosting); [RandomSpike source](https://torchio.readthedocs.io/_modules/torchio/transforms/augmentation/intensity/random_spike.html); [PyPI](https://pypi.org/project/torchio/0.17.30/)

### Inferences
(Engineering judgement, not sourced facts.)
- **Recommended core engine ("hybrid analytic + k-space"):** keep the prototype's analytic approach, but upgrade the phantom from a procedural head to voxel T1/T2/PD/T2*/chemical-shift maps (or label map plus tissue table). Then:
  1. Compute the image with closed-form steady-state equations. These are textbook formulas: SE/FSE `S = PD·(1−e^(−TR/T1))·e^(−TE/T2)`; IR/FLAIR/STIR `S = PD·|1−2e^(−TI/T1)+e^(−TR/T1)|·e^(−TE/T2)`; spoiled GRE `S = PD·sinα·(1−E1)/(1−cosα·E1)·e^(−TE/T2*)` with `E1=e^(−TR/T1)`; bSSFP uses its standard closed form. Add a fat/water flag for chemical shift and fat-sat.
  2. FFT to k-space, then apply the acquisition model there: matrix and FOV cropping, which give aliasing/wrap when FOV is smaller than the object; partial Fourier; ETL-based T2 blurring for FSE; motion and ghost phase errors; spikes (zipper/herringbone); Gibbs truncation; parallel-imaging noise amplification (g-factor map); coil sensitivity maps for surface-coil shading.
  3. Add Gaussian or Rician noise scaled by a relative-SNR formula: voxel volume × √(N_phase × NEX × N_freq / BW) × field-strength and coil factors.
  4. Inverse FFT and display.

  At 256² per slice this is milliseconds per slice in WebGL2/WebGPU, or even WASM on a mid-range Android phone. That matches the "compute in browser, static server" design SimMRI uses for large classes.
- **Where Bloch simulation earns its place:** for "physics explainer" modes (spin-echo formation, stimulated echoes, RF pulse profiles, off-resonance/bSSFP banding, flow), run a small Bloch simulation (1D/2D, thousands of isochromats) client-side in WebGPU/WASM. Optionally offer a server-side KomaMRI "high-fidelity scan" queue, as MRSeqStudio does. Don't make the core console depend on per-user GPU servers. This mainly helps cost; it also helps with the Corsmed patent, which covers cloud/web pulse-sequence simulation with slice selection in a web interface.
- **Precomputed image library (lookup tables):** realistic but combinatorially explosive. Only practical for "clinical case" mode, for example pathology cases rendered from real DICOM at fixed protocols. Better used as a complement to the analytic engine than as the core.
- **AI synthesis:** use it offline to *create* T1/T2/PD maps from ordinary licensed clinical scans (SyMTIC / parameter-embedding style). That widens the anatomy and pathology library without needing qMRI acquisitions. Don't run it live in the browser.
- **Realism ranking for a radiographer audience:** real-qMRI-map analytic + k-space artifacts ≈ commercial-looking images for SE/FSE/IR/GRE weighting. Bloch adds fidelity mainly for SSFP, flow, off-resonance and sequence-timing effects, which matter more to physicists than to radiographers learning protocols.
- **Licensing of engines:** KomaMRI is the most reusable server engine. I could not confirm its licence (see Gaps). Virtual Scanner (AGPL) and SpinSight/JEMRIS (GPL) carry copyleft obligations that conflict with a closed commercial SaaS. The AGPL in particular extends source-disclosure to network use. Use them as references, not as code dependencies, unless legal review agrees.
- **IP:** get a freedom-to-operate opinion on US 12,260,951 B2 and US 12,326,484 B2 (and any Indian or EP equivalents) before launching a web console with slice planning. Purely local analytic computation is a different technical approach, but only counsel can assess claim scope.

### Gaps
- I could not confirm the licences of KomaMRI (believed MIT) or MRiLab from the search results.
- No independent technical description of Corsmed's latency, server architecture or phantoms; corsmed.com could not be fetched.
- I found no published WebGPU Bloch simulator or browser-side benchmark.
- The exact Stanisz 2005 table values were not retrieved, and the full text is needed.
- POSSUM (FSL) and MRXCAT details/licences were not retrieved because the search budget ran out.

---

## 2. Digital phantoms and datasets for realistic anatomy, and licensing implications

### Takeaway
Few anatomically detailed phantoms are clearly licensed for commercial use. IXI (CC BY-SA 3.0) and some OpenNeuro/Dryad qMRI datasets look most usable. MIDA, XCAT, BrainWeb, fastMRI and SKM-TEA are either restricted to research/education use or have unclear terms. A commercial product will probably need its own licensed qMRI acquisitions, for example a synthetic MRI protocol on consenting volunteers at a partner Indian centre, or a negotiated licence.

### Cited Findings
- **BrainWeb (McGill BIC):** a simulated brain database with 20 normal anatomical models (via the `brainweb` Python package). Its pages describe it as constantly "under development" and ask users to cite the original work. I found no explicit licence or commercial-use terms. A third-party derivative (multimodal tumour dataset built from the 20 BrainWeb phantoms) is CC-BY, but that licence covers the derivative only. — [BrainWeb](https://brainweb.bic.mni.mcgill.ca/); [McGill BIC page](https://www.mcgill.ca/bic/software/brainweb-mri-simulator); [PyPI brainweb](https://pypi.org/project/brainweb/0.3.1/); [mm-brain-MR derivative](https://lit.fe.uni-lj.si/data/research/resources/mm-brain-MR/mm-brain-MR.pdf)
- **MIDA (IT'IS Foundation / FDA; Iacono et al., *PLoS One* 2015):** a multimodal head-and-neck model. The paper resolves 153 structures, but the released V1.0 has 115 structures plus background, and the thalamic-nuclei map is withheld because of third-party licence limits. It is "free of charge for everyone (except for handling fees)" under a licence agreement for privacy protection. I found no explicit commercial-use permission. — [IT'IS MIDA page](https://itis.swiss/virtual-population/regional-human-models/mida-model); [FDA MIDA page (archived 2022)](https://public4.pagefreezer.com:443/content/FDA/15-02-2022T20:48/https://www.fda.gov/about-fda/cdrh-offices/mida-multimodal-imaging-based-model-human-head-and-neck); [PMC4406723](https://pmc.ncbi.nlm.nih.gov/articles/PMC4406723)
- **XCAT (Duke):** 4D extended cardiac-torso phantoms for multimodality imaging research. The Duke team describes a series of 60 adult and 90 paediatric 4D whole-body models, requested via cvit.duke.edu. I found no licence fee or commercial terms. — [OSTI: 4D XCAT](https://www.osti.gov/biblio/22098534); [NIH grant TR&D Project 1](https://api.ai-analytics.org/grant/nih/10805363)
- **IXI:** about 600 MR brain images from normal, healthy subjects, released under CC BY-SA 3.0. Users must credit brain-development.org. This comes from secondary sources (TorchIO docs, FLamby, a GitHub mirror). — [TorchIO datasets](https://torchio.readthedocs.io/datasets.html); [FLamby Fed-IXI](https://owkin.github.io/FLamby/fed_ixi.html); [Preprocessed IXI (GitHub)](https://github.com/OpenXAIProject/Preprocessed_IXI_Dataset)
- **fastMRI (NYU):** data is for "internal research or educational use" under a data-use agreement, with no redistribution without permission. RSNA Atlas lists it as non-commercial research and education. — [fastMRI site](https://fastmri.med.nyu.edu/); [RSNA Radiology: AI paper](https://pubs.rsna.org/doi/full/10.1148/ryai.2020190007); [RSNA Atlas card](https://atlas.rsna.org/cards/d1b61aca-bb93-4f24-98f2-fc2722c2cdef)
- **SKM-TEA (Stanford knee, quantitative DESS):** distributed under Stanford University School of Medicine terms; usage is on the GitHub page. I did not retrieve the exact non-commercial wording. — [arXiv 2203.06823](https://arxiv.org/pdf/2203.06823)
- **OpenNeuro ds005851:** lifespan qMRI from 138 healthy participants aged 19–75, with R1, R2*, PD and MTsat maps (hMRI toolbox). This is a strong candidate source for adult brain T1/PD/T2* maps; note it has no T2. — [OHBM 2025 abstract](https://orbi.uliege.be/bitstream/2268/325811/1/OHBM2025_abstract_AgingData_submission.pdf)
- **OpenNeuro ds004611 (Romascano et al., 2024):** developmental T1/T2 relaxometry, ages 3–17. — [CIBM](https://cibm.ch/?p=19295)
- **Dryad (SAFE 3D MRF):** whole-brain 1 mm isotropic T1, T2 and PD maps from 20 healthy adults at 3T, plus coil sensitivity maps and paired B0/B1 field maps. This is the closest match to a ready-made "T1/T2/PD + coil maps" phantom set. — [Dryad dataset](https://datadryad.org/dataset/doi:10.5061/dryad.brv15dvpj)

### Inferences
- **Licence tiers (to hand to the separate legal research):**
  - Likely usable commercially, with attribution and share-alike: IXI (CC BY-SA 3.0). Share-alike may require derived phantom maps to be released under the same licence.
  - Possibly usable commercially: OpenNeuro datasets (commonly CC0, but verify per dataset) and Dryad (CC0 is Dryad's default, but verify).
  - Research/education only or unclear: fastMRI, SKM-TEA, MIDA, XCAT, BrainWeb.
- IXI and fastMRI are *weighted* images, not quantitative maps. To use them in an analytic engine you need segmentation (e.g. SynthSeg/FreeSurfer) into a label map plus literature T1/T2/PD values (Stanisz, IT'IS DB), or AI-derived maps (Section 1). A label-map phantom looks "cartoonish" unless you add within-tissue texture, for example by modulating PD/T1 with the original image intensity.
- **Body regions radiographers scan most** (knee, lumbar spine, shoulder, brain) need non-brain phantoms. The open options are mostly knee (SKM-TEA, fastMRI), and both are restricted. Commissioning a small proprietary qMRI library at an Indian partner hospital is probably the cleanest IP route. That means about 10–20 consenting volunteers, with brain, spine, knee and shoulder each scanned with MDME/QALAS or MP2RAGE + multi-echo T2, under ethics approval and a DPDP-compliant consent form. Then the phantoms are owned outright.
- Data size estimate: one 256×256×180 region with T1, T2, PD and a fat map in float16 is about 94 MB raw. A uint8 label map plus texture modulation is about 12 MB, and either compresses well with gzip/Brotli/Zstd. That is fine for CDN delivery and offline PWA caching.

### Gaps
- BrainWeb, XCAT and SKM-TEA licence texts were not retrieved, and the MIDA licence agreement text was not read.
- I did not confirm the CC0 status of ds005851, ds004611 or the Dryad dataset.
- No open spine or shoulder qMRI phantom dataset was found (search budget ended).

---

## 3. Features educators expect in a console simulator

### Takeaway
Across published simulators and vendor offerings, the expected core is:
- a console-like UI with patient/exam registration
- protocol selection
- slice planning on localisers
- tunable parameters with visible image consequences
- instructor-set scanning assignments with parameter-level review, grading and analytics

Gaps that educators and reviews call out are safety screening, patient preparation/positioning, and realistic clinical workflow. These are differentiators a new product can own.

### Cited Findings
- The Valladolid web simulator was designed from identified requirements so trainees can practise tasks such as setting slice position and selecting the correct protocol, in an interface modelled on a real scanner console. A later version added an intelligent tutoring system, described as a first for MR simulators. — [UVa record](https://lpi.tel.uva.es/node/841); [UVa thesis record](https://uvadoc.uva.es/handle/10324/80629)
- eduMRIsim lets students run a simplified clinical workflow: select an anatomical model, enter exam date and name, plan scans, then view and export results. Educators rated "clinical workflow resemblance" lowest (3.6/5), below user-friendliness (4.3) and educational value (4.5). — [ISMRM 2025 #1958](https://archive.ismrm.org/2025/1958.html); [TU/e project](https://boost.tue.nl/projects/educational-magnetic-resonance-imaging-simulator-edumrisim)
- Virtual Scanner has a "Standard Mode" that "mimics the workflow on a clinical MR console to help train MR technicians". — [ISMRM 2020 #1039](https://archive.ismrm.org/2020/1039.html)
- Corsmed (vendor claims): browser-based with no install, a UI that mirrors common GE/Siemens/Philips layouts, field strengths of 0.31, 0.4, 0.55, 1.5 and 3T, and a "Body Parts and Slice Planning" settings section. Its LMS lets students submit images for scanning assignments, and instructors see the parameters used, plus grading, course management and progress analytics. — [Corsmed MRI simulator](https://corsmed.com/mri-simulator); [Corsmed settings list](https://corsmed.com/complete-mri-simulator-settings-list); [Corsmed LMS](https://www.corsmed.com/mri-simulator/lms)
- Corsmed says ARMRIT accepts Corsmed training for up to 250 of the 1,000 required clinical hours. This is a vendor claim I did not verify with ARMRIT. — [Corsmed for education](https://www.corsmed.com/mri-simulator/for-education)
- The AI-assisted web simulator (Burhanuddin et al.) gives parameter-setting, artifact-reduction and protocol suggestions through a rule-based/ontology assistant. — [LinkedIn listing](https://my.linkedin.com/in/normala-ibrahim-400a9362)
- SpinSight's teaching value comes from showing parameters, sequence diagram, k-space and image together with low latency. — [ISMRM 2025 #1968](https://archive.ismrm.org/2025/1968.html)
- Chaka & Hardy (*Radiography* 2021) found that the one original MRI CBS study in their review used a simulator that only simulated the scanner console (set protocols, start scans). — [Bradford Scholars record](https://bradscholars.brad.ac.uk/entities/publication/5b0e2c8d-c6a8-4d4b-9abb-0d4d48f3e695)
- A low-cost tabletop MRI scanner gave a high-fidelity learning experience but "could not fully simulate" patient safety checks, preparation and positioning. (Reported in a 2025 *Education Sciences* paper on using a research MRI scanner with medical radiation science students.) — [MDPI Educ. Sci. 15(7):930](https://mdpi.com/2227-7102/15/7/930)
- **Safety:** a 2022 serious game for MR safety training had learners screen virtual patients and handle an MR-related accident. The authors concluded it raises MR safety awareness and complements face-to-face training. A 2024 scoping review found radiographer training gaps in complex screening: image review, and screening unconscious or unresponsive patients. — [The Asia Pacific Scholar 2022](https://doaj.org/article/a53c6e95989c4f7baaa1234ec94deca9); [Radiographer screening scoping review](https://katalog.lib.cas.cz/KNAV/EdsRecord/edselp,S1078817423001153)
- **LMS integration:** LTI 1.3 Advantage returns grades through Assignment and Grade Services (AGS), which replaces LTI 1.1 Basic Outcomes. It is sandboxed to the tool's own line items and built on OAuth 2.0 / OpenID Connect. Moodle supports LTI 1.3 as a platform via "External tool", including deep linking, grades and roster access. Grade passback should be tested per LMS because caching behaviour differs. — [Fora Soft: grade passback](https://www.forasoft.com/learn/elearning-video/glossary/terms-elearning/grade-passback); [LTIaaS: Moodle LTI 1.3](https://docs.ltiaas.com/learn/does-moodle-support-lti-1-3); [Libertify SCORM vs xAPI vs LTI](https://www.libertify.com/?p=48820)

### Inferences
Proposed feature tiers, engineering judgement grounded in the above.

- **MVP (must have):**
  - patient registration (name/ID/weight/height, used for SAR)
  - coil selection, which changes SNR and coverage via coil sensitivity maps
  - a protocol tree per body region
  - 3-plane localiser with drag/rotate slice-stack planning, saturation bands and FOV box
  - parameters: TR, TE, TI, flip angle, ETL, matrix, FOV, slice thickness/gap, NEX, bandwidth, phase direction, phase oversampling, fat-sat, parallel factor
  - live interdependence readouts: scan time, relative SNR, min TE/TR limits, a SAR/B1+rms indicator with IEC normal/first-level mode warnings, and voxel size
  - core artifacts: aliasing, chemical shift, motion/ghosting, susceptibility near metal and air–tissue interfaces, zipper/RF spike, Gibbs, truncation/partial-volume
  - instructor task builder ("acquire sagittal T2 FSE lumbar spine with no wrap, under 4 min"), auto-scoring against target parameters and planning tolerances, and a gradebook
- **Differentiators that address gaps educators flag:**
  - MR safety screening scenarios (branching virtual patients: implants, pacemakers, tattoos, unconscious patient, MR Conditional labels), zoning and quench/emergency drills
  - patient preparation and positioning (coil placement, centring, landmarking)
  - contrast administration workflow: eGFR check, weight-based dose, timing of post-contrast series
  - clinical cases with pathology
- **Institution features:**
  - multi-tenant college accounts, cohort management and analytics
  - LTI 1.3 (AGS + deep linking) for Moodle/Canvas, plus a SCORM 1.2/2004 wrapper for older LMSs
  - offline mode for labs with poor connectivity
- **India-specific:** align task banks with Indian BSc/MSc MRT/MIT syllabi, and support English plus optionally Malayalam/Hindi UI strings. This is judgement; curriculum research is separate.

### Gaps
- I did not obtain a peer-reviewed survey of educator feature priorities, and no Indian educator requirements study was found.
- Corsmed's specific coil, SAR, artifact and virtual-patient features could not be confirmed (page fetch blocked).
- No source detail on SCORM's runtime score API was retrieved; the comparison is from general knowledge only.

---

## 4. Web tech stack (rendering/compute, viewers, front-end, PWA/mobile, backend, multi-tenancy, anti-piracy)

### Takeaway
In late 2026 WebGPU ships in all major desktop browsers and in Chrome on Android, with Firefox Android still uncertain. WebGL2 remains the safe baseline, and Niivue (BSD-2) or Cornerstone3D (MIT) cover medical viewing. India is about 94% Android, so the engine must run acceptably on mid-range Android Chrome with a WebGL2/WASM fallback. A Supabase-style managed backend plus a zero-egress CDN keeps running costs low.

### Cited Findings
- WebGPU is supported across major browsers per web.dev, with these details:
  - Safari 26 (macOS, iOS, iPadOS, visionOS 26) shipped autumn 2025.
  - Firefox desktop has it on Windows from v141 and on Apple-silicon macOS Tahoe from v145.
  - Chrome on Android has had it since v121, on Android 12+ with Qualcomm/ARM GPUs.
  - Khronos lists Chromium on older Android via a compatibility mode (Feb 2026).
  - Firefox on Android and Linux was not confirmed as shipped.

  — [web.dev: WebGPU supported in major browsers](https://web.dev/blog/webgpu-supported-major-browsers); [Khronos WebGL & WebGPU (SIGGRAPH 2026)](https://www.khronos.org/developers/linkto/webgl-and-webgpu-sigg26)
- Android held 93.89% of India's mobile OS share in September 2026, with iOS at 6.05%. — [StatCounter India mobile OS](https://gs.statcounter.com/os-market-share/mobile/india)
- NiiVue is a WebGL 2.0 medical image viewer for NIfTI, NRRD, MGH, MHD and meshes, licensed BSD-2-Clause and installed from npm. Some Safari versions need WebGL2 enabled. — [jupyterlab-niivue (PyPI)](https://pypi.org/project/jupyterlab-niivue/); [NiiVue monorepo wiki](https://github.com/niivue/niivue-vscode/wiki); [reflex-niivue](https://pypi.org/project/reflex-niivue/0.0.1.dev3/)
- Cornerstone3D is a JavaScript library for medical image visualisation on HTML5 canvas and WebGL, with Stack and Volume viewports and 3D rendering using web standards. Mirrors and package listings show it as MIT-licensed. — [Cornerstone3D overview](https://www.cornerstonejs.org/docs/getting-started/overview); [Cornerstone core concepts](https://www.cornerstonejs.org/docs/concepts/cornerstone-core/); [yarn @cornerstonejs/core](https://classic.yarnpkg.com/en/package/@cornerstonejs/core)
- SimMRI/VirtMRI shows a fully client-side MRI simulator served as static files, which its authors say is well suited for large student groups. — [ISMRM 2023 #2396](https://archive.ismrm.org/2023/2396.html)
- Supabase Pro costs $25/month and includes 100,000 MAU (then $0.00325/MAU), 250 GB pooled egress (then about $0.09/GB), an 8 GB database and a $10 compute credit. Free tier: 50,000 MAU and 5 GB egress. — [Supabase pricing](https://supabase.com/pricing?utm=airanks.net); [Supabase billing docs](https://Supabase.io/docs/guides/platform/org-based-billing); [CloudZero summary](https://www.cloudzero.com/blog/supabase-pricing/)
- Cloudflare R2 charges about $0.015/GB-month for storage with no egress fees; Class A operations cost $4.50/million and Class B $0.36/million. The free tier is 10 GB storage, 1M Class A and 10M Class B operations per month. By comparison, AWS S3 egress is about $0.09/GB after 100 GB free. These figures come from third-party summaries; verify on Cloudflare's site. — [Cloudflare R2 calculator](https://r2-calculator.cloudflare.com/); [Filebase R2 pricing 2026](https://filebase.com/blog/cloudflare-r2-pricing-costs-savings-and-alternatives-in-2026/); [Mecanik R2 vs S3](https://mecanik.dev/en/posts/cloudflare-r2-pricing-explained-real-costs-vs-s3-and-backblaze/)

### Inferences
Recommended stack, engineering judgement.

- **Engine:** TypeScript core with a compute back end abstracted behind one interface:
  1. WebGPU compute shaders (WGSL) for signal equations, FFT and artifacts
  2. WebGL2 fragment-shader fallback, using ping-pong textures for FFT
  3. WASM (Rust or C++ via Emscripten, SIMD) CPU fallback

  Pick the back end at runtime by feature detection. Keep the physics in pure functions with unit tests against reference values; a KomaMRI-generated golden set works well for this.
- **Viewer:** NiiVue for the localiser/MPR planning views (lightweight, BSD-2, good at NIfTI phantoms and overlays), or Cornerstone3D if DICOM-style tools and OHIF-like hanging are needed. Build the console chrome (exam card, protocol tree, parameter cards, scan queue) as a custom React or Svelte UI. Next.js is the mainstream hiring pool in India, which makes React easier to staff.
- **PWA/offline:** a service worker caches the app shell and phantom packs (IndexedDB/Cache Storage). Licences are checked online, then a time-limited offline token (e.g. 7–14 days) lets labs work without connectivity.
- **Mobile:** target 256² matrices and single-slice live preview on phones, with full multi-slice volumes on desktop. A realistic console needs a big screen, so tablets/laptops are the main target and phones the "practice/revision" mode.
- **Backend:**
  - Supabase (Postgres + Auth + Row-Level Security for multi-tenant college isolation, Storage, Edge Functions). Firebase is the equivalent alternative.
  - Razorpay/Stripe for payments (India GST invoicing).
  - Event analytics: xAPI-style statements stored in Postgres, or PostHog.
  - An LTI 1.3 tool service, self-built or via a hosted LTI-as-a-service.
  - Keep student data in an India region if a college or DPDP compliance requires it.
- **Anti-piracy (realistic expectations):**
  - Browser code can always be copied, so the moat is the *content* (licensed phantoms/cases), *institution features* and *updates*.
  - Measures: per-user auth plus short-lived signed URLs for phantom packs; phantom data encrypted at rest with keys delivered after login (deters casual copying, not determined attackers); code minification/obfuscation; per-seat concurrency limits; visible user watermarking on exported images; licence enforcement at the college/SSO level.
  - Keep the "hero" assets (pathology cases, high-res phantoms) off the offline cache unless the licence allows it.

### Gaps
- No WebGPU performance benchmarks for MRI-type workloads on low-end Android were found.
- Firefox Android WebGPU status is unconfirmed.
- I did not verify the Cornerstone3D 3.x release notes or the core NiiVue LICENSE file directly.
- The India DPDP Act/Rules implementation timeline was not retrieved (search budget exhausted), and this matters for student data handling.
- No pricing was retrieved for an LTI-as-a-service or for GPU cloud instances (needed if a server-side Bloch mode is offered).

---

## 5. Effort and cost: MVP vs full product, hosting for N users, maintenance, and options for a non-programmer founder (with Indian rates)

### Takeaway
A client-side analytic simulator is a modest software project with very low hosting cost. Most of the effort goes into UI/workflow, content (phantoms, protocols, tasks) and institution features, not physics. Indicative Indian freelance rates are about $20–52/hr for full-stack developers, so a credible MVP is roughly a low-to-mid ₹ tens-of-lakhs build. Hosting is tens of US dollars per month for thousands of students if compute stays in the browser.

### Cited Findings
- 2026 rate cards put Indian freelance full-stack developers at $20–$52/hr: juniors about $14–$24, seniors about $30–$72. — [SecondTalent: cost to hire in India](https://www.secondtalent.com/cost-to-hire/india/)
- Salaried React developers in India: ₹38K–₹6.3L per month (SecondTalent, Sep 2026) and ₹40K–₹3L per month (CodingClave). New SaaS hires mostly ask for "Next.js full-stack" rather than pure React. — [SecondTalent React India rate card](https://www.secondtalent.com/developer-rate-card/react-developer-india/); [CodingClave 2026](https://codingclave.com/guides/hire-react-developer-india-2026)
- Single marketplace listings can be much lower; for example, a Mumbai React/Node developer with 5+ years at $10/hr on Hubstaff Talent. — [Hubstaff Talent profile](https://hubstafftalent.net/profiles/mayank-mishra)
- Agencies suit complex or ongoing projects with firm deadlines, and vendor/staff-augmentation rates run above freelance rates. — [Navtechy: hire full-stack India](https://navtechy.com/blog/hire-full-stack-developer-india)
- Hosting unit prices: Supabase Pro $25/month with 100K MAU, and Cloudflare R2 zero egress (see Section 4 citations). — [Supabase pricing](https://supabase.com/pricing?utm=airanks.net); [R2 calculator](https://r2-calculator.cloudflare.com/)
- Contrast: server-side GPU simulation (coreMRI) runs on AWS GPU instances, so compute cost scales with simulation load. — [PMC6524794](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6524794/)

### Inferences
All estimates below are engineering judgement, not sourced figures.

- **Effort, MVP:** the "Section 3 MVP" feature set (brain plus one MSK region, about 8–10 sequences, 6–8 artifacts, planning, tasks/auto-scoring, accounts, college admin, basic payments).
  - Breakdown: physics/rendering engine 250–400 h; console UI and planning 350–500 h; backend/auth/multi-tenant/payments 150–250 h; content (phantom preparation, protocol tables, task bank) 150–300 h, which needs a radiographer/physicist (the founder); QA/testing on devices 100–150 h.
  - **Total about 1,000–1,600 developer hours**, i.e. 6–9 months for one experienced full-stack/graphics developer, or 3–5 months for a team of 2–3 plus the founder as domain lead.
- **Effort, full product:** adds multiple body regions, pathology case library, safety and contrast scenarios, LTI 1.3 + SCORM, analytics dashboards, offline PWA, i18n, an optional server-side Bloch "physics lab" mode and accessibility. About 4,000–7,000 hours: 12–18 months for 3–5 people (2 front-end/graphics, 1 backend, 1 QA/devops part-time, plus a part-time MR physicist reviewer).
- **Cost, Indian freelance at $20–35/hr mid-level:** MVP about $20k–$56k, roughly ₹17–50 lakh at an assumed ₹85–90/USD. Full product about $80k–$245k. At the low end, salaried hires (₹0.6–1.5 L/month each) on a 12-month 3-person team come to about ₹25–55 lakh plus overheads. Agencies typically cost 1.5–2.5× freelance rates but include project management and QA.
- **Hosting for N users, client-side compute model:**
  - Phantom packs total about 2–5 GB in R2: about $0.03–0.08/month storage. A student downloading 200 MB/month costs $0 egress on R2; 10,000 students means about 2 TB/month, which would be about $180/month on S3 at $0.09/GB.
  - Supabase Pro plus a small compute add-on: about $25–$75/month up to 100K MAU.
  - Domain, email and error monitoring: about $20–50/month.
  - **Total about $50–150/month for 1,000–20,000 students.**
  - A server-side Bloch mode changes this a lot: GPU instances cost per hour and must be sized for peak concurrent classes, likely hundreds to thousands of USD/month at scale. Unpriced; see Gaps.
- **Ongoing maintenance:** about 15–25% of build effort per year (browser/GPU driver changes, LMS integration updates, content additions, support). Budget about 0.5–1 FTE once multiple colleges are live.
- **Options for a non-programmer founder:**
  1. **Keep the prototype as the specification:** a working single-page app with analytic equations is a strong spec. Write acceptance tests from it (expected relative signal, scan time).
  2. **Hire one strong senior freelancer or a small Kerala/Kochi/Thiruvananthapuram studio** (Technopark/Infopark ecosystem) for the engine and console under milestone contracts. Keep IP assignment, source-code escrow and Git repository ownership in the founder's name.
  3. **Use low-code only for the non-core parts:** marketing site, admin dashboards (Retool/Appsmith), billing. The console itself needs custom code.
  4. **AI-assisted development** (coding agents) makes a solo founder plus a part-time reviewer viable for the prototype and MVP. A paid professional should still do a code and security review before handling student data or payments.
  5. **Bring in an MR physicist consultant** for 20–40 hours to validate the equations and artifact behaviour.

### Gaps
- No Upwork or Clutch primary rate data was retrieved, and no Kerala-specific rate data was found; the figures come from rate-card/agency sites that may skew high or low.
- No published effort or cost data for building an MRI simulator was found.
- No GPU cloud pricing was retrieved.
- No evidence was found on the reliability of AI-assisted development for non-programmer founders; this is judgement only.

---

## 6. Validation: how simulator realism and educational effectiveness have been evaluated, and how to validate with Indian colleges

### Takeaway
The evidence base is thin. One randomised pre-test/post-test classroom study (Valladolid simulator, n=60) showed significant learning gains. Other studies report usability (SUS, Likelihood to Recommend) and educator/student Likert ratings, and vendor outcome claims are uncontrolled. A 2021 *Radiography* review explicitly calls for rigorous evaluation. That is an opening for a well-designed multi-college Indian study.

### Cited Findings
- **Treceño-Fernández et al., *Sensors* 2021, 21(18):6011:** randomised pre-test/post-test with a control group (traditional teaching) and an experimental group (simulator), 60 students at a main hospital in Madrid, over a single day. The simulator group did significantly better on post-test and gain, with a significant effect size. The authors position the simulator as a complement to conventional teaching. They also state that, to their knowledge, no earlier attempt had been made to evaluate MR simulators' impact in an educational process. — [Sensors/MDPI](https://www.mdpi.com/1424-8220/21/18/6011); [PMC8468339](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8468339/)
- **Treceño-Fernández et al., *J Med Syst* 2020:** acceptance in two real educational scenarios was measured with the System Usability Scale (SUS) and Likelihood to Recommend (LTR), with satisfactory results. — [UVa record](https://lpi.tel.uva.es/node/841)
- **eduMRIsim (ISMRM 2025):** 20 educators rated user-friendliness 4.3/5, educational value 4.5/5 and clinical-workflow resemblance 3.6/5. — [ISMRM 2025 #1958](https://archive.ismrm.org/2025/1958.html)
- **AI-assisted web simulator (Burhanuddin et al.):** usability testing with 30 students and instructors scored 85.1% for usability and 84.7% for learning effectiveness (weak source). — [LinkedIn listing](https://my.linkedin.com/in/normala-ibrahim-400a9362)
- **Chaka & Hardy, *Radiography* 2021; 27(2):733–739:** a literature review of 663 articles (2010–2020). It found limited use of computer-based simulation (CBS) in CT/MRI radiography education, mainly as a pre-clinical aid in pre-registration teaching. Benefits for knowledge and skills "have not been fully assessed through rigorous academic assessments and metrics", and continued development and evaluation is "essential". — [Bradford Scholars](https://bradscholars.brad.ac.uk/entities/publication/5b0e2c8d-c6a8-4d4b-9abb-0d4d48f3e695); [OUCI](https://ouci.dntb.gov.ua/works/4N6GOdO4)
- **Scoping review protocol** on simulation research across radiography specialties, including MRI (Vestbøstad, Karlgren & Olsen, *Systematic Reviews* 2020). — [Systematic Reviews](https://link.springer.com/article/10.1186/s13643-020-01531-2)
- **Western Norway University of Applied Sciences (HVL)** project studying students' experience with the Corsmed simulator and whether it aids MRI physics learning. I found aims only, no results. — [HVL project](https://www.hvl.no/prosjekt/2709384/)
- **Vendor outcome claims (uncontrolled):** Corsmed case studies report 100% graduation and employment at BCIT, and 100% employment plus 100% national certification pass rate in most years at NAIT. — [Corsmed BCIT](https://corsmed.com/case-studies/british-columbia-institute-of-technology); [Corsmed NAIT](https://corsmed.com/case-studies/northern-alberta-institute-technology); [Corsmed Teesside](https://www.corsmed.com/case-studies/teesside-university)
- **3D VR simulation in radiography (*Radiography* 2021):** students perceived 3D immersive VR simulation as a valuable learning resource. This shows the perception-survey design common in the field. — [BL record](https://eld.bl.uk/catalog/100165342776_0x000001)
- **Technical realism validation precedent:** MRSeqStudio compared simulated GRE/bSSFP against mtrk and gammaSTAR using absolute differences and SSIM. KomaMRI validated against JEMRIS (<0.1% mean absolute difference). — [arXiv 2512.00011](https://arxiv.org/html/2512.00011v1); [arXiv 2301.02702](https://arxiv.org/pdf/2301.02702)

### Inferences
Proposed validation plan for Indian colleges, engineering and education-research judgement.

1. **Technical/physics validation:**
   - Compare simulator relative signal/contrast against (a) KomaMRI reference simulations of the same phantom and (b) real scans of a phantom or volunteer at a partner centre using matched protocols.
   - Report ROI contrast ratios, SSIM, and scan-time/SAR agreement with the vendor console. Scan time should match exactly; SNR and SAR should match in relative trend.
2. **Face/content validity:**
   - A panel of experienced MR radiographers and educators (e.g. 10–20 across Kerala, Karnataka and Tamil Nadu colleges) runs blinded "real vs simulated" image discrimination plus Likert ratings of console realism and workflow resemblance. This is the dimension where eduMRIsim scored lowest.
3. **Usability:**
   - SUS plus LTR (the Treceño approach), so results can be compared directly with published simulators.
4. **Learning effectiveness:**
   - A multi-college randomised or cluster-randomised pre/post-test study (simulator vs usual teaching), following the *Sensors* 2021 design.
   - Add a practical skills OSCE-style station on a real scanner or a delayed-retention test, to go beyond one-day knowledge gains, which is the gap Chaka & Hardy identify.
   - Measure Kirkpatrick levels 1–3 where possible.
5. **Publication target:**
   - *Radiography*, *Journal of Medical Imaging and Radiation Sciences*, or the Indian Journal of Radiology & Imaging, with an ISMRT/ISMRM abstract first.
   - Get Institutional Ethics Committee approval at each college, and handle student data consent under India's DPDP regime.

### Gaps
- No Indian study of MRI simulator use in radiography education was found.
- The full text of the *Sensors* 2021 paper (exact scores and effect size values) could not be fetched.
- No published "real vs simulated image" blinded discrimination study for an MRI education simulator was found.
- The HVL/Corsmed study results are not located.
- ARMRIT acceptance of simulator hours was not independently verified.
