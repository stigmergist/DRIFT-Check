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

## [2026-04-21] maintain | add visual explanation rules and pilot diagrams
- Scope: Added mandatory diagram guidance to instructions and embedded Mermaid diagrams in pages where structure benefits from visualisation.
- Files changed: `.github/copilot-instructions.md`, `wiki/capability_stack.md`, `wiki/context.md`, `wiki/fragility.md`, `wiki/decision_thresholds.md`, `wiki/log.md`
- Summary: Added a required "Visual explanations" section in instructions (when to diagram, Mermaid-first rule, interpretation line requirement, and lint checks for missing visuals). Added pilot diagrams for layered dependencies (`capability_stack.md`), context-state decision flow (`context.md`), failure propagation (`fragility.md`), and reversibility/absorption threshold mapping (`decision_thresholds.md`). Each diagram includes a plain-language interpretation line.
- Follow-ups: Extend diagrams to additional dependency-heavy pages during future refresh cycles.

## [2026-04-21] maintain | full diagram rollout on core structural pages
- Scope: Added diagrams to all remaining high-value pages identified for visual support.
- Files changed: `wiki/state.md`, `wiki/misfit.md`, `wiki/value.md`, `wiki/probe.md`, `wiki/reversibility.md`, `wiki/absorption_capacity.md`, `wiki/alignment.md`, `wiki/proceed.md`, `wiki/align_context.md`, `wiki/stop.md`, `wiki/log.md`
- Summary: Added Mermaid diagrams plus plain-language interpretation lines to all requested pages. Coverage includes state observation loop, action-state fit map, value/progress split, probe cycle, reversibility classes, absorption response, verbal-vs-behavioural alignment, and context transition maps for Proceed/Align/Stop. Verified `ALL_LINKS_OK` after edits.
- Follow-ups: Consider adding diagrams to `programme.md` and `external_validity.md` in next pass.

## [2026-04-21] ingest | ingest all new background documents
- Scope: Ingested all pending background sources and integrated new atomic concepts into the wiki graph.
- Files changed: `wiki/incentive_conflict.md` (new), `wiki/value_drift.md` (new), `wiki/alignment.md`, `wiki/align_context.md`, `wiki/external_validity.md`, `wiki/value.md`, `wiki/stop.md`, `wiki/programme.md`, `wiki/observation.md`, `wiki/index.md`, `wiki/_concepts_vocabulary.md`, `wiki/sources.md`, `wiki/log.md`
- Summary: Completed ingest for `background/incentive-vs-alignment.md`, `background/external_validity_and_value_drift.md`, and `background/aphorisms.md`. Added two new atomic concept pages (`incentive_conflict`, `value_drift`), strengthened links across alignment/value/stop/programme pages, and incorporated practitioner posture cues from aphorisms into observation and programme language.
- Follow-ups: Run lint for backlink density and readability on the two new concept pages; consider adding diagrams to `programme.md` and `external_validity.md`.

## [2026-04-21] refresh index | rebuild intro and entry points
- Scope: Rebuilt index intro and entry-point guidance to match updated index quality instructions.
- Files changed: `wiki/index.md`, `wiki/log.md`
- Summary: Updated opening section to use a single-sentence DRIFT description followed by a concise 2–4 sentence purpose explanation in decision-maker language. Rewrote start-here entry points around observable situations (recurring issues, commit/pause uncertainty, fragmented execution) and aligned links to core navigation pages.
- Follow-ups: Keep entry-point wording synced with future changes to top-level concept framing.

## [2026-04-21] maintain | integrate ingest coverage gate with linked idea group detection
- Scope: Strengthened wiki operating instructions to prevent missed grouped concepts during ingest.
- Files changed: `.github/copilot-instructions.md`, `wiki/log.md`
- Summary: Added a mandatory Source Concept Inventory step, explicit linked idea group detection for groups of 2, 3, 4, 5, and 6, and a completion gate requiring mapped or intentionally excluded groups. Expanded lint rules to verify section-level source coverage and grouped-set representation in wiki pages. Extended source registry schema to include concept coverage status, unmapped concepts, and last gap scan date.
- Follow-ups: Apply the new source registry fields during the next `ingest all pending` or `show source coverage` operation.

