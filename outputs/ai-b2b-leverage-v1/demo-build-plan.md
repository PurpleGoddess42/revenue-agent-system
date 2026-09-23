# Demo Build Plan — ai-b2b-leverage-v1

**Status: PLAN ONLY. Nothing has been built.** This document describes what we would build, how, and why — for the operator's approval before any implementation work starts, per the permanent working standard's "Now / Next / Mature" and "beginner-friendly explanation" requirements. No agent (Simone, Camille, Naomi, Victoria) was invoked to produce this — it's coordinator-level technical planning, since none of the four specialists' jobs cover software build planning.

**What this demo is for:** Naomi's approved content strategy promises a prospect they can "watch it work" before committing to anything. That promise is only honest once this demo actually exists and runs reliably. This plan defines the smallest version of that demo that can credibly prove the offer's core mechanics.

---

## What the demo must prove (from your requirements)

1. A simple support request (order status/tracking) is identified and handled correctly, using fictional data.
2. A higher-risk/complicated request is correctly recognized and escalated to a human, with context organized for that person.
3. A fictional abandoned-cart event triggers an appropriate automated recovery follow-up.

Nothing beyond these three. This is a proof environment to win a first client, not a production system — see "What this demo is explicitly NOT," below.

## The recommended approach, in plain English

We build a small, self-contained **demo web page** — think of it like a simple, single-purpose website, not an "app" in the app-store sense. It runs in any web browser. It is not connected to Shopify, Gorgias, Zendesk, or Klaviyo — those don't exist for a business that doesn't have a client yet, and the demo doesn't need them. Instead, the page contains a small made-up dataset (a handful of fictional customers and orders) built into it, and walks through three short scenarios, one for each proof point above.

**Why not use real Shopify/Gorgias/Zendesk/Klaviyo trial accounts instead?** Two reasons. First, cost/complexity: setting up and configuring real trial accounts to behave exactly like the three scenarios need would take real time and could hit trial limitations, for no real benefit — the prospect doesn't need to see the literal Gorgias interface, they need to see the underlying capability. Second, and more important: if the demo looked like it was running live inside a specific real vendor's product without actually being connected to one, that could read as misleading — Naomi's content and Camille's original demo notes both required the demo to be clearly labeled as a demonstration, never implied to be a live system. A clean, honestly-labeled standalone demo avoids that risk entirely while proving exactly the same thing.

## Two build options for the "AI" part — pick one

**Option A — Scripted demo (recommended default).** The three scenarios are pre-written: when the prospect clicks "Where's my order?", the demo shows a realistic, well-written AI response pulling from the fictional order data. When they click the harder scenario, it shows the AI correctly declining to resolve it and handing off to a human with a context summary. When they view the cart-abandonment scenario, it shows the resulting recovery message. Nothing is "live" or unpredictable — every word is written in advance, tested once, and then behaves identically every time.
- **Cost:** $0. No accounts, no ongoing charges, ever.
- **Reliability:** Perfect — it will never say something odd or embarrassing during a demo or recording.
- **Honesty check:** This is a completely standard, honest way to demonstrate a planned system before it's fully built (similar to a product mockup or prototype) — it becomes dishonest only if presented as "this is a live, currently-running AI handling real traffic," which nothing in the approved content claims. Naomi's copy already says "I built a sandbox version" — a sandbox is expected to be controlled, not live production traffic.

