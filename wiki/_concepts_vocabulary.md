# DRIFT Concepts Vocabulary

This is the canonical list of key DRIFT concepts that should be cross-linked and highlighted in wiki pages. Update this file whenever new concepts are ingested; the Copilot instructions reference this list to drive linking and highlighting behavior.

## Core Decision-Making

- `context` — whether conditions are clear enough, aligned enough, and valuable enough to act now
- `proceed` — conditions are clear and aligned; action is sensible  
- `align_context` — shared understanding is weak; alignment work is needed before moving
- `probe` — cause and effect are unclear; testing is needed to understand the system
- `stop` — value is uncertain enough that continuing may increase waste
- `solution_quality` — checks action soundness through desirable, feasible, viable and interaction effects
- `quality_mismatch_signals` — observable signs that want/can/worth quality dimensions are out of balance
- `innovation_spiral` — repeated quality-test loops (D/F/V and U/V/S) that move from exploration to delivery
- `investment_vs_fit` — separates effort increase decisions from value and state-action fit evidence
- `capability` — reliable and efficient outcome production
- `misfit` — gap between observed system state and action being applied
- `observation` — anchor interpretation in what the system is actually doing
- `judgement` — choosing what matters and what to ignore
- `decision_thresholds` — confidence level required before committing to action, set by reversibility, absorption, and consequence
- `speed_dominant_contexts` — exception handling for contexts where delay reduces success probability

## Capability State and Action

- `state` — what the system is actually doing right now
- `stabilise` — restore control and reliability when outcomes are inconsistent
- `rationalise` — reduce unnecessary complexity once reliability exists
- `optimise` — improve performance and efficiency after reliability is established

## System Dynamics and Constraints

- `alignment` — consistent behaviour across the system, not meeting-room agreement
- `incentive_conflict` — execution divergence caused by metrics, incentives, or constraints rather than misunderstanding
- `uncertainty` — variable outcomes for the same action
- `complexity` — many different approaches to the same outcome
- `fragility` — small issues propagating into larger failures
- `signals_and_noise` — separating real patterns from distraction
- `absorption_capacity` — capacity to survive being wrong and still function
- `reversibility` — how recoverable a wrong decision or action is
- `scaling` — amplification of existing behaviour, good or bad
- `local_optimisation` — local gains that harm the wider system
- `parallelism` — safe change load relative to system state and absorption

## Foundational Relationships

- `agency` — what can actually be changed vs. what must be navigated as constraint
- `value` — impact, not activity; value exists when outputs are used for change
- `value_drift` — improving internal performance while external relevance or demand weakens
- `progress` — improvement in reliable, efficient outcome production
- `programme` — change as a structured, testable value hypothesis
- `visibility_control_tension` — what is visible is often what is least controllable; reliability is created where it cannot be seen

## Structural Concepts

- `capability_stack` — layered dependencies that produce value; each layer relies on stability below
- `external_validity` — whether the system is still worth being good at
- `innovation` — exploration under uncertainty; learning by doing
- `capability_ceiling` — structural limit where additional optimisation yields little system-level value

## Usage Guide

When writing or editing wiki pages:

1. **Link key concepts on first mention.** If you write a concept name from this list, link to its page.
2. **Bold canonical concepts at first mention in a new context.** Example: "This is why **misfit** emerges—applying the wrong action to the current state."
3. **In 'See also' sections, link every genuinely related concept.** Aim for 4–8 links per page; every link should be justified by the page content.
4. **Update this file whenever new concept pages are created.** Add the concept name, category, and one-line description.

## Metadata

- Last updated: 2026-04-21
- Total concepts: 43
- Related: `wiki/index.md` (categorical index), `.github/copilot-instructions.md` (ingest schema)
