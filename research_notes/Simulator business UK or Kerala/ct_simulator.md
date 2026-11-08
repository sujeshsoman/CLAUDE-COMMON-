# CT Scanner Console Simulator for Radiographer Training: Market and Technical Feasibility (as of 8 November 2026)

**How these notes were sourced.** Every page fetch failed. scanflo.io, www.aerb.gov.in and www.gov.uk all returned DNS "ENOTFOUND" in this session, even though they were said to be allowed. So **every figure below is [SEARCH]**: it comes from a search-result summary, not from reading the page. None is [LIVE]. Search summaries sometimes misread tables and dates. Where that looked likely, a caveat is given. Physics relationships that come from background knowledge, not from a source found in this session, are marked **[background knowledge]** and appear only under Inferences.

---

## 1. Competitors: who sells CT simulators for radiographer training, what they do, how they are delivered, and what they cost

### Takeaway
The CT-training simulator market is small and split into five groups:
- one UK desktop or VR incumbent (Shaderware TomoVR, which now appears to be marketed through RadSimTech)
- one US VR/desktop product sold inside US$1,700–2,500 course bundles (ScanLabCT)
- vendor-locked cloud consoles for each manufacturer's own customers (Siemens SmartSimulator)
- academic or free tools (CTSim from UCD and HVL, IAEA RadSimCT, jsctsim)
- open-source physics toolkits for developers (XCIST, TIGRE, gVirtualXray)

No competitor was found that is all of these at once: browser-only, priced for individual learners in India or the Gulf, and multi-vendor in console style. No ScanFlo CT product could be confirmed.

### Cited Findings