## [2026-04-21] ingest | close grouped quality concept gaps from DRIFT_CHECK_THINKING
- Scope: Added missing solution-quality grouped concepts and completed control-file integration under the new grouped-set ingest rules.
- Files changed: `wiki/solution_quality.md`, `wiki/quality_mismatch_signals.md`, `wiki/drift_check.md`, `wiki/proceed.md`, `wiki/probe.md`, `wiki/misfit.md`, `wiki/index.md`, `wiki/_concepts_vocabulary.md`, `wiki/sources.md`, `wiki/log.md`
- Summary: Created focused pages for the grouped quality set (Desirable, Feasible, Viable and Usable, Valuable, Sustainable), linked them into context/action pages, and updated vocabulary and source coverage metadata so the set is explicit, discoverable, and lintable.
- Follow-ups: Run strict lint for grouped-set coverage across all ingested sources and add any remaining cross-link clusters where grouped concepts are still fragmented.

## [2026-04-21] ingest | innovation spiral and structural limit grouped concepts
- Scope: Ingested new background source and surfaced additional grouped concepts not fully represented in the wiki.
- Files changed: `wiki/innovation_spiral.md` (new), `wiki/capability_ceiling.md` (new), `wiki/innovation.md`, `wiki/stop.md`, `wiki/optimise.md`, `wiki/external_validity.md`, `wiki/index.md`, `wiki/_concepts_vocabulary.md`, `wiki/sources.md`, `wiki/log.md`
- Summary: Added a first-class innovation spiral page covering grouped quality loops (F/V/D and U/V/S), stage-dependent NO/STOP value, and commitment boundary logic. Added capability ceiling as a structural-limit concept for diminishing-return optimisation patterns. Integrated both concepts across core pages and updated source registry mappings, including the new `background/innovation-spiral.md` source.
- Follow-ups: Run full grouped-set lint across all sources and assess whether any additional pair/triad clusters still need dedicated pages.

## [2026-04-21] gap check | DRIFT_CHECK_THINKING coverage scan
- Scope: Compared `DRIFT_CHECK_THINKING.md` against current wiki pages for concept, explanation depth, grouped-set coverage, and navigation links.
- Files changed: `wiki/sources.md`, `wiki/log.md`
- Summary: Core DRIFT decision concepts remain covered, but operator-facing concepts are partial or missing as first-class wiki knowledge: interaction boundary, graduated visibility, parallelism, investment-vs-fit, and speed-dominant exceptions. Opportunity register created with named gaps, evidence, and question prompts.
- Follow-ups: If approved, create focused pages and cross-link cluster for the five missing concepts, then refresh index and vocabulary.

## [2026-04-21] ingest | speed-dominant exception handling
- Scope: Ingested new background source for speed-dominant contexts and integrated exception-handling links across core decision pages.
- Files changed: `wiki/speed_dominant_contexts.md` (new), `wiki/drift_check.md`, `wiki/judgement.md`, `wiki/decision_thresholds.md`, `wiki/index.md`, `wiki/_concepts_vocabulary.md`, `wiki/sources.md`, `wiki/log.md`
- Summary: Added a first-class page for speed-dominant contexts (delay-harms-success conditions), including structural signals, relaxed-vs-mandatory checks, misuse failure modes, and guardrails. Linked the concept into DRIFT Check, Judgement, and Decision Thresholds to prevent over-cautious misapplication.
- Follow-ups: Continue gap closure for remaining DRIFT_CHECK_THINKING concepts (`interaction boundary`, `graduated visibility`, `parallelism`, `investment-vs-fit`).

