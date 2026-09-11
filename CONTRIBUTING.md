# Contributing

Thanks for your interest in Chinese WebNovel Master.

This repository is a knowledge and workflow skill. Contributions are mostly documentation, not code.

---

## Ways To Contribute

* Report a broken or empty file
* Propose a new platform knowledge base
* Propose a new tool document
* Improve an existing pattern analysis
* Fix typos, broken links or inconsistent terminology

---

## Before You Start

Open an issue first for anything larger than a typo.

State:

* What is missing or wrong
* Which file it affects
* What the reader of that file should be able to do afterwards

---

## Repository Layout

| Directory | Contents |
|-----------|----------|
| SKILL.md | Entry point and workflow definition |
| prompts/ | Agent role prompts |
| tools/ | Reusable procedure documents |
| knowledge/ | Pattern and market knowledge bases |
| examples/ | Worked end-to-end examples |
| docs/ | Architecture, workflow and quickstart notes |

---

## Writing Rules

All documents are written in English.

Follow the house style:

* Short sentences, one idea per line
* `---` between major sections
* Tables for structured data
* Imperative mood for rules
* No marketing language

Every rule must be actionable.

If a rule cannot be applied to a draft, it does not belong here.

---

## Adding A Knowledge Base

Place the file in `knowledge/` and follow the standard structure:

1. Audience
2. Core Characteristics
3. Reader Retention Factors
4. Success Checklist

Name the file after the platform, lowercase with underscores.

Reference it from SKILL.md if it changes behavior.

---

## Adding A Tool

Place the file in `tools/` and cover:

1. Purpose
2. When To Use
3. The procedure or template
4. Quality Bar
5. Output Format

Tools must be invocable by an agent without further interpretation.

Register the tool in the Tools table in SKILL.md.

---

## Commit Messages

Use a type prefix:

| Prefix | Use |
|--------|-----|
| feat | New knowledge base or tool |
| fix | Correction to an existing document |
| docs | README, ROADMAP, CHANGELOG |
| chore | Structure or housekeeping |

Example: `feat(knowledge): add feilu patterns`

---

## Pull Requests

One concern per pull request.

Describe what changed and why.

Link the related issue when one exists.

---

## What Not To Submit

* Novel manuscripts or story drafts
* Personal data or credentials
* Platform scraped content that violates terms of service
* Files that duplicate an existing document

---

## Review Checklist

Before opening a pull request, confirm:

* The document follows the house style
* The file structure matches its directory convention
* SKILL.md is updated when behavior changes
* No empty placeholder files are introduced
