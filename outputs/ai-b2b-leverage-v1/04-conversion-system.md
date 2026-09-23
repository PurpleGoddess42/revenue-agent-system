# Conversion System — ai-b2b-leverage-v1 (Victoria, Conversion Director)

**Scope:** sized for a solo operator with zero list, zero CRM, zero clients, closing exactly ONE Founding Client ($2,500-$4,000, order-status/tracking only, phased payment). Grounded in `02-offer-strategy.md` (Camille, Sections 12-13), `03-content-strategy.md` (Naomi), and the demo already built at `demo/`.

**Status:** Approved, with second-pass revisions applied per `06-strategic-review.md` — Section 9 (outbound prospecting) is new; Sections 2-4, 7 have targeted additions (marked "added on second-pass review"). Everything else is unchanged from the original approved version.

## 0. Assumption check (per the working standard — done before designing anything)

Naming every piece of infrastructure a normal funnel would silently assume, and the free/simple version to use instead:

| Assumption a normal funnel would make | Reality here | Simplest fix |
|---|---|---|
| An email list/ESP (Mailchimp, Klaviyo) for a drip sequence | Zero list exists | Not needed — every "sequence" below is 1:1 manual replies, not batch email. No ESP required. |
| A CRM to track leads | None exists | A single Google Sheet, one row per prospect: name, source, date contacted, qualifying answers, stage, next follow-up date. Free, five minutes to set up — a tracker, not automation. |
| A booking tool (Calendly, etc.) | None exists | Not required. Propose 2-3 specific time windows directly in the DM/email. Optional later upgrade (Calendly free tier) only if volume ever justifies it. |
| A way to accept the phased payment | None exists | **Genuinely needed** — a free Stripe account with a Payment Link (no monthly fee, ~2.9%+$0.30 per transaction only when used) or a PayPal invoice as fallback. Set this up before the first "yes," not after. The one real infrastructure dependency this system can't function without. |
| A contract/e-signature tool | None exists | Not a blocker — a one-to-two-page written agreement sent as a PDF, confirmed by the prospect replying "Agreed, let's go" with their name typed, is real and enforceable enough for a first small engagement. Paid e-sign tools are a fine later upgrade, not needed now. |
| A hosted, public landing page | None exists | Addressed directly in Section 4 — the answer is no, not yet, and why. |

Nothing below assumes the operator already has anything in the left-hand column.

## 1. Lead magnet

**No traditional lead magnet (downloadable PDF/guide) should be built.** This is a single high-touch B2B sale to a handful of warm-network prospects, not a volume funnel where a downloadable asset earns a stranger's email address.

**The sandbox demo itself is the lead magnet.** It already exists (`demo/index.html`) and does exactly what a lead magnet is supposed to do: give something real and useful away for free, before asking for money, making the paid offer feel like the obvious next step. Naomi's content already promises this — this confirms the demo is the whole lead-magnet layer, nothing else needs to be built alongside it.

**Execution note:** the demo currently runs by opening a local HTML file. To send as a link (not only screen-share live), host it free on GitHub Pages or Netlify's free tier (already flagged as optional in the demo's own README) — lets a DM reply include a clickable link instead of requiring a scheduled screen-share per prospect.

## 2. Call to action

Builds on Naomi's CTA exactly as written, not replacing it:

- **LinkedIn post:** CTA at the post's closing line — "comment 'STACK' or send me a DM." Delivered once, no separate pinned comment needed.
- **Newsletter/email:** CTA is the closing line — "hit reply." Sent directly to warm-network prospects.
- **What happens the moment either fires:** a LinkedIn comment of "STACK" or a DM gets Script A below; a newsletter reply gets Script B. Both happen within the same business day if possible — for low-volume warm outreach, speed of first reply is one of the only free conversion levers available.

**This is only half the system.** Content-driven inbound (above) runs in parallel with active outbound prospecting (Section 9, added on second-pass review) — the plan does not rely on organic reach or an assumed warm network to generate the first contact.

## 3. Word-for-word CTA / DM scripts

*("Qualifying" just means asking a couple of quick questions to confirm fit before spending time on a full walkthrough — a time-saver, not a sales tactic.)*

### (a) First reply — LinkedIn comment "STACK" or DM

