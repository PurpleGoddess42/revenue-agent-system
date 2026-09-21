# Revenue Operating System — Runbook

This explains, in plain English, how the whole system runs from start to
finish. You (the "coordinator" in the agent files) are the one driving this —
either you personally, or a Claude Code session acting on your behalf. The
four specialist agents never talk to each other directly; every handoff goes
through you.

## What a "subagent" is, quickly

Each file in `.claude/agents/` describes one specialist: its job, what it's
allowed to touch, and exactly what it must hand back. When Claude Code runs
one of these agents, that agent gets a **clean slate** — it only knows what
you put in front of it (the business brief and whatever prior deliverables
you paste in). It does not automatically see this whole conversation, and it
does not automatically see the other three agents' files. That isolation is
the point: it keeps each specialist focused only on its own lane.

## Before you start

1. Fill in `business-brief.md` completely, including a **run slug**
   (e.g. `fitness-coaching-v1`). This is the only file that changes between
   runs.
2. Create the folder for this run's outputs: `outputs/<run-slug>/`.

## Step 1 — Market Signal Researcher

**Invoke:** the `market-signal-researcher` agent.
**Give it:** the full contents of `business-brief.md`.

**Verify before moving on** — its response must include all 8 required
sections from its agent file (verdict, ranked pain points with evidence,
audience segments, existing solutions/gaps, buying signals, the honest
counter-case, flagged assumptions, and handoff notes). If any section is
missing, thin, or unsupported by evidence, **send it back** to the same
agent naming the specific gap — don't patch it yourself and don't move on
with incomplete research; everything downstream depends on this being real.

**Save the approved output to:** `outputs/<run-slug>/01-market-signal-research.md`

## Step 2 — Offer Architect

**Invoke:** the `offer-architect` agent.
**Give it:** `business-brief.md` + the saved market research from Step 1.

**Verify before moving on** — all 11 required fields must be concretely
filled in (a specific buyer, not a demographic; an actual price, not "TBD";
a real promise sentence, not a placeholder). Send back anything vague or
generic, naming the field.

**Save the approved output to:** `outputs/<run-slug>/02-offer-strategy.md`

## Step 3 — Content Angle Strategist

**Invoke:** the `content-angle-strategist` agent.
**Give it:** `business-brief.md` + Step 1's research + Step 2's offer
strategy.

**Verify before moving on** — check that it returned actual deliverables,
not descriptions of deliverables. A hook must be a script line, not "an
attention-grabbing opener." A thumbnail concept must include real text and
a visual description. Titles must be real titles. Send back anything that
reads like a strategy note instead of a usable asset.

**Save the approved output to:** `outputs/<run-slug>/03-content-strategy.md`

## Step 4 — Conversion System Builder

**Invoke:** the `conversion-system-builder` agent.
**Give it:** `business-brief.md` + Step 1 + Step 2 + Step 3's outputs.

**Verify before moving on** — every email in the sequence needs its own
subject line and angle; the CTA needs to be word-for-word, not "add a call
to action here"; the lead magnet must connect logically to the paid offer.
Send back anything incomplete.

**Save the approved output to:** `outputs/<run-slug>/04-conversion-system.md`

## Step 5 — Assemble the first-pass strategy

As coordinator, combine Steps 1-4 into one document — this is not new
thinking, just assembling what the specialists already produced in order,
with clear section headers.

**Save to:** `outputs/<run-slug>/05-full-strategy-v1.md`

## Step 6 — Second-pass strategic review

Don't treat Step 5 as final. Send the full assembled strategy (Step 5's
file) to two agents in **critique mode**:

- **`offer-architect`** — ask it the critique-mode questions from its agent
  file (audience specificity, urgency, promise believability, offer
  strength, realistic money-making potential).
- **`conversion-system-builder`** — ask it the critique-mode questions from
  its agent file (lead-magnet-to-offer fit, path logic, CTA strength,
  realistic money-making potential).

Also sanity-check the one question that's yours as coordinator, not
theirs: **is the content angle actually interesting enough to earn
attention in the first place?** Look at the titles/hooks from Step 3 with
fresh eyes and note honestly if they'd make you personally click.

**Save the combined critique to:** `outputs/<run-slug>/06-strategic-review.md`

## Step 7 — Final revenue strategy

Take the Step 6 critique and decide, for each flagged weakness, whether to:

- Send the relevant piece back to the specialist that owns it (offer issues
  → Offer Architect; content issues → Content Angle Strategist; conversion
  issues → Conversion System Builder) with the specific fix requested, or
- Accept a noted limitation as-is if it's a reasonable tradeoff given the
  brief (e.g. "no higher-value next step yet" for a from-zero creator).

Fold the fixes into a final document.

**Save to:** `outputs/<run-slug>/07-final-revenue-strategy.md`

This file is the deliverable — everything the creator needs to research,
build, film, and sell, in one place.

## Running it again for a new idea

The agents and this runbook don't change. To run a new idea:

1. Update `business-brief.md` with the new idea and a new run slug (save the
   old brief into its own output folder first if you want to keep it, e.g.
   `outputs/<old-slug>/business-brief.md`).
2. Create a new `outputs/<new-slug>/` folder.
3. Repeat Steps 1-7 above.

Nothing about the agents themselves needs editing between runs — that's
what makes this a reusable system rather than a one-off workflow.

## Who can do what (permissions, at a glance)

| Agent | Can research the web | Can read prior outputs | Can write files |
|---|---|---|---|
| Market Signal Researcher | Yes | Reads `business-brief.md` | No |
| Offer Architect | No | Reads brief + research | No |
| Content Angle Strategist | No | Reads brief + research + offer | No |
| Conversion System Builder | No | Reads brief + research + offer + content | No |

None of the four specialists write files. That's deliberate: **you (the
coordinator) own all file writes**, so there's always one place responsible
for what actually lands in `outputs/`, and no agent can silently overwrite
another specialist's work or a prior run's history.
