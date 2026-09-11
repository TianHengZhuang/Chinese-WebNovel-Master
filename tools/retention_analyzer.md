# retention_analyzer

## Purpose

Score drafted chapters and arcs for reader retention risk before publishing.

Retention is a cost-benefit decision made by the reader:

Cost = attention and time.

Benefit = payoff, progress, emotion.

When cost exceeds benefit, the reader leaves.

---

## When To Use

After drafting a chapter.

After completing an arc.

Before the Editor pass.

When a published chapter shows a completion-rate drop.

---

## Metrics And Weights

| Metric | Weight | What It Measures | Fail Signal |
|--------|--------|------------------|-------------|
| Hook Strength | 25% | Does the ending force continuation? | Chapter can be closed at any point |
| Conflict Density | 20% | How many scenes carry active conflict? | Scenes of daily life drift |
| Curiosity Gap | 20% | Unanswered questions the reader cares about | Everything explained too early |
| Momentum | 20% | Does every scene change the story state? | Status quo maintained |
| Emotional Engagement | 15% | Does the reader have a stake? | Passive protagonist |

---

## Scoring Rubric

Score each metric 0-10.

| Score | Meaning | Action |
|-------|---------|--------|
| 8-10 | Pass | Ship |
| 6-7 | Watch | Fix the weakest one |
| 0-5 | Fail | Rewrite the section |

---

## Retention Score

Retention Score = (sum of metric score x weight) x 10

Result range: 0-100.

Risk Level:

| Score | Risk |
|-------|------|
| 85-100 | Low |
| 70-84 | Medium |
| 0-69 | High |

---

## Scope

Chapter level: score Hook Strength, Conflict Density, Momentum.

Arc level: score all five metrics.

---

## Failure Diagnostics

| Signal | Likely Cause | Fix |
|--------|--------------|-----|
| Low Hook Strength | Flat endings | Run tools/hook_generator.md |
| Low Conflict Density | Slice-of-life drift | Cut or merge scenes without conflict |
| Low Curiosity Gap | All questions answered early | Delay one reveal |
| Low Momentum | Status quo scenes | Give every scene a goal and a cost |
| Low Emotional Engagement | Passive protagonist | Give the protagonist something to lose |

---

## Baseline

A passing chapter scores:

Hook >= 8

Conflict >= 8

Retention >= 8

Below baseline: revise before output.

---

## Output Format

Chapter / Arc:

Metrics table

Retention Score:

Risk Level:

Top 3 Fixes:

Verdict: SHIP / REVISE / REWRITE
