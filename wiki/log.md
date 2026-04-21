# Wiki Log

Append-only chronological record of ingest, query, lint, and maintenance operations.

## [2026-04-21] bootstrap | initialize wiki scaffold
- Scope: Created operating schema and wiki control files.
- Files changed: `.github/copilot-instructions.md`, `wiki/README.md`, `wiki/index.md`, `wiki/log.md`, `wiki/sources.md`
- Summary: Established persistent LLM wiki workflow and control structure.

## [2026-04-21] ingest | bootstrap core and docs sources
- Scope: First-pass synthesis pages generated from root and docs source files.
- Files changed: `wiki/core_overview.md`, `wiki/drift_principles_synthesis.md`, `wiki/drift_operating_prompt_guide.md`, `wiki/docs_companion_map.md`, `wiki/l1_context_guide.md`, `wiki/l2_action_fit_guide.md`, `wiki/method_mapping.md`, `wiki/index.md`, `wiki/sources.md`
- Summary: Bootstrapped foundational wiki pages and cross-links; recorded source coverage including empty `background/` state.
- Follow-ups: Ingest any future `background/*` files and run `lint wiki` after next 3 to 5 ingests.

## [2026-04-21] ingest | ingest all
- Scope: Full ingest sweep across configured raw sources.
- Files changed: `wiki/log.md`
- Summary: No new or stale raw source files detected in root markdown set, `docs/`, or `background/`; existing wiki synthesis remains current.
- Follow-ups: Add files to `background/` or update raw sources, then rerun `ingest all`.

## [2026-04-21] maintain | semantic ingest schema update
- Scope: Strengthened ingest behavior to require semantic decomposition and relationship mapping.
- Files changed: `.github/copilot-instructions.md`, `wiki/log.md`
- Summary: Updated schema so ingestion breaks content into concepts/entities, tracks relationships and claims, and favors composable semantic pages.

## [2026-04-21] ingest | ingest all (semantic decomposition)
- Scope: Re-ingested all configured raw sources under semantic ingest rules.
- Files changed: `wiki/entity_drift_check.md`, `wiki/concept_context.md`, `wiki/concept_capability.md`, `wiki/concept_action_types.md`, `wiki/concept_observation.md`, `wiki/concept_misfit.md`, `wiki/concept_value_progress.md`, `wiki/core_overview.md`, `wiki/drift_principles_synthesis.md`, `wiki/drift_operating_prompt_guide.md`, `wiki/l1_context_guide.md`, `wiki/l2_action_fit_guide.md`, `wiki/method_mapping.md`, `wiki/index.md`, `wiki/sources.md`, `wiki/log.md`
- Summary: Built atomic concept/entity pages, added relationship and claim sections, linked semantic pages bidirectionally with existing synthesis pages, and refreshed source-to-page mapping.
- Follow-ups: Run `lint wiki` to detect orphans and contradiction gaps after semantic expansion.

## [2026-04-21] ingest | ingest all (readability and knowledge refresh)
- Scope: Re-ingested all wiki content to prioritize human-readable, explanatory knowledge pages while preserving semantic links and evidence traces.
- Files changed: `.github/copilot-instructions.md`, `wiki/core_overview.md`, `wiki/entity_drift_check.md`, `wiki/concept_context.md`, `wiki/concept_capability.md`, `wiki/concept_action_types.md`, `wiki/concept_observation.md`, `wiki/concept_misfit.md`, `wiki/concept_value_progress.md`, `wiki/drift_principles_synthesis.md`, `wiki/drift_operating_prompt_guide.md`, `wiki/l1_context_guide.md`, `wiki/l2_action_fit_guide.md`, `wiki/method_mapping.md`, `wiki/docs_companion_map.md`, `wiki/index.md`, `wiki/log.md`
- Summary: Reframed pages into plain-language narrative sections (`What It Means`, `Why It Matters`, `How It Connects`) so the wiki reads like a knowledge base for understanding concepts, not a rigid schema.
- Follow-ups: Run `lint wiki` to find orphan links and highlight contested claims that need deeper source triangulation.