> Hey [Name] — thanks for the comment. Quick version: I build a system that automatically resolves order-status/tracking tickets inside the helpdesk you already use (Gorgias or Zendesk), and hands anything it's not sure about straight to a real person instead of guessing. I built a working demo of it — takes about 2 minutes to watch, no pitch attached.
>
> Two quick questions so I don't waste your time: are you running Shopify + Gorgias or Zendesk right now, and roughly how many support tickets is your team handling in a normal week?
>
> If it sounds like a fit, I can send you the demo link right now, or hop on a quick 10-minute call this week and walk you through it live — whichever's easier for you. One thing to be upfront about: this is a working prototype I built to show you exactly how this would run inside your stack — not a live client system yet.

### (b) Reply to a newsletter reply

> Hey [Name] — glad it was useful. Quick check first: are you on Shopify with Gorgias or Zendesk for support, and roughly what's your ticket volume like in a normal week?
>
> If that lines up, here's the honest version: I don't have client logos to show yet, but I do have a working sandbox demo you can watch in about 2 minutes — [demo link]. Quick disclosure: this is a working prototype I built myself, not a live system already running for a client — it shows exactly how the real thing would work once it's built inside your actual helpdesk. It shows the system resolving a normal ticket correctly, then correctly handing a harder one to a person instead of guessing at it.
>
> Take a look and let me know what you think. If it looks like a fit, happy to jump on a quick call and figure out whether this is worth doing for your store.

### (c) Qualifying questions (listed separately so nothing gets skipped)

1. "Are you running Shopify + Gorgias or Zendesk for support right now?" — confirms the offer is technically buildable without a bigger scoping conversation.
2. "Roughly how many support tickets are you dealing with in a normal week?" — confirms enough volume for a countable before/after result (per Camille 13.2: low-hundreds to low-thousands/month).
3. "Is this something you'd be able to decide on yourself, or is there someone else who'd need to weigh in?" — confirms no procurement committee (per Camille 13.1/13.2).

