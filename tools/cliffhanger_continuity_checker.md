# cliffhanger_continuity_checker

## Purpose

Audit a run of consecutive chapter endings for continuity, variety and debt.

Hooks are a chain. A broken chain loses the reader even when every chapter is good.

---

## When To Use

After every ten chapters.

Before a batch release.

Before a platform submission.

Immediately after a chapter that felt hard to end.

---

## Three Checks

### Check 1: Hook Debt

Every hook is a promise.

Every promise must be paid.

Build a ledger of the last ten chapter endings.

| Chapter | Hook Type | Promise Made | Paid In |
|---------|-----------|--------------|---------|

Rule:

Any promise older than five chapters becomes a debt flag.

Any debt flag older than ten chapters is a structural failure.

---

### Check 2: Hook Variety

| Chapter | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 |
|---------|---|---|---|---|---|---|---|---|---|----|
| Hook Type | | | | | | | | | | |

Rule:

No hook type may appear in two consecutive chapters.

No single hook type may appear more than three times in ten chapters.

Violation: rewrite the repeated ending via tools/hook_generator.md.

---

### Check 3: Escalation

Compare stakes chapter to chapter.

Question to answer for each pair:

Does this ending raise the stakes over the previous ending?

Rule:

Stakes must never reset downward without a payoff first.

A downshift is allowed only immediately after a major payoff.

---

## Failure Patterns

| Pattern | Description | Fix |
|---------|-------------|-----|
| Hook treadmill | New hook every chapter, none paid | Pay the oldest debt |
| Hook echo | Same type repeated | Rotate types |
| Stake reset | Stakes drop with no payoff | Insert a payoff or raise stakes |
| False hook | Promise never intended to be paid | Delete or convert into a real setup |
| Dead ending | Chapter ends on routine activity | Rewrite with tools/hook_generator.md |

---

## Procedure

1. List the last ten chapter endings.
2. Fill the hook ledger.
3. Fill the variety grid.
4. Compare the escalation of each pair.
5. Flag every failure pattern.
6. Rewrite flagged endings.
7. Sync the surviving setups into tools/story_bible.md.

---

## Output Format

Chapter Range:

Hook Ledger table:

Variety Grid:

Debt Flags:

Escalation Failures:

Rewrites Required:

Verdict: CONTINUE / FIX ENDINGS / RESTRUCTURE
