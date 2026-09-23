# Sandbox Demo — how to use it

This is the Option A demo from `../demo-build-plan.md`: a single, self-contained
web page (`index.html`) that walks through the three required proof points using
entirely fictional data. It costs $0 to run, needs no accounts, no API keys, and
is not connected to Shopify, Gorgias, Zendesk, Klaviyo, or any real system.

## How to open it

Just double-click `index.html`, or drag it into any web browser (Chrome, Safari,
Edge, Firefox all work). No installation, no server, no internet connection
required — it runs entirely on your computer.

## What it shows, in order

1. **Order Status** — a customer asks where their order is; the assistant looks
   it up and answers correctly, then marks the ticket "Resolved automatically."
2. **Escalation** — a customer with a repeat, angry, above-threshold refund
   request is correctly *not* auto-resolved — it's handed to a human with a
   clear summary card (who, why, order history, suggested next step).
3. **Cart Recovery** — a fictional abandoned cart automatically triggers a
   follow-up message with a discount code.

Each scenario has a "▶ Play scenario" button that reveals the conversation a
message at a time, like a live chat — this makes it easy to narrate while
recording or presenting live, rather than dumping a wall of text at once.

## Before you show this to anyone

- **Replace `[Your Company Name]`** — it appears twice in `index.html` (the
  page header and the recap section). Use Find & Replace for
  `[Your Company Name]` once you've settled on a name.
- **Everything else is intentionally fictional** — the customers (Marcus R.,
  Priya D., Sarah T.), order numbers, dollar amounts, and messages were all
  invented for this demo. Do not swap in any real customer's information.
- The "DEMO — fictional data only" label at the top is deliberate — per the
  working standard and the approved content strategy, this should never be
  presented as a live, currently-running system.

## How to record or present it

- **To record:** use your computer's built-in screen recorder (Mac:
  Cmd+Shift+5; Windows: Xbox Game Bar, `Win+G`) and narrate each scenario as
  you click through it. A 60-90 second recording covering all three scenarios
  is plenty — this is the video Naomi's content strategy references.
- **To present live:** share your screen on a call and click through it
  yourself — since everything is scripted, nothing unpredictable can happen.
- Click "↺ Restart demo" at the end to reset it for another take or another
  viewing.

## What this is not

Not a real support system, not connected to any client's data, and not what
gets delivered once someone actually signs on as a Founding Client — that's a
real, separate build against their real Shopify/Gorgias-or-Zendesk/Klaviyo
accounts, described in `../02-offer-strategy.md` Section 12.

## If you later want the Option B upgrade (live AI instead of scripted)

Not necessary to win a first client, but if you want it later: this would mean
connecting the page to the Anthropic API so a prospect can type their own
question instead of clicking a fixed scenario. That requires you to create a
free Anthropic API account and provide an API key — ask for this as a follow-up
task when you're ready, so it can be scoped and estimated on its own.