## [2026-04-21] ingest | parallelism and investment-fit controls
- Scope: Ingested two background sources and integrated operator control concepts for change load and effort escalation.
- Files changed: `wiki/parallelism.md` (new), `wiki/investment_vs_fit.md` (new), `wiki/scaling.md`, `wiki/programme.md`, `wiki/drift_check.md`, `wiki/index.md`, `wiki/_concepts_vocabulary.md`, `wiki/sources.md`, `wiki/log.md`
- Summary: Added first-class pages for `parallelism` (change-load vs state interaction) and `investment_vs_fit` (value-plus-fit gating before increasing effort). Linked both concepts into scaling, programme, and DRIFT Check so activity-vs-outcome and load-vs-absorption risks are explicit in navigation.
- Follow-ups: Continue gap closure for remaining DRIFT_CHECK_THINKING concepts (`interaction boundary`, `graduated visibility`).

## [2026-04-21] ingest | interaction boundary, graduated visibility, and risk governance modes
- Scope: Ingested modified `DRIFT_CHECK_THINKING.md` and new `background/risk-types-and-audit.md` into dedicated concept pages and graph links.
- Files changed: `wiki/interaction_boundary.md` (new), `wiki/graduated_visibility.md` (new), `wiki/risk_types.md` (new), `wiki/control_learning.md` (new), `wiki/risk_governance.md` (new), `wiki/drift_check.md`, `wiki/judgement.md`, `wiki/signals_and_noise.md`, `wiki/index.md`, `wiki/_concepts_vocabulary.md`, `wiki/sources.md`, `wiki/log.md`
- Summary: Closed previously unmapped DRIFT_CHECK operator concepts by adding first-class pages for interaction boundary and graduated visibility. Ingested risk source into three atomic pages covering risk type distinction, control-vs-learning posture, and governance/audit adaptation. Updated index, vocabulary, and source registry to complete traceability.
- Follow-ups: Run `lint wiki` to verify backlink density and check for long-sentence regressions in newly added pages.

Source Concept Inventory (this ingest):
- `DRIFT_CHECK_THINKING.md` -> Interaction Boundary -> `interaction_boundary.md` (create): makes user judgement non-delegable when questions are asked.
- `DRIFT_CHECK_THINKING.md` -> Graduated Visibility -> `graduated_visibility.md` (create): calibrates model explicitness to user clarity.
- `DRIFT_CHECK_THINKING.md` -> Control vs Learning checks -> `control_learning.md` (update/create mapping): avoids standardising before understanding.
- `background/risk-types-and-audit.md` -> Type 1 vs Type 2 distinction -> `risk_types.md` (create): foundational risk-behaviour split.
- `background/risk-types-and-audit.md` -> Posture and treatment intent -> `control_learning.md` (create): same tools, different intent by risk type.
- `background/risk-types-and-audit.md` -> ERM, audit, committee, KRI adaptation -> `risk_governance.md` (create): governance mode must match uncertainty.

Linked Idea Group Mapping (this ingest):
- Size 2 pair: Type 1 vs Type 2 -> `risk_types.md`.
- Size 2 pair: Control vs Learning posture -> `control_learning.md`.
- Size 3 triad: Low/Medium/High clarity visibility levels -> `graduated_visibility.md`.
- Size 4 set: Reduce/Limit/Observe/Accept treatments -> `control_learning.md`.
- Size 5 set: Data/Cyber/AI/Operations/Third-party mixed domains -> `risk_types.md`.
- Size 6 set: Cause-Effect/Behaviour/Objective/Success/Failure/Progress comparison -> `risk_types.md`.

