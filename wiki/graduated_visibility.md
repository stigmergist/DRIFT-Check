# Graduated Visibility

Graduated visibility means adjusting how explicitly DRIFT language appears in a response based on user clarity.

When someone is stuck, the structure should be more visible. When someone is already reasoning well, the structure should fade into plain language. This keeps the tool useful without making every response feel like a framework lecture.

## Three visibility levels

Low clarity:
- make context versus action explicit
- use one or two labels to orient the user
- prioritise structure over detail

Medium clarity:
- reinforce what is already correct
- use labels only where they reduce confusion
- focus on the key tension

High clarity:
- avoid explicit model teaching
- focus on consequences and edge cases
- extend judgement instead of naming categories

## Escalation rule

If confusion persists, increase visibility gradually.

If the user starts using the language accurately, reduce visibility gradually.

In plain terms: show more model when clarity is low, and less model when clarity is high.

## Failure mode

Too much visibility creates over-labelling and slows decisions. Too little visibility leaves the user without enough structure to separate context from action.

See also: [drift_check.md](drift_check.md), [interaction_boundary.md](interaction_boundary.md), [judgement.md](judgement.md), [context.md](context.md), [misfit.md](misfit.md), [probe.md](probe.md)
