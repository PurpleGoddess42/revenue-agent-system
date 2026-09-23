# Batch 1 — High Priority Deeper Verification Pass

**Date of this pass:** 2026-09-23
**Companies covered:** Beardbrand, Comme Avant, Maison Miru, Travel Cat (Your Cat Backpack)
**Purpose:** A final verification pass on the 4 companies already labeled HIGH PRIORITY in `batch-1-tracker.csv`, before any outreach is prepared. No outreach was sent or drafted as part of this pass. No facts were invented; anything not confirmable is marked UNKNOWN.

**Method note (read this before the per-company sections):** This session's outbound network access goes through a sandboxed egress proxy. Direct browsing of all four target domains (beardbrand.com, comme-avant.bio, maisonmiru.com, yourcatbackpack.com) was attempted first via a fetch tool and was blocked by that proxy in every case (`EGRESS_BLOCKED`), as it was in the original research batch. A fetch of the Gorgias case-study pages themselves (gorgias.com) and of a third-party tech-stack tool (aftership.com) was also attempted and was likewise blocked. Per the task instructions, the verification below relies on web search instead — recent (last 1–2 years where findable) search results, cached page snippets, third-party aggregators, review platforms (Trustpilot, BBB), and public LinkedIn/press content. Anything that could not be confirmed this way is marked UNKNOWN rather than assumed. This is a real limitation of this pass, not a gap in effort — it is disclosed so the operator can, if they choose, manually visit each site before outreach to close the remaining UNKNOWNs (particularly: is a live chat widget currently on each storefront, and is it Gorgias-branded).

---

## 1. BEARDBRAND

### 1. Company
- **Brand/legal name:** Beardbrand (Beardbrand LLC) — VERIFIED FACT (consistent across own site, Wikipedia, aggregators).
- **Website:** beardbrand.com — VERIFIED FACT.
- **Country/location:** United States, Austin, Texas (registered mailing address P.O. Box 13124, Austin, TX 78711) — VERIFIED FACT (found via customer-service directory listing).
- **What they sell:** Men's grooming products — beard oil, balm, wash, and hair/skin care — VERIFIED FACT.
- **DTC?** Yes — sells directly to consumers through its own Shopify storefront — VERIFIED FACT (per Practical Ecommerce reporting on their Shopify/Shopify Plus migration, unchanged from the first pass).

