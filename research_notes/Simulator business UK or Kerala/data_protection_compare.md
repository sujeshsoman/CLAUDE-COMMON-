# Data protection, cyber-security and online-consumer rules: UK base vs India (Kerala) base for an online MRI/CT simulator platform (as of 8 November 2026)

General information, not legal advice. Every figure and date is tagged with where it came from. **[LIVE]** means I read it on the primary page itself, fetched with curl through this session's allowlist. **[SEARCH]** means it came only from a search-result summary or secondary commentary.

Hosts I could not reach:
- ico.org.uk returns HTTP 403 even through curl.
- cert-in.org.in, egazette.gov.in, static.pib.gov.in and all law-firm sites are outside the allowlist (CONNECT 403).
- WebFetch could not resolve any host, so every [LIVE] item was fetched with curl.

ICO guidance, the CERT-In primary text and all Gulf material therefore rest on [SEARCH] sources.

Scenario assumptions: student accounts, card/UPI payments, progress tracking, product analytics, marketing emails, and college/hospital licences. Users are in India (many 17–18), the UK and the Gulf. Images are synthetic, so no patient or health data is processed.

---

## 1. UK base: UK GDPR + DPA 2018 as amended by the Data (Use and Access) Act 2025: what changed and what is in force by Nov 2026

### Takeaway
By November 2026 almost all of the DUAA's data-protection and PECR changes are in force. The main package started on 5 February 2026, the new complaints-handling duty on 19 June 2026, and the ICO became the "Information Commission" on 30 September 2026. For a small edtech the changes mostly reduce friction: cookie-consent exemptions for analytics, recognised legitimate interests, and lighter transfer rules. Three things raise the stakes: PECR fines now reach GDPR level, there is a new "children's higher protection matters" duty, and controllers must now run a complaints process.

