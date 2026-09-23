# Prospecting System — Founding Client #1

**Objective:** acquire ONE Founding Client (the $2,500-$4,000, order-status/tracking-only implementation defined in `outputs/ai-b2b-leverage-v1/02-offer-strategy.md` Section 13 and `outputs/ai-b2b-leverage-v1/07-final-revenue-strategy.md`). This system operationalizes the outbound prospecting approach already designed in `outputs/ai-b2b-leverage-v1/04-conversion-system.md` Section 9 into concrete templates you can actually use.

**Status: system built, not yet run.** No real companies have been researched, no messages have been drafted for a real prospect, and nothing has been sent. This document and the tracker template are the tool; using the tool on real prospects is the next step, after you approve this system.

**Hard rules this system follows, always:**
- No purchased lead lists, no scraped personal data, no bypassing logins/paywalls, no pretending to be someone else to get information.
- No inventing information. If a fact (like exact revenue) isn't publicly verifiable, it's recorded as an **estimate** with a stated confidence level — never presented as a known fact.
- No automatic sending. The system prepares research and draft messages; a human (you) reviews and sends every single one.
- No new paid software. Everything here runs on things that are free: a spreadsheet (Google Sheets, Excel, or similar) and a web browser.

---

## 1. Finding prospects — what we're looking for

**Plain-English target:** a real, operating online store, small enough that the owner can say "yes" to a $2,500-$4,000 project without asking anyone else, but established enough to actually have that money and a real customer-support workload worth automating.

**DTC** means "Direct-to-Consumer" — a brand that sells its own products straight to shoppers online (as opposed to only selling through other retailers). We're looking for DTC e-commerce brands with:

- **Accessible decision-making:** founder-led, or a small enough team that one person (owner, CEO, or a Head of Customer Experience/Operations) can approve this without a committee.
- **Business stage:** signals consistent with roughly $1M-$5M in annual revenue. **We never claim to know a private company's actual revenue** — we only note *observable proxies* (see the field list below) and label them clearly as estimates.
- **Active operation:** the store is clearly live and selling right now, not abandoned or a side-project that hasn't shipped an order in months.
- **Meaningful order/customer volume:** enough real customers that "where is my order" questions are a genuine, recurring workload — not a brand-new store with a handful of total sales.
- **Support relevance:** their business involves shipped physical products (so tracking/delivery questions naturally happen) and they have some kind of visible customer-support setup already (a chat widget, a help center, a support email).
- **Neither too big nor too small:**
  - *Avoid giant/enterprise brands* — they have internal teams, procurement processes, and existing vendor relationships; per the approved strategy, they're the *mature* target, not the first client.
  - *Avoid hobby/tiny stores* — if there's no real order volume or the business doesn't look like it generates real income yet, they're unlikely to genuinely afford or need this.

## 2. Qualifying prospects — the research fields

For every prospect, the following is researched and recorded (this is the column list in `prospect-tracker-template.csv`). **Every field is filled with what's actually found, or left blank/marked "unknown" — never guessed.**

| Field | What it captures | How it's found |
|---|---|---|
| Company/Brand | The business's name | Their website |
| Website | The store's URL | — |
| What they sell | Product category, in one line | Browsing the store |
| Business stage/size signals (ESTIMATE) | Proxies like employee count on LinkedIn, store age, catalog size, review counts, social following | LinkedIn company page, Wayback Machine (a free tool that shows how old a website is), the store itself |
| E-commerce platform | Shopify, WooCommerce, etc., if identifiable | Viewing the page's public source code, or a free tool like BuiltWith |
| Support/help-center setup | Visible chat widget, listed support email, help-center link | Visiting the site as a normal shopper |
| Evidence order-tracking/support is relevant | E.g., a visible "Track Your Order" page, FAQ entries about shipping | Browsing the site |
| Evidence of meaningful order/customer activity | Review counts, "X,000+ customers" claims, social proof numbers | Product/review pages, About page |
| Signs of operational pain or automation opportunity | E.g., a job posting for a support role, public complaints about slow responses, visibly overwhelmed social media replies | Job boards, public reviews (Trustpilot, Google, BBB), social media comments |
| Existing automation/support tools | Gorgias, Zendesk, Klaviyo, or similar, if identifiable | The chat widget itself, public job postings mentioning the tool by name |
| Likely decision-maker role | Founder, CEO, Co-Founder, Head of CX/Ops | About page, LinkedIn |
| Decision-maker name (only if publicly verifiable) | An actual name, only when confidently confirmed | About page, LinkedIn company page's "People" tab, press mentions |
| Public professional contact path | A LinkedIn profile URL or a publicly listed business contact form/email — never a scraped personal email | LinkedIn, the company's own "Contact" page |
| Why this fits the Founding Client offer | A short synthesis note connecting the evidence above to the offer | Written after the research above is done |
| Possible objection / reason NOT to pursue | An honest counter-note — e.g., "may already use an enterprise tool," "team looks larger than expected" | Written after the research above is done |
| Confidence level | High / Medium / Low, for the uncertain fields specifically (mainly the size estimate) | A judgment call, stated plainly |

## 3. Scoring and prioritizing

Every researched prospect gets one label: **HIGH PRIORITY**, **POSSIBLE**, or **NOT A FIT**. The label is driven by four things together — **need** (do they seem to have this problem), **ability to pay** (are they a real, established business), **accessibility** (can we actually reach and get a yes from the decision-maker), and **fit** (does the order-status/tracking workflow specifically make sense for them) — never by size alone. **A large, impressive-looking brand is not automatically high priority — per the approved strategy, a brand that's outgrown a founder-led "yes" is actually a worse fit for this specific offer, not a better one.**

