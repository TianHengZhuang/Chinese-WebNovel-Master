# Roadmap

Chinese WebNovel Master evolution plan.

## Released

### v2.9.0 — Niche Genre Packs: Sports / Esports / Workplace / Food (2026-10-21)

- knowledge/genre_sports_patterns.md: competitive sports — match realism, signature-skill + weakness, team/rivalry economy, golden-finger limits, failure modes
- knowledge/genre_esports_patterns.md: esports — game engine, meta/patch/ban pressure, pro ecosystem and fandom, golden-finger limits, failure modes
- knowledge/genre_workplace_patterns.md: workplace/career — industry credibility, power map, reversal economy, golden-finger limits, failure modes
- knowledge/genre_food_patterns.md: food fiction — five-sense sensory engine, craft/ingredient limits, customer-reaction payoff, golden-finger limits, failure modes
- README.md registers all four packs in the genre index and project structure

### v2.8.0 — Genre Expansion: Detective & Era Crossover (2026-10-14)

- knowledge/genre_detective_patterns.md: case architecture, fair-play contract, clue types, suspect pool math, interrogation rhythm, evidence-chain and procedure rules, power-advantage limits
- knowledge/genre_era_crossover_patterns.md: era base + second genre engine, combination matrix, era escrow, first-payoff placement, texture budget, language rules, failure modes
- README.md registers both packs in the genre index and project structure

### v2.7.0 — Submission Coverage Complete (2026-09-22)

- knowledge/submit_17k.md / submit_boluobao.md / submit_ciweimao.md / submit_tadu.md / submit_xiaoxiang.md / submit_hongxiu.md: remaining six platform submit packs (all 12 platforms covered)
- tools/chapter_fix_list.md: per-chapter fix lists generated from a launch batch score (BLOCKER / SHOULD-FIX / POLISH, evidence + re-check rows, exit criteria)
- tools/submission_checklist.md: platform list covers 12 packs; HOLD batches route into chapter_fix_list
- tools/launch_batch_reviewer.md: HOLD / RESTRUCTURE verdicts route into chapter_fix_list

### v2.6.0 — Continuity & Pack Hand-off (2026-09-18)

- tools/story_continuity_checker.md: bible / name / power / timeline continuity gates
- tools/platform_submit_pack.md: checklist metadata → per-platform paste sheets
- submission_checklist gates 9–10 wired to the two tools

### v2.5.1 — Checklist Blurb Backfill (2026-09-18)

- tools/submission_checklist.md: filled metadata example and hand-off checklist

### v2.5.0 — Listing Copy Engine (2026-09-14)

- tools/blurb_synopsis_generator.md: title variants → one-liner / short blurb / long synopsis / tags / fit score
- Feeds tools/submission_checklist.md metadata without re-writing platform forms by hand

### v1.0 — Core Framework

- Multi-agent workflow (Planner → Architect → Writer → Editor → Publisher)
- Core knowledge base
- Example projects
- Tag: V1.0.0

### v1.1 — Knowledge Expansion

- Expanded platform patterns
- Improved examples
- Enhanced publishing workflows

### v2.0 — Retention Engine

- Automated evaluation mindset
- Reader retention scoring
- Platform-specific optimization engines

### v2.0.1 — Collaboration Validation (2026-09-04)

- Automated collaboration workflow validated end-to-end
- 8 additional platform knowledge bases (qimao, zongheng, ciweimao, boluobao, xiaoxiang, hongxiu, 17k, tadu)

### v2.1.0 — Consistency Layer (2026-09-08)

- tools/story_bible.md: single source of truth for cross-chapter consistency (characters, power state, factions, foreshadow ledger, continuity log)
- tools/golden_three_reviewer.md: first-three-chapters audit with GO / REVISE / REWRITE verdicts
- tools/pacing_rhythm_map.md: satisfaction-density mapping over the ten-chapter engine
- tools/character_arc_tracker.md: arc health flags (STATIC / UNMOTIVATED / DRIFT / CHEAT / FLAT)
- 4 genre knowledge bases: sci-fi, suspense, game/system, era fiction
- Writer & Editor agents bound to the story bible sync protocol
- CHANGELOG.md introduced

### v2.2.0 — Serialization Operations (2026-09-11)

- tools/publishing_calendar.md: release cadence planning, backlog safety line, launch and break strategy, risk table
- tools/cliffhanger_continuity_checker.md: hook debt ledger, hook variety grid, escalation audit
- tools/title_scorer.md: five-dimension title scoring, now registered in SKILL.md
- tools/hook_generator.md: implemented (was an empty placeholder)
- tools/retention_analyzer.md: implemented (was an empty placeholder)
- knowledge/feilu_patterns.md: implemented (was an empty placeholder)
- knowledge/jinjiang_patterns.md: implemented (was an empty placeholder)
- CONTRIBUTING.md: repository layout, house style, contribution templates

### v2.3.0 — Author Voice Layer (2026-09-11)

- tools/style_sampler.md: surface + lexical fingerprints, narrative stance, Style Profile template, FLAT / DRIFT / TABOO / CLICHE / OVERCOPY flags
- prompts/writer.md: Style Profile Sync (load, bind, self-check)
- prompts/editor.md: Step 8 Style Compliance; AI detection prefers author fingerprint
- SKILL.md: AI Style Removal honors profiles; tools table registers style_sampler

### v2.4.0 — Submission Automation (minimal slice, 2026-09-12)

- tools/submission_checklist.md: pre-upload gate, metadata pack, launch batch review
- knowledge/submit_qidian.md / submit_tomato.md / submit_jinjiang.md: platform submit packs
- SKILL.md and README register the checklist and submit packs

### v2.4.1 — Submission packs continued (2026-09-12)

- knowledge/submit_feilu.md / submit_qimao.md / submit_zongheng.md
- checklist now points at six platform packs

### v2.4.2 — Launch batch reviewer (2026-09-12)

- tools/launch_batch_reviewer.md: 5-pass batch audit and READY / HOLD / RESTRUCTURE score

### v2.4.3 — Checklist cross-links the full batch reviewer (2026-09-12)

- tools/submission_checklist.md points at tools/launch_batch_reviewer.md instead of a thinner inline table

### v2.4.4 — Tools table completeness (2026-09-13)

- README.md tools table registers all 12 tools
- ROADMAP.md records the v2.4.1–v2.4.4 released line

## Planned

### Long-Term

- Bilingual operation mode (Chinese content, bilingual author guidance)
- Community templates for reader-poll driven writing
- Full series management dashboard (characters, arcs, foreshadow across 1000+ chapters)