### Cited Findings
**Commencement status**
- The DUAA received Royal Assent on 19 June 2025 [LIVE]. The government's commencement page was last updated 12 October 2026 [LIVE]. — [GOV.UK: DUAA plans for commencement](https://www.gov.uk/guidance/data-use-and-access-act-2025-plans-for-commencement)
- Commencement No. 6 Regulations (SI 2026/82) brought most of Part 5 into force on **5 February 2026** [LIVE]. Provisions relevant here:
  - s.70 (lawfulness of processing) and Sch 4 (recognised legitimate interests)
  - s.71 and Sch 5 (purpose limitation)
  - s.76 (time limits for subject requests)
  - s.77 (information to data subjects)
  - s.80 and Sch 6 (automated decision-making)
  - s.81 (children's higher protection matters)
  - s.85 and Sch 7 (international transfers)
  - s.101 (penalty notices)
  - s.112 and Sch 12 (cookies / storage and access)
  - s.115 and Sch 13 (Commissioner's PECR enforcement powers)

  — [legislation.gov.uk: SI 2026/82](https://www.legislation.gov.uk/uksi/2026/82/made)
- s.103 (complaints by data subjects) came into force **19 June 2026** [LIVE]. The new DPA 2018 s.164A(3)–(4) complaint-handling duties apply only to complaints a controller receives on or after that date [LIVE]. — [SI 2026/82 regs 3 and 7](https://www.legislation.gov.uk/uksi/2026/82/made)
- Commencement No. 9 (SI 2026/1015) abolished the office of the Information Commissioner. Its functions moved to the new **Information Commission from 30 September 2026** [LIVE]. — [GOV.UK commencement page](https://www.gov.uk/guidance/data-use-and-access-act-2025-plans-for-commencement); [SI 2026/1167 table of earlier commencements: s.117 remaining part, 30 Sept 2026, SI 2026/1015](https://www.legislation.gov.uk/uksi/2026/1167/made)
- The latest regulations, Commencement No. 10 (SI 2026/1167, made 4 Nov 2026, in force 9 Nov 2026), deal only with births and deaths registers. They are not relevant here [LIVE]. — [SI 2026/1167](https://www.legislation.gov.uk/uksi/2026/1167/made)
- The revised UK GDPR text on legislation.gov.uk now names "the Commission" as regulator, for example in Art 33 and Art 27 [LIVE]. — [UK GDPR Art 33](https://www.legislation.gov.uk/eur/2016/679/article/33)

**Lawful bases**
- New Art 6(1)(ea): processing "necessary for the purposes of a recognised legitimate interest" is lawful only if it meets a condition in Annex 1 [LIVE]. — [UK GDPR Art 6](https://www.legislation.gov.uk/eur/2016/679/article/6)
- New Art 6(11): examples of processing that "may be" necessary for legitimate interests include "(a) processing that is necessary for the purposes of direct marketing… (c) processing that is necessary for the purposes of ensuring the security of network and information systems" [LIVE]. — [UK GDPR Art 6](https://www.legislation.gov.uk/eur/2016/679/article/6)

**Children**
- The UK age at which a child can consent to an information society service (where consent is the basis) remains **13** [LIVE]. — [UK GDPR Art 8](https://www.legislation.gov.uk/eur/2016/679/article/8)
- New Art 25(1A)–(1B) (DUAA s.81): providers of information society services "likely to be accessed by children" must take the "children's higher protection matters" into account when designing technical and organisational measures. These are how children can best be protected and supported, and the fact that children "have different needs at different ages and at different stages of development" [LIVE]. In force 5.2.2026 [LIVE]. — [DUAA s.81](https://www.legislation.gov.uk/ukpga/2025/18/section/81)

**Breach reporting and DPO**
- Breach reporting is unchanged in substance. A controller notifies "without undue delay and, where feasible, not later than **72 hours** after having become aware", unless the breach is unlikely to result in risk. Late notice needs reasons [LIVE]. — [UK GDPR Art 33](https://www.legislation.gov.uk/eur/2016/679/article/33)
- A DPO is mandatory only for:
  - public authorities;
  - core activities needing "regular and systematic monitoring of data subjects on a large scale"; or
  - large-scale special-category or criminal data [LIVE].

  — [UK GDPR Art 37](https://www.legislation.gov.uk/eur/2016/679/article/37)

**Data protection fee** (paid to the ICO, now the Commission)
- Since 17 Feb 2025 the tiers are £52 (tier 1, micro), £78 (tier 2, small/medium) and £3,763 (tier 3, large) [LIVE]. — [SI 2025/63](https://www.legislation.gov.uk/uksi/2025/63/made)
- Tier 1 applies where turnover is ≤ £632,000 **or** staff ≤ 10. Tier 2 applies where turnover is ≤ £36 million or staff ≤ 250. Paying by direct debit takes £5 off [LIVE]. — [SI 2018/480 reg 3 (as amended)](https://www.legislation.gov.uk/uksi/2018/480/regulation/3)
- The government chose a 29.8% rise over the 37.2% it consulted on [SEARCH]. — [GOV.UK fee-regime government response](https://www.gov.uk/government/consultations/data-protection-fee-regime-proposed-changes/outcome/data-protection-fee-regime-government-response)

### Inferences
- A one-person UK Ltd pays **£52 a year (£47 by direct debit)**.
- The ICO publishes the fee-exemption self-assessment, and I could not reach it. A paid edtech with marketing and analytics is very unlikely to be exempt.
- The complaints duty (in force 19 June 2026) means the privacy notice and help centre need a route for data-protection complaints, plus a process to acknowledge and respond. The exact statutory timings in DPA 2018 s.164A were not read; see Gaps.
- The recognised-legitimate-interest and direct-marketing examples help with B2B emails to colleges and hospitals. PECR, not UK GDPR, still decides whether a marketing email to an individual needs consent (section 2).

### Gaps
- I could not read the exact wording of DPA 2018 s.164A (complaint acknowledgement within 30 days?) or Annex 1's list of recognised legitimate interests. Read both at legislation.gov.uk before drafting the complaints process.
- I could not verify the ICO fee exemptions or the ICO's current guidance pages (ico.org.uk 403).

---

## 2. UK: PECR marketing emails and cookies (DUAA changes), and the Children's Code

### Takeaway
Under the new PECR Schedule A1, in force 5 Feb 2026, first-party analytics used only to improve the service no longer needs opt-in consent. It still needs clear information and a simple, free way to object. Strictly-necessary uses are widened: security, fraud, faults, login, and remembering selections. Advertising and profiling cookies still need consent. PECR fines now reach UK GDPR level. If 16–17-year-old UK users are "likely" to use the service, the Children's Code (under-18s) applies on top.

### Cited Findings
**Cookies: new PECR Schedule A1** (inserted by DUAA Sch 12, in force 5.2.2026 by SI 2026/82 reg 2(z13)) [LIVE] — [DUAA Sch 12](https://www.legislation.gov.uk/ukpga/2025/18/schedule/12)
- *Consent route:* the user is given clear and comprehensive information and consents. Consent can be signified by "amending or setting controls on the internet browser" or "using another application or programme" [LIVE].
- *Strictly necessary* (no consent, no opt-out): storage or access strictly necessary for a service the user requested. Examples: protecting information provided, device security, preventing or detecting fraud, preventing or detecting technical faults, automatic authentication, and "maintaining a record of selections made on a website, or information put into a website" [LIVE].
- *Statistical purposes* (opt-out model). All of these must hold [LIVE]:
  - the sole purpose is to collect statistics on how the service or website is used, "with a view to making improvements";
  - the information is not shared except to help make those improvements;
  - clear and comprehensive information is given;
  - the user has "a simple means of objecting, free of charge" and does not object.

  The exemption does not cover "collecting or monitoring information automatically emitted by the terminal equipment" [LIVE].
- *Website appearance and functionality preferences:* the same information plus objection model [LIVE].
- The ICO finalised its storage-and-access-technologies guidance in April 2026. It covers pixels as well as cookies, and advertising and profiling still need consent [SEARCH]. — [Womble Bond Dickinson](https://www.womblebonddickinson.com/uk/insights/articles-and-briefings/new-exceptions-non-intrusive-cookies-icos-updated-guidance-has); [Mondaq](https://www.mondaq.com/uk/privacy-protection/1794248/new-exceptions-for-non-intrusive-cookies-the-icos-updated-guidance-has-landed); [Stevens & Bolton](https://www.stevens-bolton.com/insights/102mrve/the-data-use-and-access-act-2025-ico-guidance-on-cookies-and-the-use-of-storag)
- The ICO's draft guidance suggests the statistical exemption covers aggregated data used only by the operator. Vendor commentary warns that GA4 (shares data with Google for its own purposes) may still need consent. This is interpretation, not settled law [SEARCH]. — [Search summary of ICO-guidance commentary; Womble, Mondaq as above]

**PECR enforcement**
- The PECR maximum fine rose from £500,000 to **£17.5 million or 4% of global turnover**, whichever is higher, effective 5 Feb 2026 [SEARCH for the amount]. The relevant provision, Sch 13 (PECR enforcement powers), commenced 5.2.2026 [LIVE]. — [Mayer Brown](https://www.mayerbrown.com/zh-hans/insights/publications/2025/06/the-data-use-and-access-act-pecr-reform-rules-relating-to-electronic-marketing-and-cookies-in-the-uk); [SI 2026/82](https://www.legislation.gov.uk/uksi/2026/82/made)
- DUAA s.114 (soft opt-in extended to **charities**) commenced 5.2.2026 [LIVE]. It does not help a company. — [SI 2026/82](https://www.legislation.gov.uk/uksi/2026/82/made)

**Children's Code (Age Appropriate Design Code)**
- It is a statutory code with 15 standards. It applies to information society services "likely to be accessed" by under-18s in the UK, including services not aimed at children but used by a significant number of them [SEARCH].
- Providers must either establish age with certainty appropriate to the risk or apply the standards to all users [SEARCH].
- In force since 2 Sept 2020 with a 12-month transition [SEARCH].

— [Simmons & Simmons](https://www.simmons-simmons.com/en/publications/ckgs2ty6aadwl0a43e3avb7r3/ico-s-age-appropriate-design-code-comes-into-force); [Mondaq on "likely to be accessed"](https://mondaq.com/uk/data-protection/1357102/childrens-personal-data-and-the-childrens-code-ico-issues-guidance-on-likely-to-be-accessed-by-children); [Brodies](https://brodies.com/insights/ip-technology-and-data/what-do-you-need-to-know-about-the-icos-age-appropriate-design-code/)

### Inferences
- **Marketing emails (UK users):** the soft opt-in (existing customers, similar products, opt-out offered at collection and in every message) still works for a company. Anyone else needs prior consent. Emails to named staff at colleges and NHS trusts are "corporate subscribers" under PECR and can go opt-out, but UK GDPR still applies to the named individual. These are established PECR rules, not re-read this session; verify on the ICO site.
- **Cookies:** the platform can likely run self-hosted, first-party analytics (e.g. Plausible, Matomo, or its own event table) without a consent pop-up, provided it shows clear information and a one-click objection. Meta/Google ad pixels, remarketing or GA4-with-sharing still need an opt-in banner.
- **Progress tracking inside the simulator** (scores, completed modules) is part of the service the user asked for. It is not "storage or access" for advertising, so it does not need PECR consent. It is still personal data under UK GDPR (lawful basis: contract).
- **UK UCAS-age students (16–17)** may use the service, so the Children's Code is engaged unless the platform is credibly 18+ only. Practical approach: high-privacy defaults for everyone, no nudge techniques, no profiling for marketing, geolocation off, and a short DPIA. That costs little, because the service has no social or chat features.

### Gaps
- I could not read the ICO's final April 2026 storage-and-access guidance directly (ico.org.uk 403).
- I found no ICO enforcement against edtech under the Children's Code since DUAA.

---

## 3. UK base with people or servers in India: international transfer rules (UK → India)

### Takeaway
India has **no UK adequacy regulations**. If a UK company lets its trusted person in Kerala, an Indian contractor or an India-hosted server access UK-GDPR data, that is a restricted transfer. It needs an Art 46 safeguard (the ICO's IDTA or the UK Addendum to the EU SCCs) and a documented assessment. Since 5 Feb 2026 that assessment is the lighter **"data protection test"**: protection must be "not materially lower" than in the UK, judged "reasonably and proportionately".

### Cited Findings
- Amended Art 46(1A) requires (a) Art 46(2)/(3) safeguards, such as Secretary of State standard clauses or Commission-issued clauses, **and** (b) that the controller, "acting reasonably and proportionately, considers that the data protection test is met" [LIVE]. — [UK GDPR Art 46](https://www.legislation.gov.uk/eur/2016/679/article/46)
- Art 46(6) defines the test: the protection after transfer "would not be materially lower" than under UK GDPR and DPA 2018. Art 46(7) says what is reasonable and proportionate depends on all the circumstances, "including the nature and volume of the personal data transferred". Amendments are in force 5.2.2026 [LIVE]. — [UK GDPR Art 46](https://www.legislation.gov.uk/eur/2016/679/article/46)
- Standalone UK adequacy regulations on legislation.gov.uk exist only for the Republic of Korea (2022) and the United States (2023). There are none for India [LIVE title search]. Older adequacy carried over from the EU (EEA, Japan etc.) sits in DPA 2018 transitional provisions and does not include India. — [legislation.gov.uk title search "Data Protection (Adequacy)"](https://www.legislation.gov.uk/all?title=Data%20Protection%20(Adequacy))
- ACCA guidance (Feb 2026) says India does not currently have UK adequacy and an Art 46 mechanism is needed [SEARCH]. — [ACCA](https://www.accaglobal.com/uk/en/member/sectors/smp/scaling-practices-toward-tomorrow/people-power-extended-team/data-protection/adequacy-regulations.html)
- The IDTA is the UK tool for transfers to non-adequate countries [SEARCH]. — [Privasee](https://privasee.io/post/international-data-transfer-agreement). UCL publishes a worked transfer-risk assessment for India [SEARCH]. — [UCL TRA India](https://www.ucl.ac.uk/data-protection/sites/data_protection/files/ucl_tra_india.pdf)
- The government evaluated the IDTA in August 2025 and ran a call for evidence, "Data flows you can trust", dated 15 July 2026 [LIVE: titles and dates from the GOV.UK search API only, documents not read]. — [IDTA evaluation](https://www.gov.uk/government/publications/evaluation-of-the-international-data-transfer-agreement); [Data flows you can trust](https://www.gov.uk/government/calls-for-evidence/data-flows-you-can-trust)
- The India–UK CETA has a data-protection annex (Annex 3E). Commentary says it could move India toward UK adequacy, but no adequacy decision has been adopted [SEARCH]. — [Mondaq on CETA Annex 3E](https://webiis08.mondaq.com/india/privacy-protection/1730012/analysing-the-annex-3e-data-protection-and-processing-of-personal-information-under-the-india-uk-ceta)

### Inferences
- **UK Ltd plus Kerala helper with admin access:** sign an IDTA (or Addendum) with the helper or the Indian service entity, and record a short data-protection-test note. Data is low-sensitivity (names, emails, scores, no health data); access is role-limited and encrypted. DPDP takes effect by May 2027, adding an Indian statutory baseline. The "not materially lower" test should be straightforward to document, perhaps 1–2 pages.
- **UK Ltd hosting on AWS Mumbai:** the UK users' data goes to India, so a transfer mechanism is needed. Big cloud providers normally include UK transfer terms in their data processing addenda. I did not verify AWS's terms this session.
- **India Pvt Ltd serving UK users directly:** the Indian company is itself subject to UK GDPR (Art 3(2), section 6). Under the ICO's past position, collecting data directly from UK individuals is not a "restricted transfer", but the Indian controller must still comply with UK GDPR in full. I could not re-verify that position on the ICO site.

### Gaps
- ICO transfer guidance after DUAA (ico.org.uk 403). Whether the ICO has issued a revised IDTA or Addendum, or changed the "transfer risk assessment" tool, since 5 Feb 2026.
- AWS's UK-transfer terms, not checked.

---

## 4. India base: DPDP Act 2023 + DPDP Rules 2025: phased commencement, duties, children, breach, penalties, SDF, transfers

### Takeaway
The DPDP Rules were notified on **13 November 2025** (G.S.R. 846(E)), on a three-stage timetable:
- the Board and definitions applied immediately;
- Consent Manager registration (Rule 4, Act s.6(9)) starts **13 Nov 2026**, five days from now;
- the operative duties start **18 months after publication (≈13 May 2027)**: notice, consent, security, the breach rules, children, rights, transfers, penalties, and the repeal of IT Act s.43A.

Children are under 18, so verifiable parental consent is needed, and tracking, behavioural monitoring and targeted ads aimed at children are banned. Penalties reach ₹250 crore.

In Jan–Feb 2026 MeitY floated compressing 18 months to 12, which would mean 13 Nov 2026. I found no notification adopting it. **Verify that before relying on May 2027.**

### Cited Findings
**Commencement (all [LIVE] from MeitY-hosted Gazette PDFs)**
- G.S.R. 843(E) (Act commencement, Gazette dated Thursday 13 Nov 2025) [LIVE]:
  - *On publication:* s.1(2), s.2, ss.18–26 (Board), s.35, ss.38–43, s.44(1) and (3).
  - *After one year:* s.6(9) (Consent Managers) and s.27(1)(d).
  - *After eighteen months:* ss.3–5, s.6(1)–(8) and (10), ss.7–17, s.27 (except (1)(d)), ss.28–34, ss.36–37, and **s.44(2)**.

  — [MeitY: G.S.R. 843(E)](https://www.meity.gov.in/static/uploads/2025/11/c56ceae6c383460ca69577428d36828b.pdf)
- DPDP Rules 2025, G.S.R. 846(E), Rule 1 [LIVE]:
  - Rules 1, 2 and 17–21 apply on publication.
  - Rule 4 (Consent Managers) applies "one year after".
  - Rules 3, 5–16, 22 and 23 apply "eighteen months after the date of publication".

  — [MeitY: DPDP Rules 2025](https://www.meity.gov.in/static/uploads/2025/11/53450e6e5dc0bfa85ebd78686cadad39.pdf)
- G.S.R. 844(E) of the same date established the Data Protection Board [LIVE: notification seen; text not analysed]. — [MeitY: G.S.R. 844(E)](https://www.meity.gov.in/static/uploads/2025/11/cc217843dc3bcb37b2b05bcc3b4e031f.pdf)
- A corrigendum, G.S.R. 892(E) dated 10 Dec 2025, made 8 typographical corrections to the Rules [LIVE]. — [MeitY corrigendum](https://www.meity.gov.in/static/uploads/2025/12/3c7ebbae0e5456f493f486e6845df86b.pdf)
- The usual citation for the 18-month date is 13 May 2027; a few sources give 14 May [SEARCH]. — [India Briefing](https://www.india-briefing.com/news/india-dpdp-compliance-gdpr-comparison-45702.html); [YourStory](https://yourstory.com/2025/11/digital-personal-data-protection-dpdp-rules-2025-rollout-over-18-months)

**The 12-month compression proposal (unresolved)**
- In Jan–Feb 2026 MeitY sought industry views on cutting the period from 18 to 12 months, which would make it 13 Nov 2026. Feedback was due 4 Feb 2026. March and April 2026 commentary still called it a proposal [SEARCH]. — [S.S. Rana](https://ssrana.in/articles/meity-plans-to-cut-short-dpdp-compliance-timeline-and-notify-cross-border-restrictions-for-sdfs/); [Storyboard18](https://www.storyboard18.com/amp/digital/meity-seeks-industry-views-on-fast-tracking-dpdp-act-rollout-proposes-12-month-compliance-timeline-88332.htm); [Takshashila](https://takshashila.org.in/content/blogs/20260126-meity-considers-reducing-dpdpa-compliance-timelines.html)
- A site-restricted search of meity.gov.in found no 2026 amendment to the DPDP Rules timetable. Late-2026 commentary still cites May 2027 [SEARCH]. — [India Briefing](https://www.india-briefing.com/news/india-dpdp-compliance-gdpr-comparison-45702.html)

**Scope and key duties (Act text [LIVE])** — [MeitY: DPDP Act 2023](https://www.meity.gov.in/static/uploads/2024/06/2bf1f0e9f04e6fb4f8fef35e82c42aa5.pdf)
- *Children:* s.2(f) defines a "child" as an individual "who has not completed the age of eighteen years" [LIVE].
- *Parental consent:* s.9(1) requires "verifiable consent of the parent" before processing a child's personal data [LIVE].
- *No detrimental processing:* s.9(2) bans processing "likely to cause any detrimental effect on the well-being of a child" [LIVE].
- *No tracking or targeting:* s.9(3) says a Data Fiduciary "shall not undertake tracking or behavioural monitoring of children or targeted advertising directed at children" [LIVE].
- *Legitimate uses:* s.7(a) allows processing for the specified purpose for which the person "has voluntarily provided her personal data" without separate consent, unless she objected [LIVE].
- *Grievances:* s.8(10) requires "an effective mechanism to redress the grievances" [LIVE].
- *Significant Data Fiduciary (s.10):* there is **no numeric threshold**. The government designates SDFs by notification, weighing "volume and sensitivity of personal data", risk to rights, sovereignty, electoral democracy, state security and public order [LIVE].
- *Cross-border transfers (s.16(1)):* a negative-list model. The government "may, by notification, restrict the transfer… to such country or territory outside India as may be so notified". s.16(2) preserves stricter sectoral laws [LIVE].
- *Outsourcing exemption (s.17(1)(d)):* most of the Act does not apply where "personal data of Data Principals not within the territory of India is processed pursuant to any contract entered into with any person outside the territory of India by any person based in India" [LIVE].
- *Repeal of s.43A:* s.44(2)(a) says "section 43A [IT Act] shall be omitted" [LIVE]. Under G.S.R. 843(E), s.44(2) commences at 18 months [LIVE].

**Penalties (Act Schedule) [LIVE]**

| Breach | Maximum penalty |
|---|---|
| Security safeguards (s.8(5)) | ₹250 crore |
| Breach notification (s.8(6)) | ₹200 crore |
| Children (s.9) | ₹200 crore |
| SDF duties (s.10) | ₹150 crore |
| Data Principal's own duties (s.15) | ₹10,000 |
| Any other breach | ₹50 crore |

**Rules (operative from ≈13 May 2027) [LIVE]** — [DPDP Rules 2025](https://www.meity.gov.in/static/uploads/2025/11/53450e6e5dc0bfa85ebd78686cadad39.pdf)
- *Rule 3, notice:* it must stand on its own, apart from other information. It must use clear, plain language and include:
  - an "itemised description" of the personal data;
  - the specified purposes and the goods or services provided;
  - a link for withdrawing consent "with the ease of doing so being comparable to that with which such consent was given";
  - how to exercise rights and how to complain to the Board.
- *Rule 6, reasonable security safeguards*, at minimum:
  - encryption, obfuscation, masking or tokens;
  - access control;
  - logs, monitoring and review;
  - backups and continuity;
  - log retention for **one year**;
  - security clauses in processor contracts;
  - technical and organisational measures.
- *Rule 7, breach notification:*
  - each affected person is told "without delay" via their account or registered contact, with a description, consequences, mitigations, safety steps and a contact;
  - the Board is told "without delay";
  - "within seventy-two hours" a detailed report goes to the Board: facts, cause, mitigation, findings on the culprit, remedial measures, and a report on notices given.
- *Rule 8(3):* keep personal data, "associated traffic data and other logs" for a **minimum of one year** from processing (the e-book platform illustration). The Third Schedule erasure timelines apply only to e-commerce entities with ≥2 crore Indian users, online-gaming intermediaries with ≥50 lakh, and social media with ≥2 crore. That is not this platform.
- *Rule 9, contact:* publish the business contact of the DPO "if applicable" or of a person who can answer questions.
- *Rule 10, verifiable parental consent:*
  - the platform must check that the person who identifies as the parent "is an adult who is identifiable";
  - it can rely on identity and age details it already holds, or details "voluntarily provided" by the person or "through a virtual token" from an authorised entity, including DigiLocker;
  - "Adult" means a person who has completed 18.
- *Rule 12 and Fourth Schedule, exemptions from s.9(1) and (3):*
  - **Part A item 3** covers a Data Fiduciary "who is an educational institution". The exemption is limited to "tracking and behavioural monitoring (a) for the educational activities of such institution; or (b) in the interests of safety of children enrolled". "Educational institution" means "an institution of learning that imparts education, including vocational education".
  - **Part B** covers creating a user account "for communicating by email" (limited to email) and confirming that a user is not a child.
- *Rule 13, SDF:* an annual DPIA and audit, algorithmic due diligence, and localisation of data the government specifies after a committee recommends it. SDF only.
- *Rule 14(3), grievances:* publish a response period of **not more than 90 days**.
- *Rule 15, transfers:* data "may be transferred outside the territory of India", subject to any government orders about making data available to foreign states or entities they control.

### Inferences
- **Timeline risk:** if the 12-month compression was quietly adopted, the core duties would start **13 Nov 2026**. That should be ruled out urgently on the e-Gazette, which this session could not reach. Otherwise there are six months to prepare.
- **Children are the single biggest design issue.** Indian 17-year-old first-year radiography students are "children", so direct sign-up needs verifiable parental consent (Rule 10). Per-user progress dashboards or adaptive learning could be argued to be "tracking or behavioural monitoring" (s.9(3)); the Act does not define these terms.
- **Three ways to handle under-18s:**
  1. Make direct-to-consumer (B2C) sign-up 18+, with an age declaration and a refund if someone turns out to be underage.
  2. Onboard under-18s only through **college licences**. The college, an "educational institution", is then the Data Fiduciary for its enrolled students, and the platform acts as its Data Processor under a contract. This fits the Fourth Schedule Part A item 3 exemption, limited to educational-activity tracking.
  3. Build a parental-consent flow (parent account, DigiLocker age token or similar).
- Whether a for-profit online platform is itself an "institution of learning that imparts… vocational education" is untested. That reading is arguable but risky.
- **No DPO is needed** unless the platform is designated an SDF, which is very unlikely at this scale. A named grievance and contact person is needed.
- **SDF and localisation:** the localisation in Rule 13(4) applies only to SDFs. For an ordinary fiduciary, data can be hosted anywhere unless a s.16 negative-list notification names that country (none found).

### Gaps
- No access to egazette.gov.in to confirm that no 2026 amendment to G.S.R. 846(E) or 843(E) exists.
- Whether any s.16 negative-list notification has been issued (none found in searches).
- Whether the Data Protection Board has issued guidance on age assurance or the meaning of "behavioural monitoring" for edtech.
- Reports of constitutional challenges in the Supreme Court were mentioned once [SEARCH, compliancehub.wiki] and not verified.

---

## 5. India: cyber-security and payments: CERT-In Directions 2022, IT Act s.43A / SPDI Rules, RBI card-data and e-mandate rules

### Takeaway
The CERT-In Directions of 28 April 2022 apply to every "body corporate" with no size exemption. MSMEs only got time until 25 Sept 2022. They require **6-hour incident reporting**, a named point of contact, clock sync and **180 days of logs "within the Indian jurisdiction"**. CERT-In's FAQ extends them to foreign entities serving Indian users.

IT Act s.43A and the SPDI Rules 2011 remain the live data-protection law **until ≈13 May 2027**. Card data cannot be stored by merchants (tokenisation). Recurring card or UPI debits follow the RBI's 2026 e-mandate rules (₹15,000 without extra authentication, 24-hour pre-debit notice). Gateways handle most of this.

### Cited Findings
**CERT-In Directions**
- Directions No. 20(3)/2022-CERT-In under IT Act s.70B(6), effective 60 days after issue [SEARCH]:
  - "Any service provider, intermediary, data centre, body corporate and Government organisation shall mandatorily report cyber incidents as mentioned in Annexure I to CERT-In within 6 hours";
  - ICT logs must be kept for "a rolling period of 180 days… within the Indian jurisdiction";
  - non-compliance may draw action under s.70B(7).

  — [CERT-In Directions PDF (search excerpt)](https://www.cert-in.org.in/PDF/CERT-In_Directions_70B_28.04.2022.pdf); [CERT-In FAQ (search excerpt)](https://www.cert-in.org.in/PDF/FAQs_on_CyberSecurityDirections_May2022.pdf)
- The 27 June 2022 order extended the effective date for **MSMEs to 25 Sept 2022** and deferred the KYC-validation sub-directions 5(a)/(f) for data centres, VPS, VPN and cloud providers [SEARCH]. — [CERT-In extension order (search)](https://www.cert-in.org.in/PDF/CERT-In_directions_extension_MSMEs_and_validation_27.06.2022.pdf); [MediaNama](https://www.medianama.com/2022/06/223-cert-in-extends-deadline-compliance-cybersecurity/); [IFF](https://internetfreedom.in/delaying-the-inevitable-implementation-of-cert-ins-cybersecurity-directions-gets-a-piecemeal-extension/)
- The FAQs (18 May 2022) say the Directions cover body corporates **outside India** for incidents if they provide services to Indian users, and such entities must designate a point of contact [SEARCH].
- **Sources conflict on log storage.** One firm reads the FAQ as allowing logs to be stored abroad if they can be produced to CERT-In in reasonable time. Another says foreign providers must keep certain records in India [SEARCH]. — [Khaitan & Co on FAQs](https://khaitanco.com/thought-leaderships/Decoding-the-new-CERT-In-Directions:-Government-releases-the-much-awaited-FAQs); [Mondaq](https://www.mondaq.com/india/it-and-internet/1195166/decoding-the-new-cert-in-directions-government-releases-the-much-awaited-faqs)

**IT Act s.43A / SPDI Rules**
- s.43A is omitted only when DPDP s.44(2) commences, which is the 18-month stage [LIVE]. — [DPDP Act](https://www.meity.gov.in/static/uploads/2024/06/2bf1f0e9f04e6fb4f8fef35e82c42aa5.pdf); [G.S.R. 843(E)](https://www.meity.gov.in/static/uploads/2025/11/c56ceae6c383460ca69577428d36828b.pdf)
- Commentary agrees that s.43A and the SPDI Rules stay operative until about 13 May 2027. Firms should keep an SPDI-style privacy policy, consent and security practices until then [SEARCH]. — [King Stubb & Kasiva](https://ksandk.com/data-protection-and-data-privacy/what-happens-spdi-rules-after-dpdp-enforcement/)

**RBI rules**
- *Card-on-file:* from 1 Oct 2022 no entity in the card chain other than card issuers and networks may store card-on-file data. Tokenisation replaces it, and guest checkout allows storage until T+4 or settlement [SEARCH]. — [RBI notifications (search)](https://rbi.org.in/Scripts/NotificationUser.aspx?Id=12159). The December 2021 circular, which extended the deadline to 30 June 2022 and required purging after it, was read [LIVE]. — [RBI circular Dec 2021](https://www.rbi.org.in/Scripts/NotificationUser.aspx?Id=12211)
- *E-mandates:* the RBI "Digital Payments – E-mandate Framework, 2026" is dated **21 April 2026** and effective immediately [LIVE]. It applies to recurring transactions "domestic or cross-border, using cards / PPI / UPI" [LIVE]:
  - recurring debits are allowed without extra authentication (AFA) "up to ₹15,000/- per transaction";
  - insurance, mutual funds and credit-card bills are allowed up to ₹1,00,000;
  - issuers must send a pre-transaction notification "at least 24 hours prior";
  - customers can opt out of a debit or the mandate.

  — [RBI E-mandate Framework 2026](https://www.rbi.org.in/Scripts/NotificationUser.aspx?Id=13374)

### Inferences
- **CERT-In is the one India rule that most clearly favours hosting in India.** A Kerala company, or any company serving Indian users, should keep a 180-day log store (application, auth, firewall/WAF and cloud audit logs) in an Indian region (AWS Mumbai or Hyderabad). It should also have a 6-hour incident-reporting runbook and a named point of contact.
- For a UK company the extraterritorial reach rests on a 2022 FAQ, and enforcement against small foreign edtechs is undocumented. Hosting logs in Mumbai removes the question cheaply anyway.
- **Payments:** using Razorpay, Stripe or Paddle hosted checkout means the platform never touches card numbers, which satisfies the RBI tokenisation and SPDI financial-data concerns.
- **Subscriptions under ₹15,000 per charge** (all realistic student plans) can auto-renew without extra authentication. The bank sends a 24-hour pre-debit notice. Annual college licences above ₹15,000 should go by invoice or bank transfer, not e-mandate.

### Gaps
- I could not read the CERT-In Directions, FAQ or extension order directly (cert-in.org.in blocked), so the FAQ's foreign-entity and log-location wording is from commentary only.
- I found no CERT-In enforcement against small edtechs.
- I did not read the SPDI Rules 2011 text this session. Their definition of "sensitive personal data" (passwords, financial details, health) and the privacy-policy requirement come from general knowledge and need verification.

---

## 6. Extraterritorial reach: rules that follow the customer, not the company (DPDP s.3(b), UK GDPR Art 3(2)/Art 27, Gulf PDPLs)

### Takeaway
**The base does not let the founder escape either regime.**
- DPDP applies to a UK company offering services to people in India (s.3(b)).
- UK GDPR applies to an Indian company offering services to people in the UK (Art 3(2)). It also requires a written UK Art 27 representative unless UK processing is only "occasional" and low-risk.
- UAE and Saudi PDPLs both claim reach over foreign controllers processing their residents' data. Saudi Arabia opened controller registration for overseas organisations in October 2026.

### Cited Findings
**DPDP s.3(b)**
- The Act also applies "to processing of digital personal data outside the territory of India, if such processing is in connection with any activity related to offering of goods or services to Data Principals within the territory of India" [LIVE]. — [DPDP Act s.3](https://www.meity.gov.in/static/uploads/2024/06/2bf1f0e9f04e6fb4f8fef35e82c42aa5.pdf)
- s.3(a) covers all processing "within the territory of India", so an Indian company is covered for all users. Only the s.17(1)(d) outsourcing carve-out (foreign users' data processed under contract with a foreign person) narrows this [LIVE].

**UK GDPR Art 3 and Art 27**
- Art 3(1) applies "in the context of the activities of an establishment… in the United Kingdom, regardless of whether the processing takes place in the United Kingdom or not" [LIVE].
- Art 3(2) applies to controllers not established in the UK where processing relates to "(a) the offering of goods or services, irrespective of whether a payment of the data subject is required, to such data subjects in the United Kingdom; or (b) the monitoring of their behaviour" [LIVE].

— [UK GDPR Art 3](https://www.legislation.gov.uk/eur/2016/679/article/3)
- Art 27: where Art 3(2) applies, the controller "shall designate in writing a representative in the United Kingdom" [LIVE]. The exemption covers processing that is "occasional", excludes large-scale special-category or criminal data, and is "unlikely to result in a risk". The representative is addressed by "the Commission and data subjects", and appointing one does not remove the controller's liability [LIVE]. — [UK GDPR Art 27](https://www.legislation.gov.uk/eur/2016/679/article/27)
- Commercial Art 27 representative prices (vendor pages) [SEARCH]:
  - AWS Marketplace "REP27": US$326 a year (up to 10 forwarded requests) or US$551 (unlimited);
  - euverify: £490 a year for start-ups;
  - IT Governance: €875 a year for a micro tier.

  — [AWS Marketplace listing](https://aws.amazon.com/marketplace/pp/prodview-7aidli3kkc2ya); [euverify](https://euverify.com/appoint-your-gdpr-representative-in-the-eu-uk/); [IT Governance](https://www.itgovernance.eu/shop/product/gdpr-uk-representative)

**UAE PDPL** (Federal Decree-Law 45/2021)
- Art 2(1)(c) covers controllers and processors "residing outside the State" that process personal data of data subjects inside the UAE [SEARCH].
- It excludes free zones with their own data law (DIFC, ADGM) and certain government, health and banking data [SEARCH].
- Transfers abroad need "adequate" protection, with details deferred to the Executive Regulations [SEARCH].
- The Executive Regulations' status is **disputed**: several 2026 sources say they are still unpublished, so enforceability and penalty detail are uncertain [SEARCH].

— [Mondaq overview](https://www.mondaq.com/data-protection/1389892/an-overview-of-the-uae-personal-data-protection-law); [SMEX](https://smex.org/uaes-data-protection-law-between-exceptions-and-exemptions/); [BusinessDubai](https://www.businessdubai.ae/blogs/uae-pdpl-data-protection); [Simmons & Simmons FAQ](https://www.simmons-simmons.com/en/publications/ckwugz8lu16rs0a44qvbqcbz9/uae-personal-data-protection-law-faqs)

**Saudi PDPL**
- It applies to processing outside the Kingdom of data about Saudi residents [SEARCH].
- In October 2026 SDAIA launched registration in its national register of controllers for organisations outside Saudi Arabia, including those without a Saudi commercial registration. The steps include appointing an authorised representative [SEARCH].
- Registration is mandatory only for certain categories: public entities, organisations whose core activity is data processing, and organisations handling sensitive data [SEARCH].
- Penalties reach SAR 5 million [SEARCH].
- Sources differ on whether a Saudi representative is strictly mandatory for all foreign controllers [SEARCH].

— [Clyde & Co (Oct 2026)](https://www.clydeco.com/en/insights/2026/10/sdaia-opens-controller-registration-for-overseas-o); [TCSA PDPL](https://www.tcsa.in/frameworks/pdpl); [Middle East Briefing](https://www.middleeastbriefing.com/news/navigating-saudi-arabias-personal-data-protection-law-and-regulatory-framework)

### Inferences
**UK Ltd base. Applies to every user:**
- UK GDPR, because of the UK establishment (Art 3(1)). Indian and Gulf users' data is processed to UK GDPR standards too.
- ICO fee.

On top for Indian users:
- DPDP via s.3(b), including the under-18 parental-consent and no-tracking rules;
- arguably CERT-In (FAQ);
- the E-Commerce Rules (section 7).

On top for Gulf users: the UAE and Saudi PDPLs (low practical burden while small). No UK representative is needed.

**India Pvt Ltd base. Applies to every user:**
- DPDP for all processing in India (s.3(a));
- CERT-In in full;
- SPDI and s.43A until May 2027.

On top for UK users:
- UK GDPR via Art 3(2);
- a UK Art 27 representative (≈£250–£700 a year) unless UK sales are genuinely occasional, which a marketed UK offer would not be;
- the Children's Code if UK under-18s are likely;
- PECR for marketing and cookies;
- UK consumer law (section 7).

**Net effect:** the "away" market's privacy law applies either way. A UK base means one regime (UK GDPR) as the global floor, with DPDP layered on for Indian users. An India base means DPDP as the floor plus UK GDPR for UK users, a paid UK representative, and stricter cyber rules (CERT-In) at home. Because the platform handles no health data, the substantive duties are similar in both cases.

### Gaps
- I could not read the UAE PDPL or SDAIA primary texts (hosts not allowlisted).
- Whether the UAE Executive Regulations have been gazetted.
- Saudi parental-consent rules for minors (Saudi PDPL), not researched.

---

## 7. Online consumer and subscription rules: UK (DMCC Act, CCRs, CMA) and India (E-Commerce Rules, dark patterns, refunds)

### Takeaway
UK consumer law follows UK consumers, whatever the base. The CMA has fined companies directly since April 2025, up to 10% of global turnover. The new **DMCC subscription regime is not yet in force; the government expects it in spring 2027**. It brings reminders, easy online exit, and a second 14-day cooling-off after a trial or 12-month+ auto-renewal.

The current CCR rule still applies: digital content can start immediately only with express consent and an acknowledgement that the right to cancel is lost.

In India, the E-Commerce Rules 2020 (grievance officer, 48 h / 1 month) and the CCPA's dark-patterns regime apply. That regime has been enforced against edtech: PhysicsWallah was fined in June 2026.

### Cited Findings
**UK**
- *CCR reg 37 (in force):* for digital content not on a tangible medium, the trader must not start supply within the 14-day cancellation period unless the consumer "has given express consent" and "has acknowledged that the right to cancel… will be lost". If confirmation is not provided, the consumer pays nothing for content supplied in the period [LIVE]. — [Consumer Contracts Regulations 2013 reg 37](https://www.legislation.gov.uk/uksi/2013/3134/regulation/37)
- *DMCC subscription regime*, per the government response (page updated 2 April 2026) [LIVE]:
  - clear pre-contract information;
  - reminders, "particularly before trials or 12 month+ contracts auto-renew";
  - straightforward exit, including online exit if the consumer signed up online;
  - a 14-day **renewal cooling-off** after a trial or 12-month+ auto-renewal;
  - the initial digital-content waiver is retained, but a **proportionate refund** is due if a consumer cancels in the renewal cooling-off;
  - if the trader fails to inform the consumer, the cooling-off extends up to 12 months;
  - refunds are due within 14 days;
  - terms that make cancelling auto-renewal disproportionately difficult are banned.

  "We will legislate when parliamentary time allows and we anticipate that the regime will **commence in spring 2027**" [LIVE]. — [DBT government response](https://www.gov.uk/government/consultations/consultation-on-the-implementation-of-the-new-subscription-contracts-regime/outcome/government-response-to-consultation-on-the-implementation-of-the-new-subscription-contracts-regime-web-accessible-version)
- *CMA direct enforcement:* in force since 6 April 2025, with fines up to the higher of £300,000 or 10% of global turnover [SEARCH]. — [Macfarlanes](https://www.macfarlanes.com/insights/102o47w/taking-stock-of-the-first-18-months-of-the-cmas-new-direct-consumer-enforcement/)
- The first procedural fine came in February 2026. The first substantive penalty was **£4.2 million** on AA Driving School and BSM for drip pricing (15 April 2026), with refunds to 80,000+ learners [SEARCH]. By 23 June 2026 the CMA reported >£5 million in fines and >£1.95 million in refunds [SEARCH]. — [Mondaq: first fine](https://www.mondaq.com/uk/antitrust-eu-competition/1748222/cma-issues-first-fine-under-new-direct-consumer-enforcement-powers); [Mondaq: drip pricing](https://webiis08.mondaq.com/uk/dodd-frank-consumer-protection-act/1777758/cma-imposes-first-financial-penalty-under-new-consumer-powers-in-drip-pricing-crackdown)

**India**
- *Consumer Protection (E-Commerce) Rules 2020* (G.S.R. 462(E), 23 July 2020): commentary reads them as covering foreign entities offering goods or services to Indian consumers [SEARCH]. A grievance officer must acknowledge complaints within 48 hours and redress them within one month, with name and contact displayed [SEARCH]. — [IndiaLaw summary](https://www.indialaw.in/guides/civil/consumer-protection-e-commerce-rules/); [Mondaq](https://mondaq.com/india/dodd-frank-consumer-protection-act/985606/the-consumer-protection-e-commerce-rules-2020)
- *CCPA dark-patterns guidelines:* effective 30 Nov 2023, listing 13 practices, including subscription traps and silent auto-renewal [SEARCH, from earlier notes]. — [Mondaq Dec 2023](https://mondaq.com/india/consumer-trading-unfair-trading/1398262/ccpa-issues-guidelines-for-prevention-and-regulation-of-dark-patterns-2023-effective-30-november-2023)
- *Self-audit advisory:* on 5 June 2025 the CCPA asked e-commerce platforms to self-audit within 3 months [SEARCH]. — [AZB & Partners](https://www.azbpartners.com/bank/central-consumer-protection-authority-issues-advisory-to-e-commerce-platforms-for-self-audit-to-detect-dark-patterns-on-their-platforms/)
- *PhysicsWallah (edtech) order, early June 2026:* dark patterns, including mandatory data collection to open "free" content and basket sneaking. Penalty **₹5,00,000**. McAfee India was penalised at the same time [SEARCH]. — [Mondaq](https://www.mondaq.com/india/dodd-frank-consumer-protection-act/1799382/dark-patterns-in-ed-tech-ccpa-imposes-penalty-on-physicswallah); [ETV Bharat](https://www.etvbharat.com/amp/en/bharat/ccpa-slaps-fines-on-physicswallah-mcafee-for-dark-pattern-practices-enn26060303886)

### Inferences
- **UK checkout now:** a CCR-compliant "start now, I understand I lose my 14-day right" checkbox, and an order-confirmation email repeating it. Without that, a UK student can cancel within 14 days and pay nothing.
- **Build now for spring 2027:** renewal reminders before annual renewals, a one-click online cancel, and pro-rata refunds in the 14 days after renewal. These are cheap to do now and avoid a retrofit.
- **India:** a published grievance officer and contact, a clear refund policy, and no pre-ticked add-ons. Also: no forcing sign-up or phone number to view "free" demos, which was the PhysicsWallah issue, and no hidden auto-renew.
- **Both bases:** these consumer rules follow the customer. UK rules bind sales to UK consumers whether the company is in Manchester or Kochi, and Indian rules bind sales to Indian consumers from a UK company too.
- **Licences to colleges and hospitals are B2B.** Consumer cancellation and subscription rules do not apply. Contract and data-processing terms do.

### Gaps
- I did not read the E-Commerce Rules 2020 primary text, so the exact "systematically offers" foreign-entity wording is unverified.
- I did not find any India-specific statutory refund period for digital courses; it seems to be policy-based plus the dark-patterns rules.
- No CMA enforcement found against edtech or online-course subscriptions.
- Gulf consumer law not researched.

---

## 8. Practical burden and cost, and which base is genuinely "less hassle"

### Takeaway
For a tiny, health-data-free edtech, the **data-protection burden is similar either way and is not a strong reason to choose a base**. The rules that bite hardest follow the customer: DPDP's under-18 rules for Indian students, UK GDPR, PECR and the Children's Code for UK users, and each country's consumer law. Small differences:
- A **UK base** adds only a £52 fee and IDTA paperwork if the Kerala helper or Indian hosting touches data, but puts all users under UK GDPR.
- An **India base** avoids the ICO fee but adds a UK Art 27 representative (≈£250–£700 a year), full CERT-In duties (6-hour reporting, Indian log retention) and SPDI until May 2027.

### Cited Findings
- UK fee: £52 for tier 1 (≤ £632k turnover or ≤ 10 staff), less £5 by direct debit [LIVE]. — [SI 2025/63](https://www.legislation.gov.uk/uksi/2025/63/made); [SI 2018/480 reg 3](https://www.legislation.gov.uk/uksi/2018/480/regulation/3)
- UK Art 27 representative services cost about US$326–551, £490 or €875 a year [SEARCH]. — [AWS Marketplace](https://aws.amazon.com/marketplace/pp/prodview-7aidli3kkc2ya); [euverify](https://euverify.com/appoint-your-gdpr-representative-in-the-eu-uk/); [IT Governance](https://www.itgovernance.eu/shop/product/gdpr-uk-representative)
- DPDP has no size exemption [SEARCH]. Vendor quotes run ₹15 lakh to ₹2 crore. One practitioner argues a startup with under 10,000 users can comply for under ₹50,000 a year. Fractional DPO services cost ₹2–8 lakh a year [SEARCH]. These are interested sources. — [dev.to (ecorpit)](https://dev.to/mr_manushukla/dpdp-compliance-costs-for-indian-startups-what-to-budget-before-13-may-2027-fi8); [Inc42](https://inc42.com/features/dpdp-act-compliance-indian-startups-moving-at-different-speeds/)
- A DPO is not required under UK GDPR for this profile (no large-scale systematic monitoring or special-category data) [LIVE]. — [UK GDPR Art 37](https://www.legislation.gov.uk/eur/2016/679/article/37)
- DPDP requires only a contact person unless the company is an SDF [LIVE]. — [DPDP Rules r.9](https://www.meity.gov.in/static/uploads/2025/11/53450e6e5dc0bfa85ebd78686cadad39.pdf)

### Inferences
These are my own estimates for a solo founder plus one helper. They are not sourced quotes.

**Common to both bases (≈ 4–8 working days of founder time):**
- one combined privacy notice: a UK GDPR section plus a separate standalone DPDP notice that meets Rule 3;
- a record of processing;
- a short DPIA covering children and analytics;
- breach runbooks: UK 72 h, DPDP "without delay" plus 72 h, CERT-In 6 h;
- processor contracts (AWS, payment gateway, email tool);
- a retention schedule with a ≥1-year log floor (DPDP Rules 6 and 8);
- an age gate or parental-consent flow;
- grievance and complaints handling: DPDP ≤90 days, UK s.103 process, India E-Commerce 48 h acknowledgement.

**Common cash costs:** a template or tool-generated policy pack (≈£0–£300), a cookie tool (£0 if only first-party exempt analytics are used; ≈£10–£50 a month if ad pixels are used), and an optional one-off lawyer review (≈£500–£1,500 UK or ₹25,000–₹75,000 India).

**Extra for a UK base:**
- the £52 fee;
- an IDTA plus a data-protection-test note for Kerala access or Indian hosting (≈1 day, or a lawyer template);
- the DPDP notice and parental-consent design for Indian users anyway.

**Extra for an India base:**
- a UK representative (≈£250–£700 a year);
- a CERT-In point of contact and 6-hour process;
- 180-day logs in India;
- an SPDI-compliant policy until May 2027 (then superseded);
- UK GDPR, PECR and the Children's Code for UK users anyway.

**Verdict on "less hassle":** marginally the **UK**, for data protection specifically, because it removes the Art 27 representative and makes CERT-In less certain. But the difference is a few hundred pounds and a few days. Tax, banking, payment acceptance and the founder's residence will matter far more.

**Unavoidable either way:**
- DPDP for Indian users, including under-18 parental consent and no tracking or targeted ads (from ≈May 2027, possibly sooner);
- UK GDPR, PECR and the UK consumer and subscription rules for UK users;
- the Indian E-Commerce and dark-patterns rules for Indian consumers;
- Gulf PDPLs for Gulf users;
- the payment-gateway rules (RBI tokenisation and e-mandate) for Indian card and UPI payments.

### Gaps
- No primary price data found for cookie-consent tools, policy generators or lawyer fixed fees in this session. The figures above are labelled as my estimates.
- No data found on actual ICO, Commission or Data Protection Board enforcement against micro edtechs.

---

## 9. Where should servers be? Localisation, and AWS Mumbai vs London

### Takeaway
**Neither law requires general in-country storage.** DPDP uses a negative list (s.16) with no country notified that I found, and localisation applies only to SDFs for specified data (Rule 13(4)). UK GDPR has no localisation and only regulates exports.

The one location-specific rule is **CERT-In's 180-day logs "within the Indian jurisdiction"**. A sensible split is application data in one region and a log archive in AWS Mumbai or Hyderabad if serving India. A UK company storing UK users' data in Mumbai needs a UK transfer mechanism. Data residency in London does not stop DPDP applying to Indian users.

### Cited Findings
- DPDP s.16: transfer restricted only to countries "so notified" [LIVE]. Rule 15: transfers allowed subject to government requirements about foreign-state access [LIVE]. Rule 13(4): SDF localisation of specified data [LIVE]. — [DPDP Act](https://www.meity.gov.in/static/uploads/2024/06/2bf1f0e9f04e6fb4f8fef35e82c42aa5.pdf); [DPDP Rules](https://www.meity.gov.in/static/uploads/2025/11/53450e6e5dc0bfa85ebd78686cadad39.pdf)
- CERT-In: logs kept for 180 days "within the Indian jurisdiction" [SEARCH]. Sources conflict on whether foreign entities may store them abroad if they can be produced promptly [SEARCH]. — [CERT-In Directions (search excerpt)](https://www.cert-in.org.in/PDF/CERT-In_Directions_70B_28.04.2022.pdf); [Khaitan & Co](https://khaitanco.com/thought-leaderships/Decoding-the-new-CERT-In-Directions:-Government-releases-the-much-awaited-FAQs)
- UK transfers to India need Art 46 safeguards plus the data protection test [LIVE]. — [UK GDPR Art 46](https://www.legislation.gov.uk/eur/2016/679/article/46)
- AWS regions exist for Asia Pacific (Mumbai) `ap-south-1`, Asia Pacific (Hyderabad) `ap-south-2`, Europe (London) `eu-west-2`, Middle East (UAE) `me-central-1` and Middle East (Bahrain) `me-south-1` [LIVE]. AWS has also announced a region in Saudi Arabia [LIVE]. — [AWS Regions and AZs](https://aws.amazon.com/about-aws/global-infrastructure/regions_az/)
- The RBI e-mandate framework covers cross-border recurring transactions too [LIVE]. — [RBI](https://www.rbi.org.in/Scripts/NotificationUser.aspx?Id=13374)

### Inferences
**UK Ltd, most users in India:**
- Option A, everything in London (`eu-west-2`):
  - no UK export issue for the primary data, but Kerala admin access still needs an IDTA;
  - Indian latency is higher;
  - CERT-In logs abroad rely on the contested FAQ reading.
- Option B, everything in Mumbai (`ap-south-1`):
  - best Indian latency and CERT-In-safe;
  - UK users' data is exported to India, so an IDTA or AWS transfer terms plus a data-protection-test note are needed.

  Option B is probably the better fit if India is the main market.

**India Pvt Ltd:**
- Mumbai (or Hyderabad) is natural and CERT-In-compliant.
- UK users' data in India is lawful under DPDP. UK GDPR applies to it via Art 3(2), but this is direct collection, not an export by a UK exporter. Verify the ICO's view.

**Gulf users:** there is no clear localisation duty for a foreign edtech. The UAE PDPL transfer rules are pending Executive Regulations.

**Simplest compliant default:** one primary region near most users, encryption at rest and in transit, a 180-day+ log archive in an Indian region (which also meets DPDP's 1-year log minimum if kept for a year), and documented transfer paperwork for any UK-to-India flows.

### Gaps
- I did not verify AWS's data processing addendum and its UK/IDTA coverage.
- No MeitY s.16 negative list found. Absence of evidence is not proof that none exists; the e-Gazette was not reachable.
