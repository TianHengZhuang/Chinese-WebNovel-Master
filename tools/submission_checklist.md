# submission_checklist

## Purpose

A single pre-submission gate for any platform.

Catch the failures that block review or kill click-through before the author opens the upload form.

---

## When To Use

Before the first chapter batch goes live.

Before a platform change or re-upload.

After title_scorer and golden_three_reviewer have already run.

Pairs with tools/publishing_calendar.md for launch timing.

Platform submit packs (form fields, title tone, first-chapter bar, review risks):

- knowledge/submit_qidian.md
- knowledge/submit_tomato.md
- knowledge/submit_jinjiang.md
- knowledge/submit_feilu.md
- knowledge/submit_qimao.md
- knowledge/submit_zongheng.md

---

## Gate Order

| Step | Check | Fail Action |
|------|-------|-------------|
| 1 | Title scored >= 70 on title_scorer | Rewrite title |
| 2 | Golden three verdict is GO or REVISE with fixes applied | Do not submit |
| 3 | Synopsis matches the first-three-chapter promise | Rewrite synopsis |
| 4 | Tags: 1 core identity + 1 genre + 1 hook; no banned tags | Drop illegal tags |
| 5 | Category matches the actual power system / romance weight | Reclassify |
| 6 | First chapter opens conflict within the first screen | Rewrite opening |
| 7 | No platform-banned content in the launch batch | Sanitize |
| 8 | Update plan: next 3 chapter dates on the calendar | Schedule first |

---

## Metadata Pack

Prepare these fields once. Reuse them in every platform form.

| Field | Rule |
|-------|------|
| Title | Primary + 1 short alias if the platform allows |
| Synopsis | 80-150 Chinese characters for most male-frequency sites; shorter for mobile-first |
| Tags | From knowledge/tag maps; never more than the platform max |
| Category | One primary; secondary only if the platform requires |
| Cover brief | Protagonist pose + one power visual + title legible at thumbnail size |
| Author note | One sentence pitch, no spoilers |

### Blurb backfill example

After `tools/blurb_synopsis_generator.md` picks a winner, copy the **same** pack into this checklist so platform forms stay consistent. Do not invent a second set of copy.

```markdown
## Metadata Pack (filled)

| Field | Value |
|-------|--------|
| Title | 《长夜灯火》 |
| one_liner | 灯火守夜人只能看见别人的死亡倒计时，除了自己的。 |
| short_blurb | 他掌灯十年，只照别人的终点。直到铜灯映出自己的数字：七天。 |
| long_synopsis | 偏远灯塔的守夜人陆迟，天生能看见生灵头顶的死亡倒计时。十年来他只旁观，从不插手。直到古城鼠疫爆发那夜，灯焰映出他自己的数字：七。七天之内，他必须在灯灭前找到续灯之人，否则全城灯火尽灭。 |
| tags | 玄幻, 灯火, 倒计时, 群像, 救赎 |
| Category | 玄幻 / 东方 |
| Cover brief | 灯塔剪影 + 头顶「07」数字 + 书名字号可读 |
| Author note | 一个只能看见别人死期的守夜人，只剩七天可活。 |
```

Hand-off checklist:

- [ ] Winning blurb variant already recorded (fit score ≥ 4)
- [ ] `title` / `one_liner` / `short_blurb` / `long_synopsis` / `tags` match this table
- [ ] Platform form paste uses **these** fields only — no parallel drafts

---

## Synopsis Formula

Sentence 1: who the protagonist is and what they lose or lack.

Sentence 2: the inciting advantage (system, cheat, rebirth, inheritance).

Sentence 3: the near-term goal the first 30 chapters chase.

Do not summarize the entire plot.

Do not use abstract praise (精彩 / 震撼 / 不容错过).

---

## Launch Batch Review

Run tools/launch_batch_reviewer.md on the full 3–10 chapter batch (not only the golden three).

Minimum 3 chapters. Preferred 5-10.

| Check | Pass Condition |
|-------|----------------|
| Hook debt | Each chapter ends with CONTINUE or ESCALATE on the cliffhanger ledger |
| Continuity | Story bible updated after chapter 3 |
| Pacing | No two consecutive low-density chapters |
| Style | Style Profile fingerprints held if a profile exists |

---

## Red Flags

- Submitting before golden_three_reviewer runs
- Tags that describe the author mood instead of the reader promise
- Synopsis that spoils the mid-book twist
- Launch batch shorter than 3 chapters on a platform that ranks by early retention
- Copying a competitor title within the same category week

---

## Output

Emit a short report:

1. Platform
2. Gate results (pass / fail per step)
3. Final metadata pack
4. Launch batch chapter list and dates
5. Remaining risks

Verdict: READY / HOLD / REWRITE
