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

## HAUS agent team (`.claude/agents/`)

| Agent file | Role |
|---|---|
| `haus-chief-strategy` | Chief Strategy Agent. Owns the directive, runs the monthly Core Question review, revises the strategy when the answer is no |
| `haus-audience-growth` | Audience Growth & Distribution Strategist. WHO/WHY engagement analysis, platforms, communities, moderation, metrics |
| `haus-content-creative-director` | Content Creative Director. Garment-, design-, and woman-as-subject-centered content |
| `haus-luxury-brand-director` | Luxury Brand Director. Flags "model > garment" and over-correction |
| `haus-platform-compliance` | Platform Compliance Agent. Recommendation, AI-label, and ad-policy risk, always labeled POLICY vs. STRATEGY |

## Structure

```
haus/
  directives/audience-repositioning.md   <- permanent, binding
  strategy/audience-repositioning-v1.md  <- current strategy (pillars, framing test, platforms, measurement)
  execution/
    content-review-scorecard.md          <- every post, before publishing
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
