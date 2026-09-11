# title_scorer

## Purpose

Score candidate titles for click-through before publishing.

The title is the first promise the story makes.

It decides whether the story is ever read.

---

## When To Use

During the Publisher stage.

Before platform submission.

When comparing title variants.

When a story underperforms despite strong retention.

Pairs with knowledge/title_patterns.md.

---

## Scoring Dimensions

| Dimension | Weight | What It Measures |
|-----------|--------|------------------|
| Curiosity | 30% | Does the title open a question? |
| Identity Advantage | 20% | Does it promise the reader a position of power? |
| Conflict | 20% | Is a stake expressed? |
| Concreteness | 15% | Specific nouns and numbers over abstract words |
| Platform Fit | 15% | Matches the target platform title conventions |

---

## Rubric

Score each dimension 0-10.

Curiosity: 10 means the reader cannot guess the answer.

Identity Advantage: 10 means the reader imagines themselves in the position of advantage.

Conflict: 10 means the loser and the winner are both implied.

Concreteness: 10 means every word is a visible image or a number.

Platform Fit: 10 means the title reads native to the target platform.

---

## Formula

Title Score = (sum of dimension score x weight) x 10

Result range: 0-100.

| Score | Verdict |
|-------|---------|
| 85-100 | Strong |
| 70-84 | Usable |
| 0-69 | Rewrite |

---

## Red Flags

- Generic words: 传奇 / 人生 / 旅途 / 杂记
- No noun the reader can visualize
- Length beyond the platform convention
- Spoiling the first major payoff
- Matching a title that already dominates the category

---

## Variant Protocol

Generate 5 candidates.

Score all 5.

Keep the top 2.

Never publish the first idea.

---

## Worked Examples

| Title | Curiosity | Identity | Conflict | Concreteness | Platform Fit | Score |
|-------|-----------|----------|----------|--------------|--------------|-------|
| 离婚后，我成了首富 | 8 | 9 | 8 | 7 | 9 | 82 |
| 直播鉴宝：开局捡漏亿元古画 | 9 | 8 | 7 | 10 | 9 | 86 |
| 末世：我提前囤积十万吨物资 | 9 | 9 | 8 | 10 | 9 | 90 |
| 长生从炼丹开始 | 8 | 8 | 5 | 8 | 8 | 75 |

---

## Output Format

Candidates table:

| Title | Score | Weakest Dimension |

Recommended Title:

Reason:

Next Action: publish / retest variants
