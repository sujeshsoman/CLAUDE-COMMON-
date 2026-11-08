# UK and Global Competitors: Virtual MRI (and CT) Console / Scanner Simulators for Radiographer Training (as of 8 Nov 2026)

> Method note for the report writer: this session's network policy blocked direct page fetches (WebFetch / curl to corsmed.com, healthysimulation.com, vmc.ac.uk, scanlabmr.com, ncbi, siemens-healthineers.com, imaios.com, mrimaster.com and others all failed with "host not allowed"). All findings below come from web-search result content (snippets/summaries of the cited pages), not from full-page reads. The shared web-search budget then ran out before every candidate could be checked. Treat numbers as "as indexed by search" and re-check on the live pages before publishing. Items that could not be checked are listed under Gaps.

## Q1. Which UK-based virtual MRI console simulator is the user most likely referring to?

### Takeaway
The most literal match is **MRI Education's "Virtual MRI Console"**, built in-house by Dr John Talbot (co-author of *MRI in Practice* with Dr Catherine Westbrook). It runs in a browser, is UK-run (GBP pricing, endorsed by the Society and College of Radiographers), and is sold only as part of an £800 CPD course. The other strong candidate is **Corsmed**, which is Swedish but sold heavily to UK customers (UCLH, The Christie, Cumbria, Teesside, City St George's, London Imaging Academy), so UK radiographers may easily think of it as "the UK simulator". The UK simulation companies Shaderware and RadSimTech make CT and X-ray simulators, not MRI. Virtual Medical Coaching is based in New Zealand, and its MRI module was listed as "release date TBC".

