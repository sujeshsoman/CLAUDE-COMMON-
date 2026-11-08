# Website, hosting, accounts, paywall and payments for the Mallu Radiographer MRI/CT simulator (as of 8 November 2026)

Provenance key used throughout:
- **[LIVE]** = read on the fetched primary page itself in this session (fetched with curl through the session proxy; WebFetch could not resolve any host).
- **[SEARCH]** = only from a web-search result summary (the vendor's own page was not on the network allowlist, or could not be read). Treat as indicative; verify before quoting to customers.
- **[ESTIMATE]** = my own arithmetic on cited figures; the assumptions are stated.
- **[LOCAL]** = measured on the prototype file in this repository.
- **[EARLIER REPORT, UNVERIFIED]** = carried over from `/home/user/CLAUDE-COMMON-/reports/MRI console simulator India launch.md` and not re-checked here.

Hosts reachable for primary reading: razorpay.com, stripe.com, www.paddle.com, aws.amazon.com, scanflo.io, www.corsmed.com, www.mrieducation.com, www.gov.uk, www.rbi.org.in. **Not reachable** (all figures for them are [SEARCH]): supabase.com, cloudflare.com, vercel.com, netlify.com, firebase.google.com, clerk.com, auth0.com, memberstack.com, lemonsqueezy.com, graphy.com, teachable.com, thinkific.com, kajabi.com, learnworlds.com, tagmango.com, hostinger.in, e2enetworks.com, docs.stripe.com, developer.paddle.com, and malluradiographer.com itself, so I could not check what the current site runs on. Note: razorpay.com/pricing geo-redirects to the **US** page from this proxy. India figures come from Razorpay's official machine-readable India file `razorpay.com/pricing.md` ("Region: India (IN) | Last updated: May 2026").

Prototype facts: `mri-console/index.html` is **206,173 bytes raw and 65,576 bytes gzip-compressed**, with **no external script or URL references** **[LOCAL]**. A visitor therefore downloads about 64 KB once, and the browser computes all images locally.

---

## 1. Brand and site architecture: subdomain vs path vs new brand/domain

### Takeaway
For Google, a subdomain and a subfolder perform roughly the same, so the decision is about trust, international appeal and a future sale, not SEO. Recommendation: launch the product as a **named product brand on its own domain, endorsed by Mallu Radiographer**, for example "<ProductName> by Mallu Radiographer". Keep `malluradiographer.com/mri-simulator` and `/ct-simulator` as marketing landing pages that link to the app. If a new domain cannot be chosen quickly, `app.malluradiographer.com` or `sim.malluradiographer.com` is an acceptable interim home. "Mallu" carries a documented "sometimes derogatory" tag and search-result collisions with adult content, which is a risk with UK/Gulf hospital buyers and their web filters.

### Cited Findings
- Google's John Mueller has said Google web search "is fine with using either subdomains or subdirectories". He advised that if you don't mind either way, keep everything on the same site in subdirectories, and use subdomains "where things are really kind of slightly different". [SEARCH] — [Search Engine Journal](https://www.searchenginejournal.com/google-treats-subdomains-subdirectories-john-mueller-says/254687/); [Bruce Clay](https://www.bruceclay.com/blog/subdomains-vs-subdirectories-seo/)
- Ahrefs reports that Google takes "a little longer" to learn how to crawl a site with subdomains, but per Mueller only "a matter of days". It advises against moving between subdomain and subdirectory for SEO reasons alone. [SEARCH] — [Ahrefs](https://ahrefs.com/blog/subdomain-vs-subfolder)
- Comparable products:
  - **ScanFlo** runs as a standalone product brand at scanflo.io, with a product family (ScanFlo MRI, CT, PET-CT, Anatomy, RadPath; XR "Soon"). It has separate audience pages for Universities, Hospitals, Training institutes and Students & radiographers, plus "Book a demo" for institutions. [LIVE] — [ScanFlo](https://scanflo.io/mri); [ScanFlo pricing](https://scanflo.io/pricing)
  - **Corsmed** is also a standalone brand. It offers "Sign up free" and "Try for free", and says it is "A trusted partner to institutions around the world". [LIVE] — [Corsmed](https://www.corsmed.com/)
  - **MRI Education** keeps its browser "Virtual MRI Console" inside its course brand: "Brand new for 2026 – 12 months FREE ACCESS to our amazing MRI Simulator", bundled with the course at "£800 (£900 from January)". [LIVE] — [MRI Education](https://www.mrieducation.com/)
- Dictionaries define "Mallu" as informal slang for a person from Kerala, tagged "sometimes derogatory". Commentary says Malayalis have reclaimed it, but that it has been used in belittling ways. [SEARCH] — [Kaikki/Wiktionary](https://kaikki.org/dictionary/English/meaning/M/Ma/Mallu.html); [Babelfree](https://babelfree.com/dictionary/en/meaning-of-mallu)
- A plain web search for the word "Mallu" in this session returned many spam and adult-themed pages alongside the dictionary entries. [SEARCH, observed directly in the result list]
- Trade mark: file "Mallu Radiographer" in classes 9, 41 and 42 at ₹4,500 per class by e-filing; expect a section 9 descriptiveness objection. [EARLIER REPORT, UNVERIFIED] — [IP India](https://www.ipindia.gov.in/pages/trade-marks/learn/forms-and-official-fees)

### Inferences
- **SEO is not the deciding factor.** Google treats both options about equally, and the SEO that matters (YouTube, Instagram, "MRI simulator India" landing pages) can live on malluradiographer.com whichever host the app uses.
- **Technical reality.** The app will almost certainly be hosted separately from the current website (Cloudflare Pages, CloudFront or Vercel, while the existing site is on whatever host it uses now). A subdomain (`app.` or `sim.`) needs only one DNS record. A path (`/simulators`) needs a reverse proxy or a rebuild of the main site on the same platform. For a non-programmer, a subdomain or a separate domain is simpler.
- **Trust with colleges and hospitals, and international appeal.** UK NHS and Gulf procurement teams, and their IT web filters, will see the product name in invoices, SSO allow-lists and firewall rules. A neutral product name avoids explaining "Mallu" and avoids filter categories triggered by the adult-content collisions. Malayali audiences still get the familiar endorsement ("by Mallu Radiographer").
- **Future sale.** A product with its own domain, trade mark and customer database can be sold or licensed separately from the founder's personal creator brand. A product living at `malluradiographer.com/simulators` is entangled with a personal brand that a buyer cannot take over.
- **Suggested structure:**
  - `malluradiographer.com` keeps content, YouTube embeds, the blog and Malayalam pages, plus SEO landing pages `/mri-simulator` and `/ct-simulator`.
  - `<newbrand>.com` (or interim `app.malluradiographer.com`) hosts the console, login and checkout.
  - `<newbrand>.com/institutions` serves colleges and hospitals.
  - File trade marks for the new product name too (classes 9, 41, 42), and do a clearance search before buying the domain.

### Gaps
- I could not read malluradiographer.com, so I don't know whether it is WordPress, Wix or something else. That determines whether a path-based setup is even feasible.
- I found no survey data on how UK or Gulf buyers perceive "Mallu". The risk is inferred from dictionary tags and the search-collision observation. A quick test with five NHS or Gulf colleagues would settle it.
- I did not verify how specific edtech creators in India (e.g., Xylem, Entri) split creator brand and product brand.

---

## 2. Hosting: does location matter, and what does it cost at 1k / 10k / 50k users?

### Takeaway
**No. Do not build servers in Kerala.** The simulator is a roughly 64 KB static file that computes images on the phone. Serve it from a global CDN, which has edge servers inside India, and keep the only "server" parts (login, entitlement check, premium-module delivery) on a managed service. That costs about **US$0–45 a month at 1k–50k users** with almost no maintenance. A Kerala or Indian VPS would be slower to run, need patching and backups, and save nothing. India has **no general data-localisation rule** for an edtech app. The RBI payment-data rule binds the payment gateway, not you. DPDP cross-border rules are not in force until about May 2027, and no restricted countries are listed.

### Cited Findings
**AWS CloudFront (primary page)**
- Flat-rate plans per distribution have no overage charges [LIVE] — [AWS CloudFront pricing](https://aws.amazon.com/cloudfront/pricing/):

  | Plan | Price | Requests/month | Data transfer | S3 storage included |
  |---|---|---|---|---|
  | Free | $0/month | 1M | 100 GB | 5 GB |
  | Pro | $15/month | 10M | 50 TB | 50 GB |
  | Business | $200/month | 125M | 50 TB | 1 TB |
  | Premium | $1,000/month | 500M | 50 TB | 5 TB |

- Every plan includes CDN, DNS, always-on DDoS protection, WAF, TLS certificate and serverless edge compute. Logging starts at Pro; an uptime SLA starts at Business. Blocked DDoS and WAF-blocked requests "never count against your usage allowance". [LIVE] — [AWS CloudFront pricing](https://aws.amazon.com/cloudfront/pricing/)
- Pay-as-you-go data-out (first 10 TB): about **$0.109/GB for India** vs **$0.085/GB for Europe/US**. [SEARCH] — [BlazingCDN](https://blog.blazingcdn.com/en-us/aws-cloudfront-pricing-2026-per-gb-cost-and-regional-breakdown); [egresscost](https://egresscost.com/aws/cloudfront-pricing)
- S3 per-GB prices for Mumbai vs London could not be read: the AWS S3 page fills prices with JavaScript templates. [LIVE: page fetched, values not rendered] — [AWS S3 pricing](https://aws.amazon.com/s3/pricing/)

**Cloudflare** [SEARCH]
- Pages static-asset delivery is free and unlimited/unmetered.
- Workers Paid is $5/month with 10M requests included (overage about $0.30 per million).
- R2 has **zero egress fees**, with a free 10 GB-month of storage, 1M Class A and 10M Class B operations a month.
- Sources: [makerkit Cloudflare calculator](https://makerkit.dev/pricing-calculator/cloudflare); [flarecalc R2](https://flarecalc.com/calculators/r2); [egresscost Cloudflare](https://egresscost.com/cloudflare/)

**Cloudflare in India** [SEARCH]
- Cloudflare opened Mumbai, Chennai and New Delhi in 2015, and had 12 Indian cities by April 2022. — [Cloudflare blog 2015](https://blog.cloudflare.com/cloudflare-launches-in-india-with-data-centers-in-mumbai-chennai-and-new-delhi/); [Cloudflare blog 2022](https://blog.cloudflare.com/new-cities-april-2022-edition/)
- **Free-plan caveat:** a developer measured a free-plan site served to an Indian connection from Amsterdam at about 159 ms, against about 47 ms with no CDN. He blamed missing peering with Indian ISPs and mobile networks covering over 75% of the market. Forum users report free-plan Indian traffic routed to Amsterdam, Frankfurt or Singapore. This is anecdotal; there is no official Cloudflare statement. — [punits.dev (mirror)](https://hn.jakechampion.name/reader/https://punits.dev/blog/cloudflare-latency-india)
- No Kochi PoP was found. — [cdnplanet India](https://www.cdnplanet.com/geo/india-cdn/)

**Vercel** [SEARCH] — [makerkit Vercel](https://makerkit.dev/blog/saas/vercel-cost); [We Are Founders](https://www.wearefounders.uk/vercel-pricing-2026-what-you-actually-pay-to-host-your-startup/)
- Hobby is **personal, non-commercial only**: about 100 GB transfer and 1M edge requests.
- Pro is **$20/seat/month** with about 1 TB included, then about $0.15/GB. Some sources describe the $20 as a usage credit.

**Firebase** [SEARCH] — [SuperTokens](https://supertokens.com/blog/firebase-pricing); [issoh](https://www.issoh.co.jp/md/tech/16672)
- Hosting on Spark (free): 10 GB storage and **360 MB/day** transfer; it stops serving when the quota is exceeded.
- Blaze: about $0.15/GB.
- Firebase Auth is free up to **50,000 MAU** for email/social sign-in. Phone/SMS auth needs Blaze and is billed per SMS.

**Supabase** [SEARCH] — [makerkit Supabase](https://makerkit.dev/blog/saas/supabase-pricing); [JetAdmin](https://www.jetadmin.io/blog/supabase-pricing-2026-guide-to-plans-limits-and-real-world-costs/)
- Pro is **$25/month**, including **100,000 MAU** (then $0.00325/MAU), 250 GB egress (then $0.09/GB) and 8 GB database per project (then $0.125/GB), with a $10 compute credit.
- Each project lives in one primary region. The official docs say the "Europe" general region can deploy to **London** or Zurich, across 17 regions. — [Supabase regions](https://supabase.com/docs/guides/platform/regions)
- One blog says AWS **Mumbai (ap-south-1)** became a primary region in November 2025 (single unofficial source). — [rohitraj.tech](https://rohitraj.tech/notes/supabase-vs-firebase-india-mvp-2026)

**Indian hosts** [SEARCH]
- Hostinger India cloud plans were listed at **₹599, ₹899 and ₹1,899/month** on a 48-month prepaid term, excluding GST, on 31 Aug 2026. Renewals are much higher; one source says Startup renews at ₹1,599/month, and sources conflict. — [Zoutons](https://zoutons.com/news/hostinger-cloud-hosting-price-india-2026); [HostAdvice](https://hostadvice.com/hosting-company/hostinger-reviews/hostinger-india-pricing/)
- E2E Networks' official pricing file is headlined around GPUs ("H200/H100 Starting ₹49/hr"), in INR excluding 18% GST, from Delhi NCR and Chennai data centres. It is a GPU/VM cloud, not a simple static host. — [E2E pricing](https://www.e2enetworks.com/pricing.md)
- I found no Kerala-based hosting provider with its own data centre.

**Latency** [SEARCH] — [Anurag Bhatia](https://anuragbhatia.com/post/2025/06/india-europe-high-latency/); [BSO](https://www.bso.co/low-latency-mumbai-india-connectivity/)
- Mumbai–London median round trip is about **125 ms**. Earlier figures were about 109 ms (BSO, 2016) and about 132 ms (2025 blog).
- The physical floor is about 58–72 ms. India–London latency rose about 20% after cable cuts in September 2025.
- No Kochi-specific figure was found.

**Data localisation and legal**
- RBI's "Storage of Payment System Data" directive (6 April 2018) requires payment **system providers** to store payment data only in India. Compliance responsibility is "on the authorised / approved PSOs" and the intermediaries they engage, i.e. Razorpay, Stripe India and the banks, **not on a merchant website**. [LIVE] — [RBI FAQ](https://www.rbi.org.in/Scripts/FAQView.aspx?Id=130)
- DPDP Act section 16 uses a **negative list**: transfers abroad are allowed unless the government restricts a country, and as of mid-2026 no restricted country has been notified. Section 16 and Rule 15 are not yet in force, with sources putting operation at 13–14 May 2027. Section 16(2) preserves stricter sectoral laws, such as the RBI rule. I found no edtech-specific localisation rule. [SEARCH] — [TCSA](https://www.tcsa.in/frameworks/dpdp/cross-border-transfer); [Bar & Bench](https://www.barandbench.com/columns/the-dpdp-cross-border-transfer-rules-arent-live-yet-so-why-are-contracts-being-redrafted-as-if-they-are); [KS&K](https://ksandk.com/data-protection-and-data-privacy/cross-border-data-transfers-dpdp-act-india/)
- Most DPDP duties start around 13–14 May 2027, including verifiable parental consent and no tracking for under-18s. [EARLIER REPORT, UNVERIFIED] — [Mondaq](https://www.mondaq.com/india/data-protection/1713500/regulatory-update-notification-of-the-digital-personal-data-protection-rules-2025)

### Inferences
**Location matters very little for this product.**
- The app shell is about 64 KB gzip [LOCAL], downloaded once and then cached. All image computation is local.
- Only login, the entitlement check and premium-module download touch a server, perhaps 2–5 requests per session.
- With the database in London, each request costs about 125–150 ms extra for an Indian user [SEARCH-based]. That is under a second per session and invisible next to the phone's own compute time.
- Static files come from CDN edges inside India in any case. CloudFront prices an "India" region; Cloudflare has 12+ Indian cities.

**"Kerala because it's cheaper" is backwards.**
- A global CDN plus a managed backend costs $0–45/month (table below) and needs no server administration.
- A Kerala or Indian VPS adds patching, backups, TLS renewals, DDoS exposure and single-location risk, for the same or higher cost.
- Where the *company* is based (UK or India) is a separate question from where the *servers* are. Servers can be anywhere.

**Region choice for the database**
- Choose **Supabase London** if most early paying users and institutions are UK, or if UK GDPR simplicity matters (no restricted transfer for UK users).
- Choose **Mumbai** if India dominates and the Mumbai region is confirmed in the Supabase dashboard. You can start in one region and migrate later. That is painful but possible.

**Cloudflare free-plan routing in India is a real but small risk** for a one-off 64 KB download. CloudFront's flat-rate Free/Pro plans ($0/$15) are the safer India choice if testing on Jio/Airtel from Kerala shows Cloudflare serving from Europe. Test before choosing: run `curl -I` and check the `cf-ray` suffix (e.g. BOM/MAA vs AMS) from a Kerala mobile connection.

**Indicative monthly cost [ESTIMATE].**
- Usage assumption: a heavy scenario of **20 MB per active user per month**, allowing for future CT data, phantom packs and repeat loads. That is about 20 GB at 1k users, 200 GB at 10k and 1 TB at 50k.
- About 100 API/licence requests per user per month, so 5M requests at 50k users.
- The table covers hosting and auth only, in US$. It excludes payment fees, domain, email and the cost of the founder's time.

| Stack | 1k users | 10k users | 50k users | Notes |
|---|---|---|---|---|
| **Cloudflare Pages + Workers Paid + R2 + Supabase Pro** | ~$30 | ~$30 | ~$30–35 | Static bandwidth free; Workers $5 covers 10M req; Supabase Pro covers 100k MAU [SEARCH inputs]. Supabase Free might cover 1k (limits unverified). |
| **AWS CloudFront flat-rate + S3 + Supabase Pro** | ~$25 (Free plan: 100 GB, 1M req) | ~$40 (Pro $15) | ~$40 (Pro $15: 50 TB, 10M req) | CloudFront figures [LIVE]; includes WAF/DDoS/TLS. |
| AWS CloudFront pay-as-you-go, India traffic | ~$2 + auth | ~$22 + auth | ~$109 + auth | $0.109/GB [SEARCH]; flat-rate is cheaper and capped. |
| Vercel Pro + Supabase Pro | ~$45 | ~$45 | ~$45 | Hobby not allowed commercially [SEARCH]. |
| Firebase Hosting (Blaze) + Firebase Auth | ~$3 | ~$30 | ~$150 | $0.15/GB; Auth free ≤50k MAU [SEARCH]. Spark's 360 MB/day (~11 GB/month) only suits a pilot. |
| Hostinger India cloud + WordPress plugins | ₹599–1,899 (~$7–22) first term, plus plugins (section 6) | Probably needs a larger plan or VPS | VPS/cloud server plus admin | Renewal prices are higher [SEARCH]; single origin, no edge unless a CDN is added. |

### Gaps
- I could not read Cloudflare, Supabase, Vercel or Firebase pricing pages directly. The Supabase Free plan's MAU, egress and pause-after-inactivity limits are unverified, as is whether Cloudflare Pro changes India routing (and its price).
- I could not read S3 per-GB storage prices for Mumbai vs London (rendered by JavaScript). This is immaterial at under 50 GB.
- There is no measured Kochi-to-London or Kochi-to-CDN latency. A 2-minute test from a Kerala phone (ping, or traceroute plus `cf-ray`) would settle it.
- The rules for transferring UK users' data to India (UK GDPR adequacy or IDTA) were not researched.

---

## 3. Accounts and paywall: one free demo scan without login, everything else paid

### Takeaway
Split the single HTML file into a **public demo build** that holds only the one free protocol and phantom, and **premium modules** (other anatomies, sequences, CT, exam mode). Premium modules should be served only by a server function after it checks a logged-in user's entitlement, through short-lived signed URLs or a licence token. Use **Supabase Auth** (included in the $25 Pro plan, 100k MAU) or **Firebase Auth** (free to 50k MAU). Copy ScanFlo's account rules:
- a time-limited or one-scan free trial with no card;
- prepaid 1-, 3- and 12-month packs with **no auto-renewal**;
- **sign-in on 2 devices, one in use at a time**;
- seat-based institution licences.

Client-side code can always be copied, so the defences are **not putting premium code in the public file**, watermarking, and making updates and institutional features the value.

### Cited Findings
- **ScanFlo's live model** [LIVE] — [ScanFlo pricing](https://scanflo.io/pricing):
  - "45-minute free trial, no card".
  - MRI Student ₹933/month, or "₹2,799 paid once for 3 months", "No auto-renewal". MRI Student Pro ₹1,400/month (₹4,199 for 3 months).
  - CT Student ₹833/month (₹2,499 for 3 months); CT Student Pro ₹1,333/month (₹3,999 for 3 months).
  - "Sign in on up to 2 devices, one in use at a time".
  - "Institution – Priced by seats, for your cohorts and term dates. Book a demo"; "Seat-based licensing for cohorts".
  - The MRI page says "From ₹999/month" and "licensing is per-device within your plan". — [ScanFlo MRI](https://scanflo.io/mri)
- **Corsmed** uses free sign-up ("Sign up free", "Try for free"). [LIVE] — [Corsmed](https://www.corsmed.com/)
- **MRI Education** grants simulator access as a 12-month entitlement bundled with a paid course. [LIVE] — [MRI Education](https://www.mrieducation.com/)
- The earlier report recommends one user per account, one active session, a two-device limit and watermarked exports (Marrow and Corsmed rules). It also notes India's CCPA fined PhysicsWallah ₹5 lakh in June 2026, partly for demanding data before users could open "free" content. [EARLIER REPORT, UNVERIFIED] — [Marrow fair usage](https://www.marrow.com/fair_usage); [Mondaq](https://www.mondaq.com/india/dodd-frank-consumer-protection-act/1799382/dark-patterns-in-ed-tech-ccpa-imposes-penalty-on-physicswallah)
- **Auth pricing** [SEARCH]:
  - **Supabase Auth**: included in Pro, $25/month for 100k MAU. — [makerkit](https://makerkit.dev/blog/saas/supabase-pricing)
  - **Firebase Auth**: free to 50k MAU; SMS/phone OTP billed per SMS on Blaze. — [SuperTokens](https://supertokens.com/blog/firebase-pricing)
  - **Clerk**: Pro about $25/month ($20 annual) with $0.02 per extra user. The free allowance is reported as either 10,000 or 50,000 MAU, and a pricing-page mirror mentions "100 active organizations" free. Business is about $300/month. — [Activepieces](https://www.activepieces.com/blog/clerk-pricing-2026-free-pro-and-business-plans); [CostBench](https://costbench.com/software/developer-tools/clerk/)
  - **Auth0**: free to 25,000 MAU. B2C Essentials is $35/month for 500 MAU and about $1,400/month at 20,000 MAU. — [usagepricing](https://www.usagepricing.com/blueprint/auth0); [Auth0 llms-full](https://auth0.com/llms-full.txt)
- **No-code membership tools** [SEARCH]:
  - **Memberstack** (Webflow): Basic $29/month with 4% transaction fee and up to 1,000 members; Professional $49; Business $99 (fee reported at 0.9%, falling to 0% at higher tiers). — [Toolradar](https://toolradar.com/tools/memberstack/pricing)
  - **Outseta**: $47/month for up to 1,000 contacts with a 2% fee, per its own comparison page. — [Outseta vs Memberstack](https://www.outseta.com/vs/memberstack)
  - **MemberPress** (WordPress): Launch $199.50/year plus 4.9% per payment, Stripe only. Growth $349.50 and Scale $499.50, both 0% fee. — [Cartmango](https://cartmango.com/memberpress-pricing/)

### Inferences
**Gating architecture (custom or low-code)**
1. **Public demo build** (`/demo`). The current `index.html` is rebuilt so it contains only the one free exam (e.g., head T2 axial), with the other phantoms and sequence code removed, not just hidden. No login is needed, which keeps clear of the CCPA dark-pattern issue. A "Save my result / unlock more scans" prompt appears after the scan.
2. **Login**: email OTP or magic link plus Google sign-in, via Supabase Auth. Phone OTP costs per SMS and is optional. Ask for date of birth or confirmation of 18+ to stay clear of DPDP child-data duties.
3. **Entitlements table** in Postgres: `user_id`, `product` (mri/ct), `plan`, `valid_until`, `org_id`, `max_devices`. Row-level security means users read only their own rows.
4. **Premium modules** are separate JS/WASM and data bundles in private storage (Cloudflare R2 or Supabase Storage). A server function (Cloudflare Worker or Supabase Edge Function) checks the JWT, entitlement, expiry and device, then returns a **signed URL valid for minutes** or streams the module.
5. **Device and session limits**: a `devices` table keyed by a random device ID stored in IndexedDB. Allow two registered devices and one active session at a time, using a heartbeat every few minutes and kicking the older session. This matches ScanFlo's rule.
6. **Institution seats**: an `organisations` table holds seat count, term dates and admin users, with CSV invite or email-domain auto-join. One invoice per institution (section 4).
7. **Offline use**: give premium modules a licence token that expires (e.g., 7 days) so the app works on placements with poor signal but must re-check periodically.

**Why not "hide" premium features in one file?** Anyone can open DevTools and flip a flag. With browser-computed images, whatever reaches the phone can be copied, so the realistic goals are:
- never ship unpaid modules to unpaid users;
- tie each download to a user (watermark the console with the user's email or name, and embed the user ID in exported images);
- keep shipping updates and new protocols, so copied old versions lose value;
- put institutional value (cohort dashboards, assessments, certificates) on the server.

**Prepaid packs vs subscriptions.** ScanFlo's "paid once, no auto-renewal" model sidesteps UPI AutoPay mandates, card-tokenisation rules and the ₹15,000 frictionless-debit limit (section 4). It also suits Indian students paying from a UPI app. Start with prepaid packs and add subscriptions later for UK/Gulf card users.

**No-code paywall caveat.** Memberstack, Outseta and MemberPress gate *pages*, not the JS bundle the page loads. If the premium simulator sits at a public URL, it leaks. Pair them with a protected file endpoint: on WordPress, a PHP-served download behind the login; on Webflow, Memberstack's gated content plus a separately hosted signed-URL function. Either way, a small custom function is still needed.

### Gaps
- I could not verify the Supabase Free plan's MAU limit or inactivity pausing, Clerk's current free allowance (10k vs 50k), or whether Memberstack and Outseta support Razorpay or UPI. They appear to be Stripe-based.
- I found no published data on how much account-sharing device limits actually prevent in Indian edtech.

---

## 4. Payments: Razorpay, Cashfree, Stripe UK, Paddle, Lemon Squeezy / Stripe Managed Payments, PayPal

### Takeaway
- **If the selling entity is Indian:** use **Razorpay** for everything. India UPI, cards and netbanking cost a flat **2% + 18% GST**. International cards for UK and Gulf buyers cost **up to 3% + GST** with automatic e-FIRC. Subscriptions add **0.9%** on cards.
- **If the selling entity is a UK company:** use **Stripe UK** for UK and Gulf cards (1.5% + 20p UK; 3.15% + 20p international, plus 2% if conversion is needed). Stripe UK now offers **UPI**, priced at 2% + 1.5% international + 2% conversion, with recurring payments available. Alternatively, ask Razorpay to enable its cross-border product, which lets non-Indian businesses collect UPI, cards and netbanking from Indians and settle abroad.
- **The UK-entity catch:** a foreign supplier of online education to Indian consumers must register for Indian GST (OIDAR) **with no threshold**.
- **The no-tax-admin option:** a **Merchant of Record** takes on Indian GST, UK VAT and Gulf VAT for you. Paddle charges **5% + 50¢** and supports UPI for INR, including subscriptions up to ₹15,000 per renewal. Stripe Managed Payments adds **3.5%** on top of Stripe fees. Both cost noticeably more on low-value Indian sales.

### Cited Findings
**Razorpay – India (official India pricing file, May 2026)** [LIVE] — [Razorpay India pricing.md](https://razorpay.com/pricing.md)
- "Platform fee (all domestic instruments) **2% per successful transaction**"; "GST on platform fee 18%"; setup fee, annual maintenance and refund fees all Rs. 0.
- UPI: "Zero MDR — 2% platform fee applies". The file explains: "UPI is MDR-free per RBI policy. Razorpay's 2% applies as a platform/technology fee, not as MDR."
- Corporate/business credit cards: 2.15%. Settlement on T+1 or instant.
- International cards: "**Up to 3% per successful transaction**" plus 18% GST, with "FIRC / eFIRC (export compliance) Included, auto-generated". It supports Visa, Mastercard, Amex, Diners, Discover, JCB and UnionPay, in 135 currencies across 180+ countries. Operates "under RBI's PA-CB licence".
- International bank transfers (SWIFT/ACH/SEPA/UK Faster Payments into virtual accounts): 1% plus GST, 0% FX markup.
- Subscriptions: "Cards (Visa, Mastercard, Amex, Diners) **0.9% + Platform fees per transaction**". UPI, NACH and e-mandate are "Pricing available on request". GST (18%) applies on subscription fees.
- UPI QR (standard): 0.99%.

**Razorpay Subscriptions methods** [LIVE] — [Razorpay docs](https://razorpay.com/docs/payments/subscriptions/supported-payment-methods.md)
- Supports Cards (Visa, Mastercard, RuPay standing instructions), **UPI Autopay** and Emandate (eNACH).
- UPI Autopay: mandate "Up to ₹1,00,000"; "Frictionless debits: ₹15,000 (all) / ₹1,00,000 (BFSI only)".
- Card details must be tokenised.

**Razorpay eligibility and cross-border** [LIVE] — [Razorpay international payments docs](https://razorpay.com/docs/payments/international-payments.md)
- Indian businesses onboard with: Name (Business or Individual); type of business (Individual, Sole Proprietorship, Partnership, Private Limited, LLP and others); personal PAN (for individuals) or business PAN; KYC with address proof; and **video KYC**.
- "If you are an eligible **registered business with a valid website**, you can accept international payments" by cards, bank transfer, PayPal and local methods. "If you are an **individual**, such as a freelancer, you must integrate **PayPal** to accept international payments."
- **Foreign businesses:** "Razorpay allows foreign (non-Indian) businesses to accept payments from Indian customers without any additional paperwork or registration. Your Indian customers can make payments via local payment methods such as credit cards, debit cards, UPI and netbanking. The funds are settled in your overseas bank account." This is "an on-demand feature", activated by form.
- Warning: "Your international payment will fail if you send us a dummy email id and phone number of the customer."

**Razorpay US** (for contrast) [LIVE] — [Razorpay US pricing](https://razorpay.com/us/pricing/)
- 2.70% + $0.30 per card transaction; +1.2% for non-US cards. This is not the relevant market.

**Stripe UK** [LIVE] — [Stripe UK pricing](https://stripe.com/gb/pricing); [Stripe UK local payment methods](https://stripe.com/gb/pricing/local-payment-methods); [Stripe UPI](https://stripe.com/gb/payment-method/upi)
- Cards:
  - **1.5% + 20p** standard UK cards; 2.8% + 20p premium UK cards.
  - 2.5% + 20p EEA cards.
  - **3.15% + 20p** international cards.
  - **+2%** if currency conversion is required.
- Disputes: £20 received fee and £20 countered fee.
- No-code and hosted options: **Payment Links** and **Checkout** "Included with Payments"; custom domain US$10/month; post-payment invoices 0.4% (US$2 cap).
- **Billing**: pay-as-you-go **0.7% of Billing volume**, or from £450/month on a 1-year contract.
- **Stripe Tax** Basic: 0.5% per transaction where you are registered; Tax Complete from £70/month.
- **Invoicing**: 0.4% per paid invoice.
- **UPI**:
  - Fees: "2% per successful charge" + "1.5% for international transactions" + "2% if currency conversion is required".
  - Product page: presentment currency INR; recurring payments "Yes"; payout timing 2 days.
  - Merchant countries: "Available in … **United Kingdom**, United States", Australia, Canada, Singapore, Switzerland and EEA countries.
- **Stripe Managed Payments** (merchant of record): "3.5% per successful Managed Payments transaction in addition to Payments fees". It "includes indirect tax compliance (sales tax, VAT, GST) and remittance in more than 75 countries" (pricing page) / "80+ countries" (product page). It covers "SaaS subscriptions, digital content and virtual goods", can be applied per market or product, and includes "fraud prevention, dispute responses and transaction-level support through Onelink". Billing and local payment methods are separate. — [Stripe Managed Payments](https://stripe.com/gb/managed-payments)

**Stripe India** [LIVE] — [Stripe India pricing](https://stripe.com/in/pricing)
- "Request an invite" (invite-only).
- 2% for Indian-issued Visa/Mastercard; domestic debit MDR 0.4% capped at ₹200; 3% for foreign cards (+2% if conversion); 4.3% for international cards with USD or other currency presentment.
- The earlier report noted that individuals in India cannot accept international payments through Stripe. — [Stripe support](https://support.stripe.com/questions/accepting-international-payments-from-stripe-accounts-in-india)

**Paddle** [LIVE] — [Paddle pricing](https://www.paddle.com/pricing)
- "**5% + 50¢** per Checkout transaction", as Merchant of Record, covering payments, checkout, billing, global tax and regulatory compliance, fraud, chargebacks and buyer support.
- "No monthly fees, migration fees, or hidden extras"; "Custom pricing … for high-volume, low-value transactions".
- "If you're selling product with under 10$ value you can contact us for bespoke pricing."
- "We collect the correct rate of tax, track the filing deadlines … submit sales tax returns."

**Paddle in India**
- Paddle's blog (5 Nov 2026): "India isn't a card-first market. It's a UPI-first one". In July 2026 UPI processed 23.66 billion payments vs 707 million card payments. It lists UPI with "UPI Autopay supporting subscriptions". [LIVE] — [Paddle blog](https://www.paddle.com/blog/india-payment-methods-offering-right-ways-to-pay)
- Paddle developer docs [SEARCH] — [Paddle UPI docs](https://developer.paddle.com/concepts/payment-methods/upi); [Paddle changelog](https://developer.paddle.com/changelog/2026/upi-autopay/):
  - UPI is shown automatically to customers in India paying in INR, for one-time items and subscriptions.
  - Subscription renewals are capped at **₹15,000**; a checkout with a recurring item above ₹15,000 hides UPI. The per-transaction cap is ₹1,00,000.
  - UPI AutoPay is "now available in Paddle Billing", though the changelog called it early access.
  - "UPI International" is for USD one-time items.

**Lemon Squeezy** [SEARCH] — [Dodo review](https://dodopayments.com/blogs/lemonsqueezy-review); [Fungies](https://fungies.io/lemon-squeezy-stripe-acquisition-saas-founders-2026/)
- 5% + 50¢ per transaction.
- Stripe acquired it in 2024 and is steering sellers to Stripe Managed Payments: public preview February 2026, with Lemon Squeezy's January 2026 update pointing customers to a waitlist.
- Managed Payments works with Stripe Checkout and Payment Links; subscriptions still need Stripe Billing.
- These sources are competitor-affiliated.

**Cashfree** [SEARCH] — [Cashfree pricing help](https://www.cashfree.com/docs/help/account/pricing); [Cashfree AE](https://www.cashfree.com/ae/international-payment-gateway/); [Xflow](https://www.xflowpay.com/blog/cashfree-payment-gateway-charges)
- International Visa/Mastercard: 2.99% + GST, with a 2.69% limited-time promotion on its UAE page. Amex is 2.95%.
- The international rate excludes Amex, Diners, corporate, EMI, prepaid and subscriptions.
- The PayPal integration has no extra Cashfree fee; standard PayPal pricing applies.
- PayPal's own merchant fees were not verified.

**Indian GST on a foreign seller (OIDAR)** [SEARCH] — [Communications Today](https://www.communicationstoday.co.in/?p=252346); [Grant Thornton](https://www.grantthornton.in/globalassets/1.-member-firms/india/assets/pdfs/oidar-flyer.pdf); [WB GST FAQ](https://comtax.wb.gov.in/GST/GST_FAQ/FAQ_on_OIDAR.pdf); [India Briefing](https://www.india-briefing.com/news/oidar-compliance-india-gst-registration-ntor-gstr5a-digital-tax-43951.html/)
- After the 2023 amendment, **online education services** by overseas providers to Indian consumers are OIDAR.
- The supplier uses simplified registration (Form GST REG-10) and files monthly returns (GSTR-5A) by the 20th.
- Registration is compulsory for B2C supplies **irrespective of turnover**.
- The 18% rate is widely repeated but was not checked against a notification.

**UK VAT** [LIVE] — [GOV.UK digital services VAT](https://www.gov.uk/guidance/the-vat-rules-if-you-supply-digital-services-to-private-consumers); [GOV.UK VAT registration](https://www.gov.uk/vat-registration/when-to-register)
- "If you make supplies of digital services to consumers outside the UK these are not liable to UK VAT. They may be liable to VAT in the country where the consumer is based."
- Digital services to UK consumers are liable to UK VAT. A UK business must register once taxable turnover for the last 12 months goes over **£90,000**. Businesses based outside the UK must register for UK VAT if they supply UK consumers, with no threshold.

**RBI** [LIVE] — [RBI FAQ](https://www.rbi.org.in/Scripts/FAQView.aspx?Id=130)
- The duty to store payment data in India sits on PSOs and the gateways they engage, not on merchants.

### Inferences
**Worked fee examples [ESTIMATE; FX assumed at ₹88/US$ as in the earlier report]:**

| Sale | Route | Fee | Effective |
|---|---|---|---|
| ₹999 UPI, Indian buyer | Razorpay (Indian entity): 2% + 18% GST on fee | ₹23.58 | **2.36%** |
| ₹999 card subscription | Razorpay Subscriptions: 0.9% + 2%, + GST | ≈ ₹34.2 | 3.42% |
| ₹999 UPI | Stripe UK (UK entity, GBP settlement): 2% + 1.5% + 2% | ≈ ₹55 | 5.5% |
| ₹999 | Paddle: 5% + US$0.50 (≈ ₹44) | ≈ ₹94 | **≈ 9.4%** (ask Paddle for sub-$10 pricing) |
| £25, UK card | Stripe UK: 1.5% + 20p | £0.575 | 2.3% |
| £25, UK card | Stripe UK + Managed Payments (+3.5%) | £1.45 | 5.8% |
| £25 equivalent, Gulf card needing conversion | Stripe UK: 3.15% + 20p + 2% | ≈ £1.49 | ≈ 5.95% (≈ 9.45% with Managed Payments) |
| Gulf/UK card | Razorpay India international: up to 3% + 18% GST | — | ≈ 3.54% |

**Which combination for which entity:**
- **Indian entity** (private limited or LLP; proprietorship eligibility for a UK-resident founder is a question for the entity research):
  - Razorpay Standard for India (UPI, cards, netbanking) plus Razorpay International Cards for UK and Gulf individuals. This is the cheapest combination (about 2.4% India, about 3.5% abroad).
  - Institutions pay by Razorpay Payment Links or invoice, or by bank transfer.
  - Exports of services from India are normally zero-rated under GST with a letter of undertaking (LUT). That was not researched here; confirm with a CA.
  - UK VAT: a non-UK business selling digital services to UK consumers must register for UK VAT with no threshold [LIVE gov.uk]. That is an argument for a UK MoR (Paddle or Stripe Managed Payments) for UK B2C sales even with an Indian entity.
- **UK entity** (Ltd in Manchester):
  - Stripe UK for UK, Gulf and international cards, plus Stripe UPI or Razorpay cross-border for Indians.
  - **But** this needs Indian OIDAR GST registration from the first Indian B2C sale, plus Gulf VAT exposure (not researched).
  - The simplest compliant set-up is Paddle (or Stripe Managed Payments) as MoR for all B2C sales, with direct Stripe invoicing for B2B institutions. B2B buyers self-account for tax under reverse charge, per one source. [SEARCH] — [Registerkaro](https://www.registerkaro.in/post/oidar-in-gst)
- **Hybrid** (legitimate, since Stripe and Paddle allow per-market use): Indian entity with Razorpay for India, plus Paddle as MoR for UK, Gulf and the rest of the world. Low fees where volume is high and price is low (India), and no foreign VAT filings.

**Subscriptions vs prepaid.** Start with **prepaid 1-, 3- and 12-month packs** (ScanFlo's model), which are cheapest and avoid mandate failures. Add Razorpay UPI AutoPay or Paddle subscriptions later. Keep any recurring INR price under **₹15,000 per renewal** so UPI AutoPay stays frictionless and Paddle shows UPI.

**Avoid as primary rails:**
- Stripe India: invite-only, and individuals cannot take international payments.
- PayPal alone: buyers in India rarely use it, and fees were not verified.
- Lemon Squeezy: being folded into Stripe Managed Payments, so build on Managed Payments or Paddle instead.

### Gaps
- Razorpay's cross-border (foreign-business) fees were not on the page. Paddle's exact UPI status for UK sellers in November 2026 (docs vs "early access") is unconfirmed.
- I could not confirm whether **India** is among Stripe Managed Payments' "75+/80+ countries".
- Gulf VAT (UAE 5%, Saudi 15%) on non-resident digital suppliers was not researched; it is likely handled by a MoR.
- I did not verify PayPal's merchant fees or the Cashfree domestic rate.
- How Indian GST on exports (LUT, zero-rating) applies to a founder who is non-resident in India needs a CA.

---

## 5. Course/LMS platforms (Graphy, TagMango, Teachable, Thinkific, Kajabi, LearnWorlds)

### Takeaway
Every major LMS can show the simulator inside a lesson **only as an iframe of a URL you host elsewhere**. The LMS gates the lesson page, not the iframe URL, so you still need your own auth or signed-URL check for the premium modules. LMSs add revenue share or high monthly fees and lock customer and payment data in. Use an LMS only for **video courses that sit beside** the simulator (e.g., Graphy for Indian course buyers), **not as the simulator's paywall**.

### Cited Findings
**Graphy** [SEARCH] — [xpay](https://www.xpay.sh/agent-ready-index/graphy-software/); [Cartmango](https://cartmango.com/graphy-pricing/); [SchoolMaker](https://schoolmaker.com/blog/graphy-pricing)
- India "Launch" is ₹24,999/year plus a **10% fee per sale (or ₹10, whichever is higher)**. Revenue-share plans keep 10% or 5% for Indian creators.
- US plans are $49, $149 and $399 a month at 0% fee. Graphy may show different prices to Indian visitors.
- It refunds the plan fee only within 7 days.
- The earlier report also cited Graphy's help centre: "10% + GST" revenue share [EARLIER REPORT, UNVERIFIED].

**TagMango** [SEARCH] — [Superprofile](https://superprofile.bio/blog/tagmango-alternatives); [Exly](https://exlyapp.com/blog/?p=5400); [Republic](https://Republic.co/tagmango)
- Base plan has no monthly fee and a **10% commission**.
- Paid tiers are reported at Pro $69/month (5%), Advance $189/month (2.5%) and Ultimate (₹30,000/month or $399/month) at 0% commission. Figures conflict.

**Teachable, Thinkific, Kajabi, LearnWorlds** [SEARCH] — [SchoolMaker Teachable](https://schoolmaker.com/blog/teachable-pricing.md); [Teachery comparison](https://www.teachery.co/blog/course-platform-pricing-comparison-2026); [CostBench](https://costbench.com/compare/kajabi-vs-teachable/)
- **Teachable**: Starter $39/month ($29 annual) with **7.5%** transaction fee; higher tiers 0%.
- **Thinkific**: $36–49/month with 0% platform fee on paid plans.
- **Kajabi**: Basic about $143–179/month after a January 2026 rise; 0% fee.
- **LearnWorlds**: Pro Trainer about $99/month; mostly 0% fees.
- Teachery, the source of several comparison tables, sells a competing product.

**Embedding** [SEARCH] — [Thinkific embedded content](https://support.thinkific.com/hc/en-us/articles/39446156116759); [Thinkific troubleshooting](https://support.thinkific.com/hc/en-us/articles/360030742693); [LearnWorlds embed](https://support.learnworlds.com/support/solutions/articles/12000003622)
- Thinkific's support says external lesson content runs in an **iframe** and must be iframe-compatible (Multimedia lesson type).
- LearnWorlds has an "Embed" learning activity. No official documentation was found for running arbitrary custom JS directly inside a lesson on either platform.

### Inferences
- **Gating through an LMS is leaky.** The iframe `src` URL is visible in page source, so unless the simulator itself checks a token, anyone with the URL can use it. That means building the same auth layer as in section 3, plus single sign-on between the LMS and your app, which is harder than doing it alone.
- **Cost.** At ₹999 per sale, Graphy's 10% plus Razorpay's 2.36% leaves the creator about 87.6% [ESTIMATE]. Own-site Razorpay leaves about 97.6%.
- **Lock-in.** Student emails, payment tokens and certificates live in the LMS. Migrating subscribers off Graphy or Kajabi is possible but lossy.
- **Sensible use.** Sell video courses (physics lectures, Gulf-exam preparation) on Graphy or TagMango if the audience is already there, and include a "simulator access code" that redeems on your own site. That keeps the simulator's entitlements in your database.

### Gaps
- I could not open any LMS vendor page, so all prices are [SEARCH] with conflicts.
- I did not verify whether Graphy or TagMango allow iframe embeds of external apps in lessons, or whether they offer SSO or webhooks to sync purchases to an external app.

---

## 6. Build options, costs and time to launch

### Takeaway
The simulator already exists, so the build is a **wrapper**: landing pages, auth, entitlements, payments, premium-module delivery and an institution admin. That is roughly **120–250 developer hours** [ESTIMATE], not the 1,000–1,600 hours the earlier report estimated for building the simulator itself.

| Route | Who builds it | Cost | Time | Running cost |
|---|---|---|---|---|
| 1. Custom (recommended) | Kerala/Indian freelancer | **₹0.6–6 lakh** | 3–8 weeks | ~US$30–45/month |
| 1. Custom | UK freelancer | **£5k–20k** | 3–8 weeks | ~US$30–45/month |
| 1. Custom, AI-assisted | Founder with an AI coding assistant | Tool subscriptions plus a paid security review | — | ~US$30–45/month |
| 2. No-code | Founder or freelancer | Plugins/subscriptions (see below) | Fastest | Higher fees, weaker protection |
| 3. LMS | Founder | Revenue share/monthly fees | Fastest | Highest fees; not recommended for the simulator |

Route 1 stack: static simulator on Cloudflare Pages or CloudFront, Supabase (Auth, Postgres, Storage, Edge Functions) and Razorpay and/or Paddle.

Route 2 options: WordPress + MemberPress or WooCommerce Subscriptions + Razorpay plugin on Hostinger; or Webflow + Memberstack/Outseta.

### Cited Findings
**Freelancer rates** (no Kochi-specific data found) [SEARCH] — [Freelance Rates India calculator](https://freelanceratesindia.pages.dev/calculator/freelance-rate/web-developer); [Acquaint](https://acquaintsoft.com/blog/laravel-developer-hourly-rate-by-country); [Decipherzone](https://www.decipherzone.com/blog-detail/hiring-developers-india-vs-uk-cost-guide); [Osdire](https://osdire.com/blog/how-much-does-it-cost-to-hire-a-web-developer)
- India: **₹500–2,500/hour for domestic clients** and ₹1,500–4,000/hour ($18–48) for international clients; Laravel mid-to-senior $22–55/hour.
- UK: freelance web developer **£300–600/day**. A remote-hourly dataset gives £24.35/hour, which looks low and is undated. The search summary did not attribute the UK day rate cleanly to one page.

**No-code tool prices** [SEARCH] — [WiserReview](https://wiserreview.com/blog/woocommerce-subscriptions-alternatives/); [Dupple Webflow](https://dupple.com/pricing/webflow); [Brix](https://brixtemplates.com/blog/webflow-may-2026-pricing-changes-explained)
- WooCommerce Subscriptions about **$279/year** per site.
- Webflow Site Basic $15/month (annual); Site Premium (merged CMS/Business) $25/month annual or $39 monthly.
- Memberstack, Outseta and MemberPress are in section 3; Hostinger India in section 2.

**Hosted checkouts reduce build work** [LIVE] — [Stripe UK pricing](https://stripe.com/gb/pricing); [Razorpay India pricing.md](https://razorpay.com/pricing.md); [Paddle pricing](https://www.paddle.com/pricing)
- Stripe Payment Links ("No-code links to sell online without a website") and Checkout ("Pre-built payment form") are included in standard fees.
- Razorpay Payment Links, Pages and Buttons are listed as no-code tools.
- Paddle provides an embeddable checkout and buyer support.

### Inferences
**Effort estimate for the wrapper [ESTIMATE]:**

| Task | Hours |
|---|---|
| Landing and pricing pages (MRI, CT, institutions; English, later Malayalam) | 20–40 |
| Auth plus account page | 15–30 |
| Entitlements, device/session limit, organisations and seats | 30–60 |
| Splitting `index.html` into demo and premium modules, plus signed-URL function | 25–50 |
| Payment integration with webhooks (Razorpay and/or Paddle), invoices, refunds | 20–40 |
| Admin dashboard (users, codes, institution seats) | 10–30 |

The total is about **120–250 hours**. Costs at those hours:
- Indian freelancer at ₹500–2,500/hour: **≈ ₹60,000–6,25,000**.
- Small Kerala agency: likely mid-range, but no data was found.
- UK freelancer at £300–600 per 7.5-hour day: 16–33 days, **≈ £4,800–20,000**.
- Add a pen-test (section 7) and about 5–10 hours a month of maintenance.

**AI-assisted founder build.** Feasible because the prototype is already a single self-contained file and the stack is mainstream (Supabase plus Razorpay/Paddle webhooks). The founder pays tool subscriptions and spends evenings. The risks are auth and webhook security mistakes, so budget for a **paid code review or pen-test before taking money**. Option: AI-assisted build plus about 10–20 hours of an experienced freelancer reviewing auth, row-level security and webhooks.

**No-code vs custom for this product:**
- **WordPress + MemberPress/WooCommerce:**
  - Pro: familiar, Razorpay plugins exist, and a Kerala freelancer can maintain it.
  - Con: PHP/plugin security patching; page-level gating only; device limits need extra plugins; MemberPress Launch's 4.9% fee and Stripe-only payments [SEARCH] conflict with Razorpay/UPI unless you use a higher tier or WooCommerce.
- **Webflow + Memberstack:** polished, but Memberstack is Stripe-centric, so UPI is unclear, and there is a 4% fee on Basic.
- **Custom:** cheapest to run, protects the code best, owns the data, and is easiest to sell later.

**Costed launch blueprint [ESTIMATE].**

*Phase 0, weeks 0–2:*
- Pick the product name and domain (about £10–15/year, unverified) and file trade marks.
- Rebuild `index.html` as a demo-only build.
- Host it free on Cloudflare Pages or CloudFront Free.
- Add a waitlist form.

*Phase 1, weeks 2–8:*
- Supabase Pro ($25/month) in London or Mumbai.
- Email-OTP and Google login.
- Prepaid packs via **Razorpay** (Indian entity) or **Paddle** (UK entity), using webhooks to create entitlements.
- Signed-URL delivery of premium modules.
- Two-device, one-session rule.
- Watermark.
- A manual "institution code" for colleges, invoiced by Razorpay/Stripe invoice or bank transfer.

*Phase 2, months 3–6:*
- Institution admin (seats, term dates, CSV invites).
- Optional subscriptions (UPI AutoPay or Paddle).
- Malayalam UI.
- CT simulator module on the same entitlement system.
- Pen-test before marketing to hospitals.

*Running cost:*
- Hosting and auth: about **US$30–45/month** up to 50k users.
- Payment fees: about 2.4% India and about 3.5% international via Razorpay (Indian entity), or 5% + 50¢ via Paddle.
- Maintenance: 5–10 hours a month.

### Gaps
- No credible survey of Kochi or Thiruvananthapuram freelancer or agency rates was found; the figures are national India ranges.
- The hour estimates are mine and untested against real quotes. Get 2–3 fixed-price quotes against a written spec.
- The cost of AI coding tools was not researched.

---

## 7. Security and anti-piracy basics, minimum security, pen-test cost

### Takeaway
Minimum viable security for this product:
- HTTPS everywhere (CDNs provide TLS automatically).
- Hosted payment pages, so no card data touches your servers.
- Payment-webhook signature verification.
- Supabase row-level security on every table.
- Server-side entitlement checks before any premium module is released.
- Short-lived signed URLs, rate limits and bot protection on login/OTP.
- Backups, plus a privacy policy, terms and a grievance contact.
- An OWASP Top 10 / ASVS-level review and a small pen-test before selling to hospitals: about **£2,500–5,000 in the UK or ₹25,000–1.5 lakh in India**.

Piracy cannot be eliminated for browser-computed apps, only made inconvenient and traceable.

### Cited Findings
- CloudFront flat-rate plans bundle **WAF, always-on DDoS protection and a TLS certificate**, with WAF rules from 5 (Free) to 25 (Pro). "Advanced DDoS Protection", "JavaScript Challenge" and bot management start at Business ($200/month). [LIVE] — [AWS CloudFront pricing](https://aws.amazon.com/cloudfront/pricing/)
- Stripe includes 3D Secure on standard pricing and Radar Lite fraud protection; Paddle includes "Fraud protection … Prevent card attacks, fight bad-faith chargebacks". Hosted Checkout and Payment Links keep card entry on the provider's page. [LIVE] — [Stripe UK pricing](https://stripe.com/gb/pricing); [Paddle pricing](https://www.paddle.com/pricing)
- Razorpay rejects international payments sent with dummy customer email or phone data, which matters for any "guest checkout" design. [LIVE] — [Razorpay international payments](https://razorpay.com/docs/payments/international-payments.md)
- **UK pen-test prices** [SEARCH] — [Cyphere](https://thecyphere.com/blog/penetration-testing-cost/); [JUMPSEC](https://www.jumpsec.com/guides/how-much-does-penetration-testing-cost-in-the-uk/); [Kolonell](https://kolonell.com/en/blog/web-application-penetration-test-pricing-london-2026)
  - Small business web app: **£2,500–4,000**.
  - Narrow web app assessment: £3,000–5,000 over 2–4 days.
  - London grey-box test: £5,500–16,000 at £900–1,300/day.
- **India pen-test prices** [SEARCH] — [TCSA](https://www.tcsa.in/resources/vapt-cost-india-2026); [Cybersecify](https://cybersecify.com/blog/penetration-testing-cost-india-2026/)
  - Small web app: **₹25,000–60,000**; medium ₹60,000–1.5 lakh.
  - Another vendor gives ₹50,000–3 lakh over 5–15 days.
- Selling from your own site in India requires a published grievance officer who acknowledges complaints within 48 hours. [EARLIER REPORT, UNVERIFIED] — [SS Rana](https://ssrana.in/articles/consumer-protection-e-commerce-rules-2020/)

### Inferences
**Minimum security checklist (custom build):**
- HTTPS-only with HSTS.
- Payment webhooks verified by signature and processed idempotently. Never grant access from the browser's "payment success" redirect alone.
- Supabase row-level security on every table, with the service key only in server functions.
- Premium modules in private storage, released only via short-lived signed URLs after an entitlement check.
- Rate-limit OTP and login, and add CAPTCHA/Turnstile on sign-up.
- Never log tokens. Keep dependency updates on.
- Daily database backups (Supabase Pro includes backups; not verified here).
- Admin accounts with two-factor authentication.
- A privacy notice covering UK GDPR and DPDP, terms of use forbidding sharing, and a grievance contact.
- Before hospitals sign, expect a security questionnaire: hosting region, sub-processors (Supabase/AWS, Razorpay/Paddle), data-processing agreement and breach process.

**Anti-piracy for a browser simulator, in order of value:**
1. Never ship unpaid modules (section 3).
2. Per-user visible watermark (name or email on the console and exported images) to deter screenshots being resold and to trace leaks.
3. Device and session limits.
4. Minify and obfuscate premium bundles, or compile core physics to WebAssembly. This raises effort but does not stop copying.
5. Licence tokens that expire, plus periodic online checks.
6. Rapid updates so copied versions go stale.
7. Terms of service and takedown notices for re-hosted copies.

Accept some leakage. The defensible value is updates, institutional dashboards, assessments, certificates and the creator's community.

**Pen-test timing:** a light, automated plus manual test (India or UK) before launch. A UK CREST-type test only if an NHS trust or university asks for one. Budget £2.5k–5k, or about ₹0.5–1.5 lakh in India.

### Gaps
- OWASP ASVS and Top 10 pages (owasp.org) were not fetched, so I cite no specifics.
- Supabase's backup and point-in-time recovery terms are unverified.
- I found no data on how often browser medical-education simulators are pirated.
- NHS supplier security requirements (DSPT, DTAC) for a training tool sold to trusts were not researched. They likely apply only if NHS staff data or SSO is involved.
