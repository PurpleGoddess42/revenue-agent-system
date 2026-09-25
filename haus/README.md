# HAUS BY HASSANAH

A women's fashion house (sexy, sensual, feminine, curvy, bold, glamorous,
Afrocentric, high-fashion) that uses AI fashion models for design
visuals.

This folder is separate from the B2B AI-automation run in `outputs/` and
`execution/ai-b2b-leverage-v1/`. It is a different business with its own
agent team.

## Active critical directive

**`directives/audience-repositioning.md`** is a permanent, binding
directive for all HAUS work. It shifts the audience toward women who could
become HAUS customers (directional ~80% women / 20% men). It does this by
changing *who the content speaks to*, not by making HAUS conservative.

## HAUS agent team: six agents (`.claude/agents/`)

| # | Agent file | Role |
|---|---|---|
| 1 | `haus-brand-director` | **HAUS Brand Director.** Brand identity and aesthetic per piece. Flags "model > garment" and over-correction toward conservative. |
| 2 | `haus-platform-compliance-recovery` | **Platform Compliance & Recovery Agent.** Recommendation, AI-label, and ad-policy risk, always labeled POLICY vs. STRATEGY. Owns the platform status register and restriction recovery. |
| 3 | `haus-luxury-buyer-positioning` | **Luxury Brand, Buyer & Industry Positioning Agent.** Concept → sample → sellable collection → industry, buyer, and press credibility → eventual investment readiness. |
| 4 | `haus-content-creative-director` | **Content Creative Director.** Garment-, design-, and woman-as-subject-centered content. |
| 5 | `haus-audience-growth` | **Audience Growth & Distribution Strategist.** WHO/WHY engagement quality, platforms, communities, moderation, and metrics. |
| 6 | `haus-chief-strategy` | **HAUS Chief Strategy Agent.** Coordinates agents 1-5, runs the monthly Core Question review, and revises the strategy when the answer is no. |

No HAUS agent may publish, spend money, contact outside parties, or make
commitments without Hassanah's explicit approval
(`directives/operating-rules.md` §1).

## Separation from the B2B business

This repository also holds a separate B2B AI-automation business
(root-level `business-brief.md`, `outputs/`, `execution/`, `runbooks/`, and the four
non-`haus-` agents). HAUS never uses that business's strategy, audiences,
brand, research, prompts, or outputs, and the two agent teams are never
mixed. See `directives/operating-rules.md` §4.

## Structure

```
haus/
  directives/audience-repositioning.md   <- permanent, binding (women-first repositioning)
  directives/operating-rules.md          <- permanent, binding (approval gate, evidence, separation)
  knowledge/platform-status.md           <- factual platform status register
  strategy/audience-repositioning-v1.md  <- current strategy (pillars, framing test, platforms, measurement)
  execution/
    content-review-scorecard.md          <- quality gate for every post and campaign
    audience-metrics-tracker.csv         <- weekly analytics log (baseline first)
    monthly-strategy-review.md           <- Chief Strategy monthly Core Question review
```

## Needed from the founder (blocking measurement)

1. **Current analytics exports** (gender split of followers *and* accounts
   reached, saves, shares, profile visits, clicks) from each platform.
   Until these arrive, the reported ~80-90% male figure is unverified and
   no progress can be reported.
2. Whether a website or landing page with email capture exists.
3. Whether physical garments or samples exist (for real-wear content and
   sales).
