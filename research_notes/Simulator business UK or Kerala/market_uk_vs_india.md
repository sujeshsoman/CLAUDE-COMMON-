# First market for an online MRI/CT simulator business: UK vs India (Kerala), compared on customers, willingness to pay, competition and sales channels (as of 8 Nov 2026)

**How to read the tags.**
- **[LIVE]**: I read the figure on the primary page itself, fetched with curl on 8 Nov 2026 from corsmed.com, mrieducation.com, scanflo.io, sor.org, gov.uk or rbi.org.in.
- **[SEARCH]**: the figure comes only from a search-result summary, and I did not read the page.
- **[EARLIER-NOTES]**: the figure is reused from the Nov 2026 notes in `research_notes/MRI console simulator India launch/`. Those were themselves search-based and are unverified.

**Access.**
- www.england.nhs.uk returned an AWS WAF bot-challenge page to curl, so every NHS England figure below is [SEARCH].
- These hosts were blocked by the proxy (403), so their figures are [SEARCH] too: hcpc-uk.org, collegeofradiographers.ac.uk, ucas.com, nhsemployers.org, transform.england.nhs.uk, hee.nhs.uk, itnonline.com, scanlabmr.com, malluradiographer.com, YouTube/Instagram, NORKA and ODEPC.
- WebFetch could not resolve any host. All live reads were done with curl.

