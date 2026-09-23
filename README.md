# Revenue Operating System

A reusable, multi-agent workflow that takes a business or content idea
through: **Market Signal → Offer → Content → Conversion**.

This is not one big prompt. It's four specialized Claude Code subagents,
each with its own job, boundaries, and required deliverables, run one at a
time by a coordinator (you, or a Claude Code session acting for you) who
passes each agent's output to the next and checks the work before moving
on.

## The four specialists (`.claude/agents/`)

1. **`market-signal-researcher`** — researches real demand and pain points
   before anything is built, so you know if the idea is worth pursuing.
2. **`offer-architect`** — turns validated demand into a specific, sellable
   offer (who it's for, the promise, the price, why now).
3. **`content-angle-strategist`** — turns the research and offer into
   ready-to-use content: titles, hooks, thumbnails, structure, talking
   points, across your chosen platforms.
4. **`conversion-system-builder`** — builds the path from viewer to lead to
   customer: lead magnet, CTA script, email sequence, customer journey.

The Offer Architect and Conversion System Builder are also reused for a
**second-pass strategic review** at the end, to stress-test the whole
strategy before you act on it.

## How to use this

1. Open `business-brief.md` and fill it in for your idea — this is the only
   file that changes between runs.
2. Follow `runbooks/revenue-agent-runbook.md` step by step. It explains, in
   plain English, how to invoke each agent, what to check before moving to
   the next one, and what to do if an agent's work is incomplete.
3. Find the finished strategy in `outputs/<your-run-slug>/`, ending with
   `07-final-revenue-strategy.md`.

`runbooks/working-standard.md` is a **permanent** rule (not per-run) for
how the coordinator and all four agents work with you — beginner-friendly
explanations, never designing only for the mature company, and always
naming the bridge when a strategy needs credibility/proof/infrastructure
you don't have yet. Every agent file and the main runbook point to it.

To run this again for a different idea, edit `business-brief.md` with a new
idea and a new run slug, then repeat the runbook. The agents themselves
never need to change — only the input does.

## Project structure

```
business-brief.md              <- the input you edit per run
.claude/agents/                <- the four specialist definitions
runbooks/
  revenue-agent-runbook.md     <- step-by-step execution guide
  working-standard.md          <- permanent working rules for every run
outputs/
  <run-slug>/                  <- one run's finished strategy (doesn't change once approved)
execution/
  <run-slug>/                  <- the operational tools you use to actually run the
                                   approved strategy (prospecting trackers, etc.) -
                                   see execution/README.md for how this differs from outputs/
```

Once a strategy is approved and you move into running the business day-to-day,
`execution/<run-slug>/` is where that operational work lives — kept separate
from the strategy files in `outputs/`, which stay as the historical record of
what was decided.
