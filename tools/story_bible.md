# story_bible

## Purpose

Story Bible is the single source of truth for cross-chapter consistency.

It is the memory layer between Architect output and Writer output.

It prevents:

- Character drift
- Power system breaks
- Forgotten foreshadowing
- Timeline contradictions
- Location errors

---

## When To Use

Before every chapter:

Load the bible.

After every chapter:

Update the bible.

Before every Editor pass:

Send the bible with the draft.

---

## Bible Template

### 1. Characters

For every major character:

| Field | Value |
|-------|-------|
| Name | |
| Goal | |
| Motivation | |
| Fear | |
| Weakness | |
| Secret | |
| Key Relationships | |
| Current Status | |
| Last Appearance | |

### 2. Power System State

- Current realm / level of protagonist
- Available abilities
- Active limitations
- Consumed resources / costs
- Rules established so far
- Rules not yet revealed

### 3. Factions & Locations

For every faction:

- Goal
- Relationship with protagonist
- Current state
- Known secrets

For every recurring location:

- Description anchor
- Atmosphere
- Last visit

### 4. Foreshadow Ledger

For every setup:

| Field | Value |
|-------|-------|
| Setup | |
| Introduced In | |
| Purpose | |
| Planned Reveal | |
| Status | Pending / Partially Paid / Paid |

Never delete a pending entry.

### 5. Continuity Log

| Chapter | Date/Time (in-story) | Location | Key Events | New Characters | New Objects |
|---------|---------------------|----------|------------|----------------|--------------|
| | | | | | |

---

## Sync Protocol

### Before Writing

1. Load the current bible.
2. Verify protagonist state matches the end of the last chapter.
3. Verify pending foreshadow entries relevant to this chapter.
4. Flag any proposed change that contradicts the bible.

### After Writing

1. Record the chapter in the Continuity Log.
2. Update Current Status for every character that appeared.
3. Update Power System State if anything changed.
4. Add new setups to the Foreshadow Ledger.
5. Mark paid foreshadowing as Paid.

### Editor Pass

The Editor Agent must check the draft against the bible:

- Does character behavior match Current Status?
- Does power usage respect established rules?
- Are all referenced locations consistent?
- Is every new setup logged?

---

## Rule

When the draft and the bible conflict:

The bible wins.

If the bible must change:

Explain the change in the Continuity Log before writing.
