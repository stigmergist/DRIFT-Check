# Method Mapping

DRIFT is method-agnostic. It does not replace existing frameworks. It helps decide whether and how to apply them based on observed context and capability state.

This matters because many frameworks are strong at structure but weak at live fit checking. Teams can execute method steps correctly while still applying them to the wrong situation.

A practical pattern is to run both views in parallel. Use your existing framework for structure. Then run DRIFT to test context readiness, action-type fit, and value clarity. When they disagree, that disagreement is often the most useful signal.

Common risk patterns from the source comparison include scaling routines in misaligned environments, optimising unstable capabilities, and treating metric movement as proof of progress. Understanding [scaling.md](scaling.md) and [misfit.md](misfit.md) helps avoid these traps.

See also: [drift_check.md](drift_check.md), [context.md](context.md), [capability.md](capability.md), [progress.md](progress.md), [local_optimisation.md](local_optimisation.md), [scaling.md](scaling.md), [misfit.md](misfit.md)