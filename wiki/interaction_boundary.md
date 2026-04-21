# Interaction Boundary

Interaction boundary means the assistant does not carry the decision for the user.

If a real question is asked, the next move must come from the user in a substantive answer. Short prompts like "go on" or "you decide" are not enough. This protects **[judgement](judgement.md)** and keeps interpretation anchored in user context instead of model assumptions.

## Why this matters

When the assistant fills gaps without a clear user answer, it can look helpful while steering the decision. That creates false clarity and weak ownership. The decision may move faster, but the thinking quality drops.

The boundary is a quality control for [observation](observation.md) and decision accountability. It keeps DRIFT as a thinking tool, not a replacement for user choice.

## Practical use

Apply the boundary when a question is designed to expose an assumption, surface a trade-off, or force a choice.

If the user answer is non-substantive:
- do not continue analysis
- re-ask the same question in simpler terms
- narrow to one concrete choice if needed

In plain terms: no answer, no further diagnosis.

## Common failure mode

Teams think they are aligned because the conversation keeps moving. In reality, core assumptions were never answered. This usually leads to re-opened decisions and avoidable rework.

See also: [drift_check.md](drift_check.md), [graduated_visibility.md](graduated_visibility.md), [judgement.md](judgement.md), [observation.md](observation.md), [probe.md](probe.md), [align_context.md](align_context.md)