## [2026-04-21] ingest | full granular reingest (narrative rewrite)
- Scope: Reworked ingest schema for narrative-first pages, removed prior wiki content pages, and re-ingested all raw sources into atomic concept pages.
- Files changed: `.github/copilot-instructions.md`, `wiki/capability.md`, `wiki/capability_stack.md`, `wiki/value.md`, `wiki/progress.md`, `wiki/observation.md`, `wiki/state.md`, `wiki/context.md`, `wiki/proceed.md`, `wiki/align_context.md`, `wiki/probe.md`, `wiki/stop.md`, `wiki/misfit.md`, `wiki/stabilise.md`, `wiki/rationalise.md`, `wiki/optimise.md`, `wiki/alignment.md`, `wiki/uncertainty.md`, `wiki/complexity.md`, `wiki/fragility.md`, `wiki/absorption_capacity.md`, `wiki/programme.md`, `wiki/reversibility.md`, `wiki/agency.md`, `wiki/scaling.md`, `wiki/judgement.md`, `wiki/innovation.md`, `wiki/signals_and_noise.md`, `wiki/local_optimisation.md`, `wiki/drift_check.md`, `wiki/external_validity.md`, `wiki/method_mapping.md`, `wiki/docs_companion.md`, `wiki/index.md`, `wiki/sources.md`, `wiki/log.md`
- Summary: Replaced structured synthesis pages with a finer-grained, cross-linked narrative wiki where each durable idea has its own page and formatting follows the needs of the idea.
- Follow-ups: Run `lint wiki` for orphan checks and contradiction scanning after next ingest cycle.

## [2026-04-21] lint | strict backlink and density pass
- Scope: Checked all 32 content pages for orphans, weak connections, and link integrity.
- Files changed: `wiki/drift_check.md`, `wiki/programme.md`, `wiki/state.md`, `wiki/alignment.md`, `wiki/agency.md`, `wiki/docs_companion.md`, `wiki/method_mapping.md`, `wiki/context.md`, `wiki/capability.md`, `wiki/observation.md`, `wiki/proceed.md`, `wiki/log.md`
- Summary: **Orphans eliminated:** 3 orphan pages (agency, docs_companion, method_mapping) connected to the graph. **Backlinks strengthened:** Added strategic cross-links to strengthen weakly connected pages. Final state: 0 orphans, 7 pages with 2-3 backlinks (all well-connected), all links valid.
- Follow-ups: Monitor for new content to maintain link density during future ingests.

## [2026-04-21] ingest | background/capability.md (components, value flow, failure propagation)
- Scope: Ingested new background source on capability components model, value flow mechanics, and failure propagation.
- Files changed: `wiki/capability.md`, `wiki/capability_stack.md`, `wiki/fragility.md`, `wiki/visibility_control_tension.md` (new), `wiki/index.md`, `wiki/sources.md`, `wiki/log.md`
- Summary: Enhanced three existing pages with concrete examples and observ able mechanisms; created new focused page on visibility-control tension. Updated capability.md with five-component enabler model and removed defensive "What X is not" section per accessibility guidelines. Expanded capability_stack.md with value flow direction, dependency amplification mechanics, and the visibility-control paradox. Enhanced fragility.md with failure propagation sequence and patterns. Created visibility_control_tension.md as distinct atomic idea emphasizing how value is visible at top but reliability is created at bottom.
- Follow-ups: Run `lint wiki` to check new page backlink density and validate all new cross-links.

## [2026-04-21] maintain | factored out concept vocabulary to wiki control file
- Scope: Extracted canonical concept vocabulary from copilot instructions into a maintainable wiki file.
- Files changed: `wiki/_concepts_vocabulary.md` (new), `.github/copilot-instructions.md`, `wiki/index.md`, `wiki/log.md`
- Summary: Created `wiki/_concepts_vocabulary.md` as the single source of truth for key DRIFT concepts (33 total across 5 categories). Updated copilot instructions to reference this file via "Cross-linking and concept highlighting" section and enhanced "Lint" operations to include vocabulary and linking audits. This decouples concept list from instruction files, making vocabulary updates automatic without requiring instruction changes.
- Follow-ups: Update vocabulary file whenever new concept pages are created during future ingests.

