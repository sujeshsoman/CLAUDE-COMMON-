# Legal, IP and Regulatory Issues: Launching the "Mallu Radiographer" Web MRI Console Simulator (India first, UK/Gulf later), as of November 2026

These are general research notes, not legal advice. Researched 8 November 2026. Most sources are law-firm explainers, consultancy blogs and official-portal search snippets. The research tool could not open several primary pages (cdsco.gov.in, pureglobal.com, corsmed.com and worldipreview.com would not resolve from this session), so where a point rests on a search-result summary rather than the full primary text, the notes say so. Before acting, check each point against the statute, rule or licence linked, or with a lawyer or chartered accountant. Risk levels are the researcher's judgement for a small Kerala start-up.

---

## 1. IP risk of copying real scanner consoles (Siemens syngo/Numaris, GE, Philips, Canon)

### Takeaway
Copying the general MRI workflow and functional parameters (TR, TE, flip angle, FOV, matrix, slice positioning on localisers, protocol trees) is low risk. Major jurisdictions treat functionality, menu command structures and methods of operation as unprotectable. Copying a vendor's actual screens, icons, colour scheme, logos, product names or manual text is a real legal risk: in the EU/UK a GUI can be protected as a copyright "work", in India a GUI can now be registered as a design (Calcutta HC, March 2026), and vendor names and logos are trade marks. The industry norm, and the safe route, is an original vendor-neutral console with factual, nominative-only references to vendors.

