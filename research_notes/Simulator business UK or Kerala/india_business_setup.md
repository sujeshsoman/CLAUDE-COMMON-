# Setting up and running the MRI/CT simulator business as an Indian (Kerala) entity: NRI founder in Manchester, as of November 2026

These notes are general information, not legal or tax advice. Indian company, FEMA and tax rules (including the new Income-tax Act, 2025) should be confirmed with a Kerala chartered accountant (CA) or company secretary (CS) before acting.

**Provenance tags.** [LIVE] means I read the figure on the fetched page itself, via curl through the session proxy. [SEARCH] means it comes only from a search-result summary, usually of a commercial CA or filing-service blog, and is unverified.

**Access problems.** Several primary sites could not be read:
- **www.mca.gov.in:** returned HTTP 403.
- **www.incometaxindia.gov.in:** returned "Access Denied" (HTTP 403) on every page tried.
- **Blocked by the proxy:** assets.publishing.service.gov.uk (the HMRC PDF of the India–UK treaty) and startupinfinity.startupmission.in.
- **KSUM FAQ:** the page renders by JavaScript and returned no text.

As a result, all Companies Act, Income-tax Act and treaty figures below are [SEARCH] unless marked otherwise. The figures from the KSUM site, the startupindia.gov.in recognition page, the RBI Master Direction, Razorpay and gov.uk are [LIVE].

---

## 1. Entity options (Pvt Ltd, LLP, OPC, sole proprietorship): ownership by a UK-resident NRI, incorporation and company-law compliance

### Takeaway
A **Private Limited company** with the Kerala-based person as the resident director (and ideally a minority shareholder) is the only structure that unlocks the full set of KSUM grants and loans, DPIIT recognition and the tax holiday. Pvt Ltd and LLP are each eligible for all of those benefits. An OPC is technically open to NRIs since 2021, but it is a poor fit. It cannot have a co-founder shareholder, and it is excluded from the KSUM productisation grant, the KSUM seed loan and the 80-IAC tax holiday. A sole proprietorship run by the Kerala person would put the business legally in someone else's name and cannot get DPIIT recognition.

The trade-off is compliance. Every company needs a statutory audit from day one, whatever its size. An LLP needs an audit only above ₹40 lakh turnover or ₹25 lakh contribution, but it is weaker for future equity investment.