### HIGH PRIORITY — pursue first
All of the following are true:
- A specific decision-maker (founder/CEO/Head of CX) is identified by name or role, with a public contact path (LinkedIn, contact form).
- Size signals are consistent with the $1M-$5M range (moderate employee count, an established-looking catalog/review history) — noted as an estimate, but a reasonably confident one.
- A support setup exists (chat widget, help email, or an identifiable tool) — meaning the order-status workflow has something real to plug into.
- At least one concrete signal of support workload or strain (a support job posting, visible customer complaints about response time, a help-center page suggesting volume).
- No disqualifying red flag from the NOT A FIT list below.

### POSSIBLE — worth a second look, not first-batch priority
Some real fit signals exist, but something important is missing or unconfirmed — for example: good size/stage signals but no decision-maker identified yet, or a support setup exists but no clear pain/volume signal, or the platform/tooling couldn't be confirmed. These may become HIGH PRIORITY with a little more digging, or may drop to NOT A FIT once checked further.

### NOT A FIT — do not pursue for Founding Client #1
Any one of these is disqualifying:
- Clear enterprise-scale signals: a large, well-known brand, a large support team, or public statements about a formal vendor/procurement process.
- Clear hobby/dormant-store signals: no real reviews, no evidence of recent orders, a catalog that looks unfinished or abandoned.
- Not really a fit for support automation at all (e.g., a B2B-only wholesale operation with no direct-to-consumer order volume).
- Already uses an enterprise-grade support platform or has an internal automation/data team — suggests they've outgrown this specific offer.
- No identifiable single decision-maker (a large, diffuse organization where a "founder says yes" close isn't realistic).

## 4. Personalization research — what must be found before writing outreach

Before any message is drafted, the following must be on hand (all pulled from the fields above):
- **One specific, true detail** about the brand — a recent product launch, a press mention, something notable visible on the site. Never a generic compliment.
- **Their actual support/CX setup**, if identifiable — lets the message reference their real situation instead of a generic pitch.
- **The clearest pain/opportunity signal found** — the single strongest piece of evidence from the research (e.g., the job posting, a specific complaint pattern).
- **A one-line reason the order-status/tracking workflow specifically matters to them** — connecting the evidence to the exact offer being sold, not a generic "AI can help your business" line.

## 5. Outreach preparation — draft only, never auto-sent

A prospect is only marked **OUTREACH READY** once all of the following exist in the tracker:
1. A HIGH PRIORITY (or upgraded POSSIBLE) qualification.
2. A confirmed decision-maker name/role and a public contact path.
3. The four personalization items above.
4. A drafted message (using the personalized-outreach pattern from `04-conversion-system.md` Section 9.5).

**The draft is prepared and saved in the tracker. It is never sent automatically.** You review it, edit it if you want, and send it yourself. This is a hard boundary, not a preference.

## 6. Pipeline tracking

Every prospect moves through these stages, tracked in the `Stage` column of the tracker spreadsheet:

| Stage | Plain-English meaning |
|---|---|
| **FOUND** | The company has been identified as a candidate; no research done yet. |
| **RESEARCHED** | All the qualification fields (Section 2) have been filled in. |
| **QUALIFIED** | A priority label (HIGH PRIORITY / POSSIBLE / NOT A FIT) has been assigned. |
| **OUTREACH READY** | A personalized draft message exists and is ready for your review (Section 5). |
| **CONTACTED** | You've sent the message. |
| **RESPONDED** | The prospect has replied. |
| **MEETING** | A call or deeper conversation has happened (demo walkthrough, qualifying questions per `04-conversion-system.md` Section 3). |
| **PROPOSAL** | The one-page proposal has been sent (`04-conversion-system.md` Section 4). |
| **WON** | They signed and paid the kickoff deposit. |
| **LOST / NOT A FIT** | They declined, went cold, or were disqualified at any stage — with a one-line reason noted. |

## 7. AI vs. your job

**What the AI/agents do:** research each prospect using only public information, fill in every field in the tracker, apply the qualification framework and assign a priority label, identify the personalization details, draft the outreach message, keep the tracker organized and up to date, and flag anything uncertain rather than guessing. This is the repetitive, time-consuming work — it's what the system exists to take off your plate.

**What you do:** approve which prospects are worth pursuing, approve and personally send every outreach message, have the actual conversations with anyone who responds, run the demo walkthroughs and qualifying conversations, approve final pricing/scope for each real deal, and close the relationship. Per the working standard, this isn't optional human-in-the-loop theater — these are exactly the parts of the job that require your judgment and relationship, not the AI's.

## 8. Recommended first batch size

**10 prospects, fully researched and qualified, not a bigger number.** The goal of the first batch isn't volume — it's testing whether this qualification framework actually finds good-fit companies and whether the personalized outreach gets replies. Ten is small enough to review every single one closely yourself before any message goes out, and large enough to learn something real from the results (which ones got a HIGH PRIORITY label, whether that predicted a reply, what needs to change in the framework). Once the process proves itself on this batch, later batches can move toward the ~15-20/week pace estimated in `04-conversion-system.md` Section 9.8.

## Files in this folder

- `prospect-tracker-template.csv` — import this into Google Sheets (File → Import → Upload) or Excel. One row per prospect, with every field from Section 2, plus Stage, Priority, and the drafted outreach message.