### Cited Findings
**EU/UK copyright in GUIs and functionality**
- CJEU, *BSA v Ministry of Culture* (C-393/09, 22 Dec 2010): a GUI is not a "form of expression of a computer program", so it is not protected as a *computer program* under the Software Directive 91/250/EEC. — [Kluwer Copyright Blog](https://legalblogs.wolterskluwer.com/copyright-blog/protection-of-guis-graphical-user-interfaces-some-comments-about-the-ecj-s-preliminary-ruling-in-bsa-v-ministervo-kultury/); [Husovec](https://husovec.eu/2010/12/graphic-user-interface-is-not-protected-as-a-computer-program/)
- The same judgment is widely summarised as holding that a GUI *can* still be protected by ordinary copyright (InfoSoc Directive 2001/29) if it is the author's own intellectual creation. — [Fieldfisher, "Graphical user interfaces can be protected by copyright, rules European Court"](https://www.fieldfisher.com/en/insights/graphical-user-interfaces-can-be-protected-by-copyright-rules-european-court). (The search snippet was cut off before naming the instrument. The judgment text on curia.europa.eu was not retrieved.)
- CJEU, *SAS Institute v World Programming* (C-406/10, Grand Chamber, 2 May 2012): neither the functionality of a computer program nor its programming language or data file formats is protected by copyright. WPL lawfully recreated SAS functionality by observing, studying and testing the program. — [Wikipedia summary](https://en.wikipedia.org/wiki/SAS_Institute_Inc_v_World_Programming_Ltd); [SCL report](https://www.scl.org/2451-sas-institute-inc-v-world-programming-ltd-report-and-analysis/); [boek9.nl](https://www.boek9.nl/boek9-berichten/hvjeu-sas-geen-auteursrecht-functionaliteit-programmeertaal)
- In *SAS v WPL*, copying from a protected user manual can infringe if the copied parts are the author's own intellectual creation. Back in the English High Court, WPL's manual was found to infringe SAS's manual by substantially reproducing its language. — [Wikipedia summary](https://en.wikipedia.org/wiki/SAS_Institute_Inc_v_World_Programming_Ltd); [8 New Square on [2013] EWHC 69 (Ch)](https://8newsquare.co.uk/sas-institute-inc-v-world-programming-ltd-2013-ewhc-69-ch/)

**US (persuasive only)**
- *Lotus v Borland* (1st Cir. 1995): a menu command hierarchy is an uncopyrightable "method of operation" under 17 U.S.C. §102(b). The Supreme Court affirmed by an equally divided court (516 U.S. 233, 1996). — [Wikipedia](https://en.wikipedia.org/wiki/Lotus_Development_Corp._v._Borland_International,_Inc.); [Casemine commentary](https://www.casemine.com/commentary/us/uncopyrightable-method-of-operation:-the-lotus-development-v.-borland-international-decision/view)

**India: copyright and design**
- Computer programmes are literary works under s.2(o) of the Copyright Act 1957. Commentators disagree on whether a GUI's "look and feel" is protected: one view says it can be, as expression; another says only source code is protected. — [Areness Law](https://www.arenesslaw.com/opinions/ip-protection-for-gui-in-india-labyrinth-of-confusion-and-contradictions); [SpicyIP on JioMeet v Zoom GUI](https://spicyip.com/2020/07/does-jiomeets-gui-infringe-copyright-in-zooms-software.html)
- Section 52(1)(ac) of the Copyright Act permits observing, studying or testing a program's functioning to work out the ideas and principles behind it. Section 52(1)(ad) covers copies or adaptations from a lawfully obtained copy for *non-commercial personal use*, which a commercial simulator would not be. — [Copyright (Amendment) Act 1999 text](https://kwx.liehendr.com/content/wikisource_en_all_maxi_2022-09/A/Page%3AIndian_Copyright_Act_(5th_Amendment)_1999.djvu/3) (search-result summary, secondary mirror of the amendment text)
- *NEC Corporation v Controller of Patents & Designs* (Calcutta HC, 2026:CHC-OS:69, 9 March 2026): GUIs are not excluded per se from design protection under the Designs Act 2000. A GUI shown on an electronic device may be a registrable "design". The court rejected the Controller's view that a GUI cannot be a design because it cannot be sold separately. — [Mondaq](https://www.mondaq.com/india/patent/1813770/graphical-user-interfaces-guis-qualify-for-design-registration-under-the-designs-act-calcutta-high-court); [Conventus Law](https://conventuslaw.com/report/calcutta-high-court-clears-way-for-registration-of-gui-designs-in-india/); [AsiaIPLaw](https://asiaiplaw.com/index.php/sector/copyright/guis-as-registrable-designs-in-india-from-ust-global-to-the-2026-clarification)
- Under s.15 of the Copyright Act, a registered design loses copyright protection. A government Concept Note on design-law amendments (late January 2026) specifically addresses GUI protection. — [Mondaq](https://www.mondaq.com/india/patent/1813770/graphical-user-interfaces-guis-qualify-for-design-registration-under-the-designs-act-calcutta-high-court); [WorldIPReview, 22 Apr 2026](https://www.worldipreview.com/jurisdiction-reports/india-reimagines-gui-design-protection) (headline only, page not retrievable)

**India: trade marks and nominative use**
- Trade Marks Act 1999 s.30(1): third-party use is permitted only if it follows "honest practices in industrial or commercial matters" and does not take unfair advantage of, or harm, the mark's distinctive character or repute. Section 30(2)(d) protects use for accessories or parts adapted to the mark owner's goods. The honest-practices test is a precondition to the s.30(2) exceptions. — [Mondaq: Doctrine of nominative fair use](https://www.mondaq.com/india/trademark/879442/doctrine-of-nominative-fair-use-under-trademark-law); [AZB & Partners](https://www.azbpartners.com/bank/doctrine-of-nominative-fair-use-under-trademark-law/)
- In *Toyota v Prius Auto Industries* (Delhi HC), the nominative fair use defence under s.30(2)(d) was rejected for use of TOYOTA/INNOVA marks on accessories. Commentary describes limits on font size and on wording such as "Genuine Accessories". *Consim Info v Google India* (Madras HC) set conditions for nominative fair use. — [Mondaq (2017)](https://www.mondaq.com/india/trademark/610600/nominative-fair-use-of-a-trademark-june-2017); [Mondaq (2019)](https://www.mondaq.com/india/trademark/879442/doctrine-of-nominative-fair-use-under-trademark-law)

**How existing simulator companies handle this**
- Corsmed, a commercial virtual MRI simulator, presents its platform as vendor-neutral. UCLH says this matters because it runs scanners from several manufacturers. — [Corsmed UCLH case study](https://www.corsmed.com/case-studies/nhs-university-college-london-hospitals) (vendor marketing; page could not be fetched, search summary only)
- *Virtual Scanner* (open-source, imr-framework) has a "Standard Mode" that imitates a clinical console for technologist training. It is built on vendor-neutral standards such as Pulseq. — [PyPI virtual-scanner](https://pypi.org/project/virtual-scanner/1.0.22); [JOSS paper](https://joss.theoj.org/papers/10.21105/joss.01637.pdf)
- ScanLabMR sells MRI simulator licences to students, technologists and educators. RadSim is a physical mock scanner, not a software console. — [ScanLabMR](https://scanlabmr.com/mri-simulator/); [HealthySimulation – RadSim](https://www.healthysimulation.com/vendors/radsim/)

### Inferences
- **Do (low risk):** build an original console with your own layout, icons, colour palette, fonts and wording. Use generic, textbook MRI terminology and parameter names. Use standard, generic workflow steps (patient registration → localiser → plan → sequence parameters → scan → review). Under *SAS*, *Lotus* and s.52(1)(ac), this functional layer is the least protectable part of any console.
- **Do (low risk, if done carefully):** factual, nominative statements such as "concepts transferable to Siemens, GE, Philips and Canon scanners" or "see how this parameter is labelled on different vendors", in plain text, with no logos, no stylised fonts and no implied endorsement. Add a non-affiliation notice. Note that Indian courts have read s.30 narrowly in the accessories cases (Toyota), so keep references minimal and necessary.
- **Don't (medium to high risk):**
  - pixel-copy or trace real console screenshots
  - reproduce vendor icons, splash screens, logos or colour schemes
  - copy text from vendor operator manuals or application guides (the *SAS* manual finding)
  - call the product "Siemens-style" or "syngo-like", or use vendor marks in the product name, domain or ads (e.g. "Learn syngo with Mallu Radiographer")
  - extract assets from vendor software or decompile it. This could also breach the hospital's licence or EULA terms.
- **Watch for:** vendor-specific sequence brand names (for example, the proprietary names different vendors give similar motion-correction or parallel-imaging techniques). Some may be registered marks. A generic name plus a small "vendor equivalents" table with ™/® attributions is safer than adopting a vendor's name as the menu label. Check each name before use. This point was not researched.
- **Overall risk:** a vendor-neutral UI with nominative references is low risk. A screen-faithful "syngo clone" is medium to high risk in the EU/UK, where GUIs can be InfoSoc works. In India the risk is medium and rising, because GUIs are now design-registrable and vendors may register console GUIs as designs.
- An OEM licence (e.g. Siemens Healthineers' training programmes) is the only route to legitimately reproducing a real console look. It is unlikely to be available to a small start-up early on. Not researched.

### Gaps
- No reported case or public vendor action (Siemens, GE, Philips or Canon) against an MRI or radiography training simulator was found.
- No vendor trade-mark usage guidelines (e.g. Siemens Healthineers brand rules) were retrieved.
- Whether Siemens, GE, Philips or Canon have registered console GUIs as designs in India was not checked. An Indian design-register search is recommended.
- The full CJEU texts of C-393/09 and C-406/10 and the full NEC v Controller judgment were not read. Holdings are from commentary.
- No source was found on whether Corsmed or ScanLabMR hold OEM licensing agreements.

---

## 2. Medical device regulation: is a pure training simulator a medical device / SaMD?

### Takeaway
In India, the EU and the UK, regulatory status turns on the manufacturer's *intended purpose* as stated in labelling, instructions and marketing. A simulator sold solely for education and training, with no diagnostic, monitoring or treatment purpose and no use on real patients, is outside medical device regulation. CDSCO's software guidance (draft October 2025, final reportedly July 2026) reportedly lists "education or training without a medical purpose" as out of scope. The risk comes from marketing or features that drift into clinical claims. A disclaimer does not rescue a product whose marketing implies clinical use.

### Cited Findings
- CDSCO guidance on medical device software under MDR 2017: software intended by the manufacturer for medical purposes, and meeting the definition under the Drugs and Cosmetics Act 1940 and MDR 2017, is regulated as a medical device. Software intended solely for general wellness, fitness, education or training *without a medical purpose* falls outside MDR scope. — [CDSCO guidance PDF](https://www.cdsco.gov.in/opencms/export/sites/CDSCO_WEB/Pdf-documents/Guidance-document-on-Medical-Device-Software-under-MDR-2017.pdf) (PDF could not be opened from this session; wording is from a search-result summary); [Nishith Desai Associates](https://nishithdesai.com/research-and-articles/hotline/pharma-healthcare-update/from-code-to-compliance-decoding-indias-medical-device-software-guidance-15623); [Mondaq](https://www.mondaq.com/india/healthcare/1826286/cdsco-publishes-guidance-on-medical-device-software-under-mdr-2017)
- MDR 2017 defines "intended use" as the use for which the device is intended according to the manufacturer's labelling or data supplied. CDSCO classification of software is based on intended use and the First Schedule classification rules. — [CDSCO guidance PDF](https://www.cdsco.gov.in/opencms/export/sites/CDSCO_WEB/Pdf-documents/Guidance-document-on-Medical-Device-Software-under-MDR-2017.pdf); [Conventus Law](https://conventuslaw.com/report/india-cdsco-issues-guidance-on-medical-device-software-under-the-medical-devices-rules-2017/)
- Timing: the CDSCO draft software guidance was issued 21 Oct 2025. Secondary sources report the final guidance (Doc No. CDSCO/MD/GD/MDSW/01/2026) was issued 21 July 2026. — [CDSCO draft PDF](https://cdsco.gov.in/opencms/resources/UploadCDSCOWeb/2018/UploadPublic_NoticesFiles/Draft%20guidance%20document%20on%20Medical%20Device%20Software%2021%2010%202025.pdf); [MediaNama, Nov 2025](https://www.medianama.com/2025/11/223-draft-guidelines-medical-device-software/); [PureGlobal](https://www.pureglobal.com/news/india-cdsco-medical-device-software-guidance-2026) (final-version date and number not verified against the CDSCO circular)
- EU MDR: Art. 2(1) defines a medical device by reference to specific *medical purposes* for human beings. Art. 2(12) defines "intended purpose" by the manufacturer's label, instructions for use and promotional or sales materials. Under MDCG 2019-11, software without a medical intended purpose is outside the MDR. — [OpenRegulatory, MDCG 2019-11 explained](https://openregulatory.com/mdcg/mdcg-2019-11); [European Commission MDCG 2019-11](https://health.ec.europa.eu/document/download/b45335c5-1679-4c71-a91c-fc7a4d37f12b_en)
- MDCG 2019-11 was revised (Rev.1, June 2025). — [MDR Regulator](https://mdrregulator.com/news/revised-mdcg-2019-11-guidance-updated-approach-to-qualification-and-classification-of-medical-software)
- UK MHRA guidance "Medical device stand-alone software including apps": whether software is a device depends on the medical purpose stated in labelling, instructions for use and promotional material. Diagnosis and monitoring are medical purposes. Devices fall under the UK Medical Devices Regulations 2002 (as amended). — [GOV.UK MHRA guidance PDF](https://assets.publishing.service.gov.uk/media/6abf6c8c943e890cb55e5e52/Medical_device_stand-alone_software_including_apps__including_IVDMDs.pdf); [GOV.UK publication page](https://www.gov.uk/government/publications/medical-devices-software-applications-apps)
- Disclaimers do not override intended purpose: an app placed on the market for a medical purpose must comply whatever disclaimer it carries. — [CMS Law update on MHRA guidance](https://cms.law/en/gbr/legal-updates/mhra-issues-updated-guidance-on-ehealth-stand-alone-software-including-apps)

### Inferences
- **Status:** a browser-based console simulator running on synthetic or public phantom data, used only to teach scanning technique, is very likely *not* a medical device in India, the EU or the UK. Risk is low if claims are kept clean.
- **Wording to avoid** in the app, website, ads, Instagram/YouTube posts and app-store listings:
  - "diagnose", "diagnostic quality", "clinical decision support"
  - "use on patients", "optimise your patient's scan", "protocol recommendations for your patients"
  - "detect pathology", "AI reads your scans", "validated for clinical use"
  - "upload your patient DICOM for analysis"
- **Features that could change the classification:**
  - accepting real patient scans and giving outputs about them (image-quality or artefact "assessment" of a real study, or protocol advice for a specific patient)
  - connecting to real scanners or PACS
  - computing SAR/safety limits that a user might rely on clinically
  - generating dose or contrast advice for real patients
- **Recommended disclaimers** (on the footer, the terms of service, every simulated scan screen and any certificate). These should support the intended purpose, not contradict the marketing:
  - "For education and training only. Not a medical device. Not intended for diagnosis, treatment, patient monitoring or any clinical decision. Do not use with real patients or real patient data."
  - "Simulated images are generated from synthetic models and openly licensed research datasets. They are not real patient cases."
  - "Parameters, SAR and safety values are illustrative. Always follow your scanner manufacturer's operator manual, your department's protocols and your MR safety officer."
  - "Not affiliated with, endorsed by or sponsored by Siemens Healthineers, GE HealthCare, Philips or Canon Medical Systems. All trademarks belong to their respective owners." (See Q1.)
- Keep a short internal "intended purpose statement" (one page) that mirrors CDSCO's suggested elements (intended users = radiography students and technologists; use environment = education; no medical purpose). It shows regulators and payment or app-store reviewers that the product is non-medical.

### Gaps
- The final CDSCO guidance text (July 2026) could not be opened (cdsco.gov.in blocked from this session). The exact "education or training" exclusion wording is from a search summary.
- The MHRA guidance's "non-medical functions" list was not read verbatim, so it is not confirmed whether it names education or training explicitly.
- Gulf regulators (UAE MOHAP/DHA, Saudi SFDA) were not researched for software qualification.

---

## 3. Images and data: public MRI datasets, phantoms, and hospital images

### Takeaway
For a paid product, use data that clearly allows commercial use:
- OpenNeuro (CC0, check each dataset)
- most TCIA collections (CC BY 3.0/4.0, but brain and head/neck collections moved to a restricted licence in 2022)
- IXI (CC BY-SA 3.0, which brings ShareAlike obligations on derived images)
- your own synthetic or phantom-based simulations

Avoid fastMRI and OASIS for the commercial product: both are non-commercial. HCP, BrainWeb and MIDA need the licence checked first. Images from your own hospital workplace are the highest-risk source. They carry patient-privacy (DPDP), employer and ethics problems, and head MRI can be re-identified from the face.

### Cited Findings
- **fastMRI (NYU):** access is "for the purposes of internal research or education only" under a data sharing agreement. The authors "do not allow any commercial use of the dataset itself", though they do not discourage developing or testing software with it. Commercial permission: fastmri@med.nyu.edu. — [fastMRI site](https://fastmri.med.nyu.edu/); [Radiology: AI 2020 paper](https://pubs.rsna.org/doi/full/10.1148/ryai.2020190007)
- **OpenNeuro:** newly published datasets and new versions are released under CC0, after up to a 36-month embargo. Some older datasets were CC0, PDDL or CC-BY, so check each dataset's licence field. Attribution is encouraged though CC0 does not require it. — [OpenNeuro FAQ](https://openneuro.readthedocs.io/faq.html); [Neurostars thread](https://neurostars.org/t/openneuro-dataset-licensing-question/4307)
- **TCIA:** most data is usable for "commercial, scientific and educational purposes" under CC BY 3.0 or 4.0. A small number of collections are CC BY-NC (no longer an option for new submissions). From 6 Jan 2022, all brain and head/neck collections where data could be used to reconstruct a face moved to a TCIA Limited Access License. Check each collection's citation and data usage policy. — [TCIA Data Usage Policy](https://wiki.cancerimagingarchive.net/x/c4hF); [TCIA redirection notice re head/neck](https://wiki.cancerimagingarchive.net/x/NIIiAQ)
- **IXI:** distributed under CC BY-SA 3.0 with a request to acknowledge the IXI website. — [TorchIO docs](https://docs.torchio.org/_modules/torchio/datasets/ixi.html); [FLamby docs](https://owkin.github.io/FLamby/fed_ixi.html); [NITRC IXI page](https://www.nitrc.org/projects/ixi_dataset/) (official brain-development.org page not retrieved)
- **OASIS:** data are "for non-commercial, academic research purposes only". Commercial use, including sale of data, is prohibited without prior written authorisation. Processed OASIS-3 results are also academic-only. — [OASIS DUA (July 2022 PDF)](https://sites.wustl.edu/oasisbrains/files/2024/04/DataUseAgreement_July2022-b14b9acfd16bd1b3.pdf); [OASIS access page](https://sites.wustl.edu/oasisbrains/home/access); [Hugging Face copy of DUA](https://huggingface.co/datasets/FOMO25/FOMO60K)
- **HCP (Human Connectome Project):** open-access imaging data requires a ConnectomeDB account and agreement to the Open Access Data Use Terms. Related consortium terms (AABC registered access, developing HCP) expressly prohibit commercial use or monetisation. — [HCP Young Adult data use terms](https://humanconnectome.org/study/hcp-young-adult/data-use-terms); [AABC Data Use Terms PDF](https://www.humanconnectome.org/storage/app/media/data_use_terms/AABC_Consortium_Registered_Access_Data_Use_Terms.pdf)
- **MIDA head and neck model (IT'IS / FDA):** free from IT'IS subject to a licence agreement "for protection of privacy", and must be cited as the licence stipulates. Raw MR and DTI data are not distributed, only the segmented model. Sources conflict on commercial use: Wikipedia says the models are free for non-commercial research, while the IT'IS page says the model is free for everyone apart from handling fees. — [FDA MIDA page](https://cdrh-rst.fda.gov/mida-multimodal-imaging-based-model-human-head-and-neck); [IT'IS MIDA page](https://itis.swiss/virtual-population/regional-human-models/mida-model); [Wikipedia IT'IS](https://en.wikipedia.org/wiki/Foundation_for_Research_on_Information_Technologies_in_Society)
- **BrainWeb (McGill):** simulated brain MRI from normal and MS anatomical models (20 normal models now available). The standard citation is Cocosco et al. 1997. No licence or terms-of-use statement was found in search results. — [BrainWeb](https://brainweb.bic.mni.mcgill.ca/); [McGill BIC page](https://www.mcgill.ca/bic/software/brainweb-mri-simulator)
- **Hospital and patient images (India):** the DPDP Act covers patient records and medical images, and personal data is information about an identifiable individual. — [AMLegals: Health data and the DPDP Act](https://amlegals.com/health-data-and-the-dpdp-act-a-practical-guide/); [Mondaq: DPDP in hospitals](https://www.mondaq.com/india/privacy-protection/1666622/the-applicability-of-the-dpdp-act-in-hospitals-a-new-era-for-patient-data-protection)
- ICMR's National Ethical Guidelines for biomedical and health research (2017) and the ICMR GCLP guidelines (2021) are the relevant sector guidance on confidentiality and data management. — [PMC review 2024](https://pmc.ncbi.nlm.nih.gov/articles/PMC11754748)
- UK analogy: RCR guidance on patient confidentiality in radiology information systems does not apply to properly anonymised data. — [RCR guidance (2019)](https://www.rcr.ac.uk/media/slmbkf0d/rcr-publications_guidance-on-maintaining-patient-confidentiality-when-using-radiology-department-information-systems-second-edition_november-2019.pdf)

### Inferences
**Dataset licence summary**

| Dataset | Commercial use? | Notes |
|---|---|---|
| OpenNeuro | Yes (CC0) | Check each dataset |
| TCIA (body) | Yes (most CC BY) | Attribution required. Brain and head/neck collections are now restricted |
| IXI | Yes (CC BY-SA 3.0) | Images you derive and distribute should carry CC BY-SA. Keep them as separately licensed assets, not mixed with proprietary code |
| BrainWeb | Unknown | Email McGill BIC |
| MIDA | Unclear | Read the licence via DOI 10.13099/ViP-MIDA-V1.0. It is a tissue model for simulating images, not ready-made images |
| HCP | Unclear | Read the WU-Minn Open Access terms |
| fastMRI | No | Internal research/education only; ask NYU |
| OASIS | No | Non-commercial only |

- Safest technical route: generate images by physics simulation (Bloch or signal-equation) from tissue-property maps (BrainWeb/MIDA-style phantoms, subject to licence), from your own digital phantoms, or from CC0/CC BY data. Keep an attribution page and a "data provenance register" (source, licence, version, date downloaded) for each image set.
- **Hospital images: avoid (high risk).** Do not take DICOMs or screenshots from your workplace PACS or scanner console for the product. Main risks:
  1. Patient privacy: DPDP once fully in force, plus existing confidentiality duties. DICOM headers and burned-in annotations identify patients, and head MRI can reconstruct faces (the reason TCIA restricted head collections).
  2. Employer ownership of, or contractual control over, data and work product.
  3. Lack of ethics committee approval and patient consent for commercial reuse.
  4. Possible breach of the vendor software licence if console screenshots are used.
- If hospital images are ever wanted, do it formally: written permission from the hospital, institutional ethics committee approval, proper de-identification (header scrub, burned-in text removal, defacing for head scans) and a written data-use agreement allowing commercial educational use.

### Gaps
- BrainWeb licence or terms not found.
- HCP WU-Minn Open Access Data Use Terms commercial clause not confirmed.
- MIDA licence text not retrieved.
- IXI official page not retrieved.
- No source found on whether DPDP Act/Rules expressly exclude anonymised data. The Act defines personal data by identifiability, but there is no explicit anonymisation standard. No ICMR radiology-specific anonymisation standard was found.
- Employer IP rules (Kerala government hospitals or private hospital contracts) on images and know-how were not researched. Check your own employment contract and service rules.

---

## 4. Student data: DPDP Act 2023 + DPDP Rules 2025; UK GDPR

### Takeaway
The DPDP Rules were notified in November 2025 (G.S.R. 846(E)) with a phased start. Most operational duties apply from about 13–14 May 2027, around six months from now:
- notice and consent
- security safeguards
- breach reporting
- children's verifiable parental consent

Build for them now: clear notice, consent, minimal data collection, reasonable security, a 72-hour breach plan, and age-gating, because any user under 18 needs verifiable parental consent and cannot be tracked or targeted. If you sell to UK users, the UK GDPR applies extraterritorially (Art. 3(2)) and may require a UK representative (Art. 27).

### Cited Findings
- The DPDP Rules 2025 were notified in November 2025 (sources say 13 or 14 November; Gazette G.S.R. 846(E)) with staggered commencement:
  - Data Protection Board provisions applied immediately
  - Consent Manager registration from 12 months
  - main operational obligations from 18 months (13 or 14 May 2027, sources differ)
  — [Mondaq regulatory update](https://www.mondaq.com/india/data-protection/1713500/regulatory-update-notification-of-the-digital-personal-data-protection-rules-2025); [AMLegals: immediate actions](https://amlegals.com/dpdp-rules-notified-immediate-actions/); [Storyboard18](https://www.storyboard18.com/digital/breaking-govt-notifies-final-dpdp-rules-sets-staggered-rollout-with-key-obligations-for-data-fiduciaries-84201.htm)
- Breach reporting: notify affected individuals and the Data Protection Board without delay, then file a detailed report within 72 hours. The Board can extend this on request. — [AMLegals: DPDP Rules 2025](https://amlegals.com/digital-personal-data-protection-rules-2025/); [Bitraser](https://www.bitraser.com/article/dpdp-rules-2025.php)
- Children (under 18 under the DPDP Act): processing needs verifiable parental or guardian consent, with age-assurance mechanisms. Tracking, behavioural monitoring and targeted advertising directed at children are prohibited. — [AMLegals](https://amlegals.com/digital-personal-data-protection-rules-2025/); [Lukmaan IAS explainer (Apr 2026)](https://blog.lukmaanias.com/2026/04/28/the-digital-personal-data-protection-dpdp-rules-2025/)
- General overviews of the Rules' obligations (notice, consent, security, retention, rights): — [EY India](https://www.ey.com/en_in/insights/cybersecurity/transforming-data-privacy-digital-personal-data-protection-rules-2025); [BDO India PDF](https://www.bdo.in/getmedia/87552494-85d2-4edb-95da-0f118fdb3052/The-DPDP-Rules_BDO-India_2025.pdf); [Mondaq: 8 key takeaways](https://www.mondaq.com/india/privacy-protection/1709084/8-key-takeaways-the-digital-personal-data-protection-rules-2025)
- UK GDPR Art. 3(2): an organisation outside the UK with no UK establishment must comply when it offers goods or services to individuals in the UK. Art. 27: such a controller must designate a UK representative in writing. There is an exemption for occasional, low-risk processing that excludes large-scale special-category data. Appointing a representative does not shift liability. — [legislation.gov.uk UK GDPR Art. 27](https://www.legislation.gov.uk/eur/2016/679/section/27); [BCLP](https://www.bclplaw.com/en-US/insights/who-sir-me-sir-appointing-gdpr-representatives-in-the-uk-and-the-eu.html); [Fieldfisher UK GDPR Art. 27](https://ukgdpr.fieldfisher.com/chapter-4/article-27-gdpr/)

### Inferences
**Practical DPDP checklist** for a site with student accounts, payments (via Razorpay, Stripe or similar) and analytics:

1. **Collect less.** Name, email, phone, course progress and invoice details. Avoid Aadhaar, date of birth beyond an "I am 18+" check, and hospital or employer details unless needed.
2. **Notice + consent at sign-up.** Use a standalone, plain-language notice listing:
   - the data collected
   - the purposes (account, course delivery, certificate, payments, analytics, marketing)
   - how to withdraw consent
   - how to contact you or complain to the Data Protection Board

   Keep marketing consent as a separate unticked box.
3. **Analytics and cookies:** use privacy-friendly analytics or consent-gated trackers. Do not use ad pixels or behavioural tracking for any under-18 user.
4. **Children:** the simplest course is "18+ only" in the terms with an age declaration. If you want plus-two or first-year diploma students under 18, build verifiable parental consent and turn off tracking and targeted ads for them.
5. **Processors:** sign or accept data processing terms with the hosting, payment, email and video providers. The payment gateway handles card data, so never store card numbers yourself.
6. **Security:** encryption in transit and at rest, access control, logging, backups.
7. **Breach plan:** a written runbook covering who notifies users and the Board, with a 72-hour detailed report.
8. **Rights:** handle access, correction and erasure requests, and delete accounts on request or after a defined inactivity period.

**Timing risk:** before May 2027, regulatory exposure is low to medium. After May 2027, missing basics is medium risk. The penalty schedule was not verified in this session; see Gaps.

**UK:** if UK sales are more than occasional, appoint a UK representative (commercial services cost a few hundred pounds a year; price not researched) and publish a UK-GDPR-compliant privacy notice. **Gulf:** check UAE PDPL and Saudi PDPL before launching there (not researched).

### Gaps
- The exact DPDP penalty amounts (DPDP Act Schedule) were not verified in this session. Training knowledge suggests up to ₹250 crore for security-safeguard failures, but this must be checked on indiacode.nic.in or meity.gov.in.
- The Rule 3 notice contents and the verifiable-parental-consent mechanisms (Rule 10) were not read verbatim.
- Whether the IT Act s.43A / SPDI Rules 2011 continue to apply until May 2027 was not confirmed.
- UAE and Saudi data-protection law, and ICO guidance on the representative, were not researched.

---

## 5. Brand: searching and registering "Mallu Radiographer" as a trade mark

### Takeaway
File in India in classes 41 (education and training), 42 (online, non-downloadable software / SaaS) and 9 (downloadable software and apps). Class 44 (medical services) is not needed for a training product. The official fee is ₹4,500 per class by e-filing for an individual, DPIIT start-up or small enterprise (₹9,000 otherwise), so three classes cost about ₹13,500 plus attorney fees. DPIIT start-ups get attorney fees covered under SIPP. "Radiographer" is plainly descriptive for these services. "Mallu" is a regional colloquialism that may draw a s.9 objection, but the *combination*, ideally filed with a distinctive logo, has a reasonable chance. Expect an examination report, probably a reply or hearing, a four-month opposition window after advertisement, and roughly 1–2 years to registration if unopposed.

### Cited Findings
- Official TM-A filing fee: ₹4,500 (e-filing) or ₹5,000 (physical) per class per mark for an individual, start-up or small enterprise; ₹9,000 or ₹10,000 for all others. Expedited examination carries a separate higher fee (listed at ₹20,000 for this category). — [IP India Forms & Official Fees](https://www.ipindia.gov.in/pages/trade-marks/learn/forms-and-official-fees); [IP India form and fees (TM)](https://ipindia.gov.in/Trademarks/form_and_fees_tm)
- Eligibility for the reduced fee: sources differ on whether DPIIT recognition or Udyam registration as a micro or small enterprise is needed. Individuals qualify per the fee schedule wording. — [IP India](https://www.ipindia.gov.in/pages/trade-marks/learn/forms-and-official-fees); [SS Rana: TM filing fees](https://ssrana.in/ip-laws/trademarks-in-india/tm-filing-fees-forms-india/)
- Startup India SIPP: DPIIT-recognised start-ups get a 50% rebate on trade-mark filing fees (Trade Marks Rules 2017). Under SIPP, "the Central Government shall bear the entire fees of the facilitators" for any number of patents, trade marks or designs. Facilitation fees were revised from 2 Nov 2022. — [Startup India IPR page](https://www.startupindia.gov.in/chinese_traditional/content/sih/en/intellectual-property-rights.html); [Bar & Bench: SIPP analysis](https://barandbench.com/news/analysis-of-the-scheme-for-facilitating-start-ups-intellectual-property-protection-sipp)
- Grounds of refusal: s.9 (absolute) covers marks that are non-distinctive or descriptive, including those indicating kind, quality, intended purpose or geographical origin. s.11 (relative) covers conflicts with earlier marks. Evidence of acquired distinctiveness (secondary meaning) can overcome a pure s.9 objection. — [Intepat: Sections 9 and 11](https://www.intepat.com/blog/section-9-11-grounds-refusal-trademark-india); [iPleaders: objections and oppositions](https://blog.ipleaders.in/handling-trademark-objections-and-oppositions/)
- Opposition: third parties may oppose within four months of advertisement in the Trade Marks Journal. Some practitioner sources mention a one-month extension; others call it a fixed deadline, so treat four months as the working figure. If unopposed, the Registry proceeds to registration. Advertisement usually happens several months to over a year after filing, longer if a hearing is needed. — [Mondaq: understanding opposition](https://www.mondaq.com/india/trademark/1604054/understanding-trademark-opposition-in-india-what-every-brand-owner-needs-to-know); [Kanakkupillai: Journal publication](https://www.kanakkupillai.com/learn/trademark-journal-publication-in-india/); [LawSikho](https://lawsikho.com/blog/process-obtaining-trademark-opposition-a-guide/)

### Inferences
**Search before filing (free):**
1. IP India public search (tmrsearch.ipindia.gov.in): wordmark search for "MALLU", "RADIOGRAPHER" and "MALLU RADIO*" in classes 9, 41, 42 and 44, plus a phonetic search.
2. Google, Instagram, YouTube, Facebook and LinkedIn for existing "Mallu …" education or medical creators. The word "Mallu" is common in Kerala creator brands, so look for confusingly similar *radiography or medical-education* marks.
3. Domain availability (malluradiographer.com / .in / .co.uk) and matching social handles. Register them now. They are cheap and help prove prior use.
4. A UK IPO and WIPO Global Brand Database check if UK or Gulf sales are planned.

**Registrability:**
- "Radiographer" alone is descriptive for class 41 radiography training, so expect a s.9(1)(b) objection or a request to disclaim it.
- "Mallu" is a colloquial term for Malayalis or Keralites (common knowledge, not sourced). An examiner may treat it as indicating the geographical or community origin of the services.
- Filing as a device mark (logo plus words) and claiming user date evidence improves the odds.
- Overall: medium risk of an objection, low to medium risk of final refusal.
- Note that "Mallu" can be read as a slang or derogatory term in some contexts. That is a brand-perception rather than a legal issue, so judge the audience reaction, especially for UK and Gulf markets. Not researched.

**Classes and budget:**
- Classes 41 + 42 are the core; 9 if you ship an app. Class 44 is not needed unless you offer actual imaging or medical services.
- Budget: 3 × ₹4,500 = ₹13,500 government fee. Attorney fees are typically a few thousand rupees per class (not researched), or free via an SIPP facilitator once DPIIT-recognised.
- Use ™ now. Use ® only after registration: falsely representing a mark as registered is an offence under the Trade Marks Act (s.107; not verified in this session).
- File in the name of the eventual entity, or as an individual and assign later with a recorded assignment.
- UK and Gulf: India filings do not protect abroad. Consider a Madrid Protocol extension (UK) within the six-month priority window, or national filings in the UAE or Saudi Arabia later. Not researched.

### Gaps
- No search of the live Indian register for "Mallu"-formative marks was possible from this session. Run it manually.
- No reported Indian decision on "Mallu" as a mark was found.
- Current attorney fee ranges and actual 2026 Registry processing times were not found from official sources.
- Whether the one-month opposition extension still exists under the 2017 Rules is unconfirmed (sources conflict).
- Madrid, UAE and Saudi filing costs were not researched.

---

## 6. Business setup, tax, start-up schemes and employment conflict

### Takeaway
A sole proprietorship is the quickest way to start but cannot get DPIIT start-up recognition, which unlocks SIPP, tax and KSUM benefits. A small LLP or private limited company is better once grants or investors are in view. Private limited is more investor-friendly; an LLP has lower compliance (no source compared these directly).

GST:
- Private online courses and SaaS are taxed at 18%.
- Registration is compulsory above ₹20 lakh aggregate turnover for services (Kerala is not a special-category state), and inter-state supply of services below that threshold is exempt from compulsory registration.
- Sales to foreign customers can be zero-rated exports under a Letter of Undertaking (LUT).

If you are a Kerala government employee, Rule 48 of the Kerala Government Servants' Conduct Rules 1960 requires prior sanction before engaging in any trade or business. Running a paid software business without sanction is a real disciplinary risk. Private hospital employees should check their contract.

### Cited Findings
**Startup India / DPIIT**
- Eligible entities: private limited company, LLP or registered partnership firm, plus (per newer sources) cooperatives. Sole proprietorships, HUFs and AOPs are not eligible. The entity must be no more than 10 years old (20 for the new deep-tech category). — [Taxguru: DPIIT recognition](https://taxguru.in/corporate-law/startups-dpiit-recognition-process-benefits.html); [FoxMandal: revised framework](https://foxmandal.in/news/dpiit-notifies-revised-startup-framework-introduces-deep-tech-category/)
- Turnover cap: older guides say ₹100 crore. FoxMandal reports a revised framework raising it to ₹200 crore (₹300 crore for deep-tech). The s.80-IAC tax holiday keeps its own ₹100 crore condition. — [FoxMandal](https://foxmandal.in/news/dpiit-notifies-revised-startup-framework-introduces-deep-tech-category/); [Kanakkupillai](https://www.kanakkupillai.com/learn/who-is-eligible-for-dpiit-registration/) (effective date of the change not confirmed)

**Kerala Startup Mission (KSUM) grants** (figures are from aggregators and older notices; confirm on the KSUM portal)
- Idea Grant up to ₹3 lakh (older notices ₹2 lakh). Productisation Grant up to ₹7 lakh (women/transgender variant up to ₹12 lakh in some listings). Scale-up Grant up to ₹15 lakh (older ₹12 lakh). Market Acceleration up to ₹10 lakh.
- Idea and productisation grants combined were capped at ₹7 lakh, and disbursement is phased after expert review.
— [KSUM grants portal](https://grants.startupmission.in); [StartupGrantsIndia: KSUM grant ladder](https://www.startupgrantsindia.com/schemes/kerala-startup-mission-grant-ladder); [Deccan Chronicle (older)](https://www.deccanchronicle.com/nation/current-affairs/120518/kerala-sets-norms-for-startup-funding.html); [KSUM Idea Grant site](https://sites.google.com/startupmission.in/ideagrant/home)

**GST**
- Private online courses and ed-tech platforms are generally taxed at 18%. The September 2025 GST rate changes did not create a separate rate for online courses. Education services by recognised institutions remain exempt. — [Masters India: GST on online courses](https://www.mastersindia.co/gst/gst-online-courses); [Busy.in](https://busy.in/gst-rates/online-education/)
- Registration threshold: inter-state taxable service suppliers with aggregate (all-India, PAN-based) turnover up to ₹20 lakh are exempt from compulsory registration (Notification 10/2017-Integrated Tax, 13 Oct 2017). The limit is ₹10 lakh in special-category states, and Kerala is not one. — [TaxGuru](https://taxguru.in/?p=625827); [Kanakkupillai: threshold for services](https://www.kanakkupillai.com/learn/new-gst-registration-threshold-limit-for-services/); [Spotonz: GST registration Kerala](https://www.spotonz.com/blog/gst-registration-kerala-2025/)
- OIDAR: from 1 Oct 2023 (Finance Act 2023), the "essentially automated and involving minimal human intervention" test was removed from the IGST Act s.2(17) definition, widening OIDAR. Grant Thornton lists distance teaching, coaching and education among OIDAR services. Sources conflict on whether teacher-led courses are OIDAR. — [India Briefing](https://india-briefing.com/news/indias-oidar-taxation-shift-key-changes-effective-october-1-2023-29757.html); [Grant Thornton OIDAR flyer](https://www.grantthornton.in/globalassets/1.-member-firms/india/assets/pdfs/oidar-flyer.pdf); [TaxGuru OIDAR analysis](https://taxguru.in/goods-and-service-tax/online-information-database-access-retrieval-services-oidar-analysis.html)
- Exports: an Indian supplier selling to students outside India can zero-rate the supply by filing an LUT (Form RFD-11) and quoting it on invoices. Without an LUT, IGST is paid and refunded later. — [Masters India](https://www.mastersindia.co/gst/gst-online-courses); [CA Sahuja: GST on online education and export](https://www.casahuja.com/2024/01/gst-on-online-education-and-export-of.html?m=1)

**Government-servant rules (Kerala)**
- Kerala Government Servants' Conduct Rules 1960, Rule 48: a government servant may not engage directly or indirectly in any trade or business, or take up other employment, without the previous sanction of Government. Honorary social or charitable work and *occasional* literary, artistic or scientific work are allowed without sanction but must stop if Government so directs. — [GCEK copy of the Conduct Rules (PDF)](https://www.gcek.ac.in/pdf/Government%20Servant%20Conduct%20Rules1960.pdf); [LiveLaw: Kerala HC on Rule 48 (Ciza Thomas)](https://www.livelaw.in/amp/high-court/kerala-high-court/kerala-high-court-ciza-thomas-ktu-show-cause-notice-quash-240736)
- A Kerala ruling treated a PSC employee's publishing of examination guides as "private trade" under Rules 48/58A. The court noted such violations would normally not call for major penalties. — [Indian Kanoon](https://future.indiankanoon.org/doc/3096005/) (search-result summary; check the full judgment)

### Inferences
- **Entity choice:**
  - Start as an individual or sole proprietor (PAN, bank current account, Udyam registration) only for a quick validation phase.
  - Move to an LLP (cheaper compliance) or private limited company (needed for equity investors or ESOPs) before applying for DPIIT recognition, KSUM grants or SIPP.
  - Assign the trade mark and the code IP to the entity on incorporation.
  - No source comparing costs or compliance was retrieved in this session.
- **GST:**
  - Below ₹20 lakh turnover you can operate without GST registration, including inter-state sales of services.
  - Register voluntarily if you want input tax credit, B2B hospital or college customers, or an LUT for exports, which needs registration.
  - The OIDAR classification mainly matters for foreign suppliers to Indian consumers. For an Indian supplier the main points are the 18% rate on domestic sales and zero-rated exports with an LUT.
  - UK VAT on digital services sold to UK consumers by non-UK businesses, and Gulf VAT, may apply from the first sale. Not researched.
  - Get a CA to confirm.
- **Government employee (high risk if ignored):**
  - A paid subscription business is "trade or business", not "occasional scientific work".
  - Get prior written sanction from your department, or have the business owned and run by someone else, recognising that "indirectly" is also covered.
  - Don't use work time, hospital equipment, PACS or scanner consoles to build or market it.
- **Private hospital employee (medium risk):** check moonlighting, conflict-of-interest, confidentiality and IP-assignment clauses in your appointment letter, and get written no-objection if unclear.

### Gaps
- No official startupindia.gov.in page confirming the ₹200 crore turnover limit and its date was retrieved.
- The current KSUM scheme document (2026) was not retrieved. Whether KSUM requires DPIIT recognition and a KSUM Unique ID is not confirmed here.
- No authoritative source on LLP versus private limited compliance costs.
- Income-tax treatment (presumptive taxation s.44ADA/44AD, 80-IAC) was not researched.
- UK VAT and UAE/Saudi VAT on digital education services were not researched.
- The current consolidated Kerala Conduct Rules text and the sanction procedure were not retrieved from an official Kerala Government source.

---

## 7. Consumer protection and e-commerce rules; "certificate", "accredited" and "CPD" claims

### Takeaway
Selling subscriptions from your own website makes you an e-commerce entity under the Consumer Protection (E-Commerce) Rules 2020. You must:
- display your legal name, address and customer-care details
- appoint and display a grievance officer, who must acknowledge complaints within 48 hours and resolve them within one month
- publish clear refund, cancellation and renewal terms

Avoid dark patterns. CCPA's 2023 guidelines cover subscription traps and silent auto-renewal, and CCPA fined ed-tech firm PhysicsWallah ₹5 lakh in June 2026 for dark patterns. Avoid misleading claims ("guaranteed job", "accredited"). Real third-party CPD endorsement is achievable in the UK through the College of Radiographers (CPD Now endorsement, about £278.50 + VAT per endorsement for two years for for-profit providers). No equivalent Indian accreditation route was found. Until you have one, call it a "certificate of completion".

### Cited Findings
- The Consumer Protection (E-Commerce) Rules 2020 were notified and in force from 23 July 2020. Every e-commerce entity must:
  - set up a grievance redressal mechanism
  - appoint a grievance officer and display their name, contact details and designation
  - acknowledge complaints within 48 hours and redress them within one month
  - disclose its legal name, office locations, website details and customer-care contact
  — [SS Rana](https://ssrana.in/articles/consumer-protection-e-commerce-rules-2020/); [Khaitan & Co PDF](https://khaitanco.com/sites/default/files/2020-08/Stricter%20Regulations%20on%20E-Commerce%20%E2%80%93%20The%20Consumer%20Protection%20(E-Commerce)%20Rules,%202020.pdf); [IndiaCorpLaw analysis](https://indiacorplaw.in/2020/08/25/consumer-protection-e-commerce-rules-2020-an-analysis/)
- Sellers must not falsely pose as consumers or post fake reviews, and must not refuse refunds contrary to their terms. Marketplace sellers' refund policies must be consistent with the marketplace's. The rules were later amended, with proposals in 2021. — [IndiaLaw summary](https://www.indialaw.in/guides/civil/consumer-protection-e-commerce-rules/); [Cyril Amarchand blog (2020)](https://corporate.cyrilamarchandblogs.com/2020/08/consumer-protection-e-commerce-rules-need-for-more-clarity/)
- CCPA Guidelines for Prevention and Regulation of Dark Patterns, effective 30 Nov 2023, list 13 practices, including subscription traps and silent conversion of free trials or auto-renewals. — [Mondaq (Dec 2023)](https://mondaq.com/india/consumer-trading-unfair-trading/1398262/ccpa-issues-guidelines-for-prevention-and-regulation-of-dark-patterns-2023-effective-30-november-2023); [Bar & Bench](https://www.barandbench.com/view-point/ccpa-steps-in-to-curb-dark-patterns)
- CCPA order against PhysicsWallah (1 June 2026): it found dark patterns at checkout and on "free" courses, including mandatory data collection to access "free" content (treated as a misleading advertisement under s.2(28) Consumer Protection Act 2019) and basket sneaking. Penalty ₹5,00,000. — [Mondaq: Dark patterns in ed-tech](https://www.mondaq.com/india/dodd-frank-consumer-protection-act/1799382/dark-patterns-in-ed-tech-ccpa-imposes-penalty-on-physicswallah); [IndiaLaw blog](https://www.indialaw.in/blog/competition-act/ccpa-dark-patterns-physicswallah/)
- UK College of Radiographers CPD endorsement (via CPD Now, awarded by its Approval and Accreditation Board):
  - endorsement shows content meets the professional body's CPD standards
  - it covers non-credit-bearing events and short courses that do *not* confer competence (courses intended to confer competence need "short course approval")
  - applications must match at least two core CPD Now outcomes
  - fees: NHS and education institutions £109 + VAT, for-profit businesses £278.50 + VAT, per endorsement for two years (another SCoR document gives £250 + VAT, so figures vary by date)
  — [College of Radiographers: CPD endorsement](https://www.collegeofradiographers.ac.uk/Education/Education-Approval/CPD-endorsement); [CoR fees](https://collegeofradiographers.ac.uk/education/education-approval/programme-approval/fees); [SoR: update on CPD Now endorsement](https://www.sor.org/news/import/update-on-cpd-now-endorsement-scheme)

### Inferences
**Website must-haves:**
- Terms of Service (governing law India, courts at Kerala; licence to use, not ownership; acceptable use; no sharing of logins)
- Privacy Notice (see Q4)
- Refund and Cancellation Policy: e.g. 7-day refund if under X% of content used, pro-rata or no refund after, clear renewal and cancel-anytime instructions, refunds processed in N days
- Grievance Officer block (name, email, phone, address; 48-hour acknowledgement, 1-month resolution)
- Contact page with legal entity name and address
- Medical, educational and non-affiliation disclaimers (Q1/Q2)
- GSTIN once registered
- Payment gateways (Razorpay etc.) usually require these pages before activation (not verified in this session).

**Subscriptions:** show price incl. GST, renewal date and cancellation path before payment. Send a reminder before auto-renewal or free-trial conversion. Allow one-click cancellation. Don't pre-tick add-ons. Don't gate a "free" demo behind unnecessary data collection (the PhysicsWallah findings).

**Claims:**
- OK: "certificate of completion", "practice MRI planning safely", "vendor-neutral".
- Don't say, unless true and documented: "accredited", "CPD-accredited", "approved by [council or university]", "recognised by the Kerala Paramedical Council", "guaranteed job abroad", "become MRI-certified", or "equivalent to clinical hours".
- Under s.2(28) CPA 2019 and the 2022 misleading-ad guidelines, such claims are the main enforcement risk: medium if made.
- For UK users: apply for CoR CPD Now endorsement of discrete modules. It is affordable, and it is a genuine "Endorsed by the College of Radiographers" claim, valid for two years.
- For Gulf users: DHA, DoH Abu Dhabi and Saudi SCFHS run CPD accreditation (not researched).
- For India: target endorsement or partnership by a recognised college, university or professional association (e.g. a state radiographers' association). No statutory CPD accreditation route was found under the NCAHP Act 2021.

### Gaps
- CCPA's "Guidelines for Prevention of Misleading Advertisement in Coaching Sector" (reportedly 2024) were not found in this session's searches. Whether they apply to ed-tech or skill courses is unverified.
- The text of the 2021+ amendments to the E-Commerce Rules was not retrieved.
- No information found on CPD accreditation under the National Commission for Allied and Healthcare Professions Act 2021 or by state councils.
- DHA, DoH and SCFHS CPD-provider accreditation requirements and costs were not researched.
- UK consumer law for digital content (Consumer Rights Act 2015, 14-day cancellation under the Consumer Contracts Regulations, and the DMCC Act 2024 subscription rules) was not researched. It is relevant before UK launch.