**Exchange rate used for every conversion:** RBI reference rate as on 5 Nov 2026, **₹126.3870 per £1** and **₹94.1402 per US$1**, which gives **US$1.3425 per £1** [LIVE] — [RBI home page](https://www.rbi.org.in/home.aspx). Conversions are my own arithmetic.

---

## 1. UK customer segments and their size

### Takeaway
The UK has well-funded, clearly defined buyers but limited volume:
- roughly 49k HCPC-registered radiographers, of whom about a quarter trained overseas;
- a diagnostic radiography workforce under pressure (12.8% vacancy in the last full SoR census);
- fast growth in CT/MRI capacity (125 extra NHS CT/MRI scanners between Mar 2024 and Mar 2026, 107 of them in community diagnostic centres, CDCs);
- a new national preceptorship framework for internationally recruited AHPs (May 2026).

I could not verify national student-intake numbers or an India-specific international-recruit count. The segment with the most specific evidence of a training need is internationally educated radiographers moving into CT/MRI in NHS and CDC services, alongside the trusts that train them.

### Cited Findings
**Workforce and register**
- HCPC register: 49,164 registrants listed under "radiographers". This covers diagnostic and therapeutic radiographers together [SEARCH] — [HCPC register summary](https://www.hcpc-uk.org/data/the-register/register-summary/)
- More than a quarter of HCPC radiographer registrants trained overseas: 12,160 of 46,071. In a small migrant sample, 2 of 8 respondents were from India [EARLIER-NOTES/SEARCH] — [Radiography 2024, "Mapping the migrant diagnostic radiographers in the UK"](https://www.radiographyonline.com/article/S1078-8174(24)00215-3/pdf)
- SoR Diagnostic Radiography Workforce UK Census 2022, census date 1 Nov 2022, 59 responding services [LIVE] — [SoR Census 2022 report](https://www.sor.org/getmedia/6994cd5d-0155-4a7e-a8a7-32a9bbda81c3/Diagnostic-Radiography-Workforce-UK-Census-2022-report):
  - average UK vacancy rate was 12.8% (England 12.8%, Scotland 7.5%, Wales 8.3%);
  - turnover was 10.21%;
  - respondents had recruited 8.1% of their headcount internationally in the past year and intended a further 7.5%. By headcount, 14% of band 5 staff were international recruits in the past year, with 18% expected the following year;
  - band 6 numbers were growing in CT and MRI, with a "growing number" of band 4 assistant practitioners in MRI;
  - 5.5% of staff were in postgraduate training, including CT and MRI PgCert/PgDip/MSc;
  - NHS England respondents averaged 5.5 apprenticeship posts each;
  - the foreword says low morale and vacancies leave "little time to support staff in CPD", and calls for more practice-educator roles.
- The SoR's later "Snapshot Census" (deadline extended to 14 Jun 2024) was cut down to two questions, establishment and vacancy rates [LIVE] — [SoR, 6 Jun 2024](https://www.sor.org/news/surveys/calls-to-complete-the-diagnostic-radiography-workf). I found no published 2024 or 2025 diagnostic results [SEARCH].
- Pay: an NHS Band 5 diagnostic radiographer advert (Surrey and Sussex, posted 25 Mar 2026) offers £31,049–£37,796 (≈₹39.2–47.8 lakh) [SEARCH] — [NHS Jobs advert C9326-26-0178](https://www.jobs.nhs.uk/candidate/jobadvert/C9326-26-0178)

**Students and programmes (national figures not verified)**
- No national UCAS or HESA 2025 acceptance figure for diagnostic radiography was found [SEARCH].
- SoR (Feb 2021): AHP acceptances in England rose 17.5% in 2020, and diagnostic radiography acceptances also rose. No absolute number is given [LIVE] — [SoR, 19 Feb 2021](https://www.sor.org/news/students/radiography-student-numbers-rise-in-2020)
- Individual programme sizes:
  - Derby lists 128 places for 2026 entry [SEARCH] — [Derby](https://www.derby.ac.uk/undergraduate/radiography-courses/diagnostic-radiography-bsc-hons/)
  - Huddersfield expected about 30 places for 2026-27 [SEARCH] — [Huddersfield](https://courses.hud.ac.uk/2025-26/full-time/undergraduate/diagnostic-radiography-bsc-hons)
  - At Cumbria, "nearly 20 students, about 25% of the cohort" chose the MRI pathway, which implies a cohort of about 80 [LIVE] — [Corsmed: University of Cumbria case study](https://www.corsmed.com/case-studies/university-of-cumbria)
- An aggregator lists "71 Diagnostic Imaging Degree Courses in the UK 2026". This count includes course variants, not just institutions [SEARCH] — [UniversityGuru](https://www.universityguru.com/-uk/diagnostic-imaging)
- Demand signal: the University of Liverpool's UCAS listing shows no England vacancies for 2026 entry [SEARCH] — [UCAS Liverpool](https://www.ucas.com/explore/courses/c33b0ee9-a95d-23ec-81da-45ca33bfbd93/course)
- A Cumbria lecturer says "recent changes to HCPC standards now demand more MRI training", and that students use simulator certificates in CT/MRI job interviews [LIVE] — [Corsmed: Cumbria](https://www.corsmed.com/case-studies/university-of-cumbria)

**NHS investment, CT/MRI capacity, workforce policy**
- GOV.UK press release, citing NHS England data published 3 Nov 2026 [LIVE] — [GOV.UK: "One million more scans to help catch cancer sooner"](https://www.gov.uk/government/news/one-million-more-scans-to-help-catch-cancer-sooner):
  - the NHS added 125 CT and MRI scanners between March 2024 and March 2026, and 107 of these went into CDCs;
  - CDCs carried out nearly 2.2 million CT and MRI scans in the 12 months to March 2026, about a million more than two years earlier;
  - AI acceleration software is installed on 54% of compatible NHS MRI scanners, and every trust is to be offered upgrades by 2029;
  - the £19.2m Manchester and Trafford CDC opened on 29 Oct 2026.
- 170 CDCs are operating. In April 2026, £237m was announced for 36 new or expanded centres [SEARCH] — [NHS England East of England, 15 Apr 2026](https://www.england.nhs.uk/east-of-england/2026/04/15/patients-in-east-of-england-set-for-quicker-tests-closer-to-home-as-new-and-expanded-community-diagnostic-centres-confirmed/)
- NHS Long Term Workforce Plan (2023) [SEARCH] — [NHS England LTWP](https://www.england.nhs.uk/long-read/nhs-long-term-workforce-plan-2/):
  - diagnostic radiographers are among the largest AHP shortfalls;
  - AHP training places are to rise to 17,000 by 2028/29 and to more than 18,800 by 2031/32;
  - 25–50% of diagnostic radiography entrants could come through apprenticeships by 2031/32;
  - funding covers 150 enhanced-practice radiographers a year.
  - I could not check whether a 2025/26 refresh has superseded these numbers (england.nhs.uk blocked).
- Regional Imaging Training Academies exist in 7 regions [SEARCH] — [HEE Imaging Academy 2023/24 document](https://www.hee.nhs.uk/sites/default/files/documents/2324Imaging%20Academy%20MASTERPublic.pdf); [Review of radiology academies](https://www.hee.nhs.uk/sites/default/files/documents/Review%20of%20radiology%20academies%20FINAL.pdf); [UHNM news](https://www.uhnm.nhs.uk/latest-uhnm-news/uhnm-shortlisted-for-three-hsj-digital-awards/):
  - they were expected to be "self-sustaining by 2025";
  - the Midlands academy put "c. £150K of radiography simulation funding" in 2023/24;
  - UHNM received £1.28m from NHS England Midlands for an AI upgrade to radiology training facilities.

**International recruits: preceptorship and upskilling**
- On 6 May 2026 NHS England launched the National AHP Preceptorship and Foundation Support Programme, which includes an International Recruitment Implementation Framework [LIVE] — [SoR news, 6 May 2026](https://www.sor.org/news/government-nhs/nhs-england-launches-resources-for-internationally):
  - the pathway runs pre-preceptorship → preceptorship → foundation support;
  - it has profession-specific modules, including diagnostic radiography.
- The SoR offers free e-learning for overseas-trained radiographers ("Working in the NHS", "Role of the Radiographer in the UK"). Its International Recruitment learning path includes introductory sessions for general radiography, CT and MRI, and the Clinical Imaging programme has nearly 500 e-learning sessions [LIVE] — [SoR, 14 Nov 2023](https://www.sor.org/news/role-development/sor-support-for-internationally-educated-radiograp)
- The SoR international recruitment page links an NHS England webinar from June 2023 on recruiting diagnostic radiographers for CDCs, and a "Workplace Integration Course" [LIVE] — [SoR International Recruitment](https://www.sor.org/learning-advice/career-development/international-recruitment)
- Since 20 Nov 2025, HCPC assesses international applications in one round: gaps lead to a test of competence or a refusal rather than a request for more information. The scrutiny fee is £678.38 (≈₹85,700) for applications from 29 Apr 2025 [SEARCH] — [HCPC international guidance 2025](https://www.hcpc-uk.org/globalassets/registration/application-forms/international-applications/international-applications---guidance-notes-2025.pdf)
- HCPC international application volumes, all 15 professions combined [SEARCH] — [HCPC registration report Aug 2025](https://www.hcpc-uk.org/globalassets/meetings-attachments3/education-and-training-committee/2025/03.-10-september-2025/item-08-registration-performance-report.pdf); [HCPC Council Feb 2026](https://www.hcpc-uk.org/globalassets/meetings-attachments3/council-meeting/2026/1-february/item-03-chief-executives-performance-report.pdf):
  - 1,245 international applications were received in 2025-26 up to Aug 2025;
  - 2,357 "this financial year to date" by the Feb 2026 council paper, which says volumes "remain lower than forecast";
  - neither source gives a radiographer or India breakdown.

### Inferences
- **Size of the international-recruit segment (order of magnitude only):** about 8% of headcount recruited internationally per year (2022 sample) applied to a diagnostic workforce in the tens of thousands suggests a peak of low thousands of international radiographer hires a year UK-wide. The fact that HCPC applications across all professions are "lower than forecast" in 2025-26 suggests the flow is now smaller. The India and Kerala share is unknown.
- **Where demand is concentrated:** CDC expansion has put most new scanners into CT/MRI. Combined with band 6 growth in CT/MRI and assistant practitioners moving into MRI, the strongest UK need is cross-training band 5/6 staff and new international recruits into CT/MRI, rather than first-year students.
- **Preceptorship gap:** the May 2026 framework standardises preceptorship but supplies no console-practice tool. A "pre-preceptorship" simulator pack for incoming Indian radiographers fits the framework's pre-preceptorship stage.
- **Free competition at the intro level:** the SoR's free intro CT/MRI e-learning for international recruits means a paid UK product must offer hands-on console practice, not theory.

### Gaps
- No national count of UK diagnostic radiography programmes, annual intake or NHS-commissioned places was retrieved. UCAS, HESA, HCPC and the College of Radiographers' approved-programme lists were all blocked or returned no figures.
- No HCPC data on radiographer international applications by country (India or Kerala). An HCPC FOI request would be needed.
- No MRI/CT radiographer headcount for the UK, and no published trust training-budget figure per department.
- I could not check whether the 2023 LTWP targets were revised in 2025/26 (england.nhs.uk blocked).
- No assistant-practitioner or apprentice counts beyond the 2022 census averages.

---

## 2. What UK buyers pay and how they buy (prices, procurement, compliance)

### Takeaway
UK reference prices for simulator access are high:
- **Corsmed** individual plans cost **US$1,050 for 6 months (≈£782)** or **US$1,548 for 12 months (≈£1,153)**, with a permanent free tier (head and knee only).
- **MRI Education** bundles its simulator into a **£800 course (£900 from January)**.
- **ScanFlo** charges non-Indian buyers **US$399/yr (≈£297)**.

NHS buyers pay by purchase order or through Shared Business Services (SBS). Small purchases need only one or two quotes (many trusts set the line at about £5k–£10k), and full Procurement Act tendering applies only above roughly £135k–£208k. A non-clinical training tool that holds no patient data probably does not need DTAC or DSPT, but buyers will expect security assurance such as Cyber Essentials (about £320 + VAT a year for micro firms). CPD Now endorsement costs £100–£250 + VAT per application, based on an undated SoR document.

### Cited Findings
**Corsmed (Sweden): UK incumbent**
- Individual plans [LIVE] — [Corsmed for individuals](https://www.corsmed.com/mri-simulator/for-individuals). This **corrects the earlier note that said "$129 for 12 months"**.
  - 12-month subscription: US$129/month, 12 monthly payments, **US$1,548 in total** (≈£1,153 / ₹1,45,700);
  - 6-month subscription: US$175/month, **US$1,050 in total** (≈£782 / ₹98,800);
  - both include all anatomies, pathologies and advanced cases, plus self-paced courses: 65 modules, about 65 hours, labelled "$185 value".
- Free tier [LIVE] — [Corsmed free MRI simulator](https://www.corsmed.com/free-mri-simulator):
  - "Head and knee anatomies. Seven sequences", "Free forever". The same page also says "8 core pulse sequences", so it contradicts itself;
  - paid features listed against it: LMS, 50+ anatomies, 23 pulse sequences. The /mri-simulator page instead says "25 sequences" and "30+ sequence parameters" [LIVE] — [Corsmed MRI simulator](https://www.corsmed.com/mri-simulator).
  - The launch date of 2 Nov 2026 comes from ITN [EARLIER-NOTES/SEARCH] — [ITN](https://www.itnonline.com/node/91310).
- corsmed.com/pricing returns HTTP 404 [LIVE]. Institutional prices are not published on any page I fetched [LIVE].
- UK customers named on Corsmed's own pages [LIVE] — [Corsmed home](https://www.corsmed.com/); [UCLH case study](https://www.corsmed.com/case-studies/nhs-university-college-london-hospitals); [Corsmed for healthcare](https://www.corsmed.com/mri-simulator/for-healthcare):
  - University of Cumbria;
  - UCLH NHS Foundation Trust: 7 MRI scanners at 15–20 patients each a day; MRI radiographer competence in "3–4 months instead of 6"; a 1-hour introduction is enough;
  - The Christie NHS FT (Manchester);
  - Imperial College Healthcare NHS Trust, which Corsmed says switched from ScanLabMR.
- Earlier, unverified search-based notes also list Teesside, City (London) and London Imaging Academy [EARLIER-NOTES/SEARCH] — [HealthySimulation](https://www.healthysimulation.com/vendors/corsmed/)

**MRI Education ("MRI in Practice", UK)**
- **£800 (£900 from January) all-inclusive** (≈₹1,01,100 / ₹1,13,700) [LIVE] — [MRI Education home](https://www.mrieducation.com/); [Apply](https://www.mrieducation.com/apply/); [Course dates](https://www.mrieducation.com/coursedates/):
  - covers the core course (a 9-day online event from Oct 2026, about 30 h, needing about 4 days' study leave), 10 on-demand technique lectures, 12 months of simulator access and "over 50" simulator exercises;
  - the simulator covers brain and abdomen at 0.5/1.5/3T;
  - next dates are 6–14 Mar 2027, 19–27 Jun 2027 and 9–17 Oct 2027.
- Pricing claims [LIVE] — [Apply](https://www.mrieducation.com/apply/):
  - "Other courses charge around £1000 for simulator access, ours is free";
  - its own price works out at "£26 per hour" of teaching, against a competitor charging "£72.00 per hour";
  - there is no regional pricing.
- Purchasing [LIVE] — [Apply](https://www.mrieducation.com/apply/):
  - "NHS Purchase Orders and Shared Business Services: NHS providers who wish to add us to SBS or raise a purchase order, please let us know";
  - individual access is blocked from hospital and university IP addresses. Employers must "contact us for discount pricing", and educators can ask for a group discount.
- Endorsement [LIVE] — [Course dates](https://www.mrieducation.com/coursedates/):
  - SoR CPD Now endorsed, supporting 10 listed outcomes;
  - ASMIRT 30 CPD units;
  - CPD support for 2 years.

**ScanFlo's price to non-Indian buyers**
- Outside India, MRI Student costs US$39/month or US$399/year (≈£29 / £297), and Student Pro US$49/month or US$499/year (≈£36 / £372). The currency is set by the country code of the account's phone number [LIVE] — [ScanFlo pricing](https://scanflo.io/pricing)

**ScanLab (USA)**
- Individual cohorts: US$1,000 (≈£745) or US$2,500 (≈£1,862) for 6 months. A UWE Bristol testimonial is quoted [EARLIER-NOTES/SEARCH; scanlabmr.com blocked] — [ScanLab](https://scanlabmr.com/)

**Comparable CPD and event prices**
- PAIR International Radiographers Conference 2026: £40 early-bird, £50 standard [LIVE] — [SoR event page](https://www.sor.org/events/2026-07-04-wolverhampton-pair-sig-international-radiographers-conference-2026-375)

**How NHS trusts and universities buy**
- Procurement Act 2023 thresholds, 1 Jan 2026 to 31 Dec 2027, including VAT [LIVE] — [GOV.UK thresholds guidance](https://www.gov.uk/government/publications/procurement-act-2023-guidance-documents-define-phase/guidance-thresholds-html):
  - goods and services to central government: **£135,018**;
  - goods and services to sub-central authorities: **£207,720**.
- Below-threshold rules (Part 6): sub-central bodies and NHS trusts previously used £30,000 including VAT. One summary says Foundation Trusts now fall under the lower central-government figure [SEARCH] — [GOV.UK below-threshold guidance](https://gov.uk/government/publications/procurement-act-2023-guidance-documents-define-phase/guidance-below-threshold-contracts-html). I did not verify the exact current figure.
- Trust Standing Financial Instructions (SFIs) vary [SEARCH] — [Northumbria thresholds](https://www.northumbria.nhs.uk/about-us/corporate-information/become-supplier/thresholds); [South Tees](https://www.southtees.nhs.uk/about/procurement/); [GWH SFI summary](https://gwh.nhs.uk/media/ar0fobat/gwh-standing-financial-instructions-summary-august-2023-final.pdf); [SCAS quotation procedure](https://www.scas.nhs.uk/wp-content/uploads/2023/03/Tendering-and-quotation-procedure-1.pdf). Typical tiers:
  - under £5k: 1 written or 2 verbal quotes;
  - £5k–£10k: 2 written quotes;
  - £10k–£30k: 3 written quotes;
  - above about £25k–£30k: tender;
  - some trusts allow a single quote below £10k.
  - I found nothing on procurement-card limits.
- Corsmed's UCLH case study adds that "UCLH maintains vendor neutrality in accordance with NHS procurement guidelines" and that the study "does not constitute an endorsement" [LIVE] — [UCLH case study](https://www.corsmed.com/case-studies/nhs-university-college-london-hospitals). Trusts limit how far suppliers can use them as references.

**Supplier assurance requirements**
- DTAC [SEARCH] — [NHS Transformation Directorate DTAC](https://transform.england.nhs.uk/key-tools-and-info/digital-technology-assessment-criteria-dtac); [Burges Salmon](https://www.burges-salmon.com/articles/102mnjh/new-nhs-digital-technology-assessment-criteria-what-health-tech-suppliers-need-t); [NHS Innovation Service](https://innovation.nhs.uk/news/updated-nhs-england-digital-technology-assessment-criteria-dtac-form-and-guidance/):
  - it was revised in late Feb 2026, and the new form replaces the previous one from 6 Apr 2026;
  - its scope is "software based digital health technologies" as defined by NICE;
  - it covers clinical safety (DCB0129/0160), data protection, technical security, interoperability, and usability/accessibility.
  - None of these sources explicitly carves out staff-training software.
- ScanFlo's institutional marketing stresses "No identifiable patient data, no clinical integration", invoice billing, purchase-order support, and a security summary and data-processing terms on request [LIVE] — [ScanFlo universities](https://scanflo.io/solutions/universities); [ScanFlo enterprise](https://scanflo.io/enterprise)
- Cyber Essentials, per the IASME FAQ: micro organisations (0–9 staff) £320 + VAT (≈₹40,400), small £440 + VAT, medium £500 + VAT, renewed annually. Third-party sites quote £300–£330 [SEARCH] — [IASME FAQ](https://iasme.co.uk/cyber-essentials/faq-cyber-essentials)
- CoR CPD Now endorsement [LIVE] — [SoR Scottish Council CPD endorsement policy (docx)](https://www.sor.org/getmedia/b4e9cb44-b353-4a4d-b61c-e17c137ef360/supporting_study_events._sc_policy_and_guidance_v2.docx):
  - "The standard fee for each CPD endorsement application is £250 + VAT. The fee for NHS Trusts/Boards and education institutions is £100 + VAT";
  - endorsement is valid for 2 years;
  - it is for activities that are not credit-bearing and do not confer competence;
  - applications go in at least 6 weeks (elsewhere in the same document, 3 months) before the event;
  - **the document is undated**. The CoR's current page lists a fee table with "No fee" for SoR councils and committees and "Contact" for NHS/private providers [SEARCH] — [CoR CPD endorsement](https://www.collegeofradiographers.ac.uk/Education/Education-Approval/CPD-endorsement)
  - Search summaries add that CPD Now endorsement "does not list points or hours" and requires at least two CPD Now outcomes [SEARCH].

### Inferences
- **UK price corridor for individuals:** about £0 (Corsmed free head/knee) up to about £300/yr (ScanFlo USD) and about £780–£1,150 (Corsmed paid), plus £800–£900 for the MRI Education bundle. A UK-facing package at about **£49–£149** for 3–6 months would undercut every paid competitor while still being worth about 6–19x ScanFlo's Indian per-month price. A UK Band 5 gross monthly salary of about £2,587 (£31,049 ÷ 12) makes £99 about 4% of one month's pay. All of this is my inference.
- **UK trust departmental licence:** pricing at about **£1,000–£5,000 a year** keeps a deal below most trusts' single- or two-quote thresholds. The purchase can then be signed off by a radiology service manager or practice educator through a PO or SBS, without a tender. This seems the fastest NHS route. University cohort licences are likely to need longer cycles and IT security reviews (inference).
- **Compliance:** for a browser simulator with synthetic or anonymised images, no patient data and no clinical integration, DTAC and DSPT are probably not mandatory. That is inference; the DTAC scope is "digital health technologies", and no explicit training-tool exemption was found. In practice trusts will still send IG and security questionnaires, so **Cyber Essentials (about £320 + VAT a year)** plus a short security summary and DPA, modelled on ScanFlo's, is the cheap standard answer. CPD Now endorsement (about £100–£250 + VAT, valid 2 years) is the main UK credibility marker: MRI Education leans on it heavily, and it suits a "learning package" whether or not it is a live event.
- **Founder-specific (unsourced, needs checking):** an NHS employee selling to NHS trusts, especially their own, will need to declare the interest under the trust's conflicts-of-interest or standards-of-business-conduct policy.

### Gaps
- Corsmed, ScanLab and ScanFlo institutional prices are unpublished (quote only).
- I did not check NHS Supply Chain or Crown Commercial Service frameworks for training software (hosts blocked).
- The current CoR CPD Now endorsement fee could not be confirmed on collegeofradiographers.ac.uk (blocked). The £250/£100 + VAT figures come from an undated SoR document.
- The exact current below-threshold figure for NHS trusts and Foundation Trusts under the Procurement Act was not verified on the primary page.
- No official statement was found on whether DTAC applies to non-patient-facing staff training software.

---

## 3. India (Kerala) segments: students, working technologists, colleges (verified and updated)

### Takeaway
ScanFlo (Delhi) sets the Indian price ceiling with live, published prices:
- MRI Student **₹999/month, ₹2,799/3 months or ₹9,999/year**; MRI Pro up to **₹14,999/year**;
- CT costs ₹899–₹13,999;
- all plans are one-time payments with no auto-renewal, paid by Razorpay/UPI;
- a 45-minute free trial;
- institutional seats from 10 seats on annual terms, quote only.

Kerala fresher radiographer pay of about **₹15,000–₹25,000 a month** is confirmed by mid-2026 job postings, so ScanFlo's annual Student plan costs 40–67% of a fresher's monthly pay. Individual willingness to pay is real but small. Colleges are the bigger cheques, but their price points and buying behaviour are undocumented.

### Cited Findings
**ScanFlo prices, read from the pricing page's product catalogue data** [LIVE] — [ScanFlo pricing](https://scanflo.io/pricing); [ScanFlo MRI](https://scanflo.io/mri) shows "From ₹999/month" and structured data ₹999–₹14,999; [ScanFlo CT](https://scanflo.io/ct) shows structured data ₹899–₹13,999.

| Plan | 1 month | 3 months | 1 year | USD (outside India) |
|---|---|---|---|---|
| MRI Student | ₹999 (≈£7.9) | ₹2,799 | ₹9,999 (≈£79) | $39/mo; $399/yr |
| MRI Student Pro | ₹1,499 | ₹4,199 | ₹14,999 (≈£119) | $49/mo; $139/qtr; $499/yr |
| CT Student | ₹899 | ₹2,499 | ₹8,999 | $39/mo; $399/yr |
| CT Student Pro | ₹1,399 | ₹3,999 | ₹13,999 | $49/mo; $139/qtr; $499/yr |

- ScanFlo plan terms [LIVE] — [ScanFlo pricing](https://scanflo.io/pricing):
  - Student Pro adds cardiac, spectroscopy, MRCP, prostate, pituitary, breast and fetal studies (MRI), or CT angiography, triphasic liver and enterography (CT);
  - each plan allows up to 2 devices, one in use at a time;
  - every plan is a one-time payment: "Nothing renews";
  - paid access is non-refundable once activated;
  - Indian buyers pay in INR through Razorpay (UPI, cards, netbanking, wallets);
  - the free trial is 45 minutes of console time, to be used within 7 days.
- Institutional licensing [LIVE] — [ScanFlo universities](https://scanflo.io/solutions/universities); [ScanFlo enterprise](https://scanflo.io/enterprise); [ScanFlo case studies](https://scanflo.io/case-studies); [ScanFlo about](https://scanflo.io/about):
  - "By seat, starting at 10 seats, on annual terms that match academic cycles", billed by invoice with procurement support;
  - a pilot is "10 seats for one term";
  - features include cohort dashboards, OSCE stations, countersigned hash-chained logbooks and accreditation exports.
  - The case-study page has no named customers yet ("As customer programmes mature, their stories will appear here") but claims "Thousands of radiography learners have trained on the platform".
  - The simulator was "built inside a working radiography training programme". Earlier notes link this to 3D Paramedical, Delhi/Noida [EARLIER-NOTES].

**Kerala pay (willingness-to-pay anchor), from job postings dated mid-2026** [SEARCH]:
- Kaloor (Ernakulam) fresher radiographer: ₹15,000–₹18,000/month — [evaniosjobs](https://www.evaniosjobs.com/job-details/2539082/radiographer-job-in-kaloor)
- Punalur fresher: ₹18,000–₹22,000 — [evaniosjobs](https://www.evaniosjobs.com/job-details/2506349/radiographer-job-in-punalur)
- Thiruvananthapuram (Janatha Hospital) fresher: ₹23,000–₹25,000 — [evaniosjobs](https://www.evaniosjobs.com/job-apply/2424171/radiographer-job-in-thiruvananthapuram)
- Ernakulam: ₹20,000–₹25,000 — [evaniosjobs](https://www.evaniosjobs.com/job-details/2444323/radiographer-job-in-ernakulam)
- Mavelikara X-ray technician: ₹8,000–₹15,000 — [evaniosjobs](https://www.evaniosjobs.com/job-apply/2481752/xray-technician-job-in-mavelikara)
- Meitra Hospital (Calicut) CT/MRI technologist, mid-level: ₹30,000–₹50,000 — [tryapplynow](https://www.tryapplynow.com/jobs/meitra-hospital-calicut-ct-mri-technologist-2d354624-9caa-46ae-be55-1f46ac6a7dcd)

**Fees and other anchors** [EARLIER-NOTES/SEARCH]:
- KUHS B.Sc MRT costs about ₹1.32–1.65 lakh in total — [Shiksha](https://www.shiksha.com/university/kerala-university-of-health-sciences-thrissur-64747/course-b-sc-in-medical-radiological-technology-375115)
- Private Kerala B.Sc MRT costs about ₹40,000–95,000 a year — [Campushunt](https://campushunt.in/blog/bsc-radiology-colleges-in-kerala/)
- Short MRI technician certificates cost about ₹20,000–80,000 — [Collegedunia](https://collegedunia.com/courses/radiology/mri-technician-course)
- The DME Kerala paramedical diploma matrix totals 867 seats across all diploma courses; the radiology share is unknown — [DME Kerala](https://dme.kerala.gov.in/seat-matrix/)
- NCAHP notified a competency-based 2-year D.MRIT with internship (Oct 2026) — [BattleIAS](https://battleias.com/current-affairs/2026-10-07-ncahp-notifies-autonomous-boards-and-digital-registration-for-allied-and-healthc/)

**Other Kerala players** [EARLIER-NOTES/SEARCH]:
- SIMLABS (Thrissur, launched 2026) offers VR clinical simulation, including radiology positioning and protocol selection. No MRI console product was found — [SIMLABS](https://simlab.in/)

### Inferences
- **Indian individual price corridor:** from ₹0 (Corsmed free head/knee, which is global) up to ₹999/month or ₹9,999/year (ScanFlo). With fresher pay at ₹15–25k a month, a realistic price for a Kerala student or junior technologist is about **₹499–₹999 per month, or ₹2,499–₹4,999 for a 6–12-month pack**, roughly 10–33% of one month's fresher pay. Revenue per individual is therefore about ₹2,500–₹5,000 (about £20–£40), against about £50–£150 per UK individual: **a 3–6x gap per customer**. This is my inference.
- **Kerala colleges:** ScanFlo's "10-seat, one-term pilot" model shows what Indian institutions expect. The likely deal size is a few tens of thousands to about ₹1–2 lakh a year per college, an assumption carried over from the earlier notes. Getting there needs in-person demos to principals and managements, which the founder's trusted person in Kerala could do. The NCAHP competency-based D.MRIT curriculum and logbook expectations give colleges a reason to buy (inference).
- **Pricing structure:** ScanFlo's one-time, no-auto-renew, UPI-first model is the norm Indian buyers now expect. Recurring card subscriptions will meet resistance (inference).
- **Arbitrage risk:** ScanFlo's INR price (₹9,999 ≈ $106) is about a quarter of its USD price ($399). Any INR tier needs a geographic gate, such as ScanFlo's phone-country rule, or UK and Gulf buyers will pay Indian prices (inference).

### Gaps
- No public price for ScanFlo or any rival college/seat licence, and no evidence on Kerala college buying cycles or approval layers (management, principal, university).
- No count of Kerala DRT, B.Sc MRT and M.Sc MRT seats (LBS and DME pages blocked in earlier research).
- No survey data on Indian radiography students' spending on ed-tech.
- No evidence of ScanFlo sales or partners in Kerala specifically.

---

## 4. Gulf/diaspora segment, and sizing the Kerala → UK pipeline

### Takeaway
Two diaspora flows exist, but neither is well quantified:
- **Kerala → Gulf.** This is the larger, older flow, with an established Prometric/DHA coaching industry in Kerala. Exam fees run to about US$240, with total licensing costs of about ₹50–80k.
- **Kerala/India → UK.** This is smaller, but it is where the founder's credibility is strongest. Kerala's ODEPC has advertised NHS diagnostic radiographer posts, and an organised Indian-radiographer community exists in the UK (PAIR, a SoR SIG since 2024, with 172 delegates at its 2025 conference).

I found no figure for radiographers recruited from India or Kerala to the UK each year, or for Gulf licences issued to Indian radiographers.

### Cited Findings
**Kerala → UK**
- Kerala government agency ODEPC has posted "Recruitment of Radiographers to NHS Trust Hospitals of United Kingdom", listing Band 5–7 pay, visa, flights, initial accommodation and IELTS fees covered. The listing is undated [SEARCH] — [freejobalerts copy of ODEPC notice](https://www.freejobalerts.co.in/odepc-recruitment/recruitment-radiographer-uk-odepc/)
- NORKA Roots [SEARCH] — [UK Malayalee, Nov 2022](https://ukmalayalee.com/?p=27289); [UNI India](https://test.uniindia.com/norka-roots-recruits-doctors-for-uk-wales/south/news/3496502.html):
  - in 2022 it ran a UK careers fair that included radiographers;
  - its 2025 NHS drive (NHS Wales, interviews in Kochi in July 2025) was for doctors;
  - no 2025/26 radiographer drive was found.
- PAIR (Professional Alliance of Indian Radiographers) [LIVE] — [SoR, 28 Aug 2024](https://www.sor.org/news/professionalism/pair-launches-as-sor-special-interest-group); [PAIR SIG page](https://www.sor.org/about/get-involved/special-interest-groups/pair); [SoR, 20 Jul 2026](https://www.sor.org/news/campaigns/south-asian-heritage-month-join-the-professional-a):
  - it began as a WhatsApp group in January 2021 and became an SoR Special Interest Group on 28 Aug 2024;
  - it is open to all Indian-origin radiographers in the UK, whether or not they are SoR members;
  - it offers pastoral support, career guidance, webinars ("Resonate with PAIR") and conferences;
  - its board includes Rajesh Kesavan (Chair, Birmingham Women's and Children's), Bosco Antony (Gateshead), Abraham Cheriyakavil Koshy (Alliance Medical) and **Noyal Mathew (UCLH), Director of Professional Development and Education**.
  - Note: the Name was earlier given as "Professional Association"; it is "Professional Alliance".
- Conference [LIVE] — [SoR event page](https://www.sor.org/events/2026-07-04-wolverhampton-pair-sig-international-radiographers-conference-2026-375):
  - International Radiographers Conference 2025 had **172 delegates**;
  - IRC 2026 was at the UKKCA Community Centre, Wolverhampton. The page gives two dates (Sunday 26 Jul 2026 and Saturday 4 Jul 2026);
  - tickets were £40 early-bird, £50 standard, with sponsor and exhibitor slots offered.
- Corsmed's UCLH testimonial is credited to an "MRI Practice Educator, NHS UCLH". The image asset is named "NHS UCLH – Noyal Mathew" [LIVE] — [Corsmed home](https://www.corsmed.com/); [UCLH case study](https://www.corsmed.com/case-studies/nhs-university-college-london-hospitals)
- A Malayalam news report (Sept 2024) describes the UK Indian-radiographer association as Malayalee-led [EARLIER-NOTES/SEARCH] — [Express Herald](https://expressherald.com/2024/09/08/the-association-of-indian-radiographers-working-in-britain-came-into-existence/)
- HCPC hurdles for Indian applicants [SEARCH] — [HCPC guidance 2025](https://www.hcpc-uk.org/globalassets/registration/application-forms/international-applications/international-applications---guidance-notes-2025.pdf); [NHS Employers](https://www.nhsemployers.org/articles/recruitment-overseas-allied-health-professionals):
  - scrutiny fee £678.38;
  - single-round assessment since Nov 2025;
  - IELTS Academic 7.0 overall with no band below 6.5, per guides;
  - mapping against the standards of proficiency is required.
- Pay gap: UK Band 5 is about £2,587 a month gross [SEARCH, NHS Jobs advert above], against a Kerala fresher's ₹15–25k (≈£119–£198) [SEARCH, postings above]. That is roughly a **13–22x** gap (my arithmetic).

**Kerala → Gulf**
- DHA radiographer exam [SEARCH] — [Neelim DHA](https://www.neelim.com/ar/exams/dha); [LeapScholar](https://leapscholar.com/blog/?p=84873):
  - code RAD5152, a Prometric CBT;
  - 150 MCQs in 3 hours, 55% pass mark;
  - about US$240 (≈₹22,600);
  - licence activation about AED 1,000–3,000.
- Total Gulf licensing cost is about ₹50,000–80,000. The DHA MRI-technologist licence needs 2 years' MRI experience, and MRI is about 10% of the radiographer exam [EARLIER-NOTES/SEARCH] — [LeapScholar](https://leapscholar.com/blog/dha-exam-for-radiographer-guide/); [MyDoctorLicense](https://mydoctorlicense.com/dha-license-for-resonance-magnetic-imaging-mri-technologist/); [Ziapy](https://ziapy.com/gulf-radiography-licensing-exams-dha-scfhs-qchp/)
- Gulf MRI technologist pay is about US$4,000–5,000 a month [EARLIER-NOTES/SEARCH] — [IHR Canada](https://ihrcanada.com/benefits/radiographers-in-saudi-arabia-uae-and-qatar-benefits-package-and-salary-scale-guideline/)
- Kerala coaching: Tiju's Academy, Dynamic Health Staff and Malakha Academy run Prometric/DHA coaching, but none publishes a radiographer-specific fee [SEARCH] — [Tiju's Academy](https://tijusacademy.com/best-prometr); [Dynamic Health Staff](https://www.dynamichealthstaff.com/best-prometric-centre-in-kerala)
- Kerala Migration Survey 2023: about 2.2 million emigrants, mostly to the GCC, with no occupation split for radiographers [EARLIER-NOTES/SEARCH] — [IIMAD KMS 2023](https://iimad.org/wp-content/uploads/2024/06/KMS-2023-Report.pdf)

### Inferences
- **Sizing the Kerala → UK pipeline (rough, assumption-heavy):** the UK takes perhaps hundreds to low thousands of international radiographers a year (section 1), and India is one of the main source countries (2 of 8 in a small sample). Indian arrivals are therefore plausibly in the low hundreds a year, with Kerala a large share given the Malayalee-led community. On top of that sits a larger pool of aspirants preparing for HCPC/IELTS, plus Indian-origin radiographers already in the UK who want CT/MRI rotations. I would put the reachable B2C pool at a few thousand people. This is an inference, not data.
- **Willingness to pay:** this pool pays UK-scale costs (HCPC £678 scrutiny + £370 registration per guides, plus IELTS and visa). A ₹4,999–₹9,999 or £49–£99 "NHS-ready CT/MRI console" pack is a small add-on to that spend. That makes it the segment where the founder can charge most per head without a UK institutional sale (inference).
- **Gulf segment:** larger in volume but more price-sensitive and already served by coaching centres. The better route is a partnership or bundle (simulator access sold through Kerala Prometric coaching centres) rather than direct sales (inference).
- **PAIR as a channel:** PAIR is a ready-made UK channel (webinars, a £40–£50 conference, sponsorship). However, its education director appears to be the UCLH practice educator featured in Corsmed's case study (same name, same employer). PAIR's leadership already knows and endorses the market leader, so the founder must differentiate (Indian-workflow bridging, CT, Malayalam/English support), not just "simulator access" (inference).

### Gaps
- No figure for India- or Kerala-trained radiographers joining the HCPC register each year (needs an HCPC FOI request).
- No NHS England or regional count of radiographers internationally recruited from India, and no current ODEPC/NORKA radiographer drive dates or volumes (hosts blocked).
- No count of Gulf licences issued to Indian radiographers (DHA, DOH, MOH, SCFHS, QCHP).
- No published radiographer-specific Gulf coaching fees in Kerala.
- No PAIR membership count.

---

## 5. Competition intensity in each market, and where the Mallu Radiographer audience sits

### Takeaway
**The UK is contested at the top:**
- Corsmed names UCLH, The Christie, Imperial and Cumbria, and now offers a free tier;
- MRI Education's simulator is bundled free into an £800 SoR-endorsed course;
- ScanLab has a UWE foothold;
- ScanFlo prices UK buyers at $399/yr;
- the SoR gives away free intro CT/MRI e-learning to international recruits.

**India has one direct paid rival** (ScanFlo, Delhi, which has no Kerala presence that I found) plus Corsmed's free tier. No Kerala-based console simulator exists. I found no public data on where the Mallu Radiographer audience lives; that is the single most important missing input.

### Cited Findings
**UK incumbents**
- Corsmed: UK customers named on its own pages are Cumbria, UCLH, The Christie (Manchester) and Imperial College Healthcare (switched from ScanLabMR) [LIVE] — [Corsmed home](https://www.corsmed.com/); [Corsmed for healthcare](https://www.corsmed.com/mri-simulator/for-healthcare)
- Corsmed's education pitch [LIVE] — [Corsmed for education](https://www.corsmed.com/mri-simulator/for-education):
  - "fully vendor-neutral";
  - an LMS with automatic grading;
  - "students complete 500 scan cases";
  - five extra tools: contrast timing, k-space, 3D anatomy, post-processing and image review.
- MRI Education: simulator free inside its £800/£900 course, CPD Now endorsed. It is aimed at radiographers and trainee radiologists, and blocks institutional IP addresses for individual sign-up [LIVE] — [MRI Education](https://www.mrieducation.com/); [Apply](https://www.mrieducation.com/apply/)
- ScanLab: a UWE Bristol lecturer testimonial [EARLIER-NOTES/SEARCH] — [ScanLab](https://scanlabmr.com/)
- SoR: free e-learning for international radiographers, including CT and MRI intro sessions [LIVE] — [SoR 2023](https://www.sor.org/news/role-development/sor-support-for-internationally-educated-radiograp)
- Corsmed free tier: head and knee, 7 (or 8) sequences, "free forever" [LIVE] — [Corsmed free](https://www.corsmed.com/free-mri-simulator)

**India**
- ScanFlo: MRI, CT and PET-CT live, X-ray "soon"; INR pricing; institutional seats; no named customers [LIVE] — [ScanFlo](https://scanflo.io/); [ScanFlo case studies](https://scanflo.io/case-studies)
- Siemens Healthineers India SmartSimulator (vendor-specific); SIMLABS Thrissur (VR clinical simulation, no MRI console); 3D Paramedical resells ScanFlo [EARLIER-NOTES/SEARCH] — [Siemens Healthineers India](https://www.siemens-healthineers.com/en-in/services/customer-services/upskill-services/equipment-and-clinical-education/individual-education-and-practice/smartsimulator); [SIMLABS](https://simlab.in/); [3D Paramedical](https://3dparamedical.com/mri-scanflo)

**Mallu Radiographer audience**
- Brand footprint [EARLIER-NOTES/SEARCH] — [malluradiographer.com About](https://www.malluradiographer.com/about-us/); [Topmate](https://topmate.io/sujesh_soman); [YouTube](https://www.youtube.com/c/MalluRadiographer):
  - YouTube, Facebook, Instagram @malluradiographer, a website and Topmate paid NHS-career sessions;
  - the website describes itself as "radiography education and career guidance, designed for radiographers in the UK".
- Two searches for follower and subscriber counts on 8 Nov 2026 returned nothing for this handle. The platforms and the site were blocked from curl [SEARCH] — [search returned only unrelated "Mallu" creators, e.g. iqfluence list](https://iqfluence.io/public/top-influencers/mallu-influencers)

### Inferences
- **UK universities and big teaching trusts are Corsmed's ground.** Winning them first would mean displacing a funded incumbent that now offers a free tier. Smaller trusts and CDC operators, and especially the international-recruit preceptorship niche, are less contested (inference). The founder's own region is a case in point: The Christie (Manchester) already uses Corsmed, while the new Manchester and Trafford CDC (opened 29 Oct 2026) is a local CT/MRI service needing staff.
- **India is less contested but low-value.** ScanFlo has no visible Kerala footprint, so a Malayalam/Kerala-first, low-price product faces little direct competition locally. The ceiling, however, is ₹999/month (inference).
- **What the audience implies:** the brand's content is UK/NHS careers, and its paid product (Topmate) sells NHS job guidance. Its paying audience is therefore likely Kerala-based aspirants to the UK plus Malayali radiographers already in the UK, rather than Kerala students in general. **This must be checked against the founder's own YouTube Studio and Instagram Insights geography data and Topmate booking countries before deciding** (inference).

### Gaps
- No public audience-size or geography data for Mallu Radiographer (YouTube, Instagram, Facebook, Topmate).
- No list of which UK universities use which simulator, beyond the vendors' own claims.
- I could not confirm whether any UK university or trust uses ScanFlo.

---

## 6. Recommendation inputs: revenue per customer, sales effort, fastest first revenue, and scale

### Takeaway
The per-customer value in the table below is my inference from the live competitor prices above. **Fastest first revenue: Indian (mostly Kerala) radiographers on the way to the NHS, or newly arrived**, sold B2C through the existing Mallu Radiographer audience, priced in GBP for UK-based buyers and INR for India-based aspirants. **Scale: UK NHS departmental licences** (CT/MRI training, international-recruit preceptorship, CDCs) priced below quote thresholds, **plus Kerala college seat licences** sold through the founder's trusted person. UK universities are a later, slower target because Corsmed owns that space.

### Cited Findings
Price anchors, all from sections 1–4:
- Corsmed: US$1,050 for 6 months / US$1,548 for 12 months, plus a free tier [LIVE] — [Corsmed for individuals](https://www.corsmed.com/mri-simulator/for-individuals)
- MRI Education: £800 (£900 from January), sold by NHS PO/SBS [LIVE] — [MRI Education apply](https://www.mrieducation.com/apply/)
- ScanFlo: ₹999/month to ₹14,999/year; US$399–499/year outside India; seats from 10 [LIVE] — [ScanFlo pricing](https://scanflo.io/pricing); [ScanFlo universities](https://scanflo.io/solutions/universities)
- NHS SFI quote tiers of about £5k / £10k / £25–30k [SEARCH], and Procurement Act thresholds of £135,018 / £207,720 [LIVE] — [GOV.UK](https://www.gov.uk/government/publications/procurement-act-2023-guidance-documents-define-phase/guidance-thresholds-html)
- Pay [SEARCH] (see sections 1 and 3):
  - Kerala fresher pay ₹15–25k a month;
  - UK Band 5 £31,049–£37,796 a year.
- Compliance costs:
  - Cyber Essentials £320 + VAT [SEARCH];
  - CPD Now £100–£250 + VAT [LIVE, undated document].

### Inferences
**Segment comparison.** Prices are my proposals, anchored to the competitor prices above. Conversions use ₹126.39 per £1.

| Segment | Suggested price point | Revenue per customer per year | Sales effort / cycle | Competition | Founder advantage |
|---|---|---|---|---|---|
| **A. Indian radiographers in, or bound for, the UK (B2C)**: HCPC/IELTS stage, new NHS starters, band 5 staff moving to CT/MRI | £49–£149 per 3–6 months (UK-based); ₹4,999–₹9,999 pack (India-based aspirants) | about £50–£150 (₹6,300–₹19,000) | Low: content plus link, Stripe GBP / Razorpay INR, days to first sale | Corsmed free tier and £782+ paid; ScanFlo $399; SoR free intro | **Highest**: own NHS story, Malayalam/English, UK-careers audience |
| **B. NHS trust / CDC departmental licence (B2B)**: MRI/CT training leads, practice educators, preceptorship | £1,000–£5,000 a year, a cohort of about 5–20 staff | £1k–£5k (₹1.26–6.3 lakh) | Medium: 1–2 quotes under about £5–10k, PO/SBS supplier set-up, IG questionnaire, Cyber Essentials, CPD Now helps; likely 2–6 months (assumption) | Corsmed at UCLH, Christie, Imperial; MRI Ed group deals | Peer credibility as an NHS radiographer; must declare the conflict of interest |
| **C. UK university cohort licence** | £3k–£15k a year (assumption) | £3k–£15k | High: academic-year timing, IT security and procurement, module-lead buy-in; 6–12+ months | Corsmed (Cumbria, others), ScanLab (UWE) | Low to moderate |
| **D. Kerala students / junior technologists (B2C)** | ₹499–₹999 a month, or ₹2,499–₹4,999 a year | about ₹2,500–₹5,000 (£20–£40) | Low to medium: UPI, WhatsApp and Instagram; price-sensitive; a one-time-payment norm | ScanFlo (₹999/mo, ₹9,999/yr), Corsmed free | Brand plus Malayalam |
| **E. Kerala colleges (B2B seats)** | about ₹1,000–₹3,000 per seat-year × 20–60 seats (assumption) | about ₹30k–₹1.8 lakh (£240–£1,400) | Medium: in-person demos by the trusted person, management sign-off, GST invoicing; 1–3 months (assumption) | ScanFlo seat licences (10-seat pilot) | Trusted local person, Kerala network |
| **F. Gulf-bound Kerala radiographers** | ₹2,999–₹6,999 exam/console bundle, or wholesale through coaching centres | about ₹3k–₹7k | Medium: partner channel (Prometric coaching centres) | Coaching centres' question banks; ScanFlo | Moderate; MRI is only about 10% of the exam |

- **Fastest first revenue: segment A.** It combines the highest per-head price the founder can credibly charge without institutional procurement, near-zero acquisition cost through the existing audience, and the strongest founder-market fit. One free demo scan followed by a paid "NHS CT/MRI console readiness" pack matches the planned funnel.
- **Scale: segment B, plus E as the volume engine in India.** One NHS departmental licence at about £2,000 brings in roughly as much as 400–800 Kerala individual subscriptions at ₹3,000–₹5,000 each. B is where UK revenue scales, but it needs Cyber Essentials, a security summary and DPA, CPD Now endorsement and a conflict-of-interest declaration first. E builds volume and evidence (logbooks, outcomes) at low price.
- **Sequencing:**
  1. Months 0–3: launch A in GBP and INR, using the founder's audience and PAIR webinars as channels.
  2. In parallel, run 2–3 Kerala college pilots (E) through the trusted person, modelled on ScanFlo's 10-seat, one-term pilot, to produce case-study evidence.
  3. Months 3–9: get Cyber Essentials and CPD Now endorsement, then approach small NHS trusts and CDC operators (B) with departmental licences below the quote threshold.
  4. Defer C (universities) and treat F as a partner add-on.
  This sequencing is my inference.
- **Main risks:**
  - Corsmed's free tier caps what pure "MRI practice" can charge, so a CT simulator and India-to-NHS workflow bridging are the needed differentiators;
  - geographic price arbitrage;
  - an unknown audience geography.

### Gaps
- The audience split (Kerala vs UK vs Gulf) and conversion rates for Mallu Radiographer are unknown and decisive. Pull YouTube Studio Geography, Instagram Insights top locations and Topmate booking countries.
- There is no benchmark for NHS department simulator licence prices (all vendors quote privately). Validate by asking 3–5 MRI/CT practice educators what they pay or would pay.
- Kerala college price acceptance and sales cycles are untested. Validate through the trusted person's first 5 college conversations.
- The DTAC/DSPT position for a non-patient training tool is not officially confirmed. Ask the first NHS buyer's IG team early.
