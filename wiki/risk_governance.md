# Risk Governance

Risk governance fails when it treats uncertain risk as if it were already understood.

[Type 1 and Type 2 risk](risk_types.md) need different governance modes. Type 1 risk supports structured control and assurance. Type 2 risk needs adaptive oversight that tracks learning and surprise, not just closure status.

## ERM fit and limit

[ERM](erm.md) is strong for stable, repeatable risk.

It struggles when teams are forced to score uncertainty too early. That can create confidence theatre: neat dashboards with weak understanding.

Use ERM as a container for uncertain domains:
- allow provisional definitions
- keep narrative evidence alongside scores
- update scope as signals change

## Audit mode must match risk mode

Type 1 audit:
- objective: assurance of controls
- method: control tests and sampling
- output: confidence that expected controls hold

Type 2 audit:
- objective: expose reality versus assumptions
- method: case tracing, scenario testing, interaction review
- output: insight on what is changing and what could propagate

In plain terms: you cannot prove control where the system is still being discovered.

## Committee question shift

For stable risk, ask: are we in control?

For shifting risk, ask: what are we missing?

Both questions matter, but in different proportions by risk type.

## Indicator split

[Known signals](signals_and_noise.md):
- track expected failure patterns
- useful for stable risk monitoring

[Discovery signals](signals_and_noise.md):
- track anomalies, novelty, and behavioural shifts
- useful for early warning in uncertain domains

## Capability framing

Use two capability terms to avoid confusion:
- reliability for control strength
- adaptiveness for learning strength

Combined aim: reliable where understood, adaptive where not.

See also: [erm.md](erm.md), [risk_types.md](risk_types.md), [control_learning.md](control_learning.md), [judgement.md](judgement.md), [signals_and_noise.md](signals_and_noise.md), [programme.md](programme.md), [fragility.md](fragility.md)