**Shaderware / RadSimTech: TomoVR (UK)**
- Shaderware is based in North East England. Its "Virtual Radiology" suite has four products: TomoVR (CT), ProjectionVR (X-ray), TechnicVR (X-ray physics and dose) and LectureVR [SEARCH] — [HealthySimulation vendor page](https://www.healthysimulation.com/vendors/shaderware/)
- TomoVR is described as an "advanced CT educational simulator". It lets learners "engage in patient positioning and operate complex CT consoles within a virtual environment" [SEARCH] — [HealthySimulation](https://www.healthysimulation.com/vendors/shaderware/)
- No search result confirmed whether TomoVR models topograms, dose (CTDIvol/DLP), contrast or kernels. The dose and image-quality physics content is described under TechnicVR, not TomoVR [SEARCH] — [HealthySimulation](https://www.healthysimulation.com/vendors/shaderware/)
- Pricing is quote-only: "contact us for pricing and demonstrations". No £ figure was found [SEARCH] — [shaderware.com](http://www.shaderware.com/)
- Licensing model [SEARCH] — [shaderware.com](http://www.shaderware.com/); [Shaderware student BYOD help](http://www.shaderware.com/help-student-byod.html):
  - a licence file activates the software
  - it runs for 15 days in evaluation mode without one
  - floating licences go through a licence server
  - there is a student bring-your-own-device (BYOD) route
- Scale: "hundreds of licences at well over 100 customer sites worldwide" [SEARCH] — [HealthySimulation](https://www.healthysimulation.com/vendors/shaderware/); [shaderware.com](http://www.shaderware.com/)
- A RadSimTech page is titled "TOMOVR: RadSimTech's VR for Radiologic Training (CT VR)". This suggests TomoVR is now marketed under the RadSimTech name in the UK. The relationship and the date were not confirmed [SEARCH] — [radsimtech.co.uk](https://radsimtech.co.uk/radiologic-training-with-tomovr/)
- A 2017 paper calls Shaderware "commercially available software". It describes a university-built alternative as "much more economical… albeit with reduced features and complexity". This signals that the commercial price is high enough for universities to build their own [SEARCH] — [Computers in Biology and Medicine 2017 (ScienceDirect)](https://www.sciencedirect.com/science/article/abs/pii/S0010482517303943)

**ScanLab: ScanLabCT (US), with ImagingU and MTMI bundles**
- ScanLabMR launched a CT simulator, ScanLabCT. It was reportedly released in December 2023 [SEARCH] — [AuntMinnie: "ScanLabMR launches CT simulator"](https://www.auntminnie.com/imaging-informatics/advanced-visualization/article/15659631/scanlabmr-launches-ct-simulator)
- Press coverage describes it as a "VR app [that] simulates imaging room, patient and CT unit to teach techs how to scan" [SEARCH] — [Radiology Business](https://radiologybusiness.com/topics/medical-imaging/computed-tomography-ct/vr-scanlabct-technician-training-tool)
- ScanLab markets one MRI and CT platform: "One Platform to Improve MRI & CT" [SEARCH] — [scanlabmr.com](https://scanlabmr.com/)
- **Price:** the ScanLab "CT Individual Cohorts" page lists "ScanLabCT + ImagingU" at **US$2,500**. That includes 6 months of ScanLabCT access, 1 year of the ImagingU Post-Primary Pathway course, a guided syllabus and one instructor office hour per week. The page is undated [SEARCH] — [scanlabmr.com/ct-individual-cohorts](https://scanlabmr.com/ct-individual-cohorts/)
- ImagingU's CT Post-Primary Pathway, with mock board tests and an optional ScanLabCT pairing, was announced on 12 July 2024 [SEARCH] — [AuntMinnie](https://www.auntminnie.com/radiology-education/article/15679508/imagingu-offers-new-bundled-ct-education-and-training-package)
- MTMI runs a CT training course for technologists that includes ScanLabCT practice. Its flyers give different figures, and the search summaries are not reliable on which tier each price belongs to:
  - 2025 flyer: **US$2,015**; another 2025 flyer table shows tuition of $2,970 ($2,825 early, $2,945 member)
  - 2026 flyer: **US$1,715**, with a "New Lower Price — $300 Reduction!" banner; the price table was garbled
  - 3 months of ScanLab practice after the course (2026), down from 5 months (2025)
  - MTMI membership is $39 a year
  - prerequisite is ARRT/NMTCB registration or state licensure

  [SEARCH] — [MTMI 2026 flyer](https://www.mtmi.net/sites/default/files/2025-12/CT_Training_Course_Flyer_for_2026_%282%29.pdf); [MTMI 2025 flyer](https://www.mtmi.net/sites/default/files/2025-03/CT_Training_Course_Flyer_for_2025.pdf); [MTMI course page](https://www.mtmi.net/course/ct-training-course-technologists)

**Siemens Healthineers: SmartSimulator and the Academy virtual CT courses**
- SmartSimulator is a cloud-based tool. Staff "virtually train and practice on a simulated version of a Siemens Healthineers medical device's interface" on a PC. The simulated products "are simulated on virtual machines in the cloud". Access needs a registered email address and an authenticator app. It is "only for trainings and for demonstration's purpose" [SEARCH] — [SmartSimulator / PEPconnect user manual](https://smartsimulator.siemens-healthineers.com/assets/files/PEPconnect_User_Manual.pdf); [Siemens SmartSimulator page](https://www.siemens-healthineers.com/services/customer-services/upskill-services/equipment-and-clinical-education/individual-education-and-practice/smartsimulator)
- The Siemens Healthineers Academy has a virtual "CT Essentials for the SOMATOM go" course. It is aimed at radiographers who are new to CT or starting on SOMATOM systems, and it uses "Siemens Healthineers CT simulators" with practical exercises [SEARCH] — [Siemens Healthineers Academy](https://academy.siemens-healthineers.com/en-us/ct-essentials-for-the-somatom-go-virtual)
- A UK course, "An introduction to CT on the GO – Virtual Training", covers the user interface, CT terminology, dose technologies and image reconstruction [SEARCH] — [Siemens Healthineers UK](https://siemens-healthineers.com/en-uk/education/siemens-healthineers-academy/medical-imaging/molecular-imaging/ct-for-nm-radiographers)
- Pricing: PEPconnect access is free with registration. The premium "PEPconnections" licence is priced through a sales representative. That statement comes from a Brazil-region page. No SmartSimulator price was found [SEARCH] — [Siemens PEPconnections (en-ae)](https://www.siemens-healthineers.com/en-ae/comprehensive-education-portfolio/pepconnect-and-pepconnections/pepconnections)
- A Siemens job advert recruits a "Clinical Education Specialist … for syngo Virtual Cockpit" in Forchheim. This shows Siemens investing in remote and virtual console operation and training [SEARCH] — [connexion-emploi job listing](https://connexion-emploi.com/en/o/clinical-education-specialist-m-f-diverse-for-syngo-virtual-cockpit-forchheim)

**Academic and free tools**
- **CTSim** (University College Dublin and Western Norway University of Applied Sciences, HVL):
  - a web-based simulator with freestyle and guided modes plus self-assessment
  - evaluated at the Optimax 2018 summer school, then in a BSc Radiography CT module
  - paper: Stowe et al., *Radiography* 2021
  - the rationale is that CT training is "limited in terms of practical experience with scan parameters due to patient safety and busy departments"
  - the software "has also been provided to other countries and institutions"

  [SEARCH] — [Teaching & Learning Ireland eprints: "CTSim: Changing teaching practice in radiography with simulation"](https://eprints.teachingandlearning.ie/id/eprint/5389/); [HVL project page](https://www.hvl.no/en/project/2051014/)
- **RadSimCT**: IAEA material describes it as "a web-based e-learning tool for CT to promote low dose examinations" (from a 2019 talk). Whether it is publicly available today was not confirmed [SEARCH] — [IAEA video page](https://www.iaea.org/resources/video/computer-tomography-simulator-an-e-learning-tool-to-promote-low-dose-examinations); [IAEA node](https://www.iaea.org/node/56567)
- **IAEA CT dose e-learning**: a "Radiation dose management in CT" course of 5 hours maximum and 11 modules, through NUCLEUS sign-in. A certificate needs 80% on the final quiz. A July 2025 free video series on CT optimisation is aimed mainly at medical physicists [SEARCH] — [IAEA node 36867](https://www.iaea.org/node/36867); [Devdiscourse, July 2025](https://www.devdiscourse.com/article/science-environment/3520818-iaea-rolls-out-global-video-training-series-to-optimize-ct-imaging-and-patient-safety)
- **jsctsim (JavaScript CT Simulator)**: a browser tool for CT image-quality demonstrations. It uses "a linear convolution scheme that allows fast generation of simulated images" and reconstructs with "a standard clinical filtered back projection algorithm". Its author warns it "cannot be used in estimating scanner performance or in quantitative optimization" [SEARCH] — [ECR 2015 EPOS poster C-1878](https://epos.myesr.org/poster/esr/ecr2015/C-1878)
- **CTSim (Kansas State University)** is an interactive program that teaches back-projection principles [SEARCH] — [KSU Physics CTSim](https://web.phys.ksu.edu/mmmm/software/CTSim)

**VR and other vendors**
- **Virtual Medical Coaching** (Christchurch, New Zealand) sells a VR radiography suite. Its CT, MRI and mammography modules were listed as "in development". The sources are old: a 2017 AuntMinnie article and a Vive blog post. No CT launch or CT price was found [SEARCH] — [HealthySimulation](https://www.healthysimulation.com/virtual-medical-coaching-provides-vr-radiographic-simulation-training/); [AuntMinnie 2017](https://cdn.auntminnie.com/imaging-informatics/advanced-visualization/article/15616807/virtual-coaching-takes-on-x-ray-training); [Vive blog](https://blog.vive.com/us/schools-of-the-future-using-vive-to-provide-complete-medical-imaging-education-in-vr/)
- **Scopic Software**, a development agency, has an "MRI and CT Simulators" portfolio entry. This suggests at least one client paid for a custom-built MRI and CT simulator. Client and price not found [SEARCH] — [Scopic portfolio](https://scopicsoftware.com/portfolio/mri-ct-simulators/)
- **ONE Simulation** (India) calls itself "India's leading hub for high-fidelity medical simulation training" and mentions CT scan training on its YouTube channel. No product details were found [SEARCH] — [YouTube channel mirror](https://invidious.tiekoetter.com/channel/UCPiXHwIjYN-pH-e1_rl-Aiw/posts)
- A German report on training says "Einfach mal Knöpfe am CT ausprobieren" ("just try out buttons on the CT"). This shows console simulators are being used in German technologist (MTR) education [SEARCH] — [MTA Dialog 2023](https://www.mta-dialog.de/artikel/aus-und-weiterbildung-2023-einfach-mal-knoepfe-am-ct-ausprobieren)

**Open-source physics toolkits, with licences**
- **XCIST / CatSim** (`gecatsim` on PyPI) is a physics-based simulator in Python and C/C++, with digital phantoms, the CatSim simulator and reconstruction. The licence type was not confirmed in search results [SEARCH] — [github.com/xcist/main](https://github.com/xcist/main); [PyPI gecatsim](https://pypi.org/project/gecatsim)
- **TIGRE** (CERN) is a GPU tomographic reconstruction toolbox under the **BSD licence**, with a citation requested [SEARCH] — [github.com/CERN/TIGRE](https://github.com/CERN/TIGRE)
- **gVirtualXray (gVXR)** is under the **BSD 3-Clause** licence. Its WebCT web GUI needs an NVIDIA GPU on the host for reconstruction, so it is not a pure browser client [SEARCH] — [PyPI gVXR](https://pypi.org/project/gVXR/); [WebCT post](https://gvirtualxray.sourceforge.io/applications/post-2025a)

**ScanFlo (India)**
- A search for a ScanFlo CT simulator returned nothing, and the scanflo.io fetch failed with a DNS error. **No ScanFlo CT product could be confirmed.** [no result] — search attempted; [scanflo.io fetch blocked]

**A naming collision to be aware of**
- In India, "CT simulator" commonly means a **radiotherapy CT-simulation scanner**, which is real hardware. For example, a 2026 Tata Memorial Centre tender asks for a "CT Scan 128 Slice Simulator Wide Bore Flat Bed" [SEARCH] — [Tata Memorial Centre tender notice](https://docs.infralens.in/nit/2026_TMC_908208_1/Tendernotice_1.pdf)

### Inferences
- The only clearly priced comparable is ScanLabCT, at about US$1,700–2,500 including a course and 3–6 months of access. That price is pitched at US technologists earning US salaries, which leaves a large gap for a ₹/AED/£-priced, browser-only product.
- Shaderware and TomoVR hold UK university relationships. If the founder sells to UK HEIs, TomoVR is the incumbent, and the pitch would be "browser, no install, per-student pricing, cheaper".
- Siemens SmartSimulator is a real Siemens console in the cloud, but it is tied to Siemens customers and to one manufacturer. Indian and Gulf radiographers working on GE scanners (the largest Indian installed base; see section 2) have no equivalent free vendor tool that turned up in these searches.
- The free academic tools (CTSim, RadSimCT, jsctsim) teach parameter-to-image relationships. They do not appear to simulate a full exam workflow (patient set-up → scout → plan → contrast → recon → dose report) with exam-prep framing. That workflow is the gap a commercial product can fill.
- The brand should say "CT *scanning* simulator" or "CT console trainer", not "CT simulator", in India. That avoids confusion with radiotherapy CT-sim hardware in search results and in procurement.

### Gaps
- TomoVR's actual feature list (topogram, AEC/tube-current modulation, dose display, contrast, kernels), its price and its UK customer list were not found. Shaderware/RadSimTech pages could not be fetched.
- ScanFlo: whether it has or plans a CT module is unknown, because the fetch was blocked.
- GE HealthCare, Philips and Canon CT training simulators were not found in searches. Each likely has its own customer e-learning and console emulators, but that is not verified.
- Medality and "Virtual Medical Coaching CT": no current product information found.
- XCIST licence: not confirmed (check the LICENSE file on GitHub).

---

## 2. Demand: CT vs MRI in India (and Kerala), the UK and the Gulf, plus regulatory training requirements (AERB, IR(ME)R, Gulf licensing)

### Takeaway
On every indicator found, CT is the larger modality: installed units, scan volume and job demand. The ratio is roughly 1.7× MRI by monthly scan volume in England (2026), and about 2–3× by installed units in India. The ratio in Kerala hospitals looks higher. A medical-college data point shows 85 CT scans a day against 25 MRI.

Regulators require **qualified, experienced** CT operators: AERB in India and Schedule 3 training under IR(ME)R in the UK. Nothing found says simulation counts toward those requirements. A no-radiation simulator therefore fits as **preparation and CPD**, not as a replacement for supervised clinical CT hours.

The Gulf licensing exams have explicit CT content. Saudi Arabia (SCFHS) even has a separate CT clinical promotion exam.

### Cited Findings

**India: installed base (no authoritative national total was found)**
- India has "fewer than 5,000 MRI scanners", about **3.5 per million**, against about 38 per million in the US. Source: Hyperfine press release, May 2024; a vendor figure [SEARCH] — [BusinessWire / Hyperfine, 28 May 2024](https://www.businesswire.com/news/home/20240528157535/en)
- One source puts the MRI installed base at about **4,800 units, "3X lower than CT"**. The source is undated [SEARCH] — [BioSpectrum India PDF](https://www.biospectrumindia.com/article/pdf/23424)
- The Competition Commission of India (CCI) market study of 20 August 2024 used AERB-portal data on installed CT machines:
  - GE holds about **44.8%** of installed CT machines and Siemens about **31.3%**
  - the top 5 OEMs (GE, Siemens, Canon/Toshiba, Philips, Fujifilm/Hitachi) hold about 98% of cumulative installed CT units
  - MRI shares were given by revenue (top 5 above 91%)
  - the national CT total sits in Table 6 of the study but did not appear in search snippets

  [SEARCH] — [CCI market study PDF](https://www.cci.gov.in/public/images/marketstudie/en/market-study-of-diagnostic-medical-imaging-equipment-industry-in-india1724145632.pdf); [Lexology summary](https://www.lexology.com/library/detail.aspx?g=5063278c-1c3b-4aa1-a059-9ec34e00323b)
- A secondary site says the CCI report gives GE **3,671 installed CT scanners** in India. This was not checked against the CCI table [SEARCH] — [Research Nester](https://www.researchnester.com/reports/computed-tomography-market/8338)
- Other figures that conflict or are low quality [SEARCH]:
  - "over 15,000 CT units installed nationwide", a refurbished-equipment vendor blog with no source — [Sunrays Medical 2026](https://www.sunraysmedical.com/guide/refurbished-ct-scanner-buying-guide-india-2026)
  - "3,500 CT scanners installed at hospitals in India", an old estimate from a GE launch article about a decade ago — [AuntMinnie](https://www.auntminnie.com/clinical-news/ct/article/15612048/ge-launches-ct-scanner-made-in-india)
- Annual sales of new CT units in India: **1,245 units (₹1,680 crore) in 2022** and **880 units (₹1,430 crore) in 2024** [SEARCH] — [Medical Buyer](https://medicalbuyer.co.in/a-steady-ct-scanners-market-ahead/)

**Kerala**
- Alappuzha Government Medical College Hospital averaged **85 CT scans a day against 25 MRI scans a day** (2022 report) [SEARCH] — [Onmanorama, 26 April 2022](https://www.onmanorama.com/news/kerala/2022/04/26/alappuzha-medical-college-fraud.html)
- Kottayam Medical College had one CT and one MRI in 2025, with one CT out of service. It was due to have two CT and two MRI [SEARCH] — [search summary of Kottayam MCH report (Deccan Herald/Medical Dialogues result set)](https://education.medicaldialogues.in/kerala-state-government-allots-10-crore-to-gmc-ernakulam)
- Parippally Government Medical College Hospital installed a ₹15-crore MRI on 3 November 2026 [SEARCH] — [Onmanorama, 3 November 2026](https://www.onmanorama.com/news/kerala/2026/11/03/advanced-mri-facility-installed-at-parippally-government-medical-college-hospital.html)
- A multicentre Kerala CT dose study across seven hospitals said India had no national or regional CT DRLs at the time (2018) [SEARCH] — [IJRI 2018 (Thieme)](https://www.thieme-connect.com/products/ejournals/html/10.4103/ijri.IJRI_394_17)
- No statewide count of CT or MRI units in Kerala was found.

**UK (England)**
- The NHS England Diagnostic Imaging Dataset (statistical release, 23 July 2026) reports about **50.8 million imaging tests** in England from April 2025 to March 2026. March 2026 had 4.12 million tests, of which **CT ≈ 0.71 million and MRI ≈ 0.41 million**. These look like monthly figures for March 2026; the search summary was ambiguous [SEARCH] — [NHS England Statistical Release, 23 July 2026](https://www.england.nhs.uk/statistics/wp-content/uploads/sites/2/2026/07/Statistical-Release-23rd-July-2026.pdf)
- Earlier releases give a similar ratio: CT 0.65m against MRI 0.38m (June 2026 release), and CT 0.67m against MRI 0.38m (July 2024) [SEARCH] — [Statistical Release 18 June 2026](https://www.england.nhs.uk/statistics/wp-content/uploads/sites/2/2026/06/Statistical-Release-18th-June-2026.pdf); [Statistical Release 21 November 2024](https://www.england.nhs.uk/statistics/wp-content/uploads/sites/2/2024/11/Statistical-Release-21st-November-2024-2.pdf)
- Equipment counts are held in the National Imaging Data Collection (NIDC). No UK CT scanner count was retrieved [SEARCH] — [NHS England DID page](https://www.england.nhs.uk/statistics/statistical-work-areas/diagnostic-imaging-dataset/)

**Gulf: licensing exams and jobs**
- The SCFHS (Saudi) Radiology Technology Residency **promotion blueprint (R2)** has CT-specific weights [SEARCH]:
  - Advanced CT physics: **30%**
  - Advanced CT techniques, CT image quality, and cross-sectional anatomy and pathology: up to 20% each
  - Post-processing: **10%**
  - Note: this is a residency promotion exam, not the basic licensing test.

  — [SCFHS R1/R2 blueprint (March 2025)](https://www.scfhs.org.sa/sites/default/files/2025-03/Radiology%20Technology%20Residency%20Promotion%20Exam%20Blueprint%2024-27%20-%20R1%20and%20R2.pdf)
- SCFHS also publishes a separate **"CT Clinical Promotion Exam Blueprint R3"**, dated June 2026. This shows a formal CT specialisation track in Saudi Arabia [SEARCH] — [SCFHS CT Clinical Promotion Blueprint R3](https://scfhs.org.sa/sites/default/files/2026-06/CT%20Clinical%20Promotion%20Exam%20Blueprint%20R3.pdf)
- Oman (OMSB) radiographer exam blueprint: **CT 10%** [SEARCH] — [OMSB Radiographer blueprint](https://omsb.gov.om/ContentFiles/32.%20RadiographerYYYY08DD1208SS.pdf)
- DHA radiographer exam: a third-party exam-prep site gives the exam code as "RAD5152" via Prometric. It gives the pass mark inconsistently (55% and 60%). No official DHA blueprint with a CT percentage was found. Unverified [SEARCH] — [Neelim exam prep](https://neelim.com/exam-prep/radiographer)
- A GCC licensing guide says "CT technologists are in very high demand across the GCC", with 24/7 CT coverage in most hospitals. It says multi-slice CT, CT angiography and cardiac CT skills are "highly valued", and gives a Saudi salary range of SAR 6,000–14,000 a month. This is consultancy marketing [SEARCH] — [Neelim blog: radiographer licence GCC](https://neelim.com/blog/radiographer-license-gcc)
- A Dubai job for a "Radiology Technologist CT and MRI" pays **AED 10,000–12,000 a month**. It requires a DHA licence and hands-on CT and MRI experience [SEARCH] — [Careerjet UAE listing](https://www.careerjet.ae/jobad/ae669b10da3a58d2b3a37f261f129bf4d6)
- GulfTalent listed 43 "CT scan technologist" jobs at the time of the search [SEARCH] — [GulfTalent](https://www.gulftalent.com/jobs/title/ct-scan-technologist)

**AERB (India): CT operator, RSO and licensing**
- All diagnostic radiology facility licences must go through AERB's **eLORA** portal (AERB announcement, 10 September 2014). CT units are on the consent list [SEARCH] — [PMC: eLORA in Armed Forces Hospitals](https://pmc.ncbi.nlm.nih.gov/articles/PMC5221348/); [AERB consenting process](https://www.aerb.gov.in/english/consenting-process-in-radiation-facilities)
- CT and interventional radiology facilities need a **Radiological Safety Officer (RSO)** as well as an operator and a medical practitioner. AERB's training module gives two RSO routes for CT/IR [SEARCH]:
  - a radiologist, or an X-ray technologist with recognised training and **3 years of CT/IR work experience**
  - an existing AERB-approved RSO from a radiotherapy or nuclear medicine facility, by undertaking

  — [AERB Radiation Safety Training Module: Regulatory Requirements for Diagnostic Radiology Practice](https://aerb.gov.in/images/PDF/DiagnosticRadiology/REGULATORY-REQUIREMENTS-FOR-DIAGNOSTIC-RADIOLOGY-PRACTICE.pdf); [PMC5221348](https://pmc.ncbi.nlm.nih.gov/articles/PMC5221348/)
- RSOs must be approved by the competent authority [SEARCH] — [AERB qualifications of personnel PDF](https://mgw3.aerb.gov.in/images/PDF/image/qualificationsofpersonnel.pdf)
- Measured CT parameters are checked against AERB tolerances: "expected ±20% and maximum ±40%" [SEARCH] — [Kerala CT dose study (IJRR)](https://ijrr.com/article-1-1819-en.html)

**IR(ME)R 2017 (UK): operator training**
- **Schedule 3** of IR(ME)R 2017 sets out the "adequate training" required for practitioners and operators [SEARCH] — [legislation.gov.uk, SI 2017/1322 Schedule 3](https://www.legislation.gov.uk/uksi/2017/1322/schedule/3/made)
- Training must match the operator's own functions and area of practice. A radiographer can be both IR(ME)R practitioner and operator [SEARCH] — [SoR: The Diagnostic Radiographer as the entitled IR(ME)R practitioner](https://www.sor.org/learning-advice/Professional-body-guidance-and-publications/Documents-and-publications/Policy-Guidance-Document-Library/The-Diagnostic-Radiographer-as-the-entitled-IR-(1)); [SoR IR(ME)R practitioner guidance 2018](https://www.sor.org/getmedia/1a74aac9-503d-44d3-a075-7479ee30acee/20180125_final_scor_irmer_practitioner_guidance_alt_2.pdf)
- Students who do not yet meet Schedule 3 work under supervision under Regulation 17(3) [SEARCH] — [Leeds clinical supervision document 2024–25](https://placements.leeds.ac.uk/wp-content/uploads/sites/58/2024/11/Clinical-Supervision-Document-2024-2025-1.docx)
- e-IRMER e-learning modules (e-LfH) are mapped to Schedule 3 topics [SEARCH] — [e-LfH](https://e-lfh.org.uk/?p=1695)
- IPEM's sample operator training record has separate sign-off by the trainer and by the duty holder [SEARCH] — [IPEM sample training record](https://ipem.ac.uk/media/302c4p3o/ionisi-1.pdf)
- A 2024 IR(ME)R amendment exists alongside the 2017 regulations [SEARCH] — [SDCEP radiation protection training](https://www.psm.sdcep.org.uk/topics/radiation-protection/training)
- Simulation in IR(ME)R contexts: a Welsh action plan mentions an "operator assessment form for CT and simulators", in radiotherapy [SEARCH] — [HIW action plan, Abertawe Bro Morgannwg / Singleton](https://www.hiw.org.uk/system/files/2023-06/Abertawe%2520Bro%2520Morgannwg%2520UHB%2520-%2520Singleton%2520radiotherapy%2520Services%2520-%2520Action%2520Plan.pdf)

**Education evidence that CT simulation is used and valued**
- Lee et al., *Radiography* 2020: 62 third-year students on high-fidelity CT simulation (Western Sydney University). There was no significant difference in CT knowledge between the two delivery models [SEARCH] — [Western Sydney University research portal](https://researchers.westernsydney.edu.au/en/publications/computed-tomography-learning-via-high-fidelity-simulation-for-und/)
- A 2024 study (*Interactive Learning Environments*, Monash) surveyed 60 radiography students after a 5-hour virtual CT simulator session. Students felt their learning transferred to practice more when the placement scanner **matched the simulator** [SEARCH] — [Monash research portal](https://research.monash.edu/en/publications/transferability-of-learning-from-computed-tomography-simulation-i/)
- A 2020 study of remote-access CT simulation before a 4-week placement found mixed satisfaction but clear learning outcomes [SEARCH] — [BL catalogue record](https://eld.bl.uk/catalog/100160321949_0x000001)
- A narrative review exists on immersive VR for pre-registration CT education of radiographers [SEARCH] — [Monash research portal](https://research.monash.edu/en/publications/immersive-virtual-reality-for-pre-registration-computed-tomograph/)
- The University of Cumbria is giving diagnostic radiography students immersive training [SEARCH] — [University of Cumbria news](https://news.cumbria.ac.uk/news/the-university-of-cumbria-empowers-the-next-generation-of-diagnostic-radiographers-with-immersive-training-opportunities)

### Inferences
- **CT is the bigger addressable skill.** England runs about 1.7 CT scans per MRI scan. India's installed CT base is plausibly 2–3× MRI: ~4,800–5,000 MRI against "3X" CT. Kerala medical-college throughput is about 3.4 CT scans per MRI scan (Alappuzha). On demand alone, a CT simulator addresses more working radiographers than the MRI one.
- **Estimated size of India's registered CT base:** if GE's 3,671 units (secondary source) and the 44.8% share (CCI) are both right, India has about **8,200 AERB-registered CT units** (3,671 ÷ 0.448). That sits between the old 3,500 and the unsourced 15,000. Treat it as an estimate until Table 6 of the CCI study is read.
- **Why CT practice is hard to get in India:** the AERB rules on qualified operators and RSOs, plus the 3-year CT experience requirement for the RSO route, mean juniors get little hands-on control of the console. That supports a "practise before you touch the real scanner" pitch. The product must not claim AERB recognition, accreditation or contribution to licensing hours. No source shows AERB accepting simulator time.
- **UK positioning:** IR(ME)R Schedule 3 asks for training that is relevant and documented. A simulator can support it as structured, documented pre-clinical training and CPD, for example by exporting a certificate or log for the employer's training record. It does not replace employer-signed competency. Nothing found shows a UK regulator or employer formally "accepting" simulation for CT operator entitlement.
- **Gulf positioning:** the SCFHS CT-specific promotion blueprints (CT physics 30%, image quality, post-processing 10%) map directly onto simulator content. That supports a "Gulf exam + CT skills" package. The DHA weighting is unconfirmed.
- **Indian radiographers seeking Gulf jobs:** Dubai employers advertise roles that ask for "CT and MRI" experience. A CT+MRI bundle matches the job adverts better than MRI alone.

### Gaps
- No authoritative national CT unit total for India. It is in Table 6 of the CCI August 2024 study and on the AERB portal, neither of which could be fetched.
- No Kerala statewide CT or MRI count.
- No CT technologist workforce numbers for India (e.g., MRIT/BSc graduates) or UK (CT-specialised radiographers) were found.
- AERB's exact **CT operator** qualification wording in the current Safety Code (AERB/RF-MED/SC-3) was not read. Only RSO routes were found.
- No source on whether AERB, HCPC or SoR formally recognise simulation hours.
- No DHA or QCHP blueprint with a CT percentage was found.

---

## 3. What to simulate: educator and learner needs for a CT console trainer

### Takeaway
The published curricula and exams emphasise three areas:
- CT physics and dose
- image quality and the trade-offs between parameters
- reconstruction and post-processing

Published CT simulators justify themselves by giving trainees safe practice with **scan parameters**. Studies also show that learning transfers better when the console looks like the one students meet on placement. An MVP should therefore centre on a realistic, vendor-neutral console workflow with live dose and noise feedback and DRL comparison. Contrast timing and emergency protocols come next.

### Cited Findings
- Siemens' introductory CT course covers the user interface, CT terminology, **dose technologies** and **image reconstruction** [SEARCH] — [Siemens Healthineers UK "CT on the GO – Virtual Training"](https://siemens-healthineers.com/en-uk/education/siemens-healthineers-academy/medical-imaging/molecular-imaging/ct-for-nm-radiographers)
- SCFHS CT promotion blueprint domains: **advanced CT physics (30%)**, advanced CT techniques, CT image quality, cross-sectional anatomy and pathology, and **post-processing (10%)** [SEARCH] — [SCFHS R2 blueprint](https://www.scfhs.org.sa/sites/default/files/2025-03/Radiology%20Technology%20Residency%20Promotion%20Exam%20Blueprint%2024-27%20-%20R1%20and%20R2.pdf)
- GCC employers value multi-slice CT, **CT angiography** and **cardiac CT** skills [SEARCH] — [Neelim GCC guide](https://neelim.com/blog/radiographer-license-gcc)
- CTSim was built because CT training is "limited in terms of practical experience with **scan parameters** due to patient safety and busy departments". It offers freestyle and guided modes plus self-assessment [SEARCH] — [CTSim eprint](https://eprints.teachingandlearning.ie/id/eprint/5389/)
- Students saw better transfer to practice when the simulator matched their placement scanner [SEARCH] — [Monash 2024](https://research.monash.edu/en/publications/transferability-of-learning-from-computed-tomography-simulation-i/)
- CTDIvol and DLP are the quantities used to set CT DRLs, and SSDE may help optimisation [SEARCH] — [gov.uk NDRL guidance](https://gov.uk/government/publications/diagnostic-radiology-national-diagnostic-reference-levels-ndrls/national-diagnostic-reference-levels-ndrls)
- **UK NDRL values (older version, possibly out of date):** the gov.uk page titled "National Diagnostic Reference Levels: 22 January 2016 to 14 November 2018" lists adult acute stroke head CT as CTDIvol 80 mGy (posterior fossa) and 60 mGy (cerebrum and whole brain), with **DLP 970 mGy·cm**. These derive from PHE-CRCE-013 (2011 review). The current UKHSA values were not retrieved [SEARCH] — [gov.uk NDRLs](https://gov.uk/government/publications/diagnostic-radiology-national-diagnostic-reference-levels-ndrls/national-diagnostic-reference-levels-ndrls)
- **India regional DRL benchmarks (no national DRLs at the time):** the Kerala 2018 multicentre study across 7 hospitals gives 75th percentiles [SEARCH] — [IJRI 2018](https://www.thieme-connect.com/products/ejournals/html/10.4103/ijri.IJRI_394_17):

  | Exam (single phase) | CTDIvol (mGy) | DLP (mGy·cm) | Effective dose (mSv) |
  |---|---|---|---|
  | Head | 68.1 | 1,120 | 2.1 |
  | Chest | 23.4 | 916.7 | 13.38 |
  | Abdomen | 10.6 | 509.3 | 7.7 |

- **South India 2016 proposed DRLs** [SEARCH] — [PMC6038221](https://pmc.ncbi.nlm.nih.gov/articles/PMC6038221):

  | Exam | CTDIvol (mGy) | DLP (mGy·cm) |
  |---|---|---|
  | Head | 47 | 1,041 |
  | Chest | 10 | 445 |
  | Abdomen | 12 | 550 |

- IAEA CT dose e-learning has dedicated modules on optimising dose for **children and pregnant patients** [SEARCH] — [IAEA](https://www.iaea.org/node/36867)

### Inferences
These come from the founder-radiographer context, standard CT practice and the sources above. Not individually sourced. Suggested scope:

**MVP: one "free demo scan" plus core paid content**
1. Patient set-up: supine or prone, head- or feet-first, arms up, isocentre centring with laser lights. Show that **off-centring changes AEC tube-current modulation and dose**, and adds noise or bowtie mismatch. This is a common real-world error and a strong teaching moment.
2. Scout/topogram: AP and lateral, kV and mA for the scout, scout direction. It drives AEC.
3. Planning the scan range on the scout: start and end lines, FOV/DFOV, gantry tilt for head.
4. Protocol selection with editable kV (80/100/120/140), reference mAs or noise index (AEC), rotation time, pitch, collimation and slice thickness.
5. Live dose readout: CTDIvol and DLP, compared with UK NDRL or Indian regional benchmarks, with a DRL-exceeded warning.
6. Reconstruction: slice thickness and interval, soft-tissue/lung/bone kernels, windowing presets (brain, subdural, stroke, lung, mediastinum, bone, liver), MPR.
7. Artefacts on demand: motion, metal (streaks), beam hardening (posterior fossa or shoulders), partial volume, ring, truncation from a patient outside the FOV.

**Phase 2 paid packages**
- Contrast: injector rate and volume, bolus tracking with an ROI on the aorta or pulmonary trunk and a HU trigger threshold, scan delays for arterial, portal-venous and delayed phases, test bolus.
- Emergency protocols:
  - stroke CT, CTA and CT perfusion (link to the UK stroke DRL above)
  - trauma whole-body CT
  - CTPA
  - CT KUB at low dose
- Patient safety:
  - eGFR/creatinine check before contrast
  - metformin, allergy and pregnancy screening
  - contrast-reaction scenarios (recognise and escalate)
  - paediatric dose, as stressed by the IAEA modules
- Exam-prep mode mapped to SCFHS/OMSB CT domains: physics, image quality, post-processing, cross-sectional anatomy.

**Console look**
- Studies show transfer depends on similarity to the placement scanner.
- India's base is mostly GE (~45%) and Siemens (~31%).
- So offer a vendor-neutral UI with optional "GE-like" and "Siemens-like" terminology. Examples: noise index against reference mAs/CARE Dose, scout against topogram, kernel names. Do not copy trademarked UI art.

### Gaps
- No primary educator-needs survey for CT simulation in India or the Gulf was found.
- Current UK NDRLs (latest UKHSA update) and any current AERB national CT DRLs were not retrieved, because the gov.uk and aerb.gov.in fetches were blocked.
- No source on RCR or ESUR contrast guidance was fetched in this session.

---

## 4. Technical approach: building CT in the browser on the same procedural-phantom approach as the MRI prototype

### Takeaway
A browser CT simulator is technically easier than the MRI one in physics terms. The image is essentially a HU map plus noise, blur, windowing and artefacts. A teaching-grade product can use **image-space approximations** for real-time feedback, the approach jsctsim takes (a linear convolution scheme with FBP). True forward projection and FBP in JavaScript or WebGL can be kept for an optional "physics mode", for artefacts that need it (metal streaks, beam hardening, truncation).

Permissive open-source references exist: TIGRE (BSD) and gVirtualXray (BSD-3). TCIA data is mostly CC BY. XCAT phantoms need a licence, so the existing procedural phantom remains the commercial-safe default.

### Cited Findings
- jsctsim is a JavaScript browser CT simulator. It generates images fast with "a linear convolution scheme" and reconstructs with "a standard clinical filtered back projection algorithm". It is intended for teaching, not quantitative optimisation [SEARCH] — [ECR 2015 EPOS C-1878](https://epos.myesr.org/poster/esr/ecr2015/C-1878)
- A purely web-based, open-access application teaches tomographic reconstruction by FBP and iterative methods [SEARCH] — [PMC4305051](https://pmc.ncbi.nlm.nih.gov/articles/PMC4305051)
- ctxray-reconstruction runs CT reconstruction in the browser via **WebAssembly** (Raylib and Emscripten), using the iterative Kaczmarz/ART method [SEARCH] — [ctxray-reconstruction repo mirror](https://gh.r-mj.com/SMFloris/ctxray-reconstruction)
- WebCT, from gVirtualXray, gives a web GUI for virtual CT scans. Hosting it needs an NVIDIA GPU, so the reconstruction is server-side [SEARCH] — [gVirtualXray WebCT](https://gvirtualxray.sourceforge.io/applications/post-2025a)
- TIGRE is under the BSD licence and gVXR under BSD 3-Clause [SEARCH] — [CERN/TIGRE](https://github.com/CERN/TIGRE); [PyPI gVXR](https://pypi.org/project/gVXR/)
- XCIST/CatSim is physics-based (Python and C/C++) and includes digital phantoms and reconstruction. Licence not confirmed [SEARCH] — [xcist/main](https://github.com/xcist/main)
- **TCIA data licensing:** most data are free to "use for commercial, scientific and educational purposes" under CC BY 3.0 or 4.0. A few collections carry non-commercial terms, and collection-specific terms take precedence [SEARCH] — [TCIA Data Usage Policy](https://wiki.cancerimagingarchive.net/x/c4hF)
- **XCAT (Duke):** the XCAT Brain Phantom lists an academic lab licence at **US$400 for the first year and US$200 a year after**. Commercial terms are by request [SEARCH] — [Duke CVIT XCAT Brain Phantom](https://cvit.duke.edu/resource/xcat-brain-phantom/); [XCAT 3.0 library](https://cvit.duke.edu/resource/xcat-3-0-personalized-phantom-library/)
- The authors of a 2017 study built their own X-ray simulator, "much more economical" than commercial alternatives "albeit with reduced features" [SEARCH] — [ScienceDirect 2017](https://www.sciencedirect.com/science/article/abs/pii/S0010482517303943)

### Inferences
The physics in this section is **[background knowledge]**, not from sources fetched this session. Check it against a CT physics text such as Bushberg or the IAEA handbook.

**Rendering pipeline, reusing the MRI prototype's procedural 3D phantom**
- Replace the MRI tissue parameters (T1, T2, PD) with **HU and an energy-dependent attenuation table per tissue**. Approximate HU values:

  | Tissue | HU |
  |---|---|
  | Air | −1000 |
  | Lung | −850 to −700 |
  | Fat | −100 |
  | Water | 0 |
  | Soft tissue | 30–60 |
  | Blood (unenhanced) | ~40 |
  | Bone | 400–1000+ |
  | Iodine-enhanced vessels | phase-dependent, 150–400 |

- Iodine contrast HU should **rise at lower kV**, because the measurement sits closer to iodine's K-edge. That is the teaching point for using 80–100 kV in CTA.

**Noise model**
- Image noise σ ∝ 1/√(mAs_eff × slice thickness).
- σ also depends on kV and patient size (attenuation path length), and on the kernel: sharp kernels raise noise.
- Effective mAs = mA × rotation time ÷ pitch.

**Dose model**
- CTDIvol = CTDIw ÷ pitch.
- CTDIw scales roughly with mAs and steeply with kV (approximately kV^2.5–3).
- DLP = CTDIvol × scan length.
- Effective dose ≈ DLP × a region-specific k-factor.
- Use a lookup table of CTDIw per 100 mAs at each kV, for the 16 cm head and 32 cm body phantoms.
- AEC: modulate mA along z (and angularly) from the scout's attenuation profile. Off-centring changes the apparent patient size on the scout, which changes the mA. This is easy to compute from the procedural phantom.

**Image-space vs projection approach**
- **Image-space (recommended for the MVP).** Render the HU slice from the procedural phantom, then convolve with a kernel PSF (soft or sharp), add correlated noise (filtered Gaussian), add partial-volume averaging across slice thickness, then apply window/level. This runs at interactive rates in plain JS or WebGL2 fragment shaders, so it fits a single offline HTML file like the MRI prototype.
- **Projection-domain mode (optional).** Compute a 2D parallel- or fan-beam sinogram with a ray-march in a WebGL2 shader, add Poisson noise, then FBP (ramp/Shepp-Logan filter plus backprojection on the GPU). A 512² image with about 720 views is feasible on the GPU in a browser. This mode gives **physically emergent artefacts**: metal streaks from photon starvation, beam hardening (from a polychromatic spectrum approximation), ring artefacts (from a bad detector channel) and truncation. The image-space mode can only fake these.
- **Motion** can be simulated by moving the phantom between view angles in projection mode, or by blur and doubling in image-space mode.
- **Bolus tracking:** a time-attenuation curve per vessel (a gamma-variate) drives the HU of enhanced tissues. A monitoring ROI triggers when it crosses the threshold the user sets. This is a cheap 1D model.

**Data and licensing**
- Keep the procedural phantom as the default, because it has no licensing risk.
- TCIA CC BY CT volumes could supply "real anatomy" cases, with attribution. Each collection's licence must be checked, and the data must be de-identified (TCIA already does this). Note that real volumes are already reconstructed images with fixed noise, so changing kV or mAs on them needs noise insertion and HU remapping. This is feasible as an image-space approximation.
- XCAT needs a paid licence and commercial terms by request. It is not needed for an MVP.

**Effort compared with the MRI prototype**
- The CT physics core is likely **smaller** than MRI's: no k-space, sequence timing or contrast-equation zoo.
- The work concentrates in three areas:
  - console UX (scout planning, protocol tree, injector, recon queue)
  - the dose and AEC tables
  - artefact realism
- If the MRI prototype's phantom, viewer, window/level, MPR and UI shell are reused, a CT MVP (head, chest and abdomen exams; dose readout; kernels and windows; 3–4 artefacts; one free demo scan) is plausibly a fraction of the MRI build effort. This is a rough estimate, not measured.
- Contrast phases, bolus tracking and projection-mode artefacts are the expensive add-ons.

### Gaps
- No benchmark was found for WebGL FBP performance on low-end Android phones, the likely device for many Indian learners.
- No validated open CTDIw-per-kV lookup table was retrieved. Typical manufacturer CTDI tables or published phantom measurements would be needed.
- The XCIST licence and commercial XCAT pricing were not confirmed.

---

## 5. Pricing benchmarks, and whether bundling MRI with CT changes willingness to pay

### Takeaway
The only published CT simulator prices are US course bundles at about **US$1,700–2,500**:
- ScanLabCT + ImagingU: $2,500 for 6 months' access plus a course
- MTMI course with ScanLab practice: about $1,715–2,970, depending on year and tier

Institutional products (Shaderware/TomoVR, Siemens PEPconnections/SmartSimulator) are quote-only. Free options exist in the IAEA and academic space but are not exam-oriented workflow trainers.

Incumbents bundle. ScanLab sells "One Platform … MRI & CT", and ImagingU pairs simulators with courses. That is indirect evidence that a combined MRI+CT offer is the market norm. No data was found that quantifies how bundling changes willingness to pay.

### Cited Findings
- ScanLabCT + ImagingU: **US$2,500** for 6 months of simulator access, 1 year of course, a syllabus and weekly instructor office hours. The page is undated [SEARCH] — [ScanLab CT Individual Cohorts](https://scanlabmr.com/ct-individual-cohorts/)
- MTMI CT training course with ScanLab practice. The search summaries garble the price tables, so the exact tier is uncertain [SEARCH] — [MTMI 2026 flyer](https://www.mtmi.net/sites/default/files/2025-12/CT_Training_Course_Flyer_for_2026_%282%29.pdf); [MTMI 2025 flyer](https://www.mtmi.net/sites/default/files/2025-03/CT_Training_Course_Flyer_for_2025.pdf):
  - 2026: **US$1,715** ("$300 reduction"), with 3 months of ScanLab access
  - 2025: **US$2,015**, with tuition of $2,970 ($2,825 early, $2,945 member) in another table
- MTMI membership costs **US$39 a year** [SEARCH] — [MTMI flyers](https://www.mtmi.net/sites/default/files/2025-12/CT_Training_Course_Flyer_for_2026_%282%29.pdf)
- ScanLab positions one platform for both modalities: "One Platform to Improve MRI & CT" [SEARCH] — [scanlabmr.com](https://scanlabmr.com/)
- ImagingU also offers a combined VR MRI simulation and technologist certification course [SEARCH] — [Radiology Business](https://radiologybusiness.com/topics/medical-imaging/magnetic-resonance-imaging-mri/imagingu-offers-combo-virtual-reality-mri-simulation-technologist-certification-course)
- Shaderware: "contact us for pricing" [SEARCH] — [shaderware.com](http://www.shaderware.com/)
- Siemens PEPconnect is free. The premium PEPconnections licence is priced via sales [SEARCH] — [Siemens PEPconnections](https://www.siemens-healthineers.com/en-ae/comprehensive-education-portfolio/pepconnect-and-pepconnections/pepconnections)
- IAEA CT dose e-learning and video series: the video series is reported as free of charge [SEARCH] — [Devdiscourse July 2025](https://www.devdiscourse.com/article/science-environment/3520818-iaea-rolls-out-global-video-training-series-to-optimize-ct-imaging-and-patient-safety)
- Context for willingness to pay in the Gulf: Dubai CT/MRI technologist salaries are **AED 10,000–12,000 a month** and Saudi salaries are **SAR 6,000–14,000 a month** [SEARCH] — [Careerjet UAE](https://www.careerjet.ae/jobad/ae669b10da3a58d2b3a37f261f129bf4d6); [Neelim](https://neelim.com/blog/radiographer-license-gcc)

### Inferences
- US$1,700–2,500 is a ceiling for US-certified technologists, with a course and an instructor included. It does not transfer to India. A self-serve browser simulator with no instructor should be priced well below that.
- Suggested price anchors: about **10–20% of the US bundle in the Gulf and UK**, and much lower in India. These are anchors to test with the free demo scan, not evidence-based price points. MRI pricing benchmarks from the sibling research should be used for consistency.
- **Bundling logic:**
  1. Competitors already sell MRI and CT together, so a single-modality product looks narrower.
  2. Gulf job adverts ask for "CT and MRI" experience.
  3. CT has the larger user base, so CT can be the **volume entry product** and MRI the **premium**. Alternatively, sell a discounted "MRI + CT" bundle so CT raises average order value.
- Expected effect: bundling should increase average revenue per user more than per-modality conversion. That is unquantified.
- The free demo scan should be CT, not MRI, if the goal is the widest funnel in India. For example: a CT head with a deliberately off-centred patient, showing the AEC dose change. CT scans are more common, and the "dose" hook is a radiation-safety story that resonates with AERB-minded employers. This is an inference.

### Gaps
- No Indian or Gulf price points for any CT simulator or CT-skills course were found.
- No survey or experiment quantifies how bundling affects willingness to pay for imaging simulators.
- Shaderware, RadSimTech and Siemens price levels are unknown (quote-only).

---

## 6. Bottom line: is a CT simulator worth building? (synthesis of the sections above)

### Takeaway
Yes, probably, and arguably **before** extending MRI further:
- CT is the higher-volume modality in all three target markets (England ~1.7× MRI by monthly scans; India ~2–3× by units; Kerala MCH ~3.4× by daily scans).
- Gulf exams and jobs explicitly test and ask for CT skills.
- Competitors are either expensive US bundles, quote-only institutional software, or vendor-locked tools.
- Building it reuses most of the MRI browser architecture, with simpler core physics.

The main risks:
- **regulatory over-claiming**: it must not imply AERB or IR(ME)R recognition
- **naming confusion** with radiotherapy "CT simulators" in India
- **realism**: transfer improves when the console resembles the placement scanner

### Cited Findings
- CT volume is greater than MRI in England: about 0.71m CT against 0.41m MRI (March 2026) [SEARCH] — [NHS England Statistical Release, July 2026](https://www.england.nhs.uk/statistics/wp-content/uploads/sites/2/2026/07/Statistical-Release-23rd-July-2026.pdf)
- India's MRI base of about 4,800 is "3X lower than CT" [SEARCH] — [BioSpectrum India](https://www.biospectrumindia.com/article/pdf/23424)
- Alappuzha MCH: 85 CT scans a day against 25 MRI [SEARCH] — [Onmanorama 2022](https://www.onmanorama.com/news/kerala/2022/04/26/alappuzha-medical-college-fraud.html)
- SCFHS has a dedicated CT clinical promotion exam (R3, June 2026) [SEARCH] — [SCFHS](https://scfhs.org.sa/sites/default/files/2026-06/CT%20Clinical%20Promotion%20Exam%20Blueprint%20R3.pdf)
- ScanLabCT + ImagingU costs US$2,500 [SEARCH] — [ScanLab](https://scanlabmr.com/ct-individual-cohorts/)
- Simulator–placement scanner similarity affects perceived transfer [SEARCH] — [Monash 2024](https://research.monash.edu/en/publications/transferability-of-learning-from-computed-tomography-simulation-i/)
- "CT simulator" names radiotherapy hardware in Indian tenders [SEARCH] — [Tata Memorial Centre tender](https://docs.infralens.in/nit/2026_TMC_908208_1/Tendernotice_1.pdf)

### Inferences
- Suggested sequencing:
  1. CT MVP using the image-space approach, as a single HTML/JS file reusing the MRI phantom and viewer
  2. One free CT demo scan, e.g. a head CT with an off-centring dose lesson
  3. Paid packages: Core CT (head, chest, abdomen with dose and DRLs), Emergency CT (stroke and trauma), Contrast and CTA (bolus tracking), Gulf exam prep
  4. An MRI + CT bundle
- Positioning wording: "CT scanning practice and dose-optimisation trainer. Not a substitute for supervised clinical training or AERB/IR(ME)R competency sign-off."

### Gaps
- Willingness to pay in India and Kerala was not found.
- No direct competitor scan of Indian edtech for radiographers (ScanFlo, ONE Simulation) was possible beyond search snippets, because the fetches were blocked.
