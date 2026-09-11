# style_sampler

## Purpose

Style Sampler turns an author's existing chapters into a reusable Style Profile.

Generic prose sells poorly.

Copyable voice keeps readers.

This tool extracts measurable voice fingerprints and feeds them to Writer and Editor.

It prevents:

- Uniform AI tone across chapters
- Losing a paid author's signature rhythm
- Taboo phrases slipping into clean commercial fiction
- Style drift between volumes

---

## When To Use

At project start, before the first drafted chapter.

When adopting a ghostwriting or continuation contract with sample chapters.

When a long serialization starts sounding like every other book.

When Editor keeps flagging "generic AI phrasing" and the samples already contain a better voice.

Pairs with tools/story_bible.md (plot memory) and prompts/writer.md (drafting rules).

---

## Input

Minimum sample set:

| Input | Guidance |
|-------|----------|
| Sample chapters | 3–10 completed chapters by the same author |
| Genre + platform | e.g. 番茄 / 都市系统; affects register and sentence length |
| Known voice notes | Optional author notes: "short punches", "no flowery metaphors", etc. |
| Clean target | If continuing someone else's book, samples must be from that same book when possible |

Reject samples that mix multiple authors, heavy machine rewrite, or a different genre from the target book.

---

## Sampling Procedure

### Step 1 — Clean the sample

Strip chapter titles, author notes, ads, and reader comments.

Keep narrative and dialogue only.

### Step 2 — Measure surface fingerprints

| Metric | How | Why |
|--------|-----|-----|
| Avg sentence length | characters per sentence (Chinese) or words (English) | rhythm |
| Short-punch ratio | share of sentences ≤ 8 Chinese characters | snap / force |
| Dialogue share | dialogue characters / total | talkative vs narrative voice |
| Paragraph length | avg and P90 | breath and density |
| Punctuation habits | frequency of ！……——、； | emotion style |
| Repetition crutches | top 10 openers and connectors | author tics (keep or cap) |

### Step 3 — Extract lexical fingerprints

Collect:

| Bucket | Examples (Chinese web fiction) |
|--------|--------------------------------|
| Signature openers | "下一秒"、"就在这时"、"嘶——" |
| Emotional intensifiers | "简直"、"压根"、"他妈的" (if allowed) |
| Power / status verbs | common fight and upgrade verbs in this author's samples |
| Taboo list | phrases the author never uses (e.g. no "深吸一口气") |
| Metaphor density | low / medium / high; preferred source domain (martial, food, workplace) |

### Step 4 — Capture narrative stance

Record:

- POV: first / third limited / third omniscient
- Tense feel: immediate vs retrospective
- Irony level: none / dry / satirical
- Humor: absent / banter / slapstick
- Violence: implied / kinetic / clinical
- Romance heat: fade-to-black / suggestive / explicit (must match platform rules)

### Step 5 — Write the Style Profile

Use the template below. One profile per book, not per author.

---

## Style Profile Template

```markdown
# Style Profile — <Book / Project>

## Identity
- Source samples: <file list or chapter range>
- Genre / Platform:
- Continuation or fresh book:

## Surface Fingerprints
| Metric | Target |
|--------|--------|
| Avg sentence length | |
| Short-punch ratio | |
| Dialogue share | |
| Avg paragraph length | |
| Dominant punctuation | |

## Lexical Fingerprint
### Keep (signature)
- 
### Cap (max N per chapter)
- 
### Taboo (never)
- 

## Narrative Stance
| Axis | Setting |
|------|---------|
| POV | |
| Irony | |
| Humor | |
| Violence | |
| Romance heat | |

## Rhythm Notes
- Typical chapter open pattern:
- Typical scene cut pattern:
- Typical chapter-end beat:

## Sample Passages (anchor quotes)
1. "..." — why it is the voice
2. "..."
3. "..."
```

Store the profile beside the story bible (e.g. `style_profile.md` in the project workspace).

---

## Fingerprint Flags

Editor and Writer must report:

| Flag | Meaning |
|------|---------|
| FLAT | Profile missing or unusable |
| DRIFT | Draft departs from profile metrics beyond tolerance |
| TABOO | Forbidden phrase or structure appeared |
| CLICHE | AI-generic phrasing used where a signature move exists |
| OVERCOPY | Sample tics repeated past the cap (parody of the author) |

Tolerances (default):

- Avg sentence length: ±20% of profile target
- Short-punch ratio: ±10 percentage points
- Dialogue share: ±12 percentage points
- Taboo list: zero tolerance

---

## Worked Mini-Example

Samples suggest:

| Metric | Sample | Draft | Verdict |
|--------|--------|-------|---------|
| Avg sentence | 18 chars | 31 chars | DRIFT |
| Short-punch | 22% | 8% | DRIFT |
| Dialogue | 35% | 40% | OK |
| Taboo "深吸一口气" | never | 2 hits | TABOO |

Action: shorten narration, restore punch sentences, delete taboo phrase.

---

## Output Format

1. Style Profile (template filled)
2. Sampling notes: missing samples, mixed voices, platform conflicts
3. Writer directives: 3–7 binding rules distilled from the profile
4. Editor directives: which fingerprints to score and which flags to raise

---

## Boundaries

This tool does not replace plot tools.

It does not invent a voice with no samples.

If samples conflict, prefer the most recent continuous stretch of the same book.

Platform safety rules always override author voice.