If any answer disqualifies them (no Shopify/Gorgias/Zendesk, a procurement process, or a brand clearly above ~$5M where a founder-led yes isn't realistic):

> "Appreciate you asking — honestly, this specific build is scoped for brands running Shopify + Gorgias/Zendesk where you can make the call yourself, so it might not be the right fit as-is. Happy to stay in touch in case that changes."

### (d) Live screen-share disclosure (added on second-pass review)

Spoken before clicking into the demo on a live call — no prior scripted opening existed for this path:

> "Before I click through this — just so it's clear, this is a working prototype I built to demonstrate exactly how the real system would behave. It's not connected to a live client or your actual store. Once you're a client, this same logic gets built directly inside your real Gorgias/Zendesk and Shopify."

## 4. Landing/conversion page concept

**No dedicated public landing page is needed at this stage — building one would be over-building.** A landing page exists to convert anonymous traffic from an ad or broad content funnel; every prospect here arrives through a 1:1 comment, DM, or personal reply from someone who already read the actual post/newsletter. A generic landing page would be a *downgrade* from the personal conversation already happening.

**What genuinely helps instead: a one-page written proposal**, built as a free Google Doc (shareable link, no hosting/tool cost), sent after the qualifying conversation and demo walkthrough. Contents:

1. **Header:** "[Operator/Company Name] — Founding Client Build: Order Status & Tracking Automation"
2. **What's included:** the Tier-0 scope from Camille 13.4/13.9 — one intent category, built inside their existing Gorgias/Zendesk, tested, escalation rules, handover docs, one training walkthrough.
3. **What's not included:** stated plainly (per Camille 12.8) — no Klaviyo/cart-recovery, no additional categories, no new channels.
4. **Timeline:** 2-3 weeks from signed agreement to live. *(Added on second-pass review)* If launch is delayed past [agreed date] due to technical scope discovered during the build, no additional payment is due until it's resolved, and we'll agree on a revised date together.
5. **Price and payment:** $2,500-$4,000 (confirmed after ticket-volume/complexity is seen), 50% kickoff / 50% at successful launch.
6. **What we need from you:** the limited access list from Camille 13.8 (read access to order/ticket data, macro/automation edit access — explicitly NOT full store-admin, financial, or unrelated-department access).
7. **The exchange:** permission to use real before/after numbers and a testimonial as the first case study, name used if comfortable, anonymized if not.
8. **Next step:** "Reply 'let's do this' and I'll send the kickoff payment link and the one-page agreement to sign."

## 5. Follow-up sequence (manual — no automation, no drip tool)

For a prospect who engages but doesn't say yes right away — the realistic majority outcome. All manually sent by the operator, tracked in the Google Sheet from Section 0.

### Track A — LinkedIn DM thread (one continuous conversation, no subject lines)

- **Touch 1 — Day 0 (immediate):** Scripts A/B above.
- **Touch 2 — Day 3 (no reply, or watched demo then went quiet):** "No pressure at all — just following up in case this got buried. Here's the demo again if you haven't had a chance yet: [link]. Even if the timing's not right, happy to answer any questions."
- **Touch 3 — Day 8 (still no reply):** "Last check-in on this — totally understand if it's not the right time. If you want to revisit it before Black Friday, I'm holding this Founding Client spot for now. Either way, appreciate you engaging with the post."
- **After Touch 3:** stop actively following up. Mark "cold — revisit in 60 days" in the tracker rather than continuing to message.

### Track B — Email reply thread (real subject lines apply)

- **Email 1 — Day 0:** Script B above; subject stays "Re: [original newsletter subject]."
- **Email 2 — Day 4, if no response:** Subject "Quick follow-up — the demo I mentioned." — "Hey [Name] — wanted to make sure this didn't get lost. Here's the sandbox demo again: [link]. Takes about 2 minutes — shows a normal ticket getting resolved correctly, and a harder one getting handed to a person instead of guessed at. Let me know what you think, or if now's just not the right time."
- **Email 3 — Day 10, if still no response:** Subject "Closing the loop on this." — "Hey [Name] — last note on this one so I'm not cluttering your inbox. I'm taking on one Founding Client for this build before Black Friday, phased payment, 2-3 week build. If that's still interesting, just reply and we'll pick it back up. If not, no worries at all — appreciate you reading the newsletter."
- **After Email 3:** stop. No more than three touches total per prospect.

## 6. Offer transition — how the Founding Client offer gets proposed

Introduced **after** qualifying questions confirm fit **and** after the demo has been shown — never before. A live message (DM, email, or spoken on a call):

> "Based on what you've told me, this looks like a good fit for what I'm calling the Founding Client build: I set up automated handling for just order-status and tracking questions, live inside your existing [Gorgias/Zendesk], working within 2-3 weeks. It's $2,500-$4,000 depending on scope, split 50% at kickoff and 50% once it's live and working — not all upfront. In exchange, I'd want your OK to use the real before/after numbers as my first case study, with your name if you're comfortable, or anonymized if not. Want me to send over a one-page summary of exactly what's included so you can look it over?"

If they want the one-pager, send it (Section 4), then:

> "If it looks good, just reply 'let's do this' and I'll send the kickoff payment link (50% — $[X]) along with a short one-page agreement to sign. Once that's done we can get access set up and start this week."

This mirrors Naomi's approved transition line (her Section 11), adapted from "post-CTA" language into the actual 1:1 close, without changing price or framing.

## 7. Customer journey map

| Stage | What happens | What changes in the prospect's belief/readiness |
|---|---|---|
| **0. Outbound identification & contact** *(added on second-pass review — runs in parallel with Stage 1, not after it)* | Operator researches and personally contacts a specific, verified-fit prospect per Section 9 | Moves from "never heard of the operator" to "a real person reached out with something specific and true about my business" — this is the actual first-contact engine; Stage 1 (content) is credibility support a prospect can check, not the primary source of contact at this stage. |
| 1. Content | Sees LinkedIn post or receives newsletter (either organically, or because outbound contact prompted them to check the operator's profile) | Recognizes their own situation — moves from unaware to "someone finally named my actual problem," or reinforces trust in the person who just reached out. |
| 2. CTA fires | Comments "STACK," DMs, or replies | Moves from passive reading to active curiosity — low-commitment first action. |
| 3. First reply + qualifying (Section 3) | Operator replies same-day, asks 2-3 questions | Confirms a real person responded fast and personally — trust before any ask. |
| 4. Demo walkthrough | Watches the sandbox demo resolve correctly and escalate correctly | Moves from "does this even work" to "I've seen it work" — the single biggest belief shift, since no other proof exists. |
| 5. Offer proposed + one-pager sent | Founding Client build proposed, one-pager sent | Moves from "this could work" to "here's exactly what I'd be agreeing to." |
| 6. Follow-up, if no immediate yes | 1-3 manual touches over ~10 days | Resolves lingering hesitation (usually about newness/risk) or the prospect self-selects out. |
| 7. Agreement signed + kickoff payment | Written agreement confirmed by reply, 50% kickoff via Stripe/PayPal link | Moves from prospect to client, de-risked by the small phased amount. |
| 8. Delivery (2-3 weeks) | Access collected, workflow mapped, built, tested, launched (Camille 12.5) | Belief shifts from "I hope this works" to "I'm watching it work in my own helpdesk." |
| 9. Launch payment + results collected | 50% launch payment, before/after metrics gathered (Camille 13.10) | Client experiences the proof directly — converts trust into willingness to give a testimonial. |
| 10. Testimonial/case-study ask | Written testimonial, permission to use name/results, redacted screen-recording | Client moves from customer to advocate/reference — the asset this engagement exists to produce. |

## 8. Next paid step / higher-value offer

**Scoped honestly for Client #1 specifically, not the mature $5M-$50M motion (per the working standard's now/next/mature distinction).**

Two things are legitimate to offer this client after a successful launch — nothing beyond these:

1. **A simple, low-commitment monitoring add-on** (not the full structured $500-$2K/month retainer, which Camille 13.15 explicitly flags as premature at Day 1): "If this saved you real time, I can keep an eye on it going forward — checking accuracy, updating templates as your policies change, one short monthly check-in — for around $150-$250/month, no long-term commitment, cancel anytime." Offered only *after* results are in hand, never bundled into the original close.
2. **Scope expansion as a separate small project** (per Camille 12.8): if the first workflow goes well, adding a second intent category (e.g., basic return/refund questions) toward full Tier 1 scope is a logical, quotable next step — a new small project, not a forced upsell.

**What should NOT be offered yet to this client:** Tier 2/Klaviyo lifecycle work, the full structured retainer with SLAs, or anything implying an established track record — not credible off one unproven engagement (Camille 13.15's "Day-100, not Day-1" list). The honest way to leave the door open:

> "If this works the way I think it will, there may be more we could build on top of it down the line — but let's get this one right first and see the real numbers before we talk about anything else."

**For the business overall:** the real "next paid step" is Clients #2-3 at $4,000-$6,000 (Camille 13.13) — a different prospect, not an upsell path for Client #1.

## 9. Outbound prospecting process (added on second-pass review — runs in parallel with the content, not after it)

**Plain-English framing:** this is a manual, repeatable checklist the operator runs by hand — not software, not automation, not a purchased list. Content (the LinkedIn post/newsletter) builds credibility a prospect can check once contacted; it is not the mechanism that generates the first contact. Outbound is. Both run at the same time, starting now, not sequentially. This directly addresses the strategic review's highest-priority finding: the plan cannot depend on organic reach or an assumed warm network.

### 9.1 Identifying appropriate DTC/e-commerce brands (all free/manual; paid tools flagged as optional upgrades only)

Check these signals, in this order, for any candidate brand:

- **Shopify:** visit the storefront as an ordinary shopper. View page source (right-click → "View Page Source" in any browser) and search for "cdn.shopify.com" — if present, it's Shopify. Faster alternative: BuiltWith.com has a free single-domain lookup (type the URL, see the tech stack) — the free tier, not the paid bulk/API product.
- **Gorgias or Zendesk:** look for a chat widget bubble on the storefront; check the brand's public job postings (LinkedIn Jobs, Indeed, or their own careers page) for a support-role listing mentioning "Gorgias" or "Zendesk" by name — a common, reliable signal, since companies list the exact tools a new hire needs to know.
- **Klaviyo:** sign up for the brand's own email newsletter/signup form (a normal, public action) and check the footer of the confirmation or marketing email for "Powered by Klaviyo" or a klaviyo.com unsubscribe link.
- **Revenue-range signal ($1-5M proxy — imprecise, flagged as such):** LinkedIn company page's self-reported employee count (roughly 10-60 employees is a loose proxy at this revenue band, not a confirmed figure), any funding/press mentions, and general storefront maturity (product catalog size, review counts).
- **Optional paid upgrades (not required at this volume):** LinkedIn Sales Navigator, BuiltWith's paid bulk lookup, SimilarWeb's paid traffic-estimate tier. None are needed to execute this manually for a handful of prospects a week.

### 9.2 Identifying the right decision-maker

- The brand's own website "About"/"Team" page (most DTC brands feature the founder by name and photo).
- The company's LinkedIn page → "People" tab, filtered by title: Founder, Co-Founder, CEO, Head of Customer Experience, Director of Operations, Head of CX.
- Press mentions ("Meet the founder of [Brand]" articles, local business press, podcast guest appearances) — also useful for finding a specific true detail to reference in outreach (Section 9.5).

### 9.3 Pre-contact qualifying signals (checked before reaching out, in addition to the 3 existing qualifying questions in Section 3c)

Favor brands that show:
- Storefront live for over a year (copyright year in the footer, or the free Wayback Machine archive at web.archive.org for its earliest snapshot) — a proxy for "established, not brand-new."
- Active, real job postings in the last few months (signals actual ongoing operations).
- No obvious enterprise-scale signals working against fit: a "VP of Customer Experience" posting, a dedicated in-house automation/data team, or a formal RFP/vendor-management process — any of these suggest the brand has outgrown the founder-can-say-yes-alone profile this offer needs (Camille 13.2).

These are pre-contact filters only — the three qualifying questions already in Section 3c remain the actual confirmation step once contact is made; nothing about that step changes.

### 9.4 Legitimate public information only — explicit boundaries

Everything above uses only: visiting a public storefront as an ordinary visitor, viewing public page source, using a public free single-lookup tool, browsing public LinkedIn profiles and company pages, reading public job postings and press, and signing up for a public newsletter with a real email address. **Explicitly ruled out:** scraping data in violation of a platform's terms of service, bulk-scraping LinkedIn (against its terms even for public profiles), pretexting (posing as a customer, journalist, or job applicant to extract information under false pretenses), misrepresenting who's reaching out or why, or bypassing any login/paywall/access control. This is a hard line, consistent with the brief's no-deception constraint.

### 9.5 Personalized outreach — adapted from the existing first-reply script

**LinkedIn connection request note** (short, references something specific and *true*, found via 9.1-9.2, never invented):

> "Hi [Name] — saw [Brand]'s [specific true detail — recent product launch, a press mention, something visible on the site]. I work on AI-powered support automation for Shopify DTC brands around your size. Would love to connect."

**First message, once connected (or as a LinkedIn InMail if not connecting first):**

> "Hey [Name] — congrats on [the same specific true detail]. Quick reason I reached out: [Brand]'s support/chat setup looked like [Gorgias/Zendesk, if confirmed — otherwise skip this clause]. I build a system that automatically resolves common tickets like order-status/tracking right inside the helpdesk a brand already uses, and hands anything it's unsure about straight to a person instead of guessing. I put together a 2-minute demo showing exactly how it works — happy to send the link if that's useful, no pitch attached."

If the specific tool couldn't be confirmed publicly, drop that clause and ask directly once they respond — never guess or assert a tool that wasn't actually verified.

Once they reply, this flows straight into the existing qualifying questions (Section 3c) and demo/offer flow (Sections 3, 6) unchanged — outbound only changes how the first contact happens, not anything downstream.

### 9.6 Inviting qualified prospects to the demo and business conversation

No new step needed — an outbound reply that passes the qualifying questions flows directly into the same demo-link-or-live-walkthrough flow and offer transition already defined in Sections 3 and 6. Outbound and inbound converge at this point into one identical process.

### 9.7 Tracking — extending the existing Google Sheet tracker

Add a **Source** column (Outbound / Inbound-Comment / Inbound-DM / Inbound-Newsletter-Reply) and a **Pipeline Stage** column with these stages, updated manually as each prospect moves:

`Identified → Contacted → Replied → Qualified → Demo Shown → Proposal Sent → Signed / Declined-or-Cold`

Every prospect, whether from a LinkedIn comment or cold outbound, is tracked identically from "Replied" onward — the systems fully converge; only the first two stages differ by source.

### 9.8 Realistic weekly volume (honest, manual, not a volume engine)

For one solo operator doing this by hand, a realistic pace is **roughly 15-20 new prospects researched and contacted per week**, alongside the operator's other work. This is not a scaled outbound engine; it's enough volume to build a small, real pipeline toward one Founding Client, consistent with a first-client timeline of roughly 4-6 weeks. If reply/qualification rates run low, the fix is more weeks of this same manual process, not more automation — automating outbound at this stage would reintroduce exactly the impersonal, generic-template risk this process is designed to avoid.

## What was NOT changed

Offer scope, pricing, phased-payment structure, the offer name, and Naomi's exact CTA/transition lines are taken as given and reused, not altered. No paid tool, list, CRM, or automation platform was assumed to exist — every infrastructure dependency (payment link, hosting, tracker, agreement) is named explicitly in Section 0 with its free/simple version, and Section 9's prospecting tools follow the same standard.
