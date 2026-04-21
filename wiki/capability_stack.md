# Capability Stack

A capability stack is a layered view of how an organisation creates value. Each layer depends on the layers beneath it.

The top of the stack is where value is visible to users and customers: service quality, product usefulness, delivery reliability, trust. But those visible outcomes are produced by lower layers: operating practices, enabling systems, governance decisions, data quality, and the behaviour of teams under constraints. When the lower layers are weak, the top layer can still look good for a while, usually through extra effort and local workarounds. Over time, that gap closes and the weakness becomes visible as delay, inconsistency, fragility, or cost.

Thinking in stacks prevents a common mistake: treating surface outcomes as self-contained. A delayed release is rarely only a release problem. A customer experience issue is rarely only a front-line issue. What shows up at the top is usually a reflection of conditions below.

## How value flows through a stack

Value flows bottom-to-top: lower layers create the possibility for what sits above them. A data platform enables execution capability. Execution capability enables coordination. Coordination enables delivery. Delivery enables customer outcomes.

But there is a critical asymmetry: each layer is constrained by the reliability of what it depends on. A capability cannot be more reliable than the capabilities beneath it. If it appears more stable, the system is using slack, workarounds, or extra effort to mask underlying problems.

When dependency is high and reliability is variable, that variability propagates upward and becomes amplified. An inconsistent data pipeline creates inconsistent execution, which creates inconsistent coordination outcomes, which creates inconsistent customer experience. What started as 10% variability in the base layer can become 50% variability in customer-facing delivery.

## The visibility-control paradox

Value is visible at the top of the stack. Cost, benefit, and impact are all measured at the top. But reliability — the ability to produce anything consistently — is created at the bottom.

This creates a dangerous pattern: organisations over-invest in visible layers while tolerating instability in foundational layers. They speed up the release pipeline while the underlying systems are still producing variable data. They train teams on customer empathy while the tools those teams use are unreliable. They set aggressive delivery targets while the platform supporting execution is fragile.

The result appears at the top: promised improvements do not hold, initiatives lose momentum, and costs climb. But the root cause is usually below — instability that was assumed to be "not my responsibility" or "good enough for now".

Without stack thinking, teams optimise locally. They improve what is directly in front of them and count it as success even when the wider system gets worse. This is how organisations get faster at producing things that are harder to integrate, easier to break, or less valuable to users. Stack thinking forces a broader question: did this intervention improve overall value flow, or just one local metric?

Stack thinking also changes sequencing. If a lower layer is unstable, improving an upper layer rarely lasts. The gain is borrowed from future effort. This is why DRIFT emphasises fit: interventions should match the state of each layer. Teams often need coordinated changes across multiple layers.

## Warning sign: local optimisation

A local improvement that degrades the wider system is not an improvement. Common examples are tighter controls, unstable automation, and aggressive efficiency work on brittle processes. In each case, the local result looks positive while the system gets worse.

## Capability stack and value

Value is realised at the top but created and constrained by what sits below. This means value work is never only customer-facing work. It also means internal capability investment is not overhead by default; it is often a direct condition for sustained external value.

See also: [capability.md](capability.md), [value.md](value.md), [progress.md](progress.md), [local_optimisation.md](local_optimisation.md), [fragility.md](fragility.md), [visibility_control_tension.md](visibility_control_tension.md), [scaling.md](scaling.md)
