# Running the MRI/CT simulator business through a UK entity (as of 8 November 2026)

*General information gathered for a research report. This is not tax or legal advice; the founder should confirm the position with a UK chartered accountant / chartered tax adviser (and an Indian CA for the India-side points) before acting.*

Provenance key: **[LIVE]** = read on the fetched primary page itself during this session. **[SEARCH]** = taken only from a web-search result summary (secondary or tertiary source; not read in full). Figures with neither tag are my own arithmetic from [LIVE] figures and are labelled as inferences.

Access notes for the report writer: GOV.UK, legislation.gov.uk, cbic-gst.gov.in, stripe.com, paddle.com and razorpay.com were fetched directly. **www.england.nhs.uk** returned an empty bot-challenge response, **ico.org.uk** returned 403, **www.incometaxindia.gov.in** returned 403, and **docs.stripe.com** was blocked by the proxy, so those points rely on GOV.UK equivalents or search summaries. A **Budget 2026** was delivered on **28 October 2026** [LIVE] ([GOV.UK Budget 2026](https://www.gov.uk/government/publications/budget-2026-document/budget-2026-html)); its announced changes are flagged below as "announced, not yet in force".

---

## 1. Can an ILR holder be self-employed or a company director without restriction, and what NHS rules apply?

### Takeaway
ILR carries no work restrictions, so the founder can be a sole trader, a director or a shareholder of a UK company with no immigration permission needed. The real constraints are (a) ILR lapses after more than 2 continuous years outside the UK, which matters if the founder relocates to Kerala, and (b) NHS conflict-of-interest declarations and employer IP ownership of anything made "in the course of employment".

### Cited Findings
- ILR "gives you the right to live, work and study here for as long as you like, and apply for benefits if you're eligible"; it can be used to apply for British citizenship [LIVE] — [GOV.UK: Check if you can get ILR](https://www.gov.uk/indefinite-leave-to-remain)
- ILR is lost if the holder has been outside the UK, Channel Islands and Isle of Man for **more than 2 continuous years** (5 years only for EU Settlement Scheme status); re-entry then needs a **Returning Resident visa costing £726**, which requires evidence of "strong ties to the UK" [LIVE] — [GOV.UK: Returning resident](https://www.gov.uk/returning-resident-visa)
- Companies House lets any director be appointed, but from **18 November 2025** identity verification is a legal requirement: a new company's registration must include each director's Companies House personal code [LIVE] — [GOV.UK: When you need to verify your identity](https://www.gov.uk/guidance/when-you-need-to-verify-your-identity-for-companies-house)
- NHS England's "Managing Conflicts of Interest in the NHS" guidance came into force on **1 June 2017** and applies to NHS trusts and foundation trusts [SEARCH] — [NHS England, COI guidelines (Feb 2017)](https://www.england.nhs.uk/2017/02/coi-guidelines/); [MDDUS summary](https://www.mddus.com/resources/resource-library/news-digest/2017/february/new-nhs-guidance-on-avoiding-conflicts-of-interest)
- Under that guidance, staff (clinical or non-clinical) are expected to declare outside employment, including where and when it takes place (but not earnings) [SEARCH] — [National Health Executive](https://www.nationalhealthexecutive.com/News/final-crackdown-on-conflicts-of-interest-with-tightened-rules-on-gifts-and-hospitality)
- NHS England's Q&A for clinical staff says an outside role (example given: with a pharma company) must be declared as soon as possible and in any event **within 28 days** of it arising [SEARCH] — [NHS England COI Q&A for clinical staff (PDF)](https://www.england.nhs.uk/wp-content/uploads/2017/09/coi-qa-clinical-staff.pdf)
- Trust policies revised in 2024 still implement the 2017 national guidance (for example, "decision making" staff must declare at least annually even if nil); no post-2017 revision of the national guidance was found [SEARCH] — [Sheffield Health & Social Care policy, May 2024 (PDF)](https://shsc.nhs.uk/sites/default/files/2024-06/Managing%20Conflicts%20of%20Interest%20in%20the%20NHS%20Policy%20%28CG%20001%20V3%20May%202024%29%20%281%29.pdf); [Gloucestershire Health & Care policy 2024 (PDF)](https://ghc.nhs.uk/wp-content/uploads/2024/06/Managing-Conflicts-of-Interest-Policy.pdf)
- Copyright: where a literary work (which includes software) "is made by an employee in the course of his employment, his employer is the first owner of any copyright in the work subject to any agreement to the contrary" (CDPA 1988 s11(2)) [LIVE] — [legislation.gov.uk CDPA s11](https://www.legislation.gov.uk/ukpga/1988/48/section/11)
- Inventions: an employee's invention belongs to the employer if made in the course of normal duties (or specifically assigned duties) where an invention might reasonably be expected to result (Patents Act 1977 s39) [LIVE] — [legislation.gov.uk Patents Act s39](https://www.legislation.gov.uk/ukpga/1977/37/section/39)

### Inferences
- A radiographer's normal duties do not include writing simulator software, so a simulator built in the founder's own time on their own equipment is unlikely to be "in the course of employment". The risk rises if the founder uses NHS time, NHS devices, NHS protocols/documents, screenshots of trust scanners or any patient images, or if the employment contract or trust IP policy contains a wider assignment clause. The founder should read their contract's IP clause and the trust's IP policy.
- The founder should declare the business through the trust's declarations-of-interest process before trading. They should also avoid selling to their own trust or its students in a way that looks like using their position (for example, licences to a university whose students do placements in their department), unless they have declared it and had it cleared.
- If the founder later moves to Kerala to run the business, the 2-year ILR clock matters. Spending long stretches in India also changes UK tax residence (see section 4) and can make a UK company Indian tax resident or give it an Indian PE (see section 4).

### Gaps
- The text of the founder's own trust's (for example, Manchester University NHS Foundation Trust's) secondary-employment / declarations-of-interest policy could not be retrieved; www.england.nhs.uk was unreachable from this session, so the national guidance PDF was not read in full.
- Agenda for Change handbook provisions on outside work and the Working Time Regulations 48-hour limit across jobs were not checked.
- Whether NHS England has issued a revised COI guidance after 2017 could not be confirmed.
- "Who can be a director" rules (minimum age, disqualification) were not fetched.

---

## 2. Sole trader vs limited company: formation, filings, tax rates, director pay, identity verification, accountant cost

### Takeaway
A UK private limited company now costs **£100** to incorporate online, is usually registered within 24 hours, and costs **£50 a year** for the confirmation statement (both fees rose on 1 February 2026). Corporation Tax is 19% up to £50k profit and 25% above £250k, and dividends are taxed at **10.75% / 35.75% / 39.35%** for 2026-27. For a founder who is still a higher-rate NHS earner, extracting all profit as dividends costs about 47.5% combined. A company still wins on liability protection, retaining profits at 19%, credibility with colleges and hospitals, SEIS/EIS eligibility, and avoiding Making Tax Digital for sole traders. One trap: if the founder also controls an Indian company, it probably counts as an "associated company" and halves the 19%/25% thresholds.

### Cited Findings
**Formation and Companies House fees**
- Registering a company online "costs £100" and the company "is usually registered within 24 hours"; you need at least one director and one shareholder (who can be the director), and you must register for PAYE "including yourself if you're the only director" [LIVE] — [GOV.UK: Register your company](https://www.gov.uk/limited-company-formation/register-your-company)
- Companies House fee table: incorporation **£100** online/software, **£124** paper, **£156** same-day; confirmation statement **£50** online/software, **£110** paper; voluntary strike-off £13 online; change of name £20 [LIVE] — [Companies House fees (updated 25 Sep 2026)](https://www.gov.uk/government/publications/companies-house-fees/companies-house-fees)
- These fees changed **from 1 February 2026** (incorporation digital fee to £100, confirmation statement digital fee to £50, strike-off to £13); Companies House links the income partly to its new ECCT Act enforcement powers [LIVE] — [GOV.UK news, 5 Nov 2025](https://www.gov.uk/government/news/companies-house-fees-are-changing-from-1-february-2026)

**Identity verification (ECCT Act 2023)**
- Identity verification became a legal requirement on **18 November 2025**. Existing directors provide their personal code with the company's next confirmation statement (for each company they direct). New companies must give each director's code at registration. A person who is both director and PSC must provide the code separately for each role; the PSC code is due within a 14-day window starting the day after the confirmation statement date [LIVE] — [GOV.UK: When you need to verify](https://www.gov.uk/guidance/when-you-need-to-verify-your-identity-for-companies-house)
- Verification for people who file at Companies House, corporate directors and officers of corporate PSCs is "at a later date"; in future, businesses filing for clients must register as authorised agents (ACSPs) [LIVE] — same page

**Annual accounts (ECCT Act changes, 2026 update)**
- On **23 October 2026** the government **paused** the requirement for small and micro companies to file a profit-and-loss account. Abridged accounts and "filleting" the P&L remain available after 1 April 2028 [LIVE] — [Companies House: update to accounts filing from April 2028](https://www.gov.uk/government/news/companies-house-update-to-accounts-filing-from-april-2028)
- From **April 2028**, all companies must file accounts in **iXBRL using commercial software**, and the web and paper accounts filing routes close. This applies whether the company or an accountant files. Also from April 2028: a strengthened audit-exemption eligibility statement and limits on shortening accounting reference periods [LIVE] — same page (announced, not yet in force)
- Earlier commentary had cited April 2027 for these changes; that date is superseded [SEARCH] — [PKF Smith Cooper / Rapid Formations summaries](https://www.rapidformations.co.uk/blog/companies-house-profit-and-loss-filing/)

**Corporation Tax**
- The main rate is **25%** for profits over **£250,000**; the small profits rate is **19%** for profits of **£50,000 or less**; Marginal Relief applies between them. The thresholds are reduced for short accounting periods and divided by the number of associated companies [LIVE] — [GOV.UK: Corporation Tax rates](https://www.gov.uk/corporation-tax-rates)
- Example: with 3 other associated companies the limits are divided by 4, so the lower limit is **£12,500** and the upper **£62,500**; non-UK resident companies cannot claim Marginal Relief [LIVE] — [GOV.UK: Marginal Relief](https://www.gov.uk/guidance/corporation-tax-marginal-relief)
- CTA 2010 s18E: a company is associated with another if, at any time in the preceding 12 months, "one of the two has control of the other, or both are under the control of the same person or persons". The statutory text contains no UK-residence limitation [LIVE] — [legislation.gov.uk CTA 2010 s18E](https://www.legislation.gov.uk/ukpga/2010/4/section/18E)

**Dividends, income tax, director's salary (2026-27)**
- Dividend allowance **£500**. Rates above the allowance for 6 April 2026 to 5 April 2027: basic **10.75%**, higher **35.75%**, additional **39.35%** [LIVE] — [GOV.UK: Tax on dividends](https://www.gov.uk/tax-on-dividends)
- Personal Allowance **£12,570** (withdrawn £1 for £2 above £100,000, zero at **£125,140**); basic 20% to £50,270; higher 40% to £125,140; additional 45% (England/Wales/NI) [LIVE] — [GOV.UK: Income Tax rates](https://www.gov.uk/income-tax-rates)
- Employer NIC thresholds and rates 2026-27: secondary threshold **£96/week (£5,000/year)**; employer rate **15%**; lower earnings limit **£129/week**; primary threshold **£242/week**; upper earnings limit **£967/week**; employee rates **8%** between PT and UEL and **2%** above; **Employment Allowance £10,500** [LIVE] — [GOV.UK: Rates and thresholds for employers 2026 to 2027](https://www.gov.uk/guidance/rates-and-thresholds-for-employers-2026-to-2027)
- Budget 2026 (28 Oct 2026): "no increase to the headline rates of income tax, National Insurance contributions or VAT". Savings income rates rise by 2pp on top of the 2pp already announced at Budget 2025, to **24% / 44% / 49% from 6 April 2027**; property income rates go to 24% / 44% / 49% from the same date (announced, to be legislated in Finance Bill 2026-27) [LIVE] — [Budget 2026](https://www.gov.uk/government/publications/budget-2026-document/budget-2026-html)

**Sole trader route**
- You can start trading immediately but must register for Self Assessment if self-employment income exceeds **£1,000** in a tax year (the trading allowance) [LIVE] — [GOV.UK: Set up as a sole trader](https://www.gov.uk/set-up-sole-trader); [GOV.UK: Income Tax rates](https://www.gov.uk/income-tax-rates)
- **Making Tax Digital for Income Tax** has been mandatory **from 6 April 2026** for those with self-employment plus property "qualifying income" (turnover, from the previous year's return) over **£50,000**. Others may be brought in from 6 April 2027 and can volunteer now. There are no penalty points for late quarterly updates in the first year (2026-27) [LIVE] — [GOV.UK: Sign up for MTD for Income Tax](https://www.gov.uk/guidance/sign-up-for-making-tax-digital-for-income-tax)
- Budget 2026: April 2027 joiners get no penalty points for their first four quarterly updates in 2027-28, and roll-out to "several taxpayer groups" is deferred "until further notice" [LIVE] — [Budget 2026](https://www.gov.uk/government/publications/budget-2026-document/budget-2026-html)

**Accountant cost (secondary sources only)**
- A small limited company typically pays about **£1,000–£3,000 a year** (or £80–£250 a month). A single-director, low-turnover company might budget **£100–£150 a month (about £1,200–£1,800 a year)**. A personal Self Assessment return is about **£150–£350 a year** if billed separately. VAT returns are extra, around **£100–£250 per quarter** in one source. These figures come from accountancy firms' own marketing pages [SEARCH] — [Sleek](https://sleek.com/uk/resources/how-much-does-an-accountant-cost/); [Accounts OS](https://accounts-os.com/blog/limited-company-accountant-cost-uk); [Accotax](https://accotax.co.uk/accountant-cost-for-a-small-business/); [Goforma](https://www.goforma.com/small-business-accounting/how-much-should-accounting-cost)

### Inferences
- **Worked example: higher-rate founder (still on an NHS salary), company profit £40,000, all extracted as dividends.** CT at 19% = £7,600. Dividend £32,400: £500 tax-free, then £31,900 × 35.75% = £11,404. Total tax £19,004, about **47.5%**. The same profit as a sole trader would bear 40% income tax (£16,000) plus Class 4 NIC (rate not verified this session). Extracting everything does not save tax. A company helps if profits are **left in the company** (19% now, dividend tax deferred until the founder is a lower earner, for example after leaving the NHS).
- **Basic-rate founder (after going full-time):** CT 19% plus 10.75% dividend tax gives a combined marginal rate of about **27.7%** (1 − 0.81 × 0.8925), against 20% income tax plus Class 4 NIC as a sole trader. The tax gap is small. The case for a company rests on limited liability, B2B credibility, investor schemes (SEIS/EIS need a company) and MTD avoidance.
- **Director's salary while still employed by the NHS:** the NHS job already uses the Personal Allowance, so any director's salary is taxed at 20%/40% under a BR/D0 code. A small salary (for example up to the £5,000 secondary threshold) mainly gives a CT deduction worth 19%, which is less than the income tax it triggers. Paying little or no salary while NHS-employed is therefore likely, and a salary near £12,570 makes more sense once the NHS income stops. Confirm with an accountant.
- **Employment Allowance:** the £10,500 figure is [LIVE], but the rule that a company whose only employee is a director cannot claim it was not verified this session; see Gaps.
- **Associated-company trap:** if the founder controls both a UK Ltd and an Indian Pvt Ltd (or a Kerala co-founder and the founder jointly control both), s18E's "control by the same person or persons" test, which has no residence carve-out, would make them associated. The UK company's 19% band would then fall to £25,000 and the 25% threshold to £125,000. This is a reason to think carefully before creating two companies.

### Gaps
- Class 4 NIC rates for 2026-27 and the Class 2 position were not fetched.
- The Employment Allowance exclusion for single-director companies was not verified on GOV.UK this session.
- The Marginal Relief fraction (3/200) was not re-checked this session.
- MTD thresholds for April 2027 (£30,000) and April 2028 (£20,000) were not visible on the fetched page; the Budget 2026 "deferral for several taxpayer groups" was not detailed in the section read.
- Business bank account, registered-office service and bookkeeping software costs were not researched.

---

## 3. VAT and digital-services tax obligations when a UK entity sells to the UK, EU, India and the Gulf, and how a Merchant of Record changes this

### Takeaway
Selling e-services directly creates **multiple tax registrations from the first sale abroad**. UK VAT applies only to UK consumers, with a £90,000 threshold that ignores out-of-scope overseas sales. The EU requires a non-Union OSS registration in one member state. India requires a simplified OIDAR GST registration (Form REG-10, monthly GSTR-5A, IGST, reportedly 18%). The UAE (5%) and Saudi Arabia (15%) reportedly require registration with no threshold. A **Merchant of Record** (Paddle 5% + 50¢; Stripe Managed Payments +3.5% on top of Stripe fees; Lemon Squeezy reportedly 5% + 50¢ plus surcharges) becomes the legal seller and takes on these obligations. For a one-person start-up this is the practical route for B2C sales. College and hospital licences (B2B) are usually handled under reverse charge.

### Cited Findings
**UK VAT**
- Registration is compulsory if taxable turnover in the last 12 months goes over **£90,000**, or is expected to exceed £90,000 in the next 30 days. Non-UK-established businesses must register from their first UK supply. "Taxable turnover is the total value of everything you sell that is not VAT exempt or 'out of scope'" [LIVE] — [GOV.UK: When to register for VAT](https://www.gov.uk/vat-registration/when-to-register)
- "If you are a business making supplies of digital services to UK consumers, those supplies are liable to UK VAT. If you make supplies of digital services to consumers outside the UK these are not liable to UK VAT. They may be liable to VAT in the country where the consumer is based." [LIVE] — [GOV.UK: VAT rules for digital services to private consumers](https://www.gov.uk/guidance/the-vat-rules-if-you-supply-digital-services-to-private-consumers)
- "If you supply digital services to consumers via a third party platform or marketplace, the digital platform is responsible for accounting for VAT on the supply instead of you." [LIVE] — same page
- Place of supply for cross-border B2C digital services is where the consumer usually lives. The supplier must obtain and keep **2 pieces of non-contradictory evidence** of that location. B2B customers (with a VAT number or other evidence of business status) account for VAT themselves [LIVE] — same page
- Education or training "delivered by a person over the internet ... (such as a webinar), is not considered to be an electronically supplied service because an actual person is involved"; the page treats automated/pre-recorded content differently [LIVE] — same page
- For the EU, a UK business can "register for the Non-Union VAT MOSS scheme in an EU member state" or register in each member state where it supplies consumers (GOV.UK still uses the older MOSS name) [LIVE] — same page
- Budget 2026 (announced, not yet in force): VAT **e-invoicing** is mandatory from **1 April 2029**. Online marketplace VAT liability is extended to UK businesses from **1 October 2027** (sellers that are UK VAT-registered or have £90,000+ annual sales per platform) [LIVE] — [Budget 2026](https://www.gov.uk/government/publications/budget-2026-document/budget-2026-html)

**India: GST on OIDAR services**
- CBIC's official flyer defines OIDAR as services delivered over the internet with minimal human intervention, for example e-books, software and digital content. When a supplier outside India supplies a **non-taxable online recipient** (an individual consumer, government and so on), "the supplier of services located in a non-taxable territory shall be the person liable for paying integrated tax". B2B supplies to GST-registered recipients are under **reverse charge** [LIVE] — [CBIC GST flyer: OIDAR (2017)](https://cbic-gst.gov.in/hindi/pdf/e-version-gst-fliers/OIDAR_online%20version_online%20version_20_July_2017.pdf)
- The overseas supplier takes "a single registration under the Simplified Registration Scheme in **Form GST REG-10**" with the **Principal Commissioner of Central Tax, Bengaluru West**. If a person in India represents the overseas supplier "for any purpose", that representative must register and pay IGST on the supplier's behalf; otherwise the supplier may appoint someone in India for that purpose [LIVE] — same flyer
- An overseas **intermediary** that arranges the supply is treated as the supplier unless its invoice identifies the underlying supplier and it neither collects payment, authorises delivery nor sets the terms. This is the legal basis on which a payment platform acting as reseller takes on the GST [LIVE] — same flyer
- From **1 October 2023**, Finance Act 2023 removed the "essentially automated / minimal human intervention" condition from the OIDAR definition (IGST Act s2(17)) and widened "non-taxable online recipient" to cover unregistered recipients. This brings online education and interactive tools more clearly into scope. One source notes that commencement depended on gazette notification [SEARCH] — [India Briefing](https://www.india-briefing.com/news/indias-oidar-taxation-shift-key-changes-effective-october-1-2023-29757.html); [Treelife](https://treelife.in/legal/oidar-registration-in-india/); [Mondaq](https://mondaq.com/india/sales-taxes-vat-gst/1410518/enhanced-enforcement-by-indian-gst-authorities-against-non-resident-digital-services-providers-post-amendments-with-effect-from-1-october-2023); [International Tax Review](https://www.internationaltaxreview.com/article/2bo11fw3uf78m0l96h2bk/local-insights/the-global-impact-of-changes-to-indias-gst-law)
- There is no turnover threshold; registration is required from the first B2C supply. Returns are filed **monthly on GSTR-5A by the 20th** of the following month, and IGST is commonly cited at **18%** [SEARCH] — [ClearTax](https://cleartax.in/s/oidar-gst-registration); [Grant Thornton flyer](https://www.grantthornton.in/globalassets/1.-member-firms/india/assets/pdfs/oidar-flyer.pdf)

**Gulf**
- **UAE**: a non-resident e-services supplier to UAE consumers reportedly has **no registration threshold**, must register with the FTA via EmaraTax and charge **5%**; late registration is reportedly penalised at **AED 10,000**; B2B supplies are reverse-charged. One blog says registration is needed only above AED 375,000, which conflicts with the FTA clarification reported by Khaleej Times [SEARCH] — [Avalara VATlive](https://www.avalara.com/vatlive/en/country-guides/africa-and-middle-east/united-arab-emirates/uae-vat-on-digital-and-electronic-services.html); [Khaleej Times](https://www.khaleejtimes.com/business/fta-clarifies-vat-application-for-e-commerce?amp=1); contradicted by [Farahat & Co](https://farahatco.com/blog/vat-treatment-supply-electronic-services-uae)
- **Saudi Arabia**: non-resident e-services suppliers to consumers reportedly must register with ZATCA with **no threshold** and charge **15%** (the rate rose from 5% in July 2020). Sources conflict on whether a Saudi tax representative is mandatory, and on whether registration is due within 30 days of the first supply or from the first supply [SEARCH] — [Fonoa](https://www.fonoa.com/resources/country-tax-guides/saudi-arabia/tax-on-digital-services); [Commenda](https://www.commenda.io/saudi-arabia/vat-registration-for-foreign-companies); [VATupdate](https://vatupdate.com/2023/08/07/vat-guide-for-businesses-with-customers-in-saudi-arabia)

**Merchant of Record options**
- **Paddle**: "5% + 50¢" per transaction, no monthly fee, with custom pricing available. It is described as a full MoR that takes "total adherence to sales tax and VAT rules", fraud and chargebacks, and states "we collect the correct rate of tax, track the filing deadlines ... submit sales tax returns" [LIVE] — [Paddle pricing](https://www.paddle.com/pricing)
- **Stripe Managed Payments** (Stripe's MoR): "adds **3.5%** per successful transaction to your standard Stripe processing fees", covering global indirect tax (sales tax, VAT, GST), fraud prevention and dispute responses. Billing and local payment methods are charged separately; there are no setup fees or monthly minimums. It covers tax in **80+ countries** and 35 product categories and is "designed for businesses selling digital products and software subscriptions" [LIVE] — [Stripe Managed Payments](https://stripe.com/managed-payments); [UK page](https://stripe.com/gb/managed-payments)
- **Lemon Squeezy** (owned by Stripe): base fee reportedly **5% + 50¢**, with reported surcharges of **+1.5%** international, **+1.5%** PayPal and **+0.5%** subscriptions. A competitor claims 7% + 50¢ for some international subscriptions (single source). One aggregator wrongly describes Managed Payments as "5% + $0.50", which conflicts with Stripe's own 3.5%-plus-processing pricing [SEARCH] — [Dupple](https://dupple.com/learn/cheapest-merchant-of-record-platforms); [Fungies](https://fungies.io/alternatives/lemon-squeezy); [Creem (competitor)](https://www.creem.io/blog/honest-payment-fee-breakdown-creem-vs-stripe-paddle-ls)

### Inferences
- A simulator delivered without a live teacher is an electronically supplied service in the UK framing, and almost certainly OIDAR in India after the 2023 amendment. Live mentor cohorts are a different supply: in the UK framing, education delivered by a person is not an ESS, so place-of-supply rules differ.
- Because B2C digital supplies to consumers outside the UK are "not liable to UK VAT", they appear not to count towards the UK's £90,000 threshold, which counts only taxable (not out-of-scope) turnover. A UK company selling mostly to India and the Gulf could therefore stay below UK VAT registration for a long time while owing GST/VAT abroad from sale one, unless it uses an MoR.
- **Effective MoR cost comparison:** Stripe Managed Payments on a UK card is 3.5% + 1.5% + 20p = **5% + 20p**. On an international (for example Indian) card it is 3.5% + 3.15% + 20p, plus 2% if currency conversion is needed, so up to **8.65% + 20p**. Paddle's headline is **5% + 50¢** all-in. On a ₹999 (about £9) sale the fixed 50¢/20p component adds roughly 2–5 percentage points, so price points below about £5 are expensive under any MoR.
- The CBIC "representative in India for any purpose" rule matters for the Kerala co-founder. If they act for the UK company in India (selling to colleges, support), they may become the person liable to register and pay IGST on its OIDAR supplies. That is another reason to route B2C sales through an MoR and to document the co-founder's role carefully.
- College and hospital licences to GST-registered Indian institutions fall under reverse charge, so the institution self-accounts. Many private colleges may be unregistered, however, and after 2023 sales to them might count as supplies to non-taxable online recipients. The UK company would then need an OIDAR registration, or an MoR/invoicing partner, even for B2B licences.

### Gaps
- The EU OSS threshold position (that the €10,000 EU-wide threshold applies only to EU-established suppliers, not UK ones) and the current EU scheme name were not verified on an EU source this session.
- The Indian IGST rate on OIDAR (18%), GSTR-5A due date and post-2023 text of IGST Act s2(16)/(17) were not read on CBIC this session; the CBIC flyer read is the 2017 version and predates the amendment.
- Whether online courses by a non-"educational institution" can be exempt in India was not checked.
- Qatar and Kuwait (reportedly no VAT), Oman and Bahrain digital-services VAT were not researched.
- The UK VAT education exemption ("eligible body") was not checked; it most likely does not cover a commercial simulator but this was not verified.
- Whether Paddle and Stripe Managed Payments accept a newly formed UK Ltd, or a sole trader, selling "education/training" (some MoRs restrict courses or human-delivered services) was not verified; Paddle's acceptable-use list and the Managed Payments eligible-country list were not read.
- India's 2% equalisation levy on e-commerce operators was reportedly abolished from 1 August 2024, but no source confirming this was retrieved.

---

## 4. UK tax position of the founder (worldwide income, FIG regime, UK–India treaty, PE/residence risk)

### Takeaway
As a long-term UK resident, the founder pays UK tax on worldwide income on the arising basis. The remittance basis ended on 6 April 2025, and its replacement, the 4-year FIG regime, is only for people arriving after 10 years of non-residence, so it does not apply. Dividends or salary from an Indian company, and interest on Indian deposits (including India-exempt NRE interest), are taxable in the UK, with credit for Indian tax under the 1993 UK–India treaty (India may tax dividends at up to 10%). The bigger structural risk is that running an Indian company from Manchester can make it UK-resident or give it a UK PE. Under the MLI, dual-resident companies get no treaty tie-breaker unless the two tax authorities agree.

### Cited Findings
- Residents "normally pay UK tax on all their income, whether it's from the UK or abroad"; non-residents pay UK tax only on UK income. Residence follows the statutory residence test: 183+ days is automatically resident, and fewer than 16 days (46 if not resident in the previous 3 years) is usually non-resident [LIVE] — [GOV.UK: Tax on foreign income – residence](https://www.gov.uk/tax-foreign-income/residence)
- "On 6 April 2025 the 4-year foreign income and gains regime replaced the remittance basis." It is available only to someone in their first 4 years of UK tax residence after **at least 10 consecutive years of non-UK residence**. Eligible income includes profits of a trade carried on wholly outside the UK, dividends from non-UK companies and foreign interest; foreign employment income is excluded. Claimants lose the Personal Allowance and CGT annual exemption [LIVE] — [GOV.UK: Check if you can claim the 4-year FIG regime](https://www.gov.uk/guidance/check-if-you-can-claim-the-4-year-foreign-income-and-gains-regime)
- **UK–India DTC (1993, as modified by the 2013 protocol and the MLI), Article 11 (Dividends):** dividends may be taxed in the residence state. The source state may also tax them, capped at **10%** of the gross for a resident beneficial owner (15% for certain real-estate investment vehicles) [LIVE] — [GOV.UK: UK–India synthesised text (MLI + 1993 DTC)](https://www.gov.uk/government/publications/india-tax-treaties/2020-uk-india-synthesised-text-of-the-multilateral-instrument-and-the-1993-double-taxation-convention-in-force)
- **Article 24:** Indian tax paid on Indian-source income is allowed "as a credit against any United Kingdom tax computed by reference to the same profits, income or chargeable gains". For a UK company holding at least 10% of an Indian company, the credit also covers Indian underlying corporate tax [LIVE] — same
- **Article 7 (Business profits):** an enterprise's profits are taxable only in its home state unless it carries on business in the other state through a PE, and then only profits attributable to that PE [LIVE] — same
- **Article 5 (PE):** a PE is "a fixed place of business through which the business of an enterprise is wholly or partly carried on" and includes "a place of management", a branch and an office. It also includes a **services PE**, where an enterprise furnishes services (including managerial services) in the other state through employees or other personnel for more than **90 days** in any 12-month period, or more than **30 days** for an associated enterprise [LIVE] — same
- **Article 4(3) as replaced by MLI Article 4:** for a company resident in both states, the competent authorities "shall endeavour to determine by mutual agreement" its residence, having regard to place of effective management, place of incorporation and other factors. "In the absence of such agreement, such person shall not be entitled to any relief or exemption from tax provided by [this Convention]" except as agreed [LIVE] — same
- **Article 13 (Royalties and fees for technical services):** the source state may tax royalties/FTS paid to a treaty resident, capped at **15%** of the gross for copyright/patent-type royalties after the initial years (20% in the first five years, now long past) and **10%** for equipment royalties [LIVE] — same
- **Article 17:** directors' fees paid by a company resident in one state to a director resident in the other "may be taxed in that other State" [LIVE] — same
- **UK–India Double Contributions Convention:** in force from **15 July 2026** together with the UK–India CETA trade agreement [LIVE] — [Budget 2026, measure 77](https://www.gov.uk/government/publications/budget-2026-document/budget-2026-html). Detached workers pay only into their home social-security scheme while temporarily working in the other country, for up to **60 months** (extended from 36 in a 17 June 2026 update) [LIVE] — [GOV.UK: DCC explainer](https://www.gov.uk/government/publications/uk-india-trade-deal-double-contributions-convention-explainer)
- From 6 April 2027, UK tax on savings income (including foreign interest) rises to **24% / 44% / 49%** (announced at Budget 2026, to be legislated) [LIVE] — [Budget 2026](https://www.gov.uk/government/publications/budget-2026-document/budget-2026-html)
- HMRC issues certificates of residence, used to claim treaty rates such as reduced Indian withholding [LIVE, title only from GOV.UK search] — [GOV.UK: Apply for a certificate of residence](https://www.gov.uk/guidance/apply-for-a-certificate-of-residence-or-letter-of-confirmation)

### Inferences
- The founder (ILR, usually 5+ years in the UK) cannot meet the 10-year non-residence condition, so the FIG regime is unavailable. All Indian dividends, salary, director fees, rent and interest (including NRE deposit interest, which India exempts for NRIs) are taxable in the UK as they arise, with foreign tax credit relief capped at the UK tax on the same income. With savings rates rising to 24%/44% from April 2027, Indian fixed deposits become noticeably less attractive for a UK-resident higher-rate taxpayer.
- **If the founder also owns an Indian company:** dividends to the founder suffer Indian withholding (capped at 10% with a UK certificate of residence and the Indian treaty paperwork) and then UK dividend tax at 10.75%/35.75% with credit for the Indian tax. The Indian company's own corporate tax is not creditable for an individual shareholder; Article 24(1)(b) only helps UK companies holding 10% or more.
- **Residence/PE risk:** if key decisions for an Indian company are taken by the founder in Manchester, the Indian company risks being UK-resident under UK case law (central management and control) and having a UK "place of management" PE. Under the MLI, a dual-resident company loses treaty relief unless the two tax authorities agree. The reverse also applies: a UK Ltd managed day-to-day by a Kerala director, or one with a Kerala office, risks Indian residence (place of effective management) or an Indian PE. The cleanest set-ups are a single UK company with the Kerala partner as a contractor or minority shareholder whose role is documented, or a UK company with a properly governed Indian subsidiary paying arm's-length transfer pricing.
- **College licences paid by Indian institutions** may suffer Indian withholding if Indian authorities treat the payment as a royalty (capped at 15% under Article 13). The UK company could credit this against UK CT under Article 24, limited to the UK tax on that income.
- A Kerala co-founder appointed as a director of the UK company may be taxed in the UK on any director's fees (Article 17), with credit in India.

### Gaps
- India-side rules (POEM under the Income-tax Act, now reportedly the Income-tax Act 2025 from 1 April 2026; withholding rates under domestic law; treatment of software licence fees as royalty after the Supreme Court's 2021 *Engineering Analysis* decision) were not verified; www.incometaxindia.gov.in returned 403.
- HMRC's guidance on company residence (central management and control, INTM120000 series) was not fetched.
- The UK's residence-based inheritance tax regime from April 2025 (relevant to Indian assets of a long-term resident) was not researched.
- Article 5(4)–(5) (dependent agent PE) was not read in full.

---

## 5. UK support schemes: SEIS/EIS, Innovate UK, R&D relief, Start Up Loans, Greater Manchester

### Takeaway
SEIS (investors get 50% relief; the company can raise up to £250k) and a **Start Up Loan** (up to £25k at 7.5%) are the most realistic UK supports for this business. **Innovate UK Smart grants have been paused since January 2025.** R&D relief is possible only for genuine technological advances, and it cannot cover subcontracted or contractor work done outside the UK, such as by a Kerala developer. The founder's own money will not attract SEIS relief if they hold more than 30% of the company. GC Business Growth Hub offers free support in Greater Manchester.

### Cited Findings
- **SEIS (company side):** maximum **£250,000** raised in total, including other de minimis state aid in the previous 3 years. The company must be established in the UK, have gross assets of no more than **£350,000** and fewer than **25** full-time-equivalent employees when the shares are issued, and its trade must not have been carried on for more than **3 years**. Money must be spent within 3 years, and the rules must be followed for 3 years after investment [LIVE] — [GOV.UK: Apply to use SEIS](https://www.gov.uk/guidance/venture-capital-schemes-apply-to-use-the-seed-enterprise-investment-scheme)
- **Investor relief:** SEIS gives **50%** income-tax relief on up to **£200,000** a year; EIS gives **30%** on up to **£1 million** (£2 million if at least £1 million goes into knowledge-intensive companies). Relief is denied if the investor or associates are "connected": employed by the company (except as a director in some cases) or holding more than **30%** [LIVE] — [GOV.UK: VC schemes tax relief for investors](https://www.gov.uk/guidance/venture-capital-schemes-tax-relief-for-investors)
- **Budget 2026 technical changes** (Finance Bill 2026-27, not yet in force): EIS relief stays available on the in-limit part of an over-limit investment; SEIS and EIS/VCT investments can be made on the same day; one investor's late payment will not affect other investors' relief [LIVE] — [GOV.UK TIIN, 28 Oct 2026](https://www.gov.uk/government/publications/changes-to-the-seed-enterprise-investment-scheme-enterprise-investment-scheme-and-venture-capital-trusts)
- **R&D (merged scheme, accounting periods from 1 April 2024):** the merged RDEC rate is **20%**. ERIS is for loss-making R&D-intensive SMEs (relevant R&D spend at least **30%** of total spend) and gives an extra **86%** deduction (186% in total) plus a payable credit of up to **14.5%** of the surrenderable loss. There are restrictions on payments to **overseas contractors** and **overseas externally provided workers** [LIVE] — [GOV.UK: Merged scheme and ERIS](https://www.gov.uk/guidance/research-and-development-rd-tax-relief-the-merged-scheme-and-enhanced-rd-intensive-support)
- Budget 2026: the R&D **Claim Notification Form is removed from 1 April 2027**, and the Additional Information Form is simplified from autumn 2027 (announced, not yet in force) [LIVE] — [Budget 2026](https://www.gov.uk/government/publications/budget-2026-document/budget-2026-html)
- **Start Up Loans:** government-backed unsecured **personal** loan of **£500–£25,000** at a fixed **7.5%** a year, repayable over **1–5 years**, with no application or early-repayment fee. It comes with free business-plan support and up to **12 months' mentoring**. Eligibility: live in the UK, be 18+, and have (or plan) a UK-based business fully trading for **less than 5 years**; a credit check applies [LIVE] — [GOV.UK: Apply for a Start Up Loan](https://www.gov.uk/apply-start-up-loan)
- **Innovate UK:** new Smart Grant competitions were paused from **January 2025**, with no Smart rounds in FY2025/26. A £130 million "Growth Catalyst" package and Innovation Loans (£100k–£5m) are cited as successors. New requests to Innovate UK Business Growth (formerly EDGE) were paused pending planning, with "more details ... in Spring 2026" [SEARCH] — [Ayming](https://www.ayming.co.uk/insights/news/innovate-uk-pauses-smart-grants-programme); [Kreston Reeves](https://www.krestonreeves.com/news/whats-next-for-uk-smart-grants/); [IUK Business Connect](https://iuk-business-connect.org.uk/news/new-funding-and-support-packages-for-innovative-smes/); [East Midlands Growth Hub](https://growthhub.eastmidlands-cca.gov.uk/grow/support-and-funding-for-innovation/innovate-uk-business-growth/); [Swoop](https://swoopfunding.com/uk/business-grants/innovate-uk-smart-grants/alternatives)
- **Greater Manchester:** GC Business Growth Hub (part of The Growth Company) delivers fully funded business support across the city-region and has a Digital, Creative and Technology arm. Programmes have included HOST's "Promote Your Tech" and "Fund Your Tech" masterclasses and a Business Support and Funding Finder. GOV.UK's finance-support finder lists a "Growth Start-up Support Programme – Greater Manchester" [SEARCH] — [Prolific North](https://www.prolificnorth.co.uk/?p=144029); [Business Manchester](https://www.businessmanchester.co.uk/?p=7757); [Stockport Council](https://www.stockport.gov.uk/profile/profile-business-growth-hub); [GOV.UK finder entry](https://gov.uk/business-finance-support/growth-start-up-support-programme-greater-manchester)
- Budget 2026 also refers to UKRI devolving Local Innovation Partnerships Fund settlements to Established Mayoral Authorities from 2028 (Greater Manchester is one) [LIVE] — [Budget 2026](https://www.gov.uk/government/publications/budget-2026-document/budget-2026-html)

### Inferences
- The edtech business should meet SEIS's trade and size tests: online education software is not obviously an excluded trade, but HMRC advance assurance should be sought. The founder, holding more than 30%, cannot get SEIS income-tax relief on their own subscription; SEIS is for outside angels, friends or family who pay UK tax. A Kerala co-founder with no UK tax bill gains nothing from SEIS relief.
- R&D relief is uncertain. Building a browser console with known techniques is routine development. Creating a novel real-time MRI/CT physics engine in the browser could qualify if it resolves genuine technological uncertainty, which would need a competent professional's view. Work subcontracted to Kerala developers would mostly be excluded by the overseas restrictions.
- A Start Up Loan is personal debt at 7.5%. Its main value may be the free mentoring and business-plan support.
- The NHS connection is an opening for NHS-backed health-innovation routes (for example Health Innovation Manchester or NHS clinical entrepreneur programmes), but these were not researched.

### Gaps
- UKRI/Innovate UK's own pages were not reachable, so the current status (November 2026) of Smart, Growth Catalyst, Innovation Loans and Business Growth is unconfirmed.
- SEIS excluded-trade lists and advance-assurance timing were not read.
- The R&D definition of "advance in science or technology" (DSIT guidelines) was not fetched.
- Health Innovation Manchester, NHS Clinical Entrepreneur Programme and SBRI Healthcare were not researched.
- Whether Budget 2025 raised EIS company-level limits was not verified; the investor page read shows only investor limits.

---

## 6. Taking payments from the UK (Stripe UK, INR/UPI from Indian students, Razorpay, Paddle, FX)

### Takeaway
A UK Stripe account pays **1.5% + 20p** on standard UK cards, **3.15% + 20p** on international cards, and **+2%** when currency conversion is needed. Stripe's UK price list now includes **UPI at 2% + 1.5% international + 2% FX**, but eligibility was not verified. Paddle reportedly supports **UPI for INR-priced items, including UPI AutoPay** for subscriptions (capped at ₹15,000 per renewal), and acts as MoR. Razorpay's docs mention foreign onboarding only for **US** businesses. Card-only collection from Indian students will lose some conversions, since UPI dominates Indian online payments.

### Cited Findings
- **Stripe UK standard pricing:** **1.5% + 20p** standard UK cards; **2.8% + 20p** premium UK cards; **2.5% + 20p** EEA cards; **3.15% + 20p** international cards; **+2%** if currency conversion is required. Klarna from 4.99% + 35p; Bacs Direct Debit 1% (capped at £4.00); dispute fees **£20**; multi-currency settlement 1% of payout volume; Instant Payouts 1% [LIVE] — [Stripe UK pricing](https://stripe.com/gb/pricing)
- **Stripe UK local payment methods:** "UPI ... **2%** per successful charge, **+1.5%** for international transactions, **+2%** if currency conversion is required". Stripe describes UPI as having "more than 80% share of online payments" in India [LIVE] — [Stripe UK local payment methods pricing](https://stripe.com/gb/pricing/local-payment-methods)
- Stripe's Adaptive Pricing localises prices into customers' currencies in 150+ countries, with Stripe handling the exchange rates [LIVE] — [Stripe Managed Payments](https://stripe.com/managed-payments)
- **Paddle UPI:** shown only for items priced in **INR** where the customer address is in India. Limits are **₹100,000 per transaction** and **₹15,000 per renewal** for subscriptions. **UPI AutoPay** in Paddle Billing was announced on **17 June 2026**, letting buyers approve once and have renewals collected automatically. A separate early-access "UPI International" option covers one-time USD items [SEARCH] — [Paddle developer docs: UPI](https://developer.paddle.com/concepts/payment-methods/upi); [Paddle changelog: UPI AutoPay](https://developer.paddle.com/changelog/2026/upi-autopay/)
- **Razorpay:** its international-payments docs say "American businesses can collect payments from foreign-issued cards ... Indian payment methods: American businesses can accept payments from Indian customers using payment methods such as credit cards and debit cards ... settled into the business's overseas bank account". The page did not mention UK businesses [LIVE] — [Razorpay docs: International payments](https://razorpay.com/docs/payments/international-payments/)
- A Paddle customer testimonial on the pricing page says cross-border card fees were "around 3.5% with Stripe and 4.5% with PayPal" (an anecdote, not a price list) [LIVE] — [Paddle pricing](https://www.paddle.com/pricing)

### Inferences
- **Direct Stripe UK, Indian student paying ₹999 by UPI:** about 2% + 1.5% + 2% = **5.5%** if settled in GBP, before any UPI-specific conditions. By international card: 3.15% + 20p + 2% ≈ **5.15% + 20p**. With direct Stripe, though, the UK company itself owes Indian OIDAR GST (section 3). **Via Paddle:** 5% + 50¢ all-in, with Paddle as seller handling GST. On low-priced plans the 50¢ fixed fee dominates (about 5% extra on a ₹999 ≈ £9 plan). Bundling (annual plans) helps.
- For Indian-issued cards, recurring card billing faces RBI e-mandate rules, so UPI AutoPay (via Paddle, or possibly Stripe) is the more reliable subscription route for Indian students.
- Razorpay's evidence points to US-only onboarding for foreign entities, so a UK company would not get Razorpay's domestic UPI rates (reported around 2% in the earlier report, not re-verified). The cheapest UPI acceptance would come from an Indian entity or an Indian MoR, which belongs in the Kerala-side research.
- GBP settlement of INR/AED revenue carries Stripe's 2% conversion fee. Holding multi-currency balances costs 1% of payout volume, so pricing in INR and AED and settling in GBP has a real FX cost of about 1–2%.

### Gaps
- docs.stripe.com was blocked, so whether UK Stripe accounts can actually enable UPI (any preview or invite status, recurring support, INR presentment) is unverified; only the price list was read.
- Paddle's UPI page and fees were not read directly (developer.paddle.com is not on the allowed list).
- PayPal's India restrictions (PayPal has not supported domestic India payments since 2021, per general knowledge) were not verified.
- Wise/Airwallex business-account FX costs were not researched.
- How Indian students' bank forex mark-ups and any TCS under the Liberalised Remittance Scheme apply to card payments to a foreign merchant was not researched.

---

## 7. Rough annual running cost of a UK Ltd (formation, accountant, insurance, ICO fee) in GBP

### Takeaway
On verified statutory fees plus secondary-source estimates for professional services, a small UK Ltd runs at roughly **£2,000–£5,000 a year** before payment/MoR fees, staff and hosting. Most of that is accountancy and insurance. Statutory costs are small: £100 incorporation once, a £50 confirmation statement, and a £47–£52 ICO fee.

### Cited Findings
- Incorporation **£100** (once), confirmation statement **£50 a year** (online) [LIVE] — [Companies House fees](https://www.gov.uk/government/publications/companies-house-fees/companies-house-fees)
- **ICO data protection fee:** fees rose **29.8%** across all tiers to Tier 1 **£52** (micro: turnover up to £632,000 or no more than 10 staff), Tier 2 **£78**, Tier 3 **£3,763**, with the **£5 Direct Debit discount** retained [LIVE] — [GOV.UK: Data protection fee regime – government response](https://www.gov.uk/government/consultations/data-protection-fee-regime-proposed-changes/outcome/data-protection-fee-regime-government-response). The new fees reportedly took effect on **17 February 2025** under the Data Protection (Charges and Information) (Amendment) Regulations 2025 [SEARCH] — [Lewis Silkin](https://www.lewissilkin.com/insights/2025/02/06/fee-payable-to-the-ico-to-increase-in-february-102jzb9); [Acuity Law](https://acuitylaw.com/rise-in-ico-fees-data-protection-fees-february/)
- Accountant: **£1,000–£3,000 a year** for a small Ltd, or about **£1,200–£1,800** for a solo-director low-turnover company; director Self Assessment **£150–£350**; VAT returns extra [SEARCH] — [Sleek](https://sleek.com/uk/resources/how-much-does-an-accountant-cost/); [Accounts OS](https://accounts-os.com/blog/limited-company-accountant-cost-uk); [Accotax](https://accotax.co.uk/accountant-cost-for-a-small-business/)
- **Professional indemnity:** an insurer's example quotes for software developers are **£117.37 a year** for a sole trader with no employees and **£532.42 a year** for a Ltd with two employees (£100k cover), with policies "from £6.95 per month" for up to £1m cover. General guides put typical small-business premiums at **£150–£1,200 a year** [SEARCH] — [Simply Business: software developer insurance](https://www.simplybusiness.co.uk/business-insurance/software-developers-insurance/); [Simply Business: software company insurance](https://www.simplybusiness.co.uk/business-insurance/software-company-insurance/)
- **Cyber insurance:** UK small businesses pay roughly **£100–£1,000 a year** in one guide; a 2026 broker benchmark gives **£750–£2,500** for a SaaS firm with £500k turnover and a £1m limit. The often-quoted "£1,740 average" appears to be a converted US figure. Cyber Essentials certification through an IASME body reportedly includes **£25,000** of cyber liability cover for firms under £20m turnover [SEARCH] — [Coversure](https://www.coversure.co.uk/ultimate-guide-cyber-insurance/cyber-insurance-cost/); [Connection Technologies](https://connection-technologies.co.uk/blog/cyber-insurance-uk-2026); [Get Indemnity](https://getindemnity.co.uk/business-insurance/cyber/how-much-does-cyber-insurance-cost)

### Inferences
Indicative annual budget, first full year, solo-director UK Ltd (my arithmetic; not a quote):

| Item | Low | High | Basis |
|---|---|---|---|
| Incorporation (year 1 only) | £100 | £100 | [LIVE] |
| Confirmation statement | £50 | £50 | [LIVE] |
| ICO fee (Tier 1, Direct Debit or not) | £47 | £52 | [LIVE] |
| Accountant (accounts, CT600, payroll/dividends, director SA) | £1,200 | £3,000 | [SEARCH] |
| Professional indemnity | £120 | £600 | [SEARCH] |
| Cyber insurance (or Cyber Essentials-bundled cover) | £100 | £1,500 | [SEARCH] |
| Accounting software, bank, registered office, domain/email | not researched | not researched | Gap |
| **Total before payment/MoR fees and hosting** | **≈ £1,600** | **≈ £5,300** | |

- Add VAT-return fees only once VAT-registered (above £90k UK taxable turnover, or by voluntary registration). With an MoR, foreign GST/VAT filings cost nothing extra beyond the MoR's percentage. Without one, budget for an Indian GST practitioner to file monthly GSTR-5A returns, plus UAE/KSA tax agents, none of which were researched.
- From April 2028 accounts must be filed in iXBRL via commercial software, which most accountants already use; small additional cost if self-filing.

### Gaps
- Costs of accounting software (Xero, QuickBooks, FreeAgent), business banking, registered-office/virtual-address services, Cyber Essentials certification fees, and Indian/Gulf tax-agent fees were not researched.
- The ICO fee page on ico.org.uk could not be fetched (403); the figures come from the government response on GOV.UK.

---

## 8. What changed in 2025–26, and what is announced but not yet in force (UK side)

### Takeaway
Several rules that commentators commonly cite are out of date. Companies House fees doubled on 1 February 2026; identity verification has been mandatory since 18 November 2025; the remittance basis ended on 6 April 2025; MTD for Income Tax began on 6 April 2026; Start Up Loans are now at 7.5% for businesses under 5 years old; and the April 2027 Companies House P&L-filing plan has been paused and moved. The Budget of 28 October 2026 adds announced changes for 2027–2029.

### Cited Findings
**In force (changed 2025–26)**
- Remittance basis replaced by the 4-year FIG regime, **6 April 2025** [LIVE] — [GOV.UK FIG](https://www.gov.uk/guidance/check-if-you-can-claim-the-4-year-foreign-income-and-gains-regime)
- ICO fees +29.8% (Tier 1 £52) — reported effective 17 Feb 2025 [LIVE figures / SEARCH date] — [GOV.UK response](https://www.gov.uk/government/consultations/data-protection-fee-regime-proposed-changes/outcome/data-protection-fee-regime-government-response)
- Companies House identity verification mandatory from **18 November 2025** [LIVE] — [GOV.UK](https://www.gov.uk/guidance/when-you-need-to-verify-your-identity-for-companies-house)
- Companies House fees: incorporation £100, confirmation statement £50 from **1 February 2026** [LIVE] — [GOV.UK news](https://www.gov.uk/government/news/companies-house-fees-are-changing-from-1-february-2026)
- MTD for Income Tax mandatory from **6 April 2026** above £50,000 qualifying income [LIVE] — [GOV.UK MTD](https://www.gov.uk/guidance/sign-up-for-making-tax-digital-for-income-tax)
- Dividend rates **10.75% / 35.75%** (additional 39.35%) for 2026-27 [LIVE] — [GOV.UK dividends](https://www.gov.uk/tax-on-dividends)
- Employer NIC 15% with a £5,000 secondary threshold, and Employment Allowance £10,500, for 2026-27 [LIVE] — [GOV.UK employer rates](https://www.gov.uk/guidance/rates-and-thresholds-for-employers-2026-to-2027)
- Start Up Loans at 7.5% fixed, for businesses trading less than 5 years [LIVE] — [GOV.UK](https://www.gov.uk/apply-start-up-loan)
- UK–India CETA and Double Contributions Convention in force **15 July 2026**; DCC detached-worker period 60 months [LIVE] — [Budget 2026](https://www.gov.uk/government/publications/budget-2026-document/budget-2026-html); [DCC explainer](https://www.gov.uk/government/publications/uk-india-trade-deal-double-contributions-convention-explainer)
- Budget 2026 says the UK has "concluded agreements with the Gulf Cooperation Council" [LIVE] — [Budget 2026](https://www.gov.uk/government/publications/budget-2026-document/budget-2026-html)

**Announced, not yet in force**
- R&D Claim Notification Form removed from **1 April 2027**; Additional Information Form simplified from autumn 2027 [LIVE] — [Budget 2026](https://www.gov.uk/government/publications/budget-2026-document/budget-2026-html)
- Savings and property income tax rates to **24% / 44% / 49%** from **6 April 2027** [LIVE] — same
- MTD penalty easement for April 2027 joiners; roll-out to some groups deferred [LIVE] — same
- SEIS/EIS/VCT technical fixes in Finance Bill 2026-27 [LIVE] — [GOV.UK TIIN](https://www.gov.uk/government/publications/changes-to-the-seed-enterprise-investment-scheme-enterprise-investment-scheme-and-venture-capital-trusts)
- VAT online marketplace liability extended to UK sellers from **1 October 2027** [LIVE] — [Budget 2026](https://www.gov.uk/government/publications/budget-2026-document/budget-2026-html)
- Companies House: software-only (iXBRL) accounts filing from **April 2028**; small/micro P&L filing **paused**; abridged/filleted accounts retained [LIVE] — [Companies House, 23 Oct 2026](https://www.gov.uk/government/news/companies-house-update-to-accounts-filing-from-april-2028)
- Mandatory VAT e-invoicing from **1 April 2029** [LIVE] — [Budget 2026](https://www.gov.uk/government/publications/budget-2026-document/budget-2026-html)

### Inferences
- The earlier report's figures that predate these dates (for example any "£50 incorporation / £34 confirmation statement", "6% Start Up Loan", "8.75% / 33.75% dividend rates" or "Smart grants available") should be treated as superseded.

### Gaps
- Finance Bill 2026-27 has not been published or enacted as far as this session could tell, so the Budget 2026 measures could still change.
- No check was made for UK immigration-rule changes to settlement (the 2025 "earned settlement" proposals) that might affect existing ILR holders; GOV.UK's ILR page read shows no change to ILR holders' rights.