## [2026-04-21] ingest | reingest with mandatory vocabulary update
- Scope: Re-ingested all core content under new mandatory control file update rules.
- Files changed: `.github/copilot-instructions.md`, `wiki/drift_check.md`, `wiki/context.md`, `wiki/capability.md`, `wiki/misfit.md`, `wiki/state.md`, `wiki/observation.md`, `wiki/stabilise.md`, `wiki/log.md`
- Summary: Updated ingest instructions (step 7) to make updating `_concepts_vocabulary.md` a mandatory control file requirement alongside index, sources, and log. Re-ingested key pages (entry points and core concepts) to enforce new cross-linking rules: concepts linked on first mention, bolded on first mention in new context, and "See also" sections expanded to 6–8 genuinely related links per page. Updated pages: drift_check (8→10 links), context (7→10 links), capability (8→10 links), misfit (6→10 links), state (6→7 links), observation (6→7 links), stabilise (5→8 links). All inbound/outbound links validated.
- Follow-ups: Run comprehensive lint audit on all 33 pages; check for any remaining orphans or missed concept links.

## [2026-04-21] lint | spot-check remaining 25 pages for concept linking and link density
- Scope: Audited all 33 content pages for unlinked concept mentions, weak "See also" sections (< 4 links), and orphan status.
- Files changed: `wiki/alignment.md`, `wiki/rationalise.md`, `wiki/optimise.md`, `wiki/reversibility.md`, `wiki/log.md`
- Summary: **Issues found and fixed:** 1 formatting error (alignment.md: `[state.md]` → `[state]`), 2 pages with unlinked body-text concepts (rationalise, optimise: added [fragility] links), 2 pages with weak See also sections (rationalise expanded 5→7 links, optimise expanded 5→8 links, reversibility expanded 4→6 links). **Spot-check results:** All 33 content pages have ≥4 "See also" links. 30/33 pages have 5+ links (exceeding 4–8 guidance). 0 orphan pages detected. Concept linking is strong across entry points (drift_check, context, capability, method_mapping, docs_companion) and core concepts. All links validated (ALL_LINKS_OK).
- Follow-ups: Consider whether any remaining pages would benefit from stronger internal concept linking (currently ~95% compliance with linking guidelines).

## [2026-04-21] maintain | rewrite index.md and formalize index quality standards
- Scope: Transformed wiki index from categorical listing into narrative, decision-maker-focused entry point. Formalized presentation standards in copilot instructions.
- Files changed: `wiki/index.md`, `.github/copilot-instructions.md`, `wiki/log.md`
- Summary: **Index Quality Standards added to instructions:** New subsection under "Refresh Index" documenting required standards: narrative intro (2–4 sentences, observable language), user-type entry points (3 "Start here if..." anchors for common scenarios), meaningful section headers (why concepts cluster, not just labels), decision-maker descriptions (1–2 sentences, lead with problems not definitions), optional connection hints for dependencies, and validation checklist. **index.md rewritten:** Added opening paragraph explaining DRIFT purpose and outcomes for three decision-maker personas (executives, technologists, programme managers). Added three user-type entry points: concerns about unpredictability → capability/state; about initiative worthiness → context/stop; about fragmentation → alignment/misfit. Replaced categorical headers with narrative framing: "What You Work With: The Core Decision Patterns", "When You're Deciding What to Do: Action Patterns", "How You Intervene: Building Capability", "What Actually Happens: Signals, Fragility, and the Limits of Control", "Building and Defending Value". Rewrote all 33 descriptions to lead with observable problems and consequences, not abstract definitions. Integrated vocabulary reference for secondary discovery path.
- Follow-ups: Ensure future "refresh index" operations validate conformance to these quality standards.

## [2026-04-21] maintain | correct DRIFT terminology from framework to tool
- Scope: Enforce precise terminology: DRIFT is a tool, not a decision framework.
- Files changed: `wiki/index.md`, `.github/copilot-instructions.md`, `wiki/log.md`
- Summary: Corrected opening paragraph of index.md from "DRIFT is a decision framework..." to "DRIFT is a tool...". Added new "What This Wiki Documents" section to copilot instructions explaining that DRIFT is a tool, not a framework, and that it works alongside existing frameworks and governance structures—extending thinking, not replacing expertise or accountability. Updated Accessibility section's "Avoid defending the tool" bullet to "Clarify what this tool is, not what it isn't", emphasizing that DRIFT is meant to work with existing frameworks. Terminology now aligned across index, instructions, and drift_check.md (which already correctly characterized DRIFT as a thinking tool).
- Follow-ups: Apply same precision to any future index rewrites or accessibility documentation.