### Cited Findings
**OPC rules**
- The Companies (Incorporation) Second Amendment Rules, 2021, effective 1 April 2021, allowed NRIs to form a One Person Company. The rule now says "whether resident in India or otherwise". The residency period used in the OPC rules was cut from 182 to 120 days [SEARCH] — [Mondaq](https://www.mondaq.com/india/corporate-and-company-law/1055252/nris-can-now-form-one-person-company); [S.S. Rana](https://ssrana.in/articles/india-nris-one-person-company/); [Moneylife](https://www.moneylife.in/article/mca-eases-norms-for-one-person-companies-lets-nris-in/62854.html)

**Resident director and designated partner**
- Section 149(3) of the Companies Act, 2013 is still described as requiring every company to have at least one director who stayed in India for **at least 182 days in the financial year** [SEARCH].
- For LLP designated partners, the resident test is **120 days** [SEARCH]. Sources conflict on whether the 120-day figure applies more widely; one calls it an expired COVID relaxation for companies.
- Sources: [SetIndiaBiz](https://www.setindiabiz.com/blog/resident-director-vs-designated-partner-residency-rules); [TaxAJ](https://www.taxaj.com/learn/?p=518)

**Which entity types each scheme accepts**
- **DPIIT recognition:** open only to entities "incorporated as a Private Limited Company or registered as a Partnership Firm, Limited Liability Partnership, or Cooperative Society" [LIVE]. Sole proprietorships and OPCs are not named. Applications go through the National Single Window System (nsws.gov.in), and DPIIT charges no fee [LIVE] — [Startup India recognition page](https://www.startupindia.gov.in/content/sih/en/startupgov/startup_recognition_page.html)
- **80-IAC tax holiday:** "Only Private limited or a Limited Liability Partnership is eligible", and the entity must have been incorporated after 1 April 2016 [LIVE] — [Startup India recognition page](https://www.startupindia.gov.in/content/sih/en/startupgov/startup_recognition_page.html)
- **KSUM Idea Grant:** incorporation as Pvt Ltd, LLP or OPC is mandatory before the money is paid out, and only innovators based in Kerala can apply [LIVE] — [KSUM Idea Grant](https://startupmission.kerala.gov.in/schemes/idea-grant)
- **KSUM Productisation Grant:** the startup "Must be incorporated as Pvt Ltd / LLP with active MCA status". OPC is not listed [LIVE] — [KSUM Productisation Grant](https://startupmission.kerala.gov.in/schemes/productisation-grant)
- **KSUM Seed Loan:** the startup must be "a registered company in Kerala as an LLP or Pvt. Ltd company" with DPIIT registration and 'Active'/'Active Compliant' MCA status. Form INC-22A must be done before funds are paid out [LIVE] — [KSUM Seed Fund](https://startupmission.kerala.gov.in/schemes/seed-fund)

**Incorporation cost and process (SPICe+)**
- No MCA filing fee where authorised capital is up to ₹15 lakh [SEARCH].
- Kerala stamp duty is about ₹3,025 at ₹1 lakh authorised capital (₹25 on the e-form, ₹1,000 on the MOA, ₹2,000 on the AOA). The AOA duty rises above ₹10 lakh of capital [SEARCH]. Sources give other formulas, such as 0.15% of capital, so check the portal's own calculation.
- DIN: one source says ₹500 per director, with the first two free via SPICe+; another says free for up to three. These conflict [SEARCH].
- Name reservation (RUN): ₹1,000 [SEARCH].
- Professional fees: from ₹1,999 plus government fees, up to a typical ₹7,000–25,000 in total [SEARCH].
- Kerala companies register with ROC Ernakulam [SEARCH].
- Sources: [IncorpX Kerala fees](https://www.incorpx.io/blog/company-registration-fees-kerala-complete-cost); [StartupGrantsIndia Kochi](https://www.startupgrantsindia.com/services/private-limited-company-registration/in/kochi); [Patron estimator](https://www.patronaccounting.com/tools/incorporation-cost-estimator)

**Annual company compliance**
- The board must appoint the first auditor within 30 days of incorporation. This applies to "every company … regardless of its size, turnover, or business activity", including OPCs [SEARCH].
- Form INC-20A (declaration that business has commenced) is due within 180 days of incorporation [SEARCH].
- Sources: [Patron: first auditor](https://www.patronaccounting.com/blog/first-auditor-appointment-adt1-filing-guide); [SetMyCompany](https://setmycompany.com/first-auditor-appointment-after-incorporation-india-checklist/)
- AOC-4 (accounts) is due within 30 days of the AGM, and MGT-7/7A (annual return) within 60 days. AOC-4 must be filed first [SEARCH].
- Late filing costs **₹100 per day per form**, possibly with no cap [SEARCH].
- Failing to file for three consecutive years disqualifies the directors under Section 164(2) [SEARCH].
- Sources: [Kanakkupillai](https://www.kanakkupillai.com/learn/annual-compliance-cost-for-private-limited-company-in-india/); [Patron](https://www.patronaccounting.com/private-limited-company-annual-compliance)
- **DIR-3 KYC:** the yearly director KYC is due by 30 September. Missing it costs a ₹5,000 late fee and deactivates the DIN, which blocks every MCA filing that needs that director's DSC [SEARCH] — [IncorpX DIR-3 KYC](https://www.incorpx.io/blog/director-kyc-dir3-annual-filing); [Patron DIR-3 fee](https://www.patronaccounting.com/blog/government-fee-director-kyc-dir-3-india)

**LLP compliance**
- Form 11 (annual return) is due by 30 May and Form 8 (accounts and solvency) by 30 October. Late filing costs ₹100 per day per form [SEARCH]. TaxGuru notes the LLP late-fee rules were amended from 1 April 2022, so the uncapped ₹100/day figure may be out of date.
- An LLP needs an audit only if turnover exceeds ₹40 lakh or contribution exceeds ₹25 lakh [SEARCH].
- A dormant LLP must still file both forms [SEARCH].
- Sources: [TaxGuru LLP Form 8/11](https://taxguru.in/corporate-law/annual-filing-llp-form-8-form-11.html); [LegalWiz](https://www.legalwiz.in/llp-annual-filing)

**Annual compliance cost (national vendor pricing, not Kerala-specific)**

| Item | Indicative fee [SEARCH] |
|---|---|
| Annual compliance package | from ₹25,000 |
| Statutory audit | ₹8,000–25,000 |
| ROC filings (AOC-4 and MGT-7) | ₹2,500–7,000 |
| Company income-tax return (ITR) | ₹4,000–12,000 |
| GST filing | ₹4,000–12,000 |
| Bookkeeping | ₹10,000–30,000 a year |

Low-cost bundles start at ₹2,999 a year, but their scope is unclear [SEARCH] — [Kanakkupillai](https://www.kanakkupillai.com/learn/annual-compliance-cost-for-private-limited-company-in-india/); [IncorpX](https://www.incorpx.io/blog/annual-compliance-private-limited-step-by-step)

### Inferences
- **Recommended structure:** a Pvt Ltd with two directors.
  - The Kerala person is the resident director. They meet the 182-day test and can act as the signatory for banks and the payment gateway.
  - The founder is a non-resident director and the majority shareholder.
  - The Kerala person holding a small stake makes the founding team look stronger for KSUM.
- **Where the Kerala person is load-bearing:** the KSUM seed loan wants the director's CIBIL score preferably above 750 (Section 4), and the Idea Grant is for "innovators based out of Kerala". The Kerala person therefore matters well beyond the residency test.
- **Why not an OPC:** it meets the minimum for the Idea Grant, but it rules out the productisation grant, the seed loan and the tax holiday. It also leaves no room for a co-founder shareholder.
- **Annual budget:** a realistic outsourced cost for a small Pvt Ltd is probably **₹40,000–1,00,000 a year**. That covers audit, ROC, ITR, monthly GST and bookkeeping, and assumes low transaction volume. This is my estimate, built from the [SEARCH] line items above.
- **If the founder moves to Kerala:** if he spends 182 days or more in India in a financial year, he would himself satisfy the resident-director test. His FEMA and tax status would then change. This was not researched.

### Gaps
- I could not read the Section 149(3) text on mca.gov.in (HTTP 403). The 182-day requirement is [SEARCH] only.
- Documents and process for an NRI director's DIN and DSC (passport, overseas address proof, notarisation or apostille) were not found in any result.
- Board meeting frequency (believed to be four a year under Section 173, two for OPCs and small companies) and the AGM deadline (believed to be 30 September) are unsourced. Verify both.
- No Kerala-specific CA or CS retainer quotes were found. All prices above are national online-vendor prices.
- Realistic SPICe+ turnaround for ROC Ernakulam was not found. The only figure was "7 working days" for Kolkata.

---

## 2. FEMA and FDI for the NRI shareholder, and getting money to the UK-resident founder

### Takeaway
An NRI who lives in the UK and invests on a **repatriation basis** is making foreign investment. Software and edtech fall in sectors not listed in Schedule I, so 100% is allowed under the automatic route. That brings FC-GPR reporting within 30 days, a share issue within 60 days of receiving the money, and a CA's fair-value certificate. Investing on a **non-repatriation basis** (RBI Annex 4, the NDI Rules' Schedule IV) is treated as domestic investment, which avoids the FDI filings. The catch is that sale and liquidation proceeds go only to an NRO account and the capital cannot be repatriated.

There is a little-noticed FDI risk. Foreign investment is banned in "inventory based" e-commerce, which is defined to include services sold directly to consumers. A B2C edtech company with repatriable NRI money should get a lawyer's view on this.

Profits reach the UK founder as dividends (Indian withholding of 20% plus surcharge and cess, reduced to 10% under the India–UK treaty) or as director fees or salary (deducted under Section 195 or 192).

### Cited Findings
**Entry route and the e-commerce restriction**
- "Foreign investment is permitted up to 100% on the automatic route … in sectors/activities not listed in Schedule I of the NDI Rules and not prohibited" [LIVE] — [RBI Master Direction – Foreign Investment in India, updated up to 15 June 2026](https://www.rbi.org.in/Scripts/BS_ViewMasDirections.aspx?id=11200)
- "'Foreign Investment' is any investment made by a person resident outside India on a repatriable basis in equity instruments of an Indian company or to the capital of an LLP" [LIVE] — [RBI MD](https://www.rbi.org.in/Scripts/BS_ViewMasDirections.aspx?id=11200)
- **E-commerce risk:** "'Inventory based model of e-commerce' means an e-commerce activity where inventory of goods and services is owned by e-commerce entity and is sold to the consumers directly … Foreign investment is not permitted in Inventory based model of e-commerce" (paras 2.6.2 and 2.6.4) [LIVE] — [RBI MD](https://www.rbi.org.in/Scripts/BS_ViewMasDirections.aspx?id=11200)

**Non-repatriation route (Annex 4)**
- NRIs and OCIs may buy "any capital instrument issued by a company without any limit" and contribute to "the capital of a Limited Liability Partnership without any limit" on a non-repatriation basis. Such investment "will be deemed to be domestic investment at par with the investment made by residents" [LIVE] — [RBI MD, Annex 4](https://www.rbi.org.in/Scripts/BS_ViewMasDirections.aspx?id=11200)
- Payment may come from abroad through banking channels or from NRE, FCNR(B) or NRO accounts [LIVE].
- Sale and maturity proceeds "should be credited only to the NRO account". "The amount invested … and the capital appreciation thereon cannot be repatriated abroad" [LIVE] — [RBI MD, Annex 4](https://www.rbi.org.in/Scripts/BS_ViewMasDirections.aspx?id=11200)
- NRIs may also put money into a proprietorship or firm on a non-repatriation basis. Agriculture, plantation, print media and real estate are excluded [LIVE] — [RBI MD, Annex 4(B)](https://www.rbi.org.in/Scripts/BS_ViewMasDirections.aspx?id=11200)
- If someone who was resident in India becomes non-resident, their existing holdings "shall be considered on non-repatriation basis" [LIVE] — [RBI MD para 1.3](https://www.rbi.org.in/Scripts/BS_ViewMasDirections.aspx?id=11200)

**Repatriation route: reporting and pricing**
- Form FC-GPR "is filed by the Indian company within thirty days from the date of issue of equity instruments" [LIVE] — [RBI MD, Annex 1](https://www.rbi.org.in/Scripts/BS_ViewMasDirections.aspx?id=11200)
- If shares are not issued within **sixty days** of receiving the money, it must be refunded within 15 days after that [LIVE] — [RBI MD, Annex 1 para 2.3](https://www.rbi.org.in/Scripts/BS_ViewMasDirections.aspx?id=11200)
- For an unlisted company, valuation must follow "any internationally accepted pricing methodology … on an arm's length basis duly certified by a Chartered Accountant or a SEBI registered Merchant Banker or a practicing Cost Accountant" [LIVE] — [RBI MD](https://www.rbi.org.in/Scripts/BS_ViewMasDirections.aspx?id=11200)

**LLP route (Annex 5)**
- Foreign investment in an LLP is allowed only in sectors where 100% is under the automatic route and there are "no FDI linked performance conditions". Capital must come by inward remittance or from a repatriable account [LIVE] — [RBI MD, Annex 5](https://www.rbi.org.in/Scripts/BS_ViewMasDirections.aspx?id=11200)

**Dividends to a UK resident**
- India's domestic withholding on payments to non-residents is 20% plus surcharge and cess, about 20.8–21.84% effective. The lower of the Act rate and the treaty rate applies [SEARCH] — [VJM Global](https://www.vjmglobal.com/feeds/blog/india-uk-dtaa)
- The 2013 protocol to the India–UK treaty replaced Article 11. Dividends are taxed at "15 per cent of the gross amount of the dividends where those dividends are paid out of [income from] immovable property … by an investment vehicle … and 10 per cent in all other cases" [SEARCH] — [UK–India DTA protocol 2013 (HMRC PDF, not fetchable)](https://assets.publishing.service.gov.uk/media/5a80a19c40f0b62305b8c423/2013-uk-india-dta-protocol_-_in_force.pdf); [TaxGuru](https://taxguru.in/income-tax/protocol-amending-dtaa-uk-ireland-india.html)
- Some secondary guides instead give 15% for a 10%-plus holding and 10% otherwise. They conflict with the protocol wording quoted above [SEARCH].
- To get the treaty rate, the UK resident gives the company a **Tax Residency Certificate (TRC) and Form 10F** [SEARCH] — [VJM Global](https://www.vjmglobal.com/feeds/blog/india-uk-dtaa)

**Fees and salary paid to a non-resident director**
- Tax is deducted under Section 192 if the payment counts as salary, otherwise under Section 195 [SEARCH] — [TaxAdda](https://taxadda.com/tds-on-remuneration-paid-to-directors-under-section-194j1ba/)
- Sitting fees or commission paid without an employment contract fall under Section 195 at 20% plus surcharge and cess (ITAT, Enam Securities, 2021) [SEARCH]. A TRC and Form 10F are needed for treaty relief [SEARCH] — [CMA Knowledge](https://www.cmaknowledge.in/?p=1056)
- In one case, salary for services rendered outside India was held not taxable in India [SEARCH] — [TaxAdda](https://taxadda.com/tds-on-remuneration-paid-to-directors-under-section-194j1ba/)

### Inferences
- **Simplest route for a bootstrapped founder:** put in modest capital on a **non-repatriation basis** from an NRE or NRO account. The company is then treated as wholly domestic: no FC-GPR, no FDI sectoral questions, and no inventory-model e-commerce question.
- **Getting money out under that route:** dividends would be paid into the founder's NRO account and remitted from there. My understanding is that current income such as dividends, net of tax, can be remitted from an NRO account (a ceiling of USD 1 million per financial year is often cited). This is not verified in these notes.
- **When the repatriation route makes sense:** if the founder wants his capital itself to be returnable, or plans to raise foreign VC money later. The company would then need FC-GPR and a valuation certificate, and, I believe, the annual Foreign Liabilities and Assets (FLA) return.
- **Taking profits as salary instead:** salary to a UK-resident founder for work done in the UK may not be taxable in India. It would, however, be taxable in the UK and may raise UK payroll and employment-status questions. Director fees may still be taxable in India under the directors' fees article of the treaty. Both points need a cross-border adviser.
- **The inventory-model wording:** it says "goods and services … sold to the consumers directly". It was written for retail, and large edtech companies have received FDI. Even so, a B2C subscription edtech with repatriable NRI capital should get written advice. I found no source applying it to edtech.

### Gaps
- No primary text was read for the NDI Rules' Schedule I, the DPIIT FDI Policy, the Master Direction on Reporting (FC-GPR mechanics and the late-submission fee), or the FLA return.
- Form 15CA/15CB requirements for dividends and fees to a UK resident were not found.
- I could not verify Article 16 (directors' fees) of the India–UK treaty or the remittance limit and process for NRO accounts. The HMRC PDF was blocked and incometaxindia.gov.in returned 403.
- How the UK taxes Indian dividends or salary (credit for Indian tax withheld) was not researched; it is probably UK-side scope.
- No source discusses whether an NRI shareholder with ILR, who is still an Indian citizen, faces any extra FEMA conditions. The rules above apply to NRIs generally.

---

## 3. Indian tax and registrations: corporate tax, GST and export zero-rating, TDS, Kerala Professional Tax, Shops & Establishments, Udyam

### Takeaway
A new company can choose a 22% base rate, about 25.17% effective, and can claim a three-year tax holiday (80-IAC, now section 140 of the Income-tax Act, 2025) once DPIIT recognises it and it gets clearance. Angel tax is gone.

On GST:
- **Registration** is compulsory above ₹20 lakh turnover. It is needed earlier in practice for an LUT and for most payment-gateway and B2B college sales.
- **Domestic sales** carry 18% GST.
- **Overseas sales** to UK and Gulf customers can be zero-rated under an LUT, but only if all five export conditions are met, including payment in convertible foreign exchange backed by FIRA or FIRC evidence.

Two big changes landed in 2024–26: the new Income-tax Act, 2025 from 1 April 2026, and the "GST 2.0" rate overhaul from 22 September 2025.

### Cited Findings
**Corporate tax and the new Act**
- The optional concessional regime is 22% plus 10% surcharge plus cess, about 25.17%, with no other deductions allowed. Once chosen it cannot be withdrawn [SEARCH] — [Kanakkupillai](https://www.kanakkupillai.com/learn/domestic-company-tax-rate/); [Nexdigm](https://www.nexdigm.com/doing-business-in-india/company-taxation.php)
- The Income-tax Act, 2025 re-enacts this regime. Indian Kanoon labels it section 200 of the 2025 Act; another site says section 115. Section numbering is inconsistent across sources [SEARCH] — [Indian Kanoon](https://future.indiankanoon.org/doc/61464663)
- The Income-tax Act, 2025 took effect on **1 April 2026**. For tax year 2026-27 onwards, the 80-IAC deduction sits in section 140 [SEARCH] — [TaxGuru](https://taxguru.in/?p=1086474)

**Tax holiday and angel tax**
- After clearance, a recognised startup "can avail tax holiday for 3 consecutive financial years out of its first ten years since incorporation" [LIVE] — [Startup India recognition page](https://www.startupindia.gov.in/content/sih/en/startupgov/startup_recognition_page.html)
- The 2025 Budget extended the incorporation window for 80-IAC to companies incorporated before **1 April 2030** [SEARCH].
- The 80-IAC turnover cap is ₹100 crore in one source but ₹300 crore from tax year 2026-27 in RSM's summary of the Finance Act, 2026. These conflict [SEARCH] — [TaxGuru](https://taxguru.in/?p=1086474)
- Angel tax (Section 56(2)(viib)) has been abolished. Sources date it from 1 April 2025, i.e. the Finance (No. 2) Act 2024, effective for AY 2025-26 [SEARCH] — [Taxmann](https://www.taxmann.com/post/blog/dpiit-revises-startup-definition-introduces-deep-tech-framework/)

**DPIIT recognition criteria**
- Turnover must be "less than INR 200 Crores (INR 300 Crores for DeepTech startups) in any of the previous financial years". Startup status lasts "up to 10 years (20 years for DeepTech startups)" from incorporation [LIVE] — [Startup India](https://www.startupindia.gov.in/content/sih/en/startupgov/startup_recognition_page.html)
- The limit was raised from ₹100 crore by G.S.R. 108(E) of 4 February 2026 [SEARCH] — [DTNext](https://www.dtnext.in/news/business/centre-expands-definition-of-startup-turnover-limit-doubled-to-rs-200-crore)

**GST registration and rates**
- Registration is required above ₹20 lakh for service providers in most states. Kerala is not a special-category state. A ₹10 lakh limit applies in some north-eastern and hill states, though the state lists vary between sources [SEARCH].
- Inter-state service suppliers are exempt from compulsory registration below ₹20 lakh. The notification number cited varies between sources [SEARCH].
- Sources: [Kanakkupillai](https://www.kanakkupillai.com/learn/new-gst-registration-threshold-limit-for-services/); [Tally](https://tallysolutions.com/gst/gst-limit-registration-threshold-india/)
- "GST 2.0" rate changes took effect on **22 September 2025**, after the 56th GST Council. The structure is now mainly 5% and 18%, plus 40% for sin goods [SEARCH] — [Angel One](https://www.angelone.in/news/taxation/gst-2-0-effective-today-september-22-check-faqs-from-gst-rate-reforms-across-sectors); [ELP](https://elplaw.in/wp-content/uploads/2025/09/ELP-Update-56th-GST-Council-Recommendations.pdf)
- Services that fail the export test are taxed at the standard rate, "18% for most professional/digital services under GST 2.0" [SEARCH] — [TheTaxCorp](https://thetaxcorp.in/article/export-of-services-under-gst-complete-guide-to-zero-rating-lut-and-refunds)

**Exports under GST**
- "Export of services under GST is zero-rated only when all five Section 2(6) conditions are met together." Payment must be "in convertible foreign currency within the timeline prescribed by RBI" [LIVE] — [Razorpay blog](https://razorpay.com/blog/conditions-for-export-of-services-under-gst/)
- For remote services such as SaaS and IT, "the place of supply is the location of the recipient". "FIRCs or FIRAs are essential documents for claiming GST refunds on service exports" [LIVE] — [Razorpay blog](https://razorpay.com/blog/conditions-for-export-of-services-under-gst/)
- The same page says the **Finance Act 2026 (effective 30 March 2026)** removed clause (b) of IGST Section 13(8), so intermediary services now follow the default place-of-supply rule [LIVE: the page's own claim, not checked against CBIC].
- An LUT lets exports go out without paying IGST and must be renewed every financial year. The alternative is to pay IGST and claim a refund (RFD-01) [SEARCH] — [Kanakkupillai](https://www.kanakkupillai.com/learn/gst-on-foreign-clients/); [TheTaxCorp](https://thetaxcorp.in/article/export-of-services-under-gst-complete-guide-to-zero-rating-lut-and-refunds)
- **Rulings on education services:** one advance ruling denied export status to overseas education advisory because the place of supply was in India [SEARCH] — [GST Council AAR](https://www.gstcouncil.gov.in/sites/default/files/AAR/guj_aar_09_2021_uupl_20.01.2021.pdf). A High Court treated services to foreign universities as exports, and the Supreme Court dismissed the SLP [SEARCH] — [Taxmann](https://www.taxmann.com/post/blog/sc-dismisses-slp-referral-services-to-foreign-universities-treated-as-export)

**Kerala Professional Tax**
- Rates were revised by notification no. 1149/2024/LSGD (27 June 2024), effective **1 October 2024**.
- Half-yearly slabs are ₹320, ₹450, ₹600, ₹750, ₹1,000 and ₹1,250, giving a maximum of ₹2,500 a year.
- Tax is collected half-yearly by the local body.
- Companies operating in a municipal area for 60 days or more also pay, up to ₹2,500 a year [SEARCH].
- Sites still showing a ₹120 lowest slab are out of date [SEARCH].
- Sources: [Kredily](https://kredily.com/compliance/professional-tax-kerala/); [Ascent HR](https://ascent-hr.com/notification/change-in-rates-of-professional-tax/)

**Udyam (MSME) registration**
- Free and permanent, with no renewal. Bank sources claim benefits such as collateral-free loans, subsidies, tender preference and protection against delayed payment [SEARCH] — [Kotak](https://www.kotak.bank.in/en/stories-in-focus/loans/business-loan/udyam-registration-certificate-benefits-msme.html)
- Razorpay asks for an Udyam certificate, if the business has one, during international-payments onboarding [LIVE] — [Razorpay international payments docs](https://razorpay.com/docs/payments/international-payments.md)

### Inferences
- **Register for GST voluntarily from day one.** Exports need a GSTIN and an LUT to be zero-rated and to recover input GST on software, hosting and rent. Colleges and hospitals buying licences will also want GST invoices.
- **Domestic pricing:** quote Indian individual plans GST-inclusive (18%).
- **Overseas sales:** a UK or Gulf radiographer paying by international card for remote access to a browser simulator should meet the export test, since the recipient is located abroad. Keep IP and billing-country evidence and the PA-CB's FIRA.
- **Two weak spots for export status:**
  - Payments in INR from abroad, or from Nepal or Bhutan, may not qualify.
  - Indian residents who pay with a foreign card are not exports at all.
- **Expected tax position:** with 80-IAC (if granted) and early-stage losses, the company may pay little income tax for several years.
- **Tax on extracting profit:** dividends are paid from post-tax profit, so tax applies at two levels. The concessional regime cannot be combined with 80-IAC. The CA must model which regime to choose.

### Gaps
The following were not found or could not be verified:
- The Income-tax Act, 2025 text on incometaxindia.gov.in (403).
- The rate for smaller companies under the normal regime (believed 25% for turnover up to ₹400 crore).
- The LLP tax rate (believed 30% plus cess).
- The CBIC rate notification confirming 18% on online or "OIDAR"-type education services.
- GSTR-1 and GSTR-3B frequency, QRMP eligibility (believed up to ₹5 crore), late fees (believed ₹50 a day, or ₹20 for nil returns), and the GSTR-9 exemption threshold.
- TDS return obligations: quarterly 24Q/26Q, and TAN registration.
- The Kerala Shops & Establishments registration process and fee. No result found.
- Udyam-specific benefits: 45-day payment protection, the MSME Samadhaan portal, and Section 43B(h).

---

## 4. Kerala and central government support: KSUM, Startup India and procurement

### Takeaway
KSUM's live scheme pages show a clear non-dilutive ladder:

| Scheme | Type | Up to |
|---|---|---|
| Idea Grant | Grant | ₹3 lakh |
| Productisation Grant | Grant | ₹7 lakh |
| Market Acceleration Grant | Grant | ₹10 lakh |
| Scaleup Grant | Grant | ₹15 lakh |
| Seed Loan | Loan at 6% | ₹15 lakh |
| Scaleup Seed Fund | Loan | ₹25 lakh |
| Startup India Seed Fund (central) | Grant/seed fund | ₹20 lakh grant / ₹50 lakh seed fund |

On top of that come procurement preferences, under which Kerala government bodies can buy directly from KSUM Unique ID startups up to ₹50 lakh, and an NRI programme ("Startup Infinity"). Every one of these needs a Kerala-registered Pvt Ltd or LLP (OPC only for the Idea Grant), a KSUM Unique ID, and a founder or director presence in Kerala.

### Cited Findings
**Grants (all from KSUM's Early Stage Funding page [LIVE] — [KSUM Early Stage Funding](https://startupmission.kerala.gov.in/schemes/early-stage-funding))**
- Idea Grant "Upto 3 Lakhs".
- Productisation Grant "Upto 7 Lakhs"; Women/Transgender Productisation Grant "Upto 12 Lakhs".
- Market Acceleration Grant "Upto 10 Lakhs" (customer pilots, go-to-market, certifications).
- Scaleup Grant "Upto 15 Lakhs".
- BCDD Grant (OBC/OEC founders) "Upto 10 Lakhs".
- Startup India Grant "Upto 20 Lakhs".
- Nidhi Prayas "Upto 10 Lakhs" (coming soon).
- Patent reimbursement: India patent up to ₹2 lakh, US patent up to ₹10 lakh (coming soon).

**Loans and seed funds [LIVE] — [KSUM Early Stage Funding](https://startupmission.kerala.gov.in/schemes/early-stage-funding)**
- Seed Loan "Upto 15 Lakhs".
- Scaleup Seed Fund "Upto 25 Lakhs".
- Startup India Seed Fund "Upto 50 Lakhs".
- Women Soft Loan "Upto 15 Lakhs".
- Nidhi Seed Support ₹25 lakh to ₹1 crore.

**Idea Grant conditions [LIVE] — [KSUM Idea Grant](https://startupmission.kerala.gov.in/schemes/idea-grant)**
- Open to startups at the ideation, design or proof-of-concept stage.
- "Only innovative technology-based products are considered".
- A Unique ID is not needed to apply but is mandatory before the money is paid.
- An expert committee scores team, innovation, marketing, financials and the plan for using the grant.
- Money is paid in tranches, generally 50% first.
- Required documents include a CA-certified No Dues and Margin Money certificate with UDIN, a balance sheet for the last two years, and stamp paper.
- A rejected applicant can reapply after 3 months.

**Productisation Grant conditions [LIVE] — [KSUM Productisation Grant](https://startupmission.kerala.gov.in/schemes/productisation-grant)**
- A KSUM Unique ID is mandatory when applying.
- A startup that already had the Idea Grant can claim only the remaining ₹4 lakh.
- The startup must put up **20% margin money** at the second tranche.
- The second tranche needs an audited utilisation certificate.

**Seed Loan conditions [LIVE] — [KSUM Seed Fund](https://startupmission.kerala.gov.in/schemes/seed-fund)**
- A "soft loan at 6% simple interest per annum", with a 12-month moratorium and then 36 monthly instalments. Prepaying carries no penalty.
- The loan is made against purchase orders and "not generally given for service startups".
- The director's CIBIL score should preferably be above 750.
- The startup must hold DPIIT recognition and 'Active Compliant' MCA status.
- The startup must have no dues to government bodies.

**NRI programme and incubation [LIVE]**
- **Startup Infinity** "engages the global NRI community … Enable NRI participation in Kerala's startup and innovation ecosystem; Facilitate cross-border business setup and scaling models" — [KSUM Market Expansion page](https://startupmission.kerala.gov.in/schemes/business). Its microsite (startupinfinity.startupmission.in) was blocked, so the details are unknown.
- The same page lists an International/National Exposure Programme (money to attend events) and a Delegation Scheme [LIVE].
- Incubation programmes [LIVE] — [KSUM Incubation & Acceleration](https://startupmission.kerala.gov.in/schemes/incubation-acceleration):
  - Pre-incubation (SparkX, for Idea Grant recipients) lasts 45 days to 3 months.
  - Incubation (GrowthX, "coming soon", for productisation recipients) lasts 3–6 months.
  - Acceleration is a 3-month programme. It includes "LeapX – B2B SaaS" for revenue-stage startups and "LeapX AVGC XR".
- KSUM runs a Fund of Funds with SEBI-registered AIFs, a Creative Economy Fund, investor cafés and pitch days, and the "Seeding Kerala" investor meet [LIVE] — [KSUM Investments](https://startupmission.kerala.gov.in/schemes/investment)

**Procurement**
- A 2022 government order allows direct purchase from KSUM-registered startups up to ₹50 lakh, excluding GST.
- In 2023 the ceiling was raised from ₹1 crore to ₹3 crore, with a limited tender between ₹50 lakh and ₹3 crore [SEARCH].
- Sources: [YourStory](https://yourstory.com/2023/05/kerala-govt-raises-ceiling-on-purchase-of-products); [KILA/LSGD document](https://tpms.kila.ac.in/uploads/1723540880.pdf)
- Startup India publishes a Department of Expenditure clarification on relaxing public-procurement norms for startups [LIVE: link title only] — [Startup India](https://www.startupindia.gov.in/content/sih/en/startupgov/startup_recognition_page.html)

### Inferences
- **Fit with the product:** a browser MRI/CT simulator is a "technology-based product", so it fits KSUM's grant rules. Grants go to a product, not a service, which suits a SaaS simulator better than a training-services business.
- **Realistic non-dilutive total:** Idea plus Productisation (₹7 lakh combined), then Market Acceleration (₹10 lakh), then possibly a seed loan. That is roughly ₹17 lakh in grants plus a ₹15 lakh loan, if every application succeeds. This is my sum of the [LIVE] caps, not a forecast.
- **Fixed costs of applying:** the 50% tranche structure, the 20% margin money, CA certificates and attending in person at KSUM offices to sign the agreement mean the Kerala co-founder will have to do the legwork.
- **Procurement as a sales channel:** government medical colleges, the DME and Kerala hospital bodies could in principle license the simulator directly, up to ₹50 lakh without a tender, once the company has a KSUM Unique ID. This is a real advantage of a Kerala entity that a UK company cannot use.

### Gaps
- KSUM Unique ID eligibility (age limit, Kerala registered office, innovation test) was not read. The FAQ is rendered by JavaScript and returned no text.
- Startup Infinity's actual benefits for NRI founders were not found; the microsite was blocked.
- Incubator seat costs and how to get in (Technopark, Infopark, KSUM's Integrated Startup Complex in Kochi) were not found.
- The DPIIT self-certification benefit under labour and environmental laws was not confirmed on a live page.
- Current call dates, success rates and processing times for KSUM grants were not found. The beneficiary counters on the Idea Grant page showed "0", which looks like template placeholders.

---

## 5. Payments: Razorpay onboarding and fees, UPI AutoPay, cross-border collection (FIRA, PA-CB) and selling into the UK, EU and Gulf

### Takeaway
Razorpay is the practical default:
- **Domestic:** 2% plus GST on cards, UPI, netbanking and wallets; 3% on Amex, Diners, corporate cards and EMI.
- **International:** 3% plus GST on international cards; 1% plus GST on international bank transfers through the "MoneySaver Export Account".
- **Subscriptions:** an extra 0.99%.
- **New merchants** activated from 1 July 2026 get 0% on domestic payments for 90 days or ₹5 lakh, whichever comes first.

KYC needs the company's documents plus an Indian authorised signatory with a PAN and Aadhaar, and video KYC for international payments. In practice that makes the Kerala co-founder the signatory.

**Biggest finding for overseas sales.** An Indian company selling digital services to **UK consumers must register for UK VAT from the first sale**, because a UK business only registers above £90,000. EU consumers likewise mean VAT under the non-Union OSS scheme from the first euro, and UAE (5%) and Saudi (15%) consumers mean registration with no threshold. Paddle, a merchant of record, accepts software sellers and courses they create, which could absorb this burden.

### Cited Findings
**Razorpay fees [LIVE] — [Razorpay pricing explainer (dated 13 Feb 2026, describes offers from 1 July 2026)](https://razorpay.com/blog/razorpay-payment-gateway-pricing-explained/)**
- **Standard domestic:** "2% plus applicable GST, with no setup fee or annual maintenance charge". This applies to UPI too: "Zero bank MDR on standard bank-to-bank UPI does not waive Razorpay's platform fee".
- **Domestic premium methods:** Amex and Diners 3%; EMI 3%; Credit Card on UPI 2.15%.
- **International credit and debit cards:** "3% of transaction value + GST". Optional chargeback protection adds about 1%.
- **International bank transfers:** "1% of transaction value + GST", through the MoneySaver Export Account (ACH, SEPA or SWIFT virtual accounts, "Zero forex markup").
- **International local methods and wallets:** 3.5% plus GST.
- **Subscriptions:** "0.99% (approx. 1%) subscription fee per transaction" on top of the 2% gateway fee.
- **New-merchant offer:** "0% platform fees on domestic payments for up to 90 days or ₹5 lakh in cumulative payment value" for accounts activated on or after 1 July 2026. International, Amex, Diners, corporate and EMI are excluded. A "₹199 KYC processing fee plus taxes" applies.

**Razorpay onboarding and KYC [LIVE]**
- For a Pvt Ltd, CKYC fills in the details automatically. Otherwise Razorpay asks for the Certificate of Incorporation, CIN, MOA and AOA (mandatory), the business PAN, the bank account and IFSC, and the authorised signatory's PAN and address proof (Aadhaar, Voter ID or passport). This is under the "2026 Master KYC guidelines" — [Razorpay KYC documents](https://razorpay.com/docs/build/llm-docs/payments/business-types-kyc-documents.md)
- International payments onboarding asks for the business PAN, the GSTIN certificate (if registered), the Udyam certificate (for MSMEs), business address proof and signatory details. It then needs "video KYC: Requires Aadhaar and PAN card. Live video verification with Razorpay agent" — [Razorpay International Payments docs](https://razorpay.com/docs/payments/international-payments.md)
- Registered businesses can accept international cards, international bank transfers, PayPal and local methods such as Trustly for UK and EU customers. Individuals can use only PayPal or bank transfer [LIVE] — [Razorpay International Payments docs](https://razorpay.com/docs/payments/international-payments.md)
- Razorpay says it is "RBI-regulated with PA-CB (Payment Aggregator – Cross Border) licence" [LIVE] — [Razorpay llms.txt](https://razorpay.com/docs/llms.txt)
- UPI AutoPay works through Razorpay's Recurring Payments and Subscriptions. The customer sets a maximum amount, frequency and validity period [LIVE] — [Razorpay UPI Autopay docs](https://razorpay.com/docs/build/llm-docs/payments/recurring-payments/upi.md)
- The prior report's figures were never verified: AutoPay mandates up to ₹1,00,000 and no extra authentication up to ₹15,000.

**RBI rules on cross-border payment aggregators (PA-CB)**
- The RBI's 31 October 2023 circular brought all cross-border payment facilitators under RBI regulation as PA-CBs.
- An export PA-CB must keep an Export Collection Account with an AD Category-I bank.
- "The maximum value per unit of goods / services sold / purchased shall be ₹25,00,000".
- AD banks must ensure FEMA reporting and EDPMS reconciliation [LIVE] — [RBI PA-CB circular (MD id 12561)](https://www.rbi.org.in/Scripts/BS_ViewMasDirections.aspx?id=12561)
- A consolidated Master Direction on Payment Aggregators dated **15 September 2025** repealed the older circulars on online payment gateways and export receipts. It keeps a ₹25 lakh per-transaction cap and splits PA-CBs into inward and outward types [SEARCH] — [Taxscan](https://www.taxscan.in/top-stories/rbi-issues-master-direction-on-regulation-of-payment-aggregators-strengthens-rules-on-kyc-cross-border-transactions-1432872); [Cyril Amarchand Mangaldas alert](https://www.cyrilshroff.com/wp-content/uploads/2025/10/Client-Alert-RBI-Introduces-Consolidated-Framework-for-Payment-Aggregators-3.pdf)
- FIRCs or FIRAs are "essential documents for claiming GST refunds on service exports" [LIVE] — [Razorpay blog](https://razorpay.com/blog/conditions-for-export-of-services-under-gst/)

**Selling to UK consumers [LIVE]**
- "If you are a business making supplies of digital services to UK consumers, those supplies are liable to UK VAT … If your supplies are liable to UK VAT you will need to register for UK VAT if you are based outside the UK" — [GOV.UK: VAT rules for digital services to private consumers](https://www.gov.uk/guidance/the-vat-rules-if-you-supply-digital-services-to-private-consumers)
- UK businesses register above £90,000 of taxable turnover. "You must also register (regardless of taxable turnover) if … your business is based outside the UK" — [GOV.UK: When to register for VAT](https://www.gov.uk/vat-registration/when-to-register)

**Selling to EU and Gulf consumers [SEARCH]**
- **EU:** non-EU sellers of digital services, including e-learning, use the non-Union OSS. The €10,000 threshold "does not apply to non-EU businesses", so VAT is due from the first euro — [Taxually](https://support.taxually.com/support/solutions/articles/80001155457)
- **UAE:** 5% VAT, no threshold for non-resident digital providers selling to consumers, registration before the first sale — [Avalara UAE](https://www.avalara.com/vatlive/en/country-guides/africa-and-middle-east/united-arab-emirates/uae-vat-on-digital-and-electronic-services.html)
- **Saudi Arabia:** 15% VAT, no threshold since 1 January 2018. Sources conflict on whether a local tax representative is needed — [Avalara KSA](https://www.avalara.com/vatlive/en/country-guides/africa-and-middle-east/saudi-arabia/saudi-arabia-vat-on-digital-and-e-services.html)

**Paddle as a merchant of record [LIVE] — [Paddle: what am I not allowed to sell](https://www.paddle.com/help/start/intro-to-paddle/what-am-i-not-allowed-to-sell-on-paddle)**
- "Paddle is built to serve software companies (including B2B SaaS, Consumer Software, and Games)".
- Human services not tied to software are excluded, as are "certifications or courses for which the business is not the owner or creator".

### Inferences
- **Effective fees:** about 2.36% on Indian UPI and cards and about 3.54% on UK and Gulf cards once GST is added. Add about 1.17% for Razorpay Subscriptions.
- **Paying out of India:** the 18% GST on Razorpay's fees is an input credit only if the company is GST-registered. That is another reason to register early.
- **Who signs for Razorpay:** a UK-resident NRI founder probably lacks Aadhaar, and video KYC needs Aadhaar and PAN. The Kerala resident director should be the authorised signatory for Razorpay and the bank. This is an inference from the [LIVE] KYC text; I did not verify whether NRIs can hold Aadhaar.
- **Counterpoint to "Kerala is less hassle" for overseas sales:** a Kerala company selling directly to UK, EU, UAE or Saudi consumers faces foreign VAT registrations from the first sale. A UK company selling to UK consumers registers only above £90,000. Ways to avoid this:
  - Sell to overseas consumers through a merchant of record (Paddle, or app stores) that collects and remits the VAT. The simulator is founder-built software, so it appears to fit Paddle's rules.
  - Sell business-to-business (licences to colleges and hospitals), where the customer usually reverse-charges the VAT.
- **The RBI cap is no constraint:** individual sales and college licences sit far below the ₹25 lakh cap, which matters only for very large institutional deals.

### Gaps
- I could not reach Razorpay's India pricing page itself. razorpay.com/pricing redirects to the US page because the proxy is US-based. The India rates above come from Razorpay's own [LIVE] blog explainer.
- Cashfree and PayU fees and onboarding were not researched.
- Whether Paddle pays out to an Indian company, and its fee, were not confirmed; the countries page was fetched, but it does not mention India.
- How to get FIRA or e-BRC for card collections in practice (does Razorpay issue a FIRA per settlement?) is not confirmed. DGFT's e-BRC was not researched.
- No source was found on how Indian banks handle current-account KYC for a company with an NRI director (in-person verification, OCI and passport rules).
- The Oman, Bahrain, Qatar and Kuwait VAT positions for digital services were not researched.

---

## 6. Reality check on "Kerala is cheaper and less hassle with rules and regulations"

### Takeaway
**"Cheaper" is largely true. "Less hassle" is largely false.** Kerala's labour, office and professional fees cost a fraction of Manchester's, and Kerala offers grants and procurement routes the UK lacks. But an Indian Pvt Ltd carries a heavier recurring burden, and some of it is mandatory regardless of size:
- a statutory audit every year;
- GST returns monthly or quarterly;
- TDS returns;
- Professional Tax twice a year;
- ROC annual filings and director KYC with daily or flat late fees;
- FEMA reporting if the NRI capital is repatriable;
- foreign VAT registrations from the first sale for direct B2C sales abroad.

A UK private company faces two main yearly filings, with fixed late penalties, and needs no audit at this size.

### Cited Findings
**India: penalties and recurring obligations (all [SEARCH] unless marked)**
- AOC-4 and MGT-7 late fee: ₹100 per day per form, possibly uncapped. Three years of non-filing disqualifies the directors under Section 164(2) — [Kanakkupillai](https://www.kanakkupillai.com/learn/annual-compliance-cost-for-private-limited-company-in-india/)
- DIR-3 KYC: due 30 September; ₹5,000 flat late fee; DIN deactivated, which blocks MCA filings. Banks that check the MCA portal will see the director as "Deactivated" — [IncorpX](https://www.incorpx.io/blog/director-kyc-dir3-annual-filing)
- LLP: ₹100 per day per form for Form 8 and Form 11 — [TaxGuru](https://taxguru.in/corporate-law/annual-filing-llp-form-8-form-11.html)
- First auditor within 30 days for every company "regardless of its size, turnover" — [Patron](https://www.patronaccounting.com/blog/first-auditor-appointment-adt1-filing-guide)
- Kerala Professional Tax is paid half-yearly to the local body; the company itself also pays — [Kredily](https://kredily.com/compliance/professional-tax-kerala/)
- FC-GPR within 30 days and share allotment within 60 days if NRI capital is repatriable [LIVE] — [RBI MD](https://www.rbi.org.in/Scripts/BS_ViewMasDirections.aspx?id=11200)
- The KSUM seed loan can be rejected if MCA status is "Active Non-compliant" [LIVE] — [KSUM Seed Fund](https://startupmission.kerala.gov.in/schemes/seed-fund)
- GST export zero-rating fails, taxing the sale at 18%, if any one of the five conditions is missed. "Place of supply and foreign exchange realisation are the most common compliance risk areas" [LIVE] — [Razorpay blog](https://razorpay.com/blog/conditions-for-export-of-services-under-gst/)

**UK comparison [LIVE]**
- Companies House fees: incorporation £100 online (£124 on paper); confirmation statement £50 online; page updated 25 September 2026 — [GOV.UK Companies House fees](https://www.gov.uk/government/publications/companies-house-fees/companies-house-fees)
- UK late-filing penalties for a private company's accounts: £150 (up to 1 month late), £375 (1–3 months), £750 (3–6 months), £1,500 (more than 6 months) — [GOV.UK](https://www.gov.uk/annual-accounts/penalties-for-late-filing)
- UK VAT registration threshold: £90,000 for UK-based businesses [LIVE] — [GOV.UK](https://www.gov.uk/vat-registration/when-to-register)

### Inferences
**Indian compliance calendar for a small Pvt Ltd.** This is my synthesis from the findings above plus general knowledge; items not individually sourced are marked "verify".

| When | Obligation |
|---|---|
| Monthly or quarterly | GSTR-1 and GSTR-3B (QRMP is quarterly; verify) |
| Monthly | TDS deposits once salaries or fees are paid (verify) |
| Quarterly | TDS returns (verify) |
| Every April | LUT renewal |
| Half-yearly | Kerala Professional Tax |
| Within 30 days of incorporation | First auditor appointed |
| Within 180 days of incorporation | INC-20A |
| By 30 September | DIR-3 KYC; AGM (verify) |
| After the AGM | AOC-4 within 30 days, MGT-7 within 60 days |
| Yearly | Income-tax return (date under the new Act, verify) |
| Yearly | Statutory audit |
| If repatriable FDI | FLA return (verify) and FC-GPR on each allotment |

That is roughly 30–40 filings a year, against perhaps 5–10 for a small UK limited company that is not VAT-registered.

- **Cost of mistakes:** Indian late fees are smaller in pounds than UK penalties. The real risk is non-monetary: deactivated DINs, "Active Non-compliant" status that blocks KSUM money, GST notices, and lost refunds.
- **Where Kerala genuinely wins:**
  - developer and office costs (Section 7);
  - grants of up to roughly ₹17 lakh plus a 6% loan;
  - procurement access to Kerala government buyers;
  - selling in INR through UPI AutoPay, which a UK company would struggle to do;
  - an 18% domestic GST rate that Indian customers already expect.
- **Where the UK wins:**
  - selling to UK consumers, with no VAT below £90,000;
  - less recurring paperwork;
  - no FEMA layer;
  - the founder's residence: his personal tax is all in one country if he takes salary or dividends from a UK company.
- **A hybrid worth evaluating:** a Kerala Pvt Ltd for India sales, KSUM grants and the dev team, plus sales to UK, EU and Gulf consumers through a merchant of record. This is an inference; the other researchers' UK-side notes should be compared.

### Gaps
- No systematic data was found on how often small Indian startups get GST notices, or what they report as pain points. The searches returned only vendor blogs.
- The UK side was only lightly covered: no accountant costs, Corporation Tax filings or audit-exemption thresholds. The UK-focused researcher presumably covers these.
- No source quantifies total time spent on compliance (hours a month) for an Indian micro-company.

---

## 7. Costs in Kerala: co-working, developer salaries and CA/CS retainers

### Takeaway
Kochi co-working costs roughly **₹5,000–15,000 per seat per month**, with Infopark dedicated desks listed at about ₹6,500–7,500 on myHQ. React and JavaScript developers in Kochi earn roughly:

| Level | Per year | Per month (my conversion) |
|---|---|---|
| Fresher | about ₹3.5–5 lakh | about ₹29,000–42,000 |
| Mid-level | about ₹6–8 lakh | — |
| Senior | about ₹12–15 lakh | about ₹1–1.25 lakh |

Outsourced company compliance runs from about ₹25,000 a year at the bare minimum to likely ₹40,000–1,00,000 with monthly GST and bookkeeping. All figures are [SEARCH].

### Cited Findings
**Developer salaries (Kochi and Kerala)**
- React JS developers in Kochi start at about ₹5 lakh a year, averaging about ₹7.8 lakh at two years' experience [SEARCH] — [Cutshort](https://cutshort.io/salary/react-js-developer/kochi)
- Payscale's average React developer base pay in Kochi for 2026 is about ₹6.1 lakh [SEARCH] — [Payscale](https://www.payscale.com/research/IN/Job=React_Developer/Salary/96518476/Kochi)
- Salary.com puts junior React developers in Kochi at about ₹7.4 lakh (April 2025) [SEARCH] — [Salary.com](https://www.salary.com/research/in/junior-react-developer-salary/kochi)
- At one Kochi firm, a three-year React developer earns ₹4.5–5.8 lakh; AmbitionBox flags this as low-confidence data [SEARCH] — [AmbitionBox](https://www.ambitionbox.com/salaries/apps-team-technologies-salaries/react-developer/kochi-location)
- AmbitionBox's national range for fresher React developers is about ₹1–6 lakh [SEARCH].
- Senior React developers in Kerala average about ₹14.2 lakh (range ₹13.1–14.8 lakh) [SEARCH] — [Jooble](https://in.jooble.org/salary/senior-react-developer/Kerala). A Kochi job listing for a senior role with 4+ years' experience shows expected pay of ₹12 LPA [SEARCH].

**Co-working (Kochi)**
- **Office Hub:** desks near Infopark from ₹15,000 a month for one person, up to ₹75,000 for five (Four Points by Sheraton listing) [SEARCH] — [Office Hub](https://www.office-hub.com/in/listings/1-person-coworking-office-kochi-phase-1-campus-infopark-po-kakkanad-kerala-682042-a0tQg00000NrNNpIAN)
- **myHQ:** dedicated desks on the Infopark campus at ₹6,499 and ₹7,499 per desk per month, negotiable [SEARCH] — [myHQ](https://myhq.in/kochi/dedicated/coworking-space-in-infopark-campus)
- **Regus, Kakkanad:** co-working access from ₹290 per person per day; dedicated desks priced on 24-month contracts [SEARCH] — [Regus](https://www.regus.com/en/in/kerala/kakkanad/coworking)
- **Workin.space:** minimum monthly price of ₹12,890 for a dedicated open-space desk and ₹14,350 for a private office, excluding charges; updated 16 August 2026 [SEARCH] — [Workin](https://workin.space/en/india/kochi)
- **IncorpX:** Kochi plans start around ₹7,500 per seat per month [SEARCH] — [IncorpX](https://www.incorpx.io/workspaces/kochi/coworking?verified=1)

**CA/CS fees.** These are national online-vendor prices; see Section 1. Packages start at ₹25,000 a year, audits cost ₹8,000–25,000 and bookkeeping ₹10,000–30,000 [SEARCH] — [Kanakkupillai](https://www.kanakkupillai.com/learn/annual-compliance-cost-for-private-limited-company-in-india/)

### Inferences
- **A lean Kerala team:** one mid-level React developer (about ₹6–8 lakh a year) plus one fresher (about ₹4 lakh), each with a co-working desk (about ₹7,500 a month), costs roughly **₹12–14 lakh a year (about £11,000–13,000)** before employer costs. That excludes PF and ESI, which I did not research. One UK junior developer would cost several times that. This is my arithmetic from [SEARCH] figures; I did not check exchange rates.
- **Working from home first:** the founder could skip co-working early on and use the Kerala co-founder's address as the registered office. KSUM or Technopark incubation may provide subsidised space, but no prices were found.

### Gaps
- No live salary data was read; AmbitionBox, Naukri and Glassdoor were not fetched, and every figure is [SEARCH]. Trivandrum (Technopark) salary and co-working figures specifically were not found.
- Employer statutory costs (EPF and ESI thresholds and rates) were not researched.
- Kerala-specific CA/CS retainer quotes were not found.
- KSUM incubator space rates (Integrated Startup Complex Kochi, Technopark/Thejaswini) were not found.