## [2026-04-21] lint | structural and readability pass after risk-ingest update
- Scope: Audited all wiki content pages for broken links, orphan pages, see-also link density, terminology contradictions, and readability density.
- Files changed: `wiki/log.md`
- Summary: Structural graph checks passed (`BROKEN_LINKS=0`, `ORPHANS=0`, `WEAK_SEE_ALSO=0`) across 48 content pages with 481 wiki-local concept links. Terminology check passed: no DRIFT-as-framework regressions in content pages. Source-coverage consistency held for `DRIFT_CHECK_THINKING.md` and `background/risk-types-and-audit.md` with grouped-set mappings present in `wiki/sources.md` and ingest log. Readability heuristic still flags dense prose in several legacy pages; newly ingested risk pages are within expected plain-language range.
- Follow-ups: Run a targeted readability rewrite pass on the highest-density legacy pages (`capability_stack.md`, `capability.md`, `absorption_capacity.md`, `drift_check.md`) using the >24-word-line heuristic as triage.

## [2026-04-21] lint | cross-link term scan on new risk documents
- Scope: Scanned newly added risk pages for missing inline term links (requested: Type 1 / Type 2 risk terms and related signal language).
- Files changed: `wiki/risk_governance.md`, `wiki/risk_types.md`, `wiki/control_learning.md`, `wiki/log.md`
- Summary: Added missing inline cross-links for `Type 1` and `Type 2` references, connected `Known signals` and `Discovery signals` to `signals_and_noise.md`, and linked control/learning posture language to `risk_types.md` plus action anchors (`stabilise`, `probe`).
- Follow-ups: Consider dedicated pages for `systemic risk`, `KRI split`, and `Type 1 vs Type 2 audit modes` if these terms need to become reusable entry points beyond current risk pages.

## [2026-04-21] ingest | add ERM concept page and links
- Scope: Added a first-class ERM term page and integrated it into risk-governance navigation.
- Files changed: `wiki/erm.md` (new), `wiki/risk_governance.md`, `wiki/index.md`, `wiki/_concepts_vocabulary.md`, `wiki/sources.md`, `wiki/log.md`
- Summary: Created `erm.md` to define Enterprise Risk Management in DRIFT language, including where ERM is strong and where it can create false precision in shifting risk. Added links from `risk_governance.md`, indexed the page, registered the concept in vocabulary, and updated source coverage mapping.
- Follow-ups: Optionally create dedicated pages for `systemic risk` and `KRI split` to complete the risk-governance concept cluster.

## [2026-04-21] lint | full wiki structural and readability check
- Scope: Ran a full lint scan across wiki content pages after ERM integration.
- Files changed: `wiki/log.md`
- Summary: Structural checks passed across 49 content pages and 502 wiki-local links (`BROKEN=0`, `ORPHANS=0`, `WEAK_SEE_ALSO=0`). Terminology regression check passed (`decision framework` references absent from content pages). Density checks show 9 pages with high `See also` counts (>8 links), and readability heuristic flagged 158 long prose lines (>24 words) concentrated in older legacy pages.
- Follow-ups: Consider a targeted readability pass for highest-density pages (`capability.md`, `capability_stack.md`, `absorption_capacity.md`, `drift_check.md`) and optional see-also pruning where navigation feels noisy.

## [2026-04-21] maintain | see-also pruning and top-20 readability rewrites
- Scope: Applied the two requested improvements: (1) reduce over-dense `See also` sections and (2) rewrite top 20 longest flagged prose lines.
- Files changed: `wiki/absorption_capacity.md`, `wiki/agency.md`, `wiki/align_context.md`, `wiki/alignment.md`, `wiki/capability.md`, `wiki/context.md`, `wiki/decision_thresholds.md`, `wiki/drift_check.md`, `wiki/judgement.md`, `wiki/misfit.md`, `wiki/optimise.md`, `wiki/proceed.md`, `wiki/programme.md`, `wiki/log.md`
- Summary: Pruned all pages above the 8-link threshold to within target range. Rewrote the top 20 flagged long prose lines (from `absorption_capacity`, `agency`, `align_context`, `alignment`, `capability`) into shorter plain-language sentences while preserving meaning and links.
- Follow-ups: Re-run full readability pass later for remaining long-line clusters, especially `capability_stack.md` and adjacent foundational pages.

Metrics delta:
- `HIGH_SEE_ALSO`: 9 -> 0
- `LONG_PROSE_LINES`: 158 -> 138
