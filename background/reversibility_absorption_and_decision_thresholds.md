# Reversibility, Absorption, and Decision Thresholds

## Why this document exists
Decisions are often delayed or rushed without a clear link to their risk profile. This document clarifies how reversibility and system absorption capacity should shape when and how decisions are made.

Better understanding improves:
- Timing of action vs delay
- Level of precision required before acting
- Risk taken on different classes of decisions

## Core claim
The less reversible a decision and the lower the system’s ability to absorb error, the higher the precision required before acting.  
Conversely, highly reversible decisions in high-absorption systems should be made quickly with lower precision.  
Most decision failures come from mismatching reversibility, absorption, and required certainty.

## What this is (and is not)
- Helps determine how much certainty is needed before acting.
- Helps distinguish decision types based on reversibility and system tolerance.
- Does not prescribe what decision to make.
- Does not replace judgement about value or strategy.
- Sits alongside risk, sequencing, and capability concepts.

## Key questions this document answers
1. How reversible is this decision?
2. How much error can the system absorb?
3. What happens if we are wrong?
4. How precise does this decision need to be before acting?
5. Are we delaying unnecessarily or acting too early?

## Observable signals
- Signal:
  - What to look for: Decisions repeatedly revisited or delayed despite low impact of being wrong
  - Why it matters: Indicates reversible decisions treated as irreversible
  - Common misread: “We need more certainty”

- Signal:
  - What to look for: Early commitment to decisions that are hard to unwind
  - Why it matters: Indicates irreversible decisions treated as safe to experiment
  - Common misread: “We’ll adjust later”

- Signal:
  - What to look for: System stress or failure when small mistakes occur
  - Why it matters: Indicates low absorption capacity
  - Common misread: “This was just bad luck”

## Decision implications
- If these signals are present, likely action is: Reclassify the decision type before acting
- If confidence is low, safest next step is: Test reversibility and system tolerance with smaller moves
- If value is unclear, default is: Do not increase precision effort unnecessarily
- Risks of acting too early: Irreversible damage, systemic failure, loss of optionality
- Risks of acting too late: Missed opportunities, slow learning, unnecessary analysis cost

## Failure patterns
- Pattern:
  - Typical symptom: Slow decisions on low-risk changes
  - Underlying cause: Overestimating irreversibility
  - Consequence if ignored: Reduced speed, lost opportunities

- Pattern:
  - Typical symptom: Confident early commitment with limited fallback
  - Underlying cause: Overestimating system absorption
  - Consequence if ignored: Compounded failure, difficult recovery

## Practical tests
1. If we are wrong, how easily can we undo this?
2. What breaks if this fails — locally or system-wide?
3. Would we make the same decision knowing we cannot reverse it?

## Trade-offs and tensions
- Tension:
  - Over-correction risk: Treating everything as irreversible → paralysis
  - Under-correction risk: Treating everything as reversible → fragility
  - How to balance in practice: Match decision speed and precision to reversibility and absorption

## Example scenarios

### Scenario A
- Context: Internal tool change with limited external impact
- Observable signals: Low dependency, easy rollback, minimal cost of failure
- Interpretation: High reversibility, high absorption
- Action chosen: Fast decision with minimal analysis
- What happened: Rapid iteration and improvement

### Scenario B
- Context: Core system architecture change affecting multiple dependent systems
- Observable signals: High coupling, difficult rollback, cascading impact risk
- Interpretation: Low reversibility, low absorption
- Action chosen: Delayed decision with deeper validation
- What happened: Reduced risk of systemic failure

## Links to existing concepts
- Absorption capacity
- Scaling risk
- Action–state fit
- Probe vs Proceed decision contexts
- Capability stability