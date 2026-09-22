# chapter_fix_list

## Purpose

Turn a launch batch score into **per-chapter fix lists**, so a HOLD / RESTRUCTURE verdict becomes concrete edits instead of a general "rewrite it" order.

One row per fix, one owner per chapter. Nothing gets rewritten that is not on the list.

---

## When To Use

After tools/launch_batch_reviewer.md returns HOLD or RESTRUCTURE (and after READY when polish items were logged).

Before re-running the batch review, and before submission_checklist gate 8 / gate 10.

Pairs with tools/story_bible.md, tools/cliffhanger_continuity_checker.md, tools/style_sampler.md, knowledge/submit_*.md.

---

## Inputs

| Input | Source | Required |
|-------|--------|----------|
| Batch review report | tools/launch_batch_reviewer.md (Pass results + must-fix list) | Yes |
| Chapter drafts | launch batch (3–10 chapters) | Yes |
| Story bible | tools/story_bible.md | Yes |
| Hook ledger | tools/cliffhanger_continuity_checker.md | Preferred |
| Continuity verdict | tools/story_continuity_checker.md | Preferred |
| Style Profile | tools/style_sampler.md | If one exists |
| Platform submit pack | knowledge/submit_*.md | Yes |

---

## Severity Levels

| Level | Meaning | Launch rule |
|-------|---------|-------------|
| BLOCKER | Breaks a batch-review exit criterion: chapter 1 does not install the engine, a DEAD hook, a story-bible conflict, a platform must-fix item, a tag promise the batch never shows | Fix before upload |
| SHOULD-FIX | Drains one scored dimension: FLAT hooks beyond the allowed budget, style drift, low-density stretch, relationship beat missing in a romance batch | Fix before upload if the schedule allows; otherwise record as known debt in the review |
| POLISH | Optional craft work: line edits, gag sharpening, imagery, chapter-title wording | May be fixed online after launch |

Severity is assigned from the finding's source pass, never from how easy the fix looks.

---

## Procedure

1. Take the batch review's Pass 1–5 findings and its must-fix list as the raw material.
2. Map every finding to the specific chapter(s) that caused it. A finding with no locatable chapter is a batch-level row, not a chapter row.
3. Assign severity with the table above.
4. For each row write: evidence (quote or line), the fix, and a re-check criterion that a second reader can verify.
5. Order rows chapter 1 → N inside each chapter; keep BLOCKER rows first in the file.
6. Fix in chapter order, updating tools/story_bible.md whenever a continuity row is closed.
7. Re-run tools/launch_batch_reviewer.md on the edited batch. Only the re-run score may close the list.

---

## Output Format

```text
# Chapter fix list — <work title>
Platform: <name>
Batch score: NN — HOLD|RESTRUCTURE
Source review: <date / tool>
BLOCKER: n | SHOULD-FIX: n | POLISH: n

## Chapter 1 — <chapter title>
| # | Severity | Finding | Evidence | Fix | Re-check |
|---|----------|---------|----------|-----|----------|
| 1 | BLOCKER | Engine not installed before chapter end | ch1 ends at the funeral, no advantage shown | Move the system reveal to the first 800 words | Reader can name the engine after ch1 |

## Chapter 2 — <chapter title>
...

## Batch-level
| # | Severity | Finding | Applies to | Fix | Re-check |
|---|----------|---------|-----------|-----|----------|

## Platform must-fix (from submit pack)
- [ ] <item> → chapter(s) <n> → closed in draft <rev>

## Exit Criteria
- [ ] Every BLOCKER row closed and verified in the batch text
- [ ] Story bible updated for every continuity row
- [ ] No DEAD hooks and at most one FLAT hook per 5 chapters
- [ ] Re-run batch review: score >= 80, or the HOLD reason is limited to SHOULD-FIX rows
- [ ] Remaining SHOULD-FIX / POLISH rows either fixed or accepted with a written reason
```

---

## Worked example (two rows)

```text
# Chapter fix list — 《长夜灯火》
Platform: 塔读 tadu
Batch score: 71 — HOLD
BLOCKER: 1 | SHOULD-FIX: 2 | POLISH: 1

## Chapter 1
| # | Severity | Finding | Evidence | Fix | Re-check |
|---|----------|---------|----------|-----|----------|
| 1 | BLOCKER | Hook is FLAT | ch1 ends with the lamp refilled and no new question | End on the countdown number changing on its own | Chapter ends with the reader asking a question |

## Chapter 3
| # | Severity | Finding | Evidence | Fix | Re-check |
|---|----------|---------|----------|-----|----------|
| 2 | SHOULD-FIX | Low-density stretch | fistfight occupies 1200 words, mystery does not move | Cut to 400 words and add one clue | Word count down, clue count up |
```

---

## Red Flags

- "Rewrite chapter 3" orders with no evidence line
- Fixing style drift by editing only chapter 1
- Closing a hook row by adding a hook that contradicts the tag promise
- Regenerating the entire batch instead of closing the listed rows
- Marking a DEAD hook as POLISH to make the list look shorter
- Leaving the story bible untouched after continuity fixes

---

## Exit Criteria (summary)

The list is closed only when the batch review has been re-run: score >= 80, zero DEAD hooks, zero unresolved story-bible conflicts, and the platform must-fix list empty.