### 2. Why we selected them
Original evidence: founder Eric Bandholz's own quote in Beardbrand's Gorgias case study — "We're a seven-figure business and we have essentially one person on customer support and experience" — plus a description of pre-Gorgias chaos across tools (gorgias.com/customers/beardbrand). **VERIFIED FACT** (a direct quote on the vendor's own case-study page, consistent with what the first pass found).

**Currency check:** the exact publish date of that case study could not be determined this pass (Gorgias's site does not surface one in search results, and the page itself could not be fetched due to the egress block) — **UNKNOWN** how old the quote is. A related Gorgias blog post about Beardbrand's Amazon exit is dated October 13, 2023, which suggests the broader case-study relationship is at least a few years old, not brand new. This means the "one person on support" pain point should be treated as a documented historical fact, not necessarily a description of today's staffing — worth a direct check-in before assuming it's unchanged.

No new, fresher (2024–2026) public pain signal was found this pass beyond the original case-study quote — no current job posting for a support role was located (Glassdoor currently lists no open jobs at Beardbrand; their own careers page was not directly browsable). This is **UNKNOWN**, not evidence either way — it neither confirms the pain persists nor that it's been solved.

### 3. Current customer-service setup
- **Helpdesk/support platform:** Gorgias, per the company's own case study (VERIFIED FACT, historical). **New nuance found this pass:** Beardbrand's public help center lives at `support.beardbrand.com/hc/en-us/...` — this is the standard Zendesk Guide (knowledge-base) URL pattern, and multiple live article URLs were found there (e.g., order-tracking FAQ articles) — **VERIFIED FACT** that a Zendesk-hosted knowledge base/FAQ is still live at that address. This does not contradict the Gorgias case study (a brand can move ticket handling to Gorgias while leaving a legacy Zendesk Guide knowledge base in place, since migrating a KB is a separate project from migrating tickets) — but it means the "fully on Gorgias" picture from the first pass is not the complete current picture. **REASONABLE INFERENCE:** ticket handling is on Gorgias, self-service FAQ content is still hosted on a Zendesk Guide instance.
- **Chat widget:** could not be directly confirmed. A third-party tech-stack detector (AfterShip's own brand page, referenced via search) lists Beardbrand's detected stack as Klaviyo, ReCharge, Sentry, ShipStation, Yotpo, Blotout, and Google Analytics — **Gorgias does not appear in that list.** This is a weak, ambiguous signal (third-party script detectors often miss backend helpdesk tools if no public chat widget is currently embedded, or simply have incomplete coverage) — **UNKNOWN** whether a live Gorgias chat widget is currently on the storefront; it is not proof they've dropped Gorgias.
- **E-commerce platform:** Shopify Plus — VERIFIED FACT (unchanged from first pass, Practical Ecommerce reporting).
- **Order-tracking/self-service:** account order-history lookup, a shipping-confirmation email with a tracking URL, AfterShip-powered tracking, and multiple self-service FAQ articles on shipping/tracking issues (e.g., "why does my tracking say delivered," "no information available") at support.beardbrand.com — **VERIFIED FACT**. A fallback path to email support@beardbrand.com if self-service doesn't resolve it — VERIFIED FACT. Phone support at 844-662-3273, Mon–Fri 8am–5pm, is listed on a third-party customer-service directory — treat as REASONABLE INFERENCE (not confirmed on Beardbrand's own page directly).
- **Existing AI/automation for support:** no evidence found, positive or negative — **UNKNOWN**. No mention of Gorgias AI Agent, resolution-rate metrics, or any chatbot specific to Beardbrand was found in this pass. This means the offer is not confirmed redundant, but also not confirmed to still be needed at current volume.
- **Anything that could make the offer unnecessary:** the self-service order-tracking FAQ content is fairly mature and detailed already (multiple dedicated articles), which could mean a meaningful share of "where's my order" questions are already being deflected by content rather than needing an AI agent — this is a real, if modest, consideration, not previously flagged.

### 4. Decision-maker
- **Name:** Eric Bandholz — VERIFIED FACT (Beardbrand's own About page, Wikipedia, the Gorgias case study, and numerous podcast/press appearances all name him).
- **Title:** Founder & CEO — VERIFIED FACT.
- **Why he's right:** solo/founder-controlled company; he is the one quoted personally describing the support workload in Beardbrand's own case study, and appears directly (not through a spokesperson) in interviews and on social media — a founder who can plausibly say yes alone.
- **LinkedIn:** a direct personal LinkedIn profile URL for Eric Bandholz still could not be confirmed this pass — multiple LinkedIn posts about him were found, and the Beardbrand LinkedIn company page (linkedin.com/company/beardbrand), but no `linkedin.com/in/...` URL for him personally surfaced in search results. **UNKNOWN exact URL** (unchanged from first pass).
- **Public contact path:** active public X/Twitter profile @bandholz — VERIFIED FACT. General public support channel: support@beardbrand.com / 844-662-3273 (not a personal address).

### 5. Personalization angle
Beardbrand's own published case study describes the company as having "essentially one person on customer support and experience" for a self-described seven-figure business, and 60,000+ tickets migrated off Zendesk in a single weekend — a concrete, specific, first-person detail from their own materials, not a generic compliment. A second, newly found detail: Beardbrand still runs a public self-service FAQ knowledge base (at support.beardbrand.com) with detailed, granular tracking-related articles — evidence they've already invested some effort into order-status self-service, which is a genuine, specific thing to reference ("I saw you've already built out detailed tracking FAQs — this is about handling the ones that still need a real answer").

### 6. Offer fit
**KEEP, with a caveat.** The core evidence (founder's own quote about running seven-figure support with one person) remains a strong, specific, well-documented pain signal, and the company is real, active, and founder-controlled. The caveat: this pass surfaced meaningfully wider and more conflicting revenue estimates than the first pass found — see the note below — which raises the odds Beardbrand may now be larger than the target band, and the case-study quote's age is unconfirmed. Recommend confirming current revenue/team size and current live support-tool status directly on a first call, exactly as the original tracker already flagged, but now with a stronger reason to ask (see below).

**New revenue-conflict flag (important, not previously this stark):** third-party aggregators disagree sharply on Beardbrand's current revenue — one puts online-store revenue as low as ~$1.8–1.9M, another as high as ~$11M, and a 2026 podcast interview is titled "Eric Bandholz on Building Beardbrand to $50M+ in Revenue" (a LinkedIn post referencing that interview). The $50M figure is **UNKNOWN/unverified** — it appears only in one interview title found via search, was not corroborated by any other source, and podcast titles are not a reliable stand-alone revenue disclosure (they may refer to lifetime sales, a stretch goal, or be imprecise marketing copy for the episode). The founder's own direct quote calling Beardbrand a "seven-figure business" (i.e., $1M–$9.9M) remains the single most reliable, first-person data point and is the one this report weights most heavily — but the spread across sources ($1.8M to a claimed $50M+) is wide enough that current revenue must be treated as **UNKNOWN with a wide range**, not a confident $1–5M estimate, until confirmed directly.

### Summary reason to contact
Founder-led, real documented pain quote in their own words, decade-plus of order history, but confirm current revenue band and live support-tool status before or during first contact given newly surfaced conflicting size signals.

---

## 2. COMME AVANT

### 1. Company
- **Brand/legal name:** Comme Avant — VERIFIED FACT.
- **Website:** comme-avant.bio — VERIFIED FACT.
- **Country/location:** France — headquartered/manufactured near Marseille, specifically 14 avenue Émile Zola, 13170 Les Pennes-Mirabeau, France — VERIFIED FACT (address found via a public customer-service directory listing; consistent with "made in France" positioning).
- **What they sell:** Organic, solid-format personal-care products (solid shampoo, deodorant, toothpaste powder, body cream) plus organic clothing — VERIFIED FACT (their own tagline describes "Cosmétiques, Produits Ménagers & Vêtements Biologiques" — cosmetics, household products, and organic clothing — a slightly broader catalog than the "personal care only" framing in the first pass).
- **DTC?** Yes — sells directly via its own e-commerce site — VERIFIED FACT.

### 2. Why we selected them
Co-founder Sophie Lauret's quote in Comme Avant's Gorgias case study, describing Zendesk as "challenging to use and difficult for tracking social DMs," explaining the switch to Gorgias — VERIFIED FACT (direct quote, gorgias.com/customers/comme-avant). This is a real, specific, documented statement.

**Currency check:** as with Beardbrand, the exact publish date of this case study could not be determined this pass (the page could not be directly fetched, and no date surfaced in search). **UNKNOWN** how recent this is — treat as a real but possibly not brand-new data point.

### 3. Current customer-service setup
- **Helpdesk/support platform:** Gorgias, current per the case study; Zendesk and AgoraPulse, former — VERIFIED FACT (unchanged from first pass; not independently re-confirmed as still current this pass due to the fetch block, but no contradicting evidence found).
- **Chat/contact channels confirmed this pass:** a dedicated "Contactez-nous" page (comme-avant.bio/pages/contact), a customer-service phone line (04 84 89 43 18, Mon–Fri — one source lists 10am–12pm and 2pm–4pm, another lists 2pm–5pm; the two sources disagree on the exact afternoon window, so treat the precise hours as **UNKNOWN** while the existence of limited weekday phone hours is **VERIFIED FACT**), a support email (contact@comme-avant.bio), and social-media DMs (Facebook/Instagram) — VERIFIED FACT. A separate phone line exists for professional/wholesale inquiries (04 84 89 43 59), indicating they also do some B2B/wholesale business alongside DTC — **new detail, VERIFIED FACT**, not previously noted.
- **New finding — a named support person:** Comme Avant published a blog post, "Qui est derrière notre service client?" ("Who's behind our customer service?"), which names **Karine** as the person who has been personally handling their customer service for close to 2 years, described as responding to all requests herself — **VERIFIED FACT**. This is a specific and useful detail: it suggests day-to-day support is handled by one named, individual staff member (not a team), which is a concrete small-scale-operation signal directly relevant to the offer's target profile.
- **E-commerce platform:** still not independently confirmed this pass (direct site fetch was blocked) — **UNKNOWN**, same as first pass. Gorgias's customer base skews heavily Shopify, so Shopify remains a reasonable inference, not a confirmed fact.
- **Order-tracking/self-service:** not independently confirmed this pass — **UNKNOWN** (site could not be browsed).
- **Existing AI/automation for support:** no evidence found of any AI/chatbot tool in use — **UNKNOWN/no evidence found**, i.e., nothing suggests they've already solved this with automation.
- **Anything that could make the offer unnecessary:** none found. If anything, having one named person (Karine) as the entire visible customer-service operation, plus a separate wholesale contact line, strengthens the case that a single person's time is a real constraint.

### 4. Decision-maker
- **Name:** Sophie Lauret — VERIFIED FACT.
- **Title:** confirmed this pass as **Founder and Communications Director** (Crunchbase person profile), consistent with — and slightly more specific than — the first pass's "Co-Founder, Marketing & Communications." She co-founded the company with her husband, Nil Parra — VERIFIED FACT.
- **Why she's right:** she is the named co-founder quoted directly in the company's own case study about the support-tooling decision, and is publicly the communications-facing co-founder (also serves as secretary on the board of the company's associated non-profit endowment fund, "Fonds Comme Avant," per public press coverage — VERIFIED FACT) — a founder in a two-person founding team, plausible to say yes without a large approval chain.
- **LinkedIn:** linkedin.com/in/sophielauret/ — VERIFIED FACT, re-confirmed this pass via direct search hit (also appears in French as fr.linkedin.com/in/sophielauret/fr).
- **Public contact path:** the general company contact channels above (email, phone, contact form); no separate personal public business email for Sophie Lauret specifically was found — **UNKNOWN**, use LinkedIn or the general company contact channel.

### 5. Personalization angle
The newly found "Qui est derrière notre service client?" blog post is a strong, specific, and warm personalization detail — it names Karine as the real person behind their support, describing nearly two years of personally responding to every customer request. Referencing that post (truthfully, and respectfully — this is about Karine's workload, not a criticism of her) is far more specific and human than the original angle (the Zendesk-to-Gorgias switch quote), and ties directly to the offer's premise: a single person managing all inbound tickets. The original quote from Sophie Lauret about switching off Zendesk because it was "challenging to use" remains a valid secondary angle.

### 6. Offer fit
**KEEP.** Two co-founders, a named single support person, confirmed public contact channels, an existing (if unconfirmed-current) Gorgias relationship, and a large, credible review base (~57,000 Trustpilot reviews at 4.8, unchanged from the first pass and not contradicted by anything found this pass). The size/revenue uncertainty flagged in the first pass (the large review count could indicate a business larger than the target band) remains unresolved and should still be checked directly — this pass did not find a revenue figure either way.

### 7. International check (Comme Avant only)
- **Where they actually operate:** confirmed as based and manufacturing near Marseille, France (Les Pennes-Mirabeau) — VERIFIED FACT. No evidence of US or other-country operations; this is a French domestic operation that also ships internationally to some degree (the "made in France" and shipping-related search results suggest international shipping capability exists, but the specific countries and volumes are **UNKNOWN** — not independently confirmed this pass).
- **English-language practicality:** **UNKNOWN.** No direct evidence was found this pass that Comme Avant's team, website, or customer communications operate in English — search results describe the site content primarily in French, and no English-language version of the site, English social content, or English customer-service capability was confirmed. This should be treated as a genuine open question, not assumed either way.
- **Time-zone consideration:** France operates on Central European Time (UTC+1/+2 depending on daylight saving) — a 6–9 hour difference from US time zones depending on the operator's location, a real scheduling consideration for any live call.
- **Explicit note per instructions:** none of the above is a reason to remove Comme Avant from consideration. Being based outside the US, and the live-communication language/time-zone questions, are practical planning details to resolve before or during first contact (e.g., confirming Sophie Lauret's or the team's English comfort, or planning around the time-zone gap for a call) — not a fit disqualifier. The offer itself (an AI resolution workflow inside an existing helpdesk) does not depend on the operator and client sharing a first language day-to-day, though the discovery/kickoff conversations would need a working shared language.

---

## 3. MAISON MIRU

### 1. Company
- **Brand/legal name:** Maison Miru — VERIFIED FACT.
- **Website:** maisonmiru.com — VERIFIED FACT.
- **Country/location:** United States — VERIFIED FACT (LLC entity, per ZoomInfo/Crunchbase-style aggregators; no more specific city was independently re-confirmed this pass, but nothing contradicts the original US framing).
- **What they sell:** Modular, customizable fine jewelry (earrings, necklaces) designed for everyday wear — VERIFIED FACT.
- **DTC?** Yes — VERIFIED FACT.

### 2. Why we selected them
A public Trustpilot review describing "terrible customer service" with "very delayed response," which the company itself reportedly attributed to "limited employees" — VERIFIED FACT (a direct, documented complaint, unchanged from the first pass). This remains the core pain signal.

**Currency check:** this pass re-confirmed that Maison Miru's Trustpilot presence is still just **3 reviews at a 3.2 average**, and the same complaint (delayed response, "limited employees," a fit/return complication with a gold lock accessory and a $7 return charge) is the one surfaced again — **no new or additional 2024–2026 complaint was found this pass.** This means the evidence is real but is a single, low-volume data point that has not grown or been corroborated with fresh examples since the first pass — it should be treated as weaker/thinner evidence than a pattern of multiple recent complaints would be, even though it remains a genuine, specific, documented quote.

### 3. Current customer-service setup
- **Helpdesk/support platform:** still **UNKNOWN** — no Gorgias, Zendesk, or other named helpdesk tool was found associated with Maison Miru in this pass, same as the first pass. No new evidence either confirms or rules out a specific platform.
- **Chat widget:** UNKNOWN — could not verify (site not directly browsable).
- **E-commerce platform:** Shopify Plus was cited in the first pass as a "REASONABLE INFERENCE... per search summary of their tech stack"; this pass did not find independent confirmation either way — remains **REASONABLE INFERENCE at best, not VERIFIED**.
- **Order-tracking/self-service:** a public "Contact Us" page (maisonmiru.com/pages/contact-us) and support email hello@maisonmiru.com are confirmed — VERIFIED FACT (re-confirmed this pass via direct search hit). A "Customer Care" page (maisonmiru.com/pages/customer-care) was also found this pass, described as an FAQ-style resource ("The Things People Ask") — VERIFIED FACT that such a page exists; its content on order-tracking specifically was not independently confirmed (UNKNOWN).
- **Existing AI/automation for support:** no evidence found — **UNKNOWN/no evidence found**, i.e., nothing suggests they've already solved this with automation. A search for Maison Miru specifically alongside AI-chatbot terms returned no results tying the two together.
- **Anything that could make the offer unnecessary:** none found.

### 4. Decision-maker
- **Name:** Trisha Okubo — VERIFIED FACT.
- **Title:** Founder & Creative Director — VERIFIED FACT.
- **Why she's right:** sole named founder; background confirmed this pass as a former Stanford-trained engineer with prior roles as Manager of Business & Editorial Operations at Joyus and Senior Product Manager at eBay (leading social-commerce work) — VERIFIED FACT, found via press profiles (JCK, Yahoo Lifestyle, Nasdaq, sweetyhigh.com interview). A founder with an operations/product background is plausibly hands-on with exactly this kind of workflow decision, and can likely say yes alone at this company's scale.
- **LinkedIn:** linkedin.com/in/trishaokubo/ — VERIFIED FACT, re-confirmed this pass via direct search hit.
- **Public contact path:** hello@maisonmiru.com (general company inbox, not a personal address) and the site's contact form — VERIFIED FACT.

### 5. Personalization angle
Trisha Okubo's professional background — a former Stanford engineer and eBay/Joyus product-and-operations leader who now runs a jewelry brand she describes as built around the idea that "everyone deserves to play" — is a specific, true, and flattering detail distinct from the original pain-focused angle, useful as a warmer opening reference if desired. The original angle (the documented customer complaint tied to "limited employees") remains valid but should be used carefully and respectfully, since it is a single, not-freshly-corroborated review.

### 6. Offer fit
**KEEP, but treat the core evidence as thinner than the tracker currently implies.** Maison Miru remains a good structural fit (founder-led, in-range size signals, real order-tracking relevance for gift-timed jewelry purchases, Klaviyo confirmed as part of their stack), but the single specific pain signal (the 3.2-rating Trustpilot complaint) did not gain any new corroboration this pass — it is exactly the same one data point found before. This isn't a reason to drop them, but the pitch should lean more on the structural fit (small team, gift-purchase timing sensitivity, no confirmed helpdesk automation) than on treating that one review as a strong, ongoing pattern.

---

## 4. TRAVEL CAT (YOUR CAT BACKPACK)

### 1. Company
- **Brand/legal name:** Travel Cat, doing business via the site Your Cat Backpack — VERIFIED FACT.
- **Website:** yourcatbackpack.com — VERIFIED FACT.
- **Country/location:** United States — specifically Island Park, NY per its BBB business profile — VERIFIED FACT (new, more specific location than the first pass had).
- **What they sell:** Cat travel gear — backpack-style cat carriers and travel accessories ("The Fat Cat" backpack) — VERIFIED FACT.
- **DTC?** Partially — this needs an update from the first pass. Travel Cat sells directly via its own site (DTC), but this pass found new evidence that they also distribute significantly through wholesale/retail: a company-associated interview (Octane AI's blog, discussing Emily Miethner's growth story) states the brand serves customers in "100+ countries" via DTC **and** is in **"1,200+ retail locations,"** including distribution in Canada and Japan — VERIFIED FACT (found via a direct, named source quote in that published interview, though the exact figure should be treated as a company/press self-description rather than independently audited). **Conclusion: Travel Cat is a hybrid DTC + wholesale/retail brand, not a pure DTC-only operation** — the order-status/tracking automation this offer targets would apply specifically to their own direct-to-consumer Shopify orders, not to the wholesale/retail channel, so this narrows (but doesn't eliminate) the addressable ticket volume.

### 2. Why we selected them
Multiple public Trustpilot and BBB complaints describing shipping delays and difficulty reaching a person about order issues — VERIFIED FACT (unchanged premise from the first pass).

**Currency check — this pass found the evidence is genuinely recent, which strengthens confidence in it:**
- A BBB complaint describes a customer who purchased on 11/7/23, requested a return, shipped items back 11/28/23, and had not received a refund after nearly a month, plus a $10 deduction from the refund despite an advertised "FULL REFUNDS" / free-returns policy — dated late 2023, i.e., within the "last 1-2 years" recency window as of this pass.
- A second complaint, dated **August 2024**, describes a customer struggling through "umpteen emails, 4 trips to DHL drop-offs, and 2 sets of return labels" while unable to complete a return.
- These are meaningfully more recent than a stale, multi-year-old case study — this is a genuine strength of this prospect versus the other three, where the core evidence is an undated vendor case-study quote.

### 3. Current customer-service setup
- **Helpdesk/support platform:** still **UNKNOWN** — no Gorgias, Zendesk, Re:amaze, Richpanel, or other specific helpdesk tool was found tied to Travel Cat/Your Cat Backpack in this pass, despite a targeted search. Same as first pass.
- **Chat widget:** UNKNOWN — could not verify (site not directly browsable).
- **E-commerce platform:** Shopify — VERIFIED FACT (unchanged from first pass; Judge.me review widget URLs reference a `.myshopify.com` backend domain — "the-cat-backpack.myshopify.com" — found this pass, which independently corroborates Shopify as the platform).
- **Order-tracking/self-service:** a public FAQ and an international-customer FAQ exist (per the first pass, not independently re-verified this pass since direct browsing is blocked) — carry forward as VERIFIED FACT from the prior pass, not re-confirmed fresh. A current, published return policy page (yourcatbackpack.com/pages/return-policy) exists and states backpacks/beds can be exchanged or returned for store credit by mail with a free return label, subject to a $10 processing fee — VERIFIED FACT, found this pass, and directly relevant context for the return-related complaints above (the $10 fee appears to be a standing, disclosed policy now, which slightly changes the read on the older complaint about an undisclosed deduction).
- **Existing AI/automation for support:** no evidence found — **UNKNOWN/no evidence found**.
- **Anything that could make the offer unnecessary:** none found; if anything, the hybrid DTC+wholesale model and reported multi-country distribution suggest real, non-trivial order volume and complexity, which supports rather than undercuts the case for automation.

### 4. Decision-maker
- **Names:** Emily Miethner and Ian Berk, co-founders — VERIFIED FACT (unchanged).
- **Titles:** Co-Founders — VERIFIED FACT.
- **Why they're right:** husband-and-wife co-founding team; Emily Miethner is described in her own public bio and press coverage as an active, visible founder/speaker (also runs an unrelated venture, Getaway Upstate, per ZoomInfo — worth noting she may divide attention across ventures, a mild new consideration on her personal bandwidth, though this doesn't change her authority to approve a Travel Cat project). Either could plausibly authorize a project this size in a two-person founding team.
- **LinkedIn:**
  - Emily Miethner: linkedin.com/in/emilymiethner/ — VERIFIED FACT, re-confirmed this pass.
  - Ian Berk: **linkedin.com/in/ian-berk-849aa016/** — this is a **correction** to the first pass's tracker entry, which listed `linkedin.com/in/ianberk1/`. This pass found his actual, confirmed profile directly by name and current role ("Co-Founder - Your Cat Backpack - A Travel Cat Brand") at `linkedin.com/in/ian-berk-849aa016/`; the `ianberk1` URL from the original tracker was not independently re-confirmed as his and may have been an error or a stale/incorrect handle. **Use the corrected URL.**
- **Public contact path:** general company channels (FAQ/contact page); no separate personal public business email found for either co-founder — UNKNOWN, use LinkedIn or the company's general contact channel.

### 5. Personalization angle
The recent (2023–2024), specific, documented return/refund-process complaints are a genuine, current pain signal, stronger in recency than the other three companies' core evidence — but referencing customer complaints directly requires care and respect; a softer version ("I noticed a few recent reviews about the return/refund process taking longer than customers expected") is more appropriate than quoting a complaint verbatim. A second, more positive personalization detail found this pass: Ian Berk's professional background includes managing $3M+/year in digital ad spend and building other ventures from scratch — a specific, true, complimentary detail usable as a warmer opening note if preferred over the complaint-based angle.

### 6. Offer fit
**KEEP.** The core support-strain evidence is the most current/recent of the four companies (2023–2024 dated complaints, not just an undated vendor case study), the co-founders are both identifiable with corrected public contact paths, and Shopify is independently corroborated. The new hybrid DTC+wholesale finding is a real nuance — it means the addressable "order status" ticket volume this offer would target is specifically their DTC channel, not their full multi-channel business — but does not disqualify them; DTC order-status tickets almost certainly still exist at real volume given "100+ countries" of direct customer reach. Helpdesk platform remains unconfirmed and should be established on first contact, same caveat as the original tracker.

---

## SUMMARY TABLE

| Company | Decision-maker | Role | Country | Official website | LinkedIn/contact path | Support platform | KEEP/HOLD/REMOVE | Best reason to contact |
|---|---|---|---|---|---|---|---|---|
| Beardbrand | Eric Bandholz | Founder & CEO | USA (Austin, TX) | beardbrand.com | Personal LinkedIn UNKNOWN; X: @bandholz; general: support@beardbrand.com | Gorgias (ticketing, historical/VERIFIED); Zendesk Guide still hosts public FAQ KB (VERIFIED, new finding); live chat widget status UNKNOWN | KEEP | Founder's own case-study quote about running 7-figure support with "essentially one person" — but confirm current revenue (new sources range $1.8M–$50M+, unusually wide) and live tool status before pitching |
| Comme Avant | Sophie Lauret | Founder & Communications Director (co-founder) | France (Les Pennes-Mirabeau, near Marseille) | comme-avant.bio | linkedin.com/in/sophielauret/ (VERIFIED); general: contact@comme-avant.bio, 04 84 89 43 18 | Gorgias (current, VERIFIED historically); e-commerce platform UNKNOWN | KEEP | Named support person "Karine" personally handles nearly all customer service (new finding) — a concrete single-person-workload signal; confirm English-communication comfort and current size before pitching |
| Maison Miru | Trisha Okubo | Founder & Creative Director | USA | maisonmiru.com | linkedin.com/in/trishaokubo/ (VERIFIED); general: hello@maisonmiru.com | UNKNOWN (no helpdesk platform confirmed) | KEEP | Founder-led, right-sized signals, real gift-timed order-tracking relevance — but the one documented complaint is old and uncorroborated by anything newer found this pass, so lead with structural fit, not that single review |
| Travel Cat (Your Cat Backpack) | Emily Miethner and/or Ian Berk | Co-Founders | USA (Island Park, NY) | yourcatbackpack.com | Emily: linkedin.com/in/emilymiethner/ (VERIFIED); Ian: linkedin.com/in/ian-berk-849aa016/ (VERIFIED — corrects prior tracker URL) | UNKNOWN (Shopify confirmed as platform; helpdesk tool not identified) | KEEP | Most recent, dated (2023–2024) documented return/refund-process complaints of the four — but note the business is hybrid DTC+wholesale (1,200+ retail locations), so the offer targets their DTC ticket volume specifically |

---

## Notes for the operator
- All four remain KEEP after this pass — none were downgraded to HOLD or REMOVE — but each now carries at least one specific new open question to resolve before or during first contact (Beardbrand's conflicting revenue range; Comme Avant's English/time-zone practicality; Maison Miru's thin single-complaint evidence; Travel Cat's hybrid DTC/wholesale split).
- The most actionable correction from this pass: **Ian Berk's LinkedIn URL** in the existing tracker (`linkedin.com/in/ianberk1/`) does not match what this pass found (`linkedin.com/in/ian-berk-849aa016/`) — verify directly before using either in outreach.
- Direct site browsing remained blocked in this environment for all four target domains; the operator (or a future pass with browsing access) should manually check each site's live chat widget, current helpdesk branding, and any recent AI/chatbot rollout before finalizing outreach — this is the single biggest remaining verification gap.