**Option B — Live AI demo.** Same page and same three scenarios, but instead of pre-written responses, the prospect can type their own question and a real AI model (Claude, via Anthropic's API) responds live, using the same fictional order data.
- **Cost:** Small and usage-based — realistically a few cents per demo session, not a subscription. I'm flagging this clearly per your cost rule: it's the one place a paid element could improve the demo, and here's why it might be worth it — a prospect who can type their *own* question and watch it get handled live is a more convincing, interactive experience than clicking through a fixed script.
- **Trade-off:** Slightly more setup (you'd need to create a free Anthropic API account and get a key — a few-minute signup), and a small chance the AI phrases something slightly differently than expected on a given run, which matters more if presenting live on a call than if you're recording and can just re-record a good take.

**Recommendation:** Build Option A first — it's free, foolproof, and sufficient to prove all three required points. Option B can be added later as a polish upgrade once there's time/budget for it; it is not required to win a first client.

## Exactly what the prospect will see

1. A simple landing screen: a short, honest label — something like "Demo: AI Support Assistant (fictional data, for demonstration)" — plus a one-line "click through the three examples below."
2. **Scenario 1 — Order status:** the prospect clicks a sample question like "Where's my order #1042?" The demo shows the AI looking up that fictional order and replying correctly with tracking info, in a friendly, on-brand tone.
3. **Scenario 2 — Escalation:** the prospect clicks a harder example (e.g., an angry customer demanding a refund above a set dollar amount). The demo shows the AI recognizing this is outside what it should handle alone, and switching to a "handed off to a human" screen showing a clean summary card: what the customer said, the order details, and why it was flagged — exactly what a real support agent would need to pick it up without re-reading everything.
4. **Scenario 3 — Cart recovery:** the prospect sees a fictional shopping cart get abandoned at checkout, then sees the automatic follow-up message (an email or text mockup) that would go out afterward.
5. A short recap screen tying it back to the offer ("this is what it looks like inside your own store").

## Complete workflow, start to finish

Operator sends a link (or shares their screen) → prospect (or operator, narrating) opens the page → landing screen with the honesty label → clicks/walks through Scenario 1 → Scenario 2 → Scenario 3, each taking 15-30 seconds → recap screen → operator continues the conversation about the real Founding Client offer.

## Software/platforms required

- A basic web page (HTML/CSS/JavaScript) — this is the entire "product." No database, no server required for Option A.
- A modern web browser to view it (Chrome, Safari, Edge — anything recent).
- Optional (Option B only): an Anthropic API account for live AI responses.
- Something to record or share it with: either your computer's built-in screen recorder, or simply screen-sharing live on a call.

## What's free/trial/simulated vs. what costs money

| Component | Cost | Notes |
|---|---|---|
| The web page itself | Free | Built once, reused forever, no subscription |
| Fictional order/customer data | Free | Just a small file of made-up data we write |
| Running it locally on your computer | Free | No hosting needed if you're screen-recording or sharing your screen live |
| Optional online hosting (so you can send a link instead of only screen-sharing) | Free tier available | Simple static-page hosts (e.g., GitHub Pages, Netlify's free tier) cost nothing at this scale |
| Screen recording | Free | Windows and Mac both have a built-in screen recorder; free tiers of tools like Loom also work |
| Option B: live AI responses | Small, usage-based (cents per demo run) | Only if you choose Option B — flagged above with the reasoning |

**Nothing in this plan requires buying Shopify, Gorgias, Zendesk, or Klaviyo accounts.** None of the three required proof points need them — see the next section.

## Do we actually need Shopify/Gorgias/Zendesk/Klaviyo for this first demo?

**No.** All three can be safely and credibly simulated for this stage. Real, live versions of these tools only become necessary once there's an actual paying client whose real store and helpdesk need to be connected — that's part of the paid implementation (Camille's plan), not the free demo used to win that first client.

## What accounts you personally would need to create

- **For Option A (recommended): none.**
- **For Option B (optional, later): one free Anthropic API account** (a few minutes, just an email signup) to get an API key for live AI responses.
- **If you want an online link instead of only screen-sharing:** one free account with a simple static hosting service (optional, not required — screen-recording works without this).

## What Claude Code can build/configure

- The entire demo web page: layout, styling, the three scenario walkthroughs, the "handed to a human" summary card, the cart-recovery mockup.
- The fictional order/customer/cart data, written specifically for this demo (not copied from anywhere real).
- The scripted dialogue for Option A, written to sound natural and on-brand.
- If Option B is chosen later: the code that connects the page to the Anthropic API (you'd still need to supply your own API key — see below).
- Instructions for how to open/run it locally, or simple deployment steps if you want an online link.

## What Claude Code cannot do — requires your action

- **Creating any external account** (an Anthropic API account, a hosting account, a screen-recording tool account) — signup requires your own email and, for the API, your own billing details. I can walk you through exactly what to click, but I can't create the account for you.
- **Supplying an API key**, if you choose Option B — that key is tied to your account and billing, so you'd generate it and give it to the project yourself.
- **Deciding your business/brand name** — Naomi's content already flagged this gap; the demo's labeling should use your real name/company name, not a placeholder.
- **Actually presenting the demo to a prospect or recording the video** — clicking record, narrating, and having the conversation with a real prospect is exactly the kind of relationship-building work the working standard reserves for you, not an agent.

## Integrations/APIs involved

- **Option A: none.** The whole thing is self-contained.
- **Option B: one** — the Anthropic API, for live AI responses. No Shopify, Gorgias, Zendesk, or Klaviyo APIs are involved at this stage.

## Fictional/sample data needed

A small, invented dataset — realistically 3-4 fictional customers, each with a fictional order (order number, product, shipping status/tracking info), plus one fictional shopping cart for the abandonment scenario. All names, order numbers, and products would be made up specifically for this demo, not drawn from any real business (including not accidentally reusing a real, existing brand's name).

## How we prevent real customer data from ever entering this

- There is no live client yet, so there is structurally no real customer data available to use, even by accident.
- The fictional dataset is written from scratch as part of building the demo, stored in a clearly named file (e.g., `fictional-demo-data`) so anyone looking at the project later can immediately tell it's invented, not real.
- The demo is never connected to any real store, helpdesk, or email/SMS system — it only ever reads from that one small fictional file.

## Estimated build complexity

**Low.** This is a small, single-purpose web page — no database, no user accounts (for people using it), no real integrations under Option A. It's comparable in complexity to a simple personal portfolio website, not a piece of production software.

## Realistic build time

With Claude Code doing the actual building, this realistically takes **a handful of focused work sessions — a few hours of total back-and-forth**, not days: an initial build, then a review pass where you check the wording/tone/branding and ask for adjustments, then a final polish. I'm giving a range rather than a single number because the honest answer depends on how much refinement you want on the scripted dialogue and visual look — that's a normal, expected part of getting it right, not a sign something's going wrong.

## Likely obstacles

- **Getting the escalation scenario's wording right** is more of a writing/judgment challenge than a technical one — it needs to clearly demonstrate good judgment (recognizing risk, not guessing) in just a few lines.
- **If Option B is chosen later:** occasional need to re-record if the live AI phrases something slightly off on a given take; keeping the API key private (never posting it publicly, including in this git repository).
- **Keeping the "demo" labeling honest without undercutting how impressive it looks** — a balance, not a hard technical problem.

## What eventually gets replaced with real integrations (during a paid implementation, not now)

| Demo version (now) | Replaced with, during a real paid engagement |
|---|---|
| Fictional order dataset | A live connection to the client's actual Shopify store |
| Generic demo chat interface | Configuration inside the client's real Gorgias or Zendesk account |
| Scripted or demo-AI responses | Real AI logic tuned to that client's actual policies, tone, and edge cases |
| Fictional cart-abandonment mockup | A real flow inside the client's actual Klaviyo account |

This table is also a useful thing to literally show a prospect — it visually proves you understand the difference between a demo and a real build, which itself builds credibility as a new provider being upfront about where things stand.

## How to present/record it for a prospect

- **Simplest:** use your computer's built-in screen recorder (Mac: Cmd+Shift+5; Windows: Xbox Game Bar or Snipping Tool) to record a 60-90 second walkthrough, narrating each scenario as it plays. This becomes the video referenced in Naomi's content and can be attached to a LinkedIn post, a DM, or the newsletter email.
- **Alternative:** present it live on a call by sharing your screen and clicking through it yourself, narrating in real time — works well with Option A specifically, since nothing unpredictable can happen mid-call.

## What this demo is explicitly NOT (scope boundary)

- Not connected to any real client's data or systems.
- Not a production support system — it will never actually answer a real customer.
- Not the deliverable you'd hand a paying client — the real Founding Client engagement (Camille's Section 12) is a separate, real build done after someone signs.
- Not something that needs ongoing maintenance, security review, or uptime — it only needs to run correctly when you show it.

---

## Summary decision for your approval

Build **Option A** (fully scripted, $0 cost, zero accounts needed) as the default. Option B (live AI, small usage cost, one free API account) is available as a later upgrade if you want it, but isn't necessary to win a first client. Nothing has been built yet — this is the plan only, waiting on your go-ahead.
