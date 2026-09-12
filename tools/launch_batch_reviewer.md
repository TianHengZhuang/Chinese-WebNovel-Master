# launch_batch_reviewer

## Purpose

Review the first 3–10 chapters as one launch batch, not as isolated chapters.

The launch batch is what platforms and first-week readers actually judge.

---

## When To Use

After golden_three_reviewer returns GO or REVISE (fixes applied).

Before submission_checklist gate 8.

Before the first public upload of a new work.

Pairs with tools/cliffhanger_continuity_checker.md and tools/publishing_calendar.md.

---

## Batch Inputs

| Input | Required |
|-------|----------|
| Chapter drafts (3–10) | Yes |
| Story bible (characters, power state) | Yes |
| Style Profile if one exists | Preferred |
| Target platform submit pack | Yes |
| title_scorer result | Preferred |

---

## Review Passes

### Pass 1 — Engine

Does chapter 1 install the advantage engine?

Does the engine produce at least one visible win before the batch ends?

| Verdict | Meaning |
|---------|---------|
| GO | Engine clear and pays off inside the batch |
| HOLD | Engine unclear or win lands after the batch |
| REWRITE | Chapter 1 does not install the engine |

### Pass 2 — Hook chain

Score each chapter ending: CONTINUE / FLAT / DEAD.

Require:

- No more than one FLAT ending in a 5-chapter batch
- Zero DEAD endings
- Hook type variety (not the same cliff shape every time)

### Pass 3 — Consistency

Cross-check story bible against every chapter in the batch.

Flag: power-level cheats, location teleports, forgotten injuries, tag contradictions.

### Pass 4 — Platform fit

Use the target submit pack:

- First-chapter bar
- Pace expectations (free vs paid)
- Forbidden / risky content
- Tag promises kept by the batch text

### Pass 5 — Style

If a Style Profile exists, sample the batch the same way style_sampler.md samples one chapter.

Flag FLAT / DRIFT / OVERCOPY across the batch, not only chapter 1.

---

## Scoring Sheet

| Dimension | Weight | Score 0–10 |
|-----------|--------|------------|
| Engine clarity | 25% | |
| Hook chain | 25% | |
| Consistency | 20% | |
| Platform fit | 20% | |
| Style hold | 10% | |

Batch score = weighted sum × 10 (0–100).

| Score | Verdict |
|-------|---------|
| 80–100 | READY |
| 65–79 | HOLD (fix listed items) |
| 0–64 | RESTRUCTURE |

---

## Output Format

```text
# Launch batch review — <work title>
Platform: <name>
Chapters: N (list)
Batch score: NN — READY|HOLD|RESTRUCTURE

## Pass results
1. Engine: ...
2. Hooks: ...
3. Consistency: ...
4. Platform: ...
5. Style: ...

## Must-fix before upload
- ...

## Optional polish
- ...
```

---

## Red Flags

- Reviewing only the golden three and skipping the rest of the batch
- All hooks are the same type
- Platform tags promise a trope the batch never shows
- Chapter 4+ quietly changes the engine rules
- Style Profile ignored because "chapter 1 was fine"

---

## Exit Criteria

READY only when:

- Batch score ≥ 80
- Zero DEAD hooks
- Zero unresolved story-bible conflicts
- Platform must-fix list is empty
