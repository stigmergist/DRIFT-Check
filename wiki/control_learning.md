# Control and Learning

Control and learning are both valid risk postures, but they solve different problems.

Control posture aims to reduce variation where behaviour is already understood ([Type 1 risk](risk_types.md)). Learning posture aims to expose variation where behaviour is not yet understood ([Type 2 risk](risk_types.md)).

## The core tension

Control makes systems more consistent.

Learning makes differences visible.

If you apply control too early, you can hide useful signals. If you apply learning too late, you can tolerate instability that should already be under control.

## Same treatments, different intent

The tools can look identical, but intent changes by context.

Reduce:
- control posture: prevent known failures
- learning posture: often premature before behaviour is understood

Limit:
- control posture: fallback containment
- learning posture: primary move to keep experiments safe

Observe:
- control posture: confirm controls are working
- learning posture: discover behaviour and interaction effects

Accept:
- control posture: formal risk acceptance
- learning posture: temporary acceptance while reducing uncertainty

## Practical sequence for shifting risk

When risk is unclear, use:

Contain -> Observe -> Learn -> Then control

In plain terms: stop spread first, then learn, then standardise.

## Practical test

Ask: does improvement come from consistency, or from understanding difference?

If consistency helps, bias to control and [stabilise](stabilise.md).

If difference helps, bias to learning and [probe](probe.md).

See also: [risk_types.md](risk_types.md), [risk_governance.md](risk_governance.md), [probe.md](probe.md), [stabilise.md](stabilise.md), [misfit.md](misfit.md), [signals_and_noise.md](signals_and_noise.md)
