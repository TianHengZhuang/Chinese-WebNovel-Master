# Changelog

All notable changes to Chinese WebNovel Master.

## [v2.3.1] - 2026-09-11

### Fixed

- assets/Chinese WebNovel.png — re-encoded without OpenAI / C2PA provenance metadata
- knowledge/title_patterns.md — replaced the example title「我掌控了人工智能」with「我掌控了签到系统」

## [v2.3.0] - 2026-09-11

### Added

- tools/style_sampler.md — author voice sampling: surface fingerprints (sentence length, short-punch ratio, dialogue share, punctuation), lexical keep/cap/taboo lists, narrative stance, Style Profile template, FLAT / DRIFT / TABOO / CLICHE / OVERCOPY flags with default tolerances

### Changed

- prompts/writer.md — Style Profile Sync protocol: load before drafting, bind fingerprints while writing, self-check after drafting
- prompts/editor.md — Step 8 Style Compliance against the profile; AI Writing Detection prefers author fingerprint over generic rewrite
- SKILL.md — AI Style Removal section honors Style Profiles; tools table registers style_sampler
- README.md — structure tree, tools tables, current version and version markers
- ROADMAP.md — v2.3 moved from Planned to Released

## [v2.2.0] - 2026-09-11

### Added

- tools/publishing_calendar.md — serialized release planning: update cadence, backlog safety line, launch and break strategy, risk table
- tools/cliffhanger_continuity_checker.md — hook debt ledger, hook variety grid, escalation audit with CONTINUE / FIX ENDINGS / RESTRUCTURE verdicts
- tools/title_scorer.md — five-dimension title scoring (curiosity, identity advantage, conflict, concreteness, platform fit) with worked examples
- knowledge/feilu_patterns.md — extreme pacing, payoff density, fan-fiction culture, chapter economics
- knowledge/jinjiang_patterns.md — prose quality, character depth, channel conventions, tag and warning culture, synopsis craft
- CONTRIBUTING.md — repository layout, house style, templates for new knowledge bases and tools, commit conventions

### Changed

- tools/hook_generator.md — replaced the placeholder with the full hook generation procedure (8 hook types, forbidden endings, escalation ladder)
- tools/retention_analyzer.md — replaced the placeholder with the weighted retention scoring model and failure diagnostics
- SKILL.md — tools table now registers title_scorer, publishing_calendar and cliffhanger_continuity_checker
- README.md — project structure tree, tools table and repository index aligned
- ROADMAP.md — v2.2 moved from Planned to Released

### Fixed

- Removed six reachable-but-empty placeholder files (hook_generator, retention_analyzer, title_scorer, feilu_patterns, jinjiang_patterns, CONTRIBUTING)

## [v2.1.1] - 2026-09-08

### Added

- knowledge/genre_historical_patterns.md — historical/time-travel: era research discipline, knowledge-advantage rules, status progression ladder, 6 sub-variants
- knowledge/genre_urban_supernatural_patterns.md — urban system: 7 system types (天选/任务/升级/职业/合成/天赋/规则), 7 sub-variants, 4-stage progression ladder
- knowledge/genre_romance_patterns.md — romance: 6-stage relationship arc, 8 sub-variants, female/male protagonist empowerment patterns
- knowledge/genre_mythology_patterns.md — mythological/xuanhuan: 6 power system types, world layer structure (世俗界→混沌虚空), sect politics, tribulation architecture, 7 sub-variants
- README.md — updated structure tree and genre patterns table (16 platform + 8 genre coverage)

## [v2.1.0] - 2026-09-08

### Added

- tools/story_bible.md — cross-chapter consistency bible (character state, power system state, factions & locations, foreshadow ledger, continuity log)
- tools/golden_three_reviewer.md — first-three-chapter audit with GO / REVISE / REWRITE verdicts
- tools/pacing_rhythm_map.md — satisfaction-density mapping and ten-chapter rhythm engine audits
- tools/character_arc_tracker.md — arc health tracking with STATIC / UNMOTIVATED / DRIFT / CHEAT / FLAT flags
- knowledge/genre_scifi_patterns.md — sci-fi reader expectations, scale ladder, tech discipline
- knowledge/genre_suspense_patterns.md — mystery architecture, fair-play reversal rules, clue discipline
- knowledge/genre_game_patterns.md — system-flow panels, quest chains, cost mechanics
- knowledge/genre_era_patterns.md — era coordinates, period texture, era advantage rules
- CHANGELOG.md — release history (this file)

### Changed

- prompts/writer.md — added Story Bible Sync protocol (load before writing, update after writing)
- prompts/editor.md — added Story Bible Compliance step (Step 7) to the review workflow
- SKILL.md — added Tools section listing all six tool entry points and when to invoke them
- ROADMAP.md — rewritten with release history and v2.2+ plan

## [v2.0.1] - 2026-09-04

### Added

- 8 platform knowledge bases: qimao, zongheng, ciweimao, boluobao, xiaoxiang, hongxiu, 17k, tadu
- Security policy (SECURITY.md)

### Changed

- README expanded with full platform table and version marker
- Automated collaboration workflow validated end-to-end

## [v2.0] - Retention Engine

- Retention scoring mindset embedded in skill rules
- Platform-specific optimization engines
- tools/retention_analyzer.md entry point

## [v1.1] - Knowledge Expansion

- Expanded platform knowledge (feilu, jinjiang additions)
- Improved examples
- Enhanced publishing workflows
- tools/hook_generator.md entry point

## [v1.0] - Core Framework

- Multi-agent workflow (Planner → Architect → Writer → Editor → Publisher)
- Core knowledge base (tomato, qidian, title, suspense_hooks, character, power_system)
- Example projects (urban_system, xianxia, apocalypse, romance)
- Tag: V1.0.0