### Cited Findings
- MRI Education (mrieducation.com) offers a "Virtual MRI Console", described as a new tool that tackles the MRI teaching challenge. It is "a browser-based simulator that places a functional MRI console in the hands of every student", with "immediate, interactive, consequence-free exploration" — [mrieducation.com home](https://www.mrieducation.com/); [Course information](https://www.mrieducation.com/courseinformation/)
- The console was "developed in-house by Dr John Talbot", whose doctoral thesis was in technology-enhanced learning. Talbot co-presents the MRI in Practice course with Dr Catherine Westbrook — [mrieducation.com](https://www.mrieducation.com/); [Course information](https://www.mrieducation.com/courseinformation/)
- John Talbot's LinkedIn profile lists him in the United Kingdom and mentions "a new learning platform that continues to innovate the teaching, learning and assessment of MRI" — [LinkedIn – John Talbot](https://www.linkedin.com/in/johntalbot/)
- Corsmed was founded in Stockholm, Sweden (2016, by Erik Jacobsson and Christos Xanthis) — [Vestbee](https://www.vestbee.com/insights/articles/corsmed-raises-3-5-m). This is contradicted on the year and founders by [StartupRise](https://startuprise.co.uk/corsmed-has-raised-e3-3-million-in-funding/), which gives 2019 and adds Athanasios Polimeridis as co-founder.
- Corsmed names UK customers including University of Cumbria, Teesside University, UCLH and The Christie NHS Foundation Trust among "50+ leading institutions" — [Corsmed](https://www.corsmed.com/) (as summarised in search results). The NHS, London Imaging Academy and City, University of London are also named — [HealthySimulation – Corsmed vendor page](https://www.healthysimulation.com/vendors/corsmed/)
- Shaderware is a northeast England company founded in 2006. Its "Virtual Radiography" suite has four simulations: TomoVR (CT), ProjectionVR (X-ray), LectureVR and TechnicVR. No MRI product was found — [HealthySimulation – Shaderware](https://www.healthysimulation.com/vendors/shaderware/)
- RadSimTech (Raunds, Northamptonshire, UK) says its technology "began with Shaderware" and that it was founded to take Shaderware's innovations further. It sells LectureVR, ProjectionVR, TechnicVR and TomoVR (CT VR) and supports former Shaderware products. No MRI product is listed — [RadSimTech About](https://radsimtech.co.uk/about-us/); [RadSimTech FAQ](https://radsimtech.co.uk/faq/); [TomoVR page](https://radsimtech.co.uk/radiologic-training-with-tomovr/); [Contact](https://radsimtech.co.uk/contact/)
- Virtual Medical Coaching (VMC) is described as a Christchurch (New Zealand) edtech company led by founder/CEO James Hayes, with CT, MRI and mammography simulations "in development" — [Aim2Flourish](https://aim2flourish.com/innovations/vr-technology-an-adaptive-solution-to-accessible-healthcare-education). The HealthySimulation listing shows "Magnetic Resonance Imaging (MRI) (Release date TBC)" — [HealthySimulation – VMC](https://www.healthysimulation.com/vendors/virtual-medical-coaching/). Note that HealthySimulation listings carry a disclaimer that they may be inaccurate or out of date.

### Inferences
- If the user saw a product literally called a "virtual MRI console" from a UK source, it is almost certainly MRI Education / MRI in Practice (Talbot and Westbrook). The phrase matches, the pricing is in GBP, and the course is endorsed by SCoR CPD Now.
- If the user means "the MRI simulator UK hospitals and universities use", it is almost certainly Corsmed. It is not UK-based, but its best-known case studies are NHS and UK universities. The Indian entrant should position against both.
- VMC is frequently mistaken for UK-based. It is New Zealand-headquartered, although its blog targets UK College of Radiographers guidance (see Q4), which suggests a UK sales focus. That last point is an inference.

### Gaps
- I could not confirm the registered company name, Companies House entity or registered address behind mrieducation.com. UK base is inferred from GBP pricing, a "ukpay" page ([MRI in Practice – Payment](https://www.mrieducation.com/ukpay/)), SCoR endorsement and Talbot's UK LinkedIn location.
- I could not confirm whether VMC has released an MRI module by Nov 2026, because the vmc.ac.uk and virtualmedicalcoaching.com pages could not be fetched.

## Q2. Competitor profiles: what each product does, delivery, vendor-neutrality, customers, pricing, geography, years in market

### Takeaway
The field splits into four groups:
1. **Web-based, vendor-neutral "true physics" MRI simulators sold to institutions and individuals.** Corsmed is the clear leader. ScanLab (US) is a smaller, assessment-led rival. MRI Education's console is bundled with a course. ScanFlo (India) and MRISim are newer entrants.
2. **Vendor-specific console simulators.** These include Siemens SmartSimulator, GE's simulator-based courses and IACI's GE-style console.
3. **UK CT/X-ray VR simulators with no MRI.** These are Shaderware/RadSimTech and VMC.
4. **Free academic or open-source physics tools** with weak console realism: Columbia Virtual MRI Scanner, KomaMRI, MRiLab, eduMRIsim, MRISIMUL and the MRIcontrast app.

Pricing has just been disrupted: **on 2 Nov 2026 Corsmed launched a permanently free tier**.

### Cited Findings

#### Corsmed (Stockholm, Sweden; founded 2016 per most sources) — market leader
- **Product:** a web-based MRI simulator for practising scanning in a risk-free environment — [Vestbee](https://www.vestbee.com/insights/articles/corsmed-raises-3-5-m). It is cloud-based, runs in a browser, and has "a single vendor-neutral interface that mirrors the standard workflows shared by all MRI scanner manufacturers" — [Corsmed MRI simulator page](https://www.corsmed.com/mri-simulator)
- **Feature claims:**
  - 25+ pulse sequences, 30+ adjustable parameters and "accurate artifact simulation" — [Corsmed MRI simulator page](https://www.corsmed.com/mri-simulator)
  - captures 35 MRI parameters in every image — [Corsmed FAQ](https://corsmed.com/faqs/how-much-does-corsmeds-mri-simulator-cost)
  - the full paid platform has 60+ anatomies, 30+ pulse sequences, pathology simulation and LMS integration — [Corsmed for individuals](https://www.corsmed.com/en-us/mri-simulator/for-individuals); [Free MRI Simulator](https://www.corsmed.com/free-mri-simulator)
  - an educator/LMS platform is offered — [Corsmed LMS](https://www.corsmed.com/mri-simulator/lms)
- **Realism positioning:** described as a "True MRI simulator, capable of simulating every image from scratch", used in "more than 25 countries" — [AuntMinnie vendor profile](https://www.auntminnie.com/resources/vendors/mri/software/company/15554202/corsmed). Corsmed has also published a realism white paper — [White Paper: MRI Realism](https://www.corsmed.com/news/white-paper-mri-realism-simulated-vs-true-mr-images)
- **How Corsmed categorises rivals:**
  - its guide sorts MRI simulators into five types: clinical-grade simulators, research engines, formula-based simulators, geometry-only simulators, and console simulators (image banks). It claims only clinical-grade simulators (i.e. itself) meet all three of its criteria, including whether "the image changes correctly when you adjust parameters" — [Corsmed: 5 MRI simulator types compared](https://www.corsmed.com/about-mri-simulators/the-5-types-of-mri-simulators-compared)
  - an older Corsmed article uses a different 3+1 taxonomy (image bank, closed-form, "True MRI") — [Corsmed: Different types of MRI simulators](https://www.corsmed.com/news/the-different-types-of-mri-simulators-for-training-and-education)
- **Pricing:**
  - **Free tier (launched 2 Nov 2026):** available to any student or MRI professional worldwide with no time limit, no trial period, no expiry and no credit card. It covers head and knee anatomies — [ITN](https://www.itnonline.com/content/corsmed-now-offering-free-tier-mri-simulator); [AuntMinnie](https://www.auntminnie.com/clinical-news/mri/news/16424560/corsmed-corsmed-launches-free-tier-of-mri-simulator); [Corsmed free page](https://www.corsmed.com/free-mri-simulator). The sequence count is inconsistent: the ITN article says "eight", but its list names seven (TSE, SE, GRE, FLAIR, IR spin-echo, IR-TSE, SSFSE), and Corsmed's own page says seven — [ITN Nov 2 2026](https://www.itnonline.com/node/91310); [Corsmed free page](https://www.corsmed.com/mri-simulator/free)
  - **Individual paid bundle:** simulator, Boyd's 500-page MRI textbook and 7 self-paced courses for **US$129 for 12 months**. The page markup also shows "$175/month" and is garbled, so the monthly and 6-month terms are unclear — [Corsmed for individuals](https://www.corsmed.com/en-us/mri-simulator/for-individuals)
  - an (undated) Corsmed news page lists an individual licence at **€950** — [Corsmed News](https://corsmed.com/news). It is likely older pricing; the date is unverified.
  - **Institutional:** licences for enterprise, education and clinical customers by quote — [Corsmed pricing](https://corsmed.com/pricing). "All-you-can-scan" licences are sold for 3, 6 or 12 months, and per-hour access is not offered — [Corsmed FAQ – timed access](https://www.corsmed.com/faqs/can-i-buy-timed-access-on-corsmeds-simulator-and-only-pay-per-hour-of-use). HealthySimulation's "$1–$2,500" band is a generic bracket and is not reliable — [HealthySimulation – Corsmed MRI Simulator](https://www.healthysimulation.com/vendor-product/corsmed-mri-simulator/)
- **Funding:** a seed round of $3.5M (reported elsewhere as €3.3M) co-led by Luminar Ventures and Big Pi Ventures, announced Dec 2024. It is aimed at launching fast-MRI scanning tech in clinics, obtaining FDA approval and developing the software further — [FinSMEs, Dec 2024](https://www.finsmes.com/2024/12/corsmed-raises-3-5m-in-funding.html); [Corsmed news](https://www.corsmed.com/news/corsmed-raises-3-5m-from-luminar-and-big-pi-ventures-to-save-100m-lives); [StartupRise](https://startuprise.co.uk/corsmed-has-raised-e3-3-million-in-funding/)
- **Named customers:**
  - CNI College, BCIT, University of Cumbria, Teesside University, UCLH and The Christie (company site, via search summary) — [Corsmed](https://www.corsmed.com/)
  - Lund University, London Imaging Academy and City, University of London — [HealthySimulation](https://www.healthysimulation.com/vendors/corsmed/)
  - High Desert Medical College and CNI College (US) — [CNI College case study](https://www.corsmed.com/case-studies/cni-college)
- **Accreditation claim:** ARMRIT has approved training on Corsmed's simulator as part of required clinical hours. This is a company claim, not verified with ARMRIT — [Corsmed](https://www.corsmed.com/)
- **Distribution:** South Korea via Medical Standard (Sept 2023) — [Corsmed news](https://www.corsmed.com/news/corsmed-enters-the-south-korean-market-with-medical-standard). Xylemed also lists Corsmed — [Xylemed](https://xylemed.com/corsmed/). Xylemed's role and region are unverified.

#### MRI Education / MRI in Practice "Virtual MRI Console" (UK; Dr John Talbot and Dr Catherine Westbrook)
- **Delivery:** "browser-based application requiring no software installation, plug-ins, or dedicated hardware". It runs in any modern browser on desktop, laptop or tablet — [mrieducation.com](https://www.mrieducation.com/)
- **Bundling:** bundled with a CPD-endorsed online MRI physics course covering pulse sequences, k-space, image contrast, artefacts, instrumentation and clinical technique. Users get 12 months of simulator access with "over 50 learning exercises" linking theory to practice. Free 12-month access is described as "brand new for 2026" — [mrieducation.com](https://www.mrieducation.com/)
- **Price:** **£800 all-inclusive** for 16 physics lectures, 10 technique lectures and 12 months of simulator access — [Apply page](https://www.mrieducation.com/apply/); [Course dates](https://www.mrieducation.com/coursedates/). The Australasia price is **A$1,600** — [Australasia page](https://www.mrieducation.com/australasia/). Some pages say 15 lectures, so the lecture count is inconsistent across pages.
- **Endorsements:** Society and College of Radiographers (CPD Now) and ASMIRT. Certificates require watching the core lectures in full, and the Europe page refers to a 2-year certificate — [Europe page](https://www.mrieducation.com/international/europe/europe/)
- **Schedule:** sessions listed for June 2026, Oct 2026 and Mar 2027 — [Course dates](https://www.mrieducation.com/coursedates/)
- **Geography:** regional pages exist for Australia, New Zealand, Singapore, Papua New Guinea and Europe — [Australasia](https://www.mrieducation.com/australasia/); [Europe](https://www.mrieducation.com/international/europe/europe/). There is also a brochure ("Two Amazing Courses for the Price of One") — [Brochure PDF](https://www.mrieducation.com/resources/MRI_in_Practice_Brochure.pdf)
- **Audience:** radiographers, radiologists, MRI technologists, physicists, veterinary professionals and others — [mrieducation.com](https://www.mrieducation.com/)
- **Not published:** a parameter-by-parameter feature list, or any institutional/site licence — [mrieducation.com](https://www.mrieducation.com/) (absence noted in search summary)

#### ScanLab — ScanLabMR / ScanLabCT (Orlando, Florida, USA; founded 2020)
- **Company:** describes itself as offering "the world's first quantitative MRI and CT simulators designed for education, training, and skill assessment". It has 1–10 employees, is privately held, and was founded in 2020 — [ZoomInfo](https://www.zoominfo.com/c/scanlabmr/1295281888); [Bouncewatch](https://www.bouncewatch.com/explore/startup/scanlabmr)
- **Product:** an online simulator focused on assessment, examining three key MRI knowledge/skill areas including slice prescription and contrast parameters — [ScanLabMR](https://scanlabmr.com/scanlabmr/)
- **UK presence:**
  - a UWE Bristol diagnostic radiography lecturer says it "significantly enriched the learning experience for our Undergraduate students"
  - it is pitched as helping students meet HCPC (UK) standards — [ScanLab](https://scanlabmr.com/)
- **Pricing:** individual cohorts run each spring and fall. "ScanLabMR Only" is **$1,000** and "ScanLabMR + ImagingU" is **$2,500**, each with 6 months' access and one office hour per week with an instructor. The page header also shows $2,500, so the tiers are slightly unclear — [ScanLab individual cohorts](https://scanlabmr.com/individual-cohorts/). Enterprise, education and clinical licences are by quote, with cost depending on licence type and seat count — [ScanLab FAQs](https://scanlabmr.com/faqs/)
- **Channel partners:**
  - the MTMI technologist course includes 3 months of ScanLabMRI access (listing ~637 days old, i.e. ~early 2025) — [MTMI](https://www.mtmi.net/course/mri-training-course-technologists-0)
  - an ImagingU course bundled 6 months of ScanLabMR (April 2024) — [ITN](https://www.itnonline.com/content/imagingu-introduces-new-course-mri-simulation-students-and-technologists)
- **ScanLabCT:** a VR app that simulates the imaging room, patient and CT unit to teach techs how to scan — [Radiology Business](https://radiologybusiness.com/topics/medical-imaging/computed-tomography-ct/vr-scanlabct-technician-training-tool)

#### ScanFlo (Zeka Labs Private Limited, Rohini, Delhi, India) — existing Indian entrant
- **Product:** browser-based MRI, CT, PET-CT and X-ray simulators, plus a 3D anatomy atlas and a disease-case tool called RadPath — [ScanFlo](https://scanflo.io/)
- **MRI workflow:** users plan slices on a localizer, choose a sequence, set TR/TE/TI and flip angle, and get an image that changes accordingly. There is a free trial and nothing to install — [ScanFlo MRI](https://scanflo.io/mri)
- **Pricing:** in INR in India and USD elsewhere (per search summary of the site) — [ScanFlo MRI](https://scanflo.io/mri)
- **Partner:** promoted by 3D Paramedical Institute (Delhi), which also lists training at Orbit Diagnostic Centers with 1.5T/3T scanners — [3D Paramedical](https://3dparamedical.com/mri-scanflo)
- **Evidence base:** only vendor and partner pages were found, with no independent reviews — [ScanFlo resources](https://scanflo.io/resources)

#### MRISim (mrisimlab.com) — origin unknown
- **Product:** described as "a real physics simulator, a scanner-console protocol planner, a guided course and a read-the-scan quiz". No company details surfaced — [MRISim](https://mrisimlab.com/)

#### IACI — Institute for Advanced Clinical Imaging (USA)
- **Product:** software that simulates a GE MRI scanner operator's console, for online or in-classroom clinical simulation training — [IACI MRI Simulator](https://www.iacionline.com/mri-simulator.cms)
- **Book tie-in:** "MRI Simulator software, version G", which accompanies the *MRI Simulator Lab Book, 2nd ed.* — [Abbey's listing](https://abbeys.com.au/book/mri-simulator-lab-book-second-edition-9780985376536.do)
- **Price:** not found.

#### Medical-Professionals.com — Virtual MRI Simulator CE course (USA, CE credits)
- **Product:** a 4.00 CE credit course with a virtual MRI interface for manipulating image contrast, acquisition time, SNR and spatial resolution in real time — [Medical-Professionals.com](https://www.medical-professionals.com/en/courses/virtual-mri-simulator-ce/)

#### Vendor-provided simulators (vendor-specific UIs)
- **Siemens Healthineers SmartSimulator:**
  - a cloud-based virtual version of a Siemens imaging system, run on a PC with support from a Siemens application expert. It serves both Siemens customers and academic environments, is available 24/7, and offers a free test package — [Siemens Healthineers (LATAM)](https://www.siemens-healthineers.com/latam/services/customer-services/upskill-services/equipment-and-clinical-education/individual-education-and-practice/smartsimulator); [Siemens Healthineers (DE)](https://www.siemens-healthineers.com/de/services/customer-services/upskill-services/weiterbildung/smartsimulator)
  - requires latency below 150 ms, and lists MR Protocol Manager among the supported features — [Siemens (LATAM)](https://www.siemens-healthineers.com/latam/services/customer-services/upskill-services/equipment-and-clinical-education/individual-education-and-practice/smartsimulator)
  - Siemens Academy's MR syngo Dot Workshop is an onsite course using Siemens simulation consoles — [Siemens Healthineers Academy](https://theta.academy.siemens.knowledgeanywhere.com/_/en-us/mr-syngo-dot-workshop)
- **GE HealthCare:**
  - the MR Fundamentals course (technical/service training) gives each student a dedicated simulator, a "one to one student to simulator ratio" — [GE MR Fundamentals](https://www.gehealthcare.com/courses/mr-fundamentals)
  - simulators can be shipped to customer sites — [GE technical training](https://www.gehealthcare.com/en-ca/education/technical-training)
  - technologist MRI courses are delivered remotely by GE clinical education trainers — [GE MR TVA training](https://www.gehealthcare.com/en-ca/education/magnetic-resonance-tva-training); [GE MR clinical education brochure](https://gehealthcare.com/-/jssmedia/gehc/us/files/education/clinical-education/mr_brochure_doc2866537rev3.pdf?rev=-1)
  - a Virtual Onsite Trainer telepresence device (2016) is not a replacement for initial onsite training — [DOTmed 2016](https://dotmed.com/news/story/32060)
  - history: GE's "Signa Tutor" offline technologist trainer dates to 1991 — [SPIE 1991](https://biomedicaloptics.spiedigitallibrary.org/conference-proceedings-of-spie/1446/0000/Signa-Tutor-results-and-future-directions/10.1117/12.45294.full)
- **Philips:** only a 2016 "Virtual Classroom Delivery" (HTM/service) programme was found, with no current Philips MR console simulator — [DOTmed 2016](https://es.dotmed.com/news/story/34076)

#### UK CT/X-ray simulators (relevant for an MRI+CT roadmap)
- **Shaderware:**
  - flagship TomoVR, an "advanced CT educational simulator" for patient positioning and CT console operation, used at 100+ client sites with hundreds of licences worldwide. University of the West of England is a named user. Founded 2006 in northeast England — [HealthySimulation – Shaderware](https://www.healthysimulation.com/vendors/shaderware/)
  - HealthySimulation lists SIMTICS and ScanLabMR as competitors — [HealthySimulation – Shaderware](https://www.healthysimulation.com/vendors/shaderware/)
- **RadSimTech (UK):**
  - Shaderware-derived suite including TomoVR (CT VR)
  - no specialised hardware needed; 15-day evaluation; discounted upgrades for existing Shaderware licence holders — [RadSimTech FAQ](https://radsimtech.co.uk/faq/); [RadSimTech](https://radsimtech.co.uk/)
- **Virtual Medical Coaching (NZ):**
  - X-Ray Pro VR covers ~140 projections, skull to pelvis
  - a "CTSimulate" module is described (head CT, dose reduction, post-processing, reconstruction parameters), but its release status is inconsistent across sources — [HealthySimulation – VMC](https://www.healthysimulation.com/vendors/virtual-medical-coaching/); [HealthySimulation article](https://www.healthysimulation.com/virtual-medical-coaching-provides-vr-radiographic-simulation-training/)
  - user manuals for a "2025 Release" of Radiography VR and desktop exist — [VMC help](https://help.virtualmedicalcoaching.com/radiography-user-manual)

#### Mock (physical) MRI scanners — not console simulators
- Psychology Software Tools' MRI simulator is a physical mock scanner (optional mock head coil, motion tracking) focused on scan logistics rather than image production — [HealthySimulation – imaging simulators](https://www.healthysimulation.com/medical-imaging-simulators/)
- RadSim sells a life-size mock MRI scanner — [HealthySimulation – RadSim](https://www.healthysimulation.com/fr/fournisseurs/radsim/)

#### Academic / open-source / low-cost tools
- **Virtual MRI Scanner (Columbia University):**
  - Python-based, AGPL-3.0, with a zero-footprint web-browser console GUI
  - lets users register subject info, set custom sequence parameters, and do T1/T2 mapping with ROI analysis
  - used to educate MR students and radiologists — [Open Source Imaging](https://www.opensourceimaging.org/project/virtual-mri-scanner/)
- **KomaMRI.jl:** an open-source, GPU-accelerated general MRI simulator — [PMC](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10952765/); [arXiv](https://arxiv.org/pdf/2301.02702)
- **MRiLab:** an interactive GUI for experiment design and technique prototyping — [MRiLab](https://mrilab.sourceforge.net/)
- **eduMRIsim (TU Eindhoven):** a "realistic MRI user interface" allowing students to interact with different scan modalities — [TU/e BOOST](https://boost.tue.nl/projects/mri-data-acquisition-and-processing-through-personalized-cbl)
- **MRISIMUL (EU project):** an MRI physics simulation platform with a web-access version that supports motion simulation — [CORDIS](https://cordis.europa.eu/project/id/256569/reporting)
- **MRIcontrast (iOS, SMRI Consulting):** changes TR, TE, flip angle and field strength; US$14.99 / HK$118 — [App Store](https://apps.apple.com/us/app/mricontrast/id1185084588)
- **Web-based MRI simulator with knowledge-based AI assistance (Malaysia):** listed on a LinkedIn profile; details unverified — [LinkedIn – Normala Ibrahim](https://my.linkedin.com/in/normala-ibrahim-400a9362)

### Inferences
- **Pricing anchors for India positioning:**
  - free: Corsmed head/knee tier, since Nov 2026
  - US$129/yr: Corsmed individual bundle
  - £800: MRI Education course plus console
  - US$1,000–2,500 per 6-month cohort: ScanLab
  - quote-only institutional pricing at every vendor

  The free Corsmed tier sharply raises the bar for any paid entry-level individual product. An Indian entrant probably needs a free or very-low-cost tier, and to compete on the breadth of anatomies, sequences, localisation and assessment rather than access alone.
- **Vendor-neutrality is a selling point.** Every serious independent product (Corsmed, ScanFlo, MRI Education) is browser-based and vendor-neutral. UCLH explicitly required vendor-neutrality because it runs mixed fleets (see Q3). Vendor simulators (Siemens SmartSimulator, GE) are tied to their installed base and to expert-led sessions.
- **The CT simulator space is fragmented.** In the UK it is dominated by VR desktop products (Shaderware/RadSimTech TomoVR, VMC); web-native CT console simulation looks less crowded. ScanFlo and ScanLab are the visible exceptions.
- **ScanFlo is already in India** with almost the exact concept (web, localizer planning, INR pricing, multi-modality). It is the most direct competitor for the Indian entrant, even though it is outside this UK/global brief.

### Gaps
- No verified data was found for IMAIOS e-MRI simulator features or pricing, mrimaster.com, MRI Online (radiologist-focused), Medical Simulation Corp, CAE, SimX or Oxford Medical Simulation (VR). Searches either returned nothing relevant or the budget ran out before they could be checked.
- **Vertual Ltd** (UK; VERT radiotherapy simulator, plus reportedly a projection radiography product) was not checked in this session, and its relevance to MRI is unverified.
- No current Canon or Philips MR technologist console simulator was found. The Philips data is from 2016.
- Corsmed's actual institutional price per seat or per site was not found, and neither was ScanFlo's actual INR price points.
- MRISim's owner, location and pricing are unknown.

## Q3. Reviews and published evaluations of simulator-based MRI education

### Takeaway
Independent, peer-reviewed evidence on commercial MRI console simulators is thin. The evidence found is mostly:
- vendor case studies (Corsmed–UCLH: competence in 3–4 months vs 6; Cumbria: a rise in students choosing MRI)
- one peer-reviewed classroom evaluation of an academic simulator (Sensors 2021)
- broader radiography-simulation reviews (EMJ Radiology, April 2026)

No *Radiography*-journal paper evaluating Corsmed specifically was found.

### Cited Findings
- **Corsmed–UCLH case study (vendor-authored):**
  - UCLH runs 7 MRI scanners, each scanning 15–20 patients a day, and reworked postgraduate MRI radiographer training around the simulator
  - the programme has run since 2022, led by MRI Practice Educator Noyal Mathew
  - new radiographers reach competence in 3–4 months rather than 6
  - recalls "dropped significantly", with no figures given
  - vendor-neutral design was a requirement because UCLH has multi-vendor scanners
  - home study was tried first, but structured on-site sessions proved most effective — [Corsmed UCLH case study](https://www.corsmed.com/case-studies/nhs-university-college-london-hospitals); repeated in [ITN, Nov 2026](https://www.itnonline.com/node/91310)
- **University of Cumbria (vendor case study):** nearly 20 students (~25% of the cohort) chose MRI that year — [Corsmed – Cumbria](https://www.corsmed.com/case-studies/university-of-cumbria)
- **Teesside University (vendor case study):** positive student feedback on usability — [Corsmed – Teesside](https://www.corsmed.com/en-us/success-stories/teesside-university)
- **Sensors 2021 (peer-reviewed, academic simulator, not Corsmed):** a quantitative classroom evaluation of whether an MRI simulator built to defined functional/non-functional requirements helps radiographers learn MRI theory and practice better than lectures (DOI 10.3390/s21186011, Universidad de Valladolid repository) — [PMC8468339](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8468339/); [UVaDOC PDF](https://uvadoc.uva.es/bitstream/handle/10324/59220/Magnetic-Resonance-Simulation-in-Education.pdf?sequence=1). The detailed results were not retrieved.
- **EMJ Radiology, April 2026:** "Simulation in Diagnostic Radiography Training: A Replacement for Clinical Placements?" is a 2026 review of radiography simulation. Its contents were not retrieved — [EMJ article](https://www.emjreviews.com/radiology/article/simulation-in-diagnostic-radiography-training-a-replacement-for-clinical-placements/); [PDF](https://www.emjreviews.com/wp-content/uploads/2026/04/Simulation-in-Diagnostic-Radiography-Training-A-Replacement-for-Clinical-Placements-1.pdf)
- **VR vs physical simulation (X-ray, not MRI):** a comparison in 188 first-year radiography students in South America — [PMC10258633 (J Med Radiat Sci)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10258633/)
- **2025 College of Radiographers guidance:** VMC's blog states that the 2025 CoR guidance builds simulation into radiography education. This is a vendor interpretation — [VMC blog](https://blog.virtualmedicalcoaching.com/en/simulation-is-now-built-into-radiography-education)
- **SoR / NHS context:**
  - SoR and NHS England eLfH offer free "Clinical Imaging" e-learning MRI modules to NHS staff — [SoR – Clinical Imaging eLfH](https://www.sor.org/learning-advice/learning/clinical-imaging-elfh)
  - a national MRI safety e-learning programme is free to NHS staff and academic institutions, and available to others via eIntegrity — [SoR MRI training and education](https://www.sor.org/learning-advice/professional-practice/diagnostic-imaging-pathways/mri/mri-training-and-education); [eIntegrity – SoR](https://www.eintegrity.org/medical-body/sor/)
  - none of these is a console simulator
  - North West London's imaging academy was one of 9 sites in a national pilot of virtual remote-scanning support technology (remote support, not training simulation) — [NW London ICS Training Academy](https://www.nwlondonicb.nhs.uk/professionals/referral-guidelines-and-clinical-documents/nw-london-imaging-network/Academy)
- **ARRS:** offers an online course, "Understanding MR Safety Through AI Software Simulation" — [ARRS](https://arrs.org/ARRSLIVE/Education/OnlineCourses/OC_MR21.aspx)

### Inferences
- The UCLH finding that unsupervised home study underperformed structured sessions suggests simulators sell best to institutions when bundled with an educator workflow: exercises, cohorts and supervision. For an Indian entrant, partnering with colleges and paramedical institutes (as ScanFlo does) may matter more than a direct-to-student model.
- There is room for an entrant to commission or publish its own outcome study, for example with an Indian BSc MRT programme. Peer-reviewed evidence for commercial products is scarce, and incumbents rely on case studies.

### Gaps
- Specific *Radiography* (Elsevier), JMIRS or JMRS papers on MRI console simulators could not be searched once the search budget ran out.
- App-store or review-site ratings for Corsmed, ScanLab and ScanFlo were not found.

## Q4. Gaps and complaints in existing products, and evidence of India / Middle East activity

### Takeaway
No first-hand user complaints (reviews or forums) were found. Documented constraints point to clear openings:
- price and paywalls: course-bundled at £800; cohorts at US$1,000–2,500; quote-only institutional licences
- vendor lock-in: Siemens and GE simulators require being a customer or joining expert-led sessions
- connectivity: Siemens needs under 150 ms latency
- no INR/Asian pricing from UK or global players

The free Corsmed tier (Nov 2026) partly closes the price gap. Apart from Corsmed's South Korea distributor and a Siemens SmartSimulator page on its UAE site, no evidence was found of UK or global simulator vendors selling or partnering in India or the Middle East. An Indian competitor (ScanFlo, Delhi) already exists.

### Cited Findings
- **Price and access barriers:**
  - MRI Education's console is available only inside a £800 course — [Apply](https://www.mrieducation.com/apply/)
  - ScanLab individual cohorts cost $1,000–$2,500 for 6 months — [ScanLab cohorts](https://scanlabmr.com/individual-cohorts/)
  - Corsmed institutional pricing is quote-only, with no per-hour access — [Corsmed pricing](https://corsmed.com/pricing); [Corsmed FAQ](https://www.corsmed.com/faqs/can-i-buy-timed-access-on-corsmeds-simulator-and-only-pay-per-hour-of-use)
- **Free tier limits:** Corsmed's free tier covers only head and knee with ~7 sequences. More than 60 anatomies, pathology simulation and LMS integration are paid — [Corsmed free](https://www.corsmed.com/free-mri-simulator); [Corsmed for individuals](https://www.corsmed.com/en-us/mri-simulator/for-individuals)
- **Connectivity and vendor lock-in:**
  - Siemens SmartSimulator is cloud-streamed and needs latency below 150 ms — [Siemens (LATAM)](https://www.siemens-healthineers.com/latam/services/customer-services/upskill-services/equipment-and-clinical-education/individual-education-and-practice/smartsimulator)
  - SmartSimulator reproduces Siemens UIs and is run with a Siemens application expert — [Siemens (DE)](https://www.siemens-healthineers.com/de/services/customer-services/upskill-services/weiterbildung/smartsimulator)
  - IACI simulates a GE console — [IACI](https://www.iacionline.com/mri-simulator.cms)
- **Hardware barriers:** UK CT simulators are VR or desktop installs (TomoVR), though RadSimTech says no specialised hardware is needed — [RadSimTech FAQ](https://radsimtech.co.uk/faq/)
- **Corsmed's own framing of category problems:** it publishes "Top 10 MRI simulator problems and solutions" (content not retrieved). It is a useful lead for the pain points buyers raise — [Corsmed](https://www.corsmed.com/about-mri-simulators/top-10-mri-simulator-problems-and-solutions)
- **India / Middle East / Asia evidence:**
  - Corsmed: no India, Saudi or UAE partnership found. It claims use in 25+ countries and has a Korean distributor (Medical Standard, Sept 2023) — [Corsmed Korea news](https://www.corsmed.com/news/corsmed-enters-the-south-korean-market-with-medical-standard); [AuntMinnie](https://www.auntminnie.com/resources/vendors/mri/software/company/15554202/corsmed). Its LinkedIn page exists but was not reviewed for regional activity — [LinkedIn – Corsmed](https://www.linkedin.com/company/corsmed)
  - Siemens Healthineers has a SmartSimulator page on its UAE (en-ae) site, so the vendor simulator is at least marketed in the Gulf — [Siemens Healthineers en-ae SmartSimulator](https://www.siemens-healthineers.com/en-ae/comprehensive-education-portfolio/smartsimulator)
  - MRI Education markets to Australia, New Zealand, Singapore, Papua New Guinea and Europe. No India or Middle East page surfaced — [Australasia](https://www.mrieducation.com/australasia/); [Europe](https://www.mrieducation.com/international/europe/europe/)
  - ScanFlo (Zeka Labs, Delhi) prices in INR and is promoted by a Delhi paramedical institute — [ScanFlo MRI](https://scanflo.io/mri); [3D Paramedical](https://3dparamedical.com/mri-scanflo)
- **Language:** no evidence was found of non-English UIs from Corsmed, MRI Education or ScanLab (not verified either way).

### Inferences
- **Positioning gaps an Indian entrant could exploit:**
  1. Rupee pricing and institutional licences sized for Indian BSc MRT / paramedical colleges. No UK or global player shows INR pricing, though ScanFlo does.
  2. Low-bandwidth or offline-capable web delivery, unlike Siemens' cloud streaming at under 150 ms.
  3. Protocol trees and cases matched to Indian clinical practice and the installed base (e.g. 1.5T-heavy fleets).
  4. Regional-language support.
  5. A broad free tier beyond Corsmed's head/knee.
  6. Assessment and educator dashboards aligned to Indian curricula, which mirrors how ScanLab and Corsmed target HCPC/ARMRIT requirements.

  These are inferences from the absence of evidence, not confirmed customer complaints.
- **Expect Corsmed's free tier to reach Indian students** because it is global and needs no card. The window for a free-access differentiator has narrowed as of Nov 2026.

### Gaps
- No direct user complaints (Reddit, forums, app reviews) were collected. The search budget was exhausted before forum or review searches could run.
- Not checked: ISMRM/ISMRT, UKIO and ECR exhibitor lists for MRI simulator vendors, and any Indian (IRIA, Indian Society of Radiographers and Technologists) or Gulf (Arab Health) exhibitor presence for Corsmed, ScanLab or VMC.
- No evidence was found either way on whether Shaderware/RadSimTech or VMC sell in India or the Middle East.
