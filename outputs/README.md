# Outputs

This folder holds the finished deliverables from every run of the Revenue
Operating System. Nothing in here is written by the specialist agents
themselves — the coordinator saves each approved deliverable here, per the
steps in `runbooks/revenue-agent-runbook.md`.

## Structure

Each run gets its own folder, named after the run slug you set in
`business-brief.md`:

```
outputs/
  <run-slug>/
    business-brief.md              (copy of the brief used for this run)
    01-market-signal-research.md
    02-offer-strategy.md
    03-content-strategy.md
    04-conversion-system.md
    05-full-strategy-v1.md
    06-strategic-review.md
    07-final-revenue-strategy.md    <- the deliverable to actually act on
```

Keeping a full folder per run (rather than overwriting one set of files)
means you can compare strategies across ideas later, and re-run the second
pass review on an old strategy without losing the original.

No run has been executed yet — this folder is currently just the
placeholder structure described above, ready for the first run.
