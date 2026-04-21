# Risk Types

Not all risk behaves the same way.

Some risks are stable enough for [control](control_learning.md). Others shift as people, systems, and environments interact and need [learning](control_learning.md). DRIFT separates these into **Type 1** and **Type 2** so teams do not apply one operating style to everything.

## Type 1 and Type 2

Type 1 risk:
- cause and effect are clear enough to control
- consistency is the right objective
- progress looks like fewer repeat failures

Type 2 risk:
- cause and effect are partial or moving
- understanding is the right objective
- progress looks like fewer surprises over time

In plain terms: Type 1 needs stronger control, Type 2 needs better learning.

## Mixed domains are normal

Most real domains contain both types at once.

Examples:
- data: controls can be stable while usage patterns keep changing
- cyber: known controls coexist with adaptive adversaries
- AI: pipelines can be controlled while behaviour drifts in use

This is why single-score risk views often miss what matters at the edge.

## Systemic risk shift

Systemic risk often appears when components look controlled, but interactions behave unpredictably.

The unit of risk is no longer the component. It is propagation across connected parts, which is why [fragility](fragility.md) and [signals](signals_and_noise.md) must be monitored together.

See also: [control_learning.md](control_learning.md), [risk_governance.md](risk_governance.md), [fragility.md](fragility.md), [signals_and_noise.md](signals_and_noise.md), [programme.md](programme.md), [judgement.md](judgement.md)
