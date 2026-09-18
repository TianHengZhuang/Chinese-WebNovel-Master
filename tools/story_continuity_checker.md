# story_continuity_checker

## Purpose

Audit **cross-chapter story continuity** against the story bible: names, powers, timelines, places, and open promises.

`cliffhanger_continuity_checker.md` covers **hook debt**. This tool covers **setting / character / timeline** drift that readers notice even when hooks are strong.

---

## When To Use

- After every 10 chapters
- Before platform submission
- After a large outline rewrite
- When a beta reader says “他怎么突然会飞了？”

---

## Inputs

| Input | Source |
|-------|--------|
| Story bible | `tools/story_bible.md` |
| Recent chapters | 10–20 chapter summaries or full text |
| Golden three | first-three-chapter canon |

---

## Checks

### 1. Name / title consistency

| Item | Bible | Chapters | Status |
|------|-------|----------|--------|
| Protagonist name / aliases | | | |
| Faction / sect names | | | |
| Item / artifact names | | | |

Rule: any alias introduced must appear in the bible within the same batch review.

### 2. Power / ability ledger

| Ability | Unlocked in | Limits (bible) | Violation in chapters | Status |
|---------|-------------|----------------|------------------------|--------|
| | | | | |

Rule: **no new ability without an unlock scene**. Limits must not silently disappear.

### 3. Timeline & travel

| Event | Chapter | Stated time | Place | Conflict |
|-------|---------|-------------|-------|----------|
| | | | | |

Rule: travel time between named places must not exceed bible distance table (if present) without a time-skip line.

### 4. Promise ledger (link to cliffhanger tool)

Copy unpaid hooks from `cliffhanger_continuity_checker` debt table. Mark each as:

- still open
- paid in chapter N
- retconned (must be explicit in text)

---

## Output

```markdown
## Continuity verdict: CLEAN | FIX-THEN-SUBMIT | REWRITE

### Blockers
- ...

### Soft warnings
- ...

### Bible updates required
- ...
```

### Verdict rules

| Verdict | Condition |
|---------|-----------|
| CLEAN | No blockers; bible already matches |
| FIX-THEN-SUBMIT | 1–3 soft warnings; fix names/limits only |
| REWRITE | Any power/timeline blocker that changes plot |

---

## Hand-off

1. Update `tools/story_bible.md` for accepted new canon
2. Run `tools/cliffhanger_continuity_checker.md` on the same batch
3. Only then run `tools/submission_checklist.md`