## [2026-04-21] ingest | background reversibility absorption thresholds
- Scope: Ingested new background source on reversibility, absorption capacity, and decision confidence thresholds.
- Files changed: `wiki/reversibility.md`, `wiki/absorption_capacity.md`, `wiki/decision_thresholds.md` (new), `wiki/_concepts_vocabulary.md`, `wiki/index.md`, `wiki/sources.md`, `wiki/log.md`
- Summary: Expanded reversibility and absorption capacity pages with practical decision implications, observable risk signals, and failure patterns. Added new atomic concept page `decision_thresholds.md` to capture how required confidence should vary by reversibility, absorption capacity, and consequence. Updated concept vocabulary (+1 concept, now 34 total), indexed the new page, and registered source coverage.
- Follow-ups: Run lint to check concept-link density around the new page and verify no weakly connected nodes.

## [2026-04-21] lint | strengthen decision-threshold cluster integration
- Scope: Strengthened graph integration for newly ingested decision-threshold concept.
- Files changed: `wiki/context.md`, `wiki/probe.md`, `wiki/judgement.md`, `wiki/scaling.md`, `wiki/log.md`
- Summary: Added targeted [decision_thresholds.md](decision_thresholds.md) links to context/action and judgement pages where threshold logic is explicitly relevant. Inbound links to `decision_thresholds.md` increased from 2 to 6 (`absorption_capacity`, `context`, `judgement`, `probe`, `reversibility`, `scaling`). Re-ran link validation with `ALL_LINKS_OK`.
- Follow-ups: Optionally add threshold framing to `proceed.md` and `stop.md` in the next style refresh pass.

## [2026-04-21] maintain | enforce plain-language guardrail and rewrite dense wiki phrasing
- Scope: Added explicit readability rules to instructions and re-edited dense language across concept pages.
- Files changed: `.github/copilot-instructions.md`, `wiki/align_context.md`, `wiki/alignment.md`, `wiki/capability.md`, `wiki/capability_stack.md`, `wiki/context.md`, `wiki/decision_thresholds.md`, `wiki/docs_companion.md`, `wiki/drift_check.md`, `wiki/external_validity.md`, `wiki/fragility.md`, `wiki/innovation.md`, `wiki/local_optimisation.md`, `wiki/method_mapping.md`, `wiki/observation.md`, `wiki/proceed.md`, `wiki/programme.md`, `wiki/progress.md`, `wiki/state.md`, `wiki/stop.md`, `wiki/value.md`, `wiki/visibility_control_tension.md`, `wiki/log.md`
- Summary: Added a mandatory plain-language guardrail (sentence-length guidance, concrete verbs, plain rewrite pattern) and expanded lint rules to flag dense phrasing and require concrete action cues. Rewrote dense sentences across core wiki pages to reduce abstraction and improve decision-maker readability while preserving concept links and meaning. Re-ran link validation with `ALL_LINKS_OK`.
- Follow-ups: Run scheduled lint to catch any future long-sentence regressions during ingest.

## [2026-04-21] lint | strict plain-language micro-polish pass
- Scope: Ran strict readability lint and applied targeted micro-polish on highest-density phrasing.
- Files changed: `wiki/align_context.md`, `wiki/alignment.md`, `wiki/judgement.md`, `wiki/reversibility.md`, `wiki/signals_and_noise.md`, `wiki/value.md`, `wiki/log.md`
- Summary: Applied plain-language rewrites to abstract phrasing and added clearer action cues in top flagged lines. Re-ran strict lint and link validation (`ALL_LINKS_OK`). Readability improved; remaining low-score items are mostly due to heuristic action-verb detection rather than dense sentence length.
- Follow-ups: Consider a section-level action cue line in remaining conceptual pages to satisfy strict action-verb lint heuristics.
