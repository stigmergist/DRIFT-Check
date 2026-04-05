# Layer 1 Context Matrix (v2)

Use this before choosing improvement action. Identify the current context from observable behaviour, then decide whether to move, align, probe, or stop.

## Context States

<table style="width:100%; table-layout:fixed; border-collapse:collapse;">
<colgroup><col style="width:14%"><col style="width:30%"><col style="width:30%"><col style="width:26%"></colgroup>
<thead>
<tr>
  <th style="padding:6px 13px; border:1px solid #d0d7de; background:#f6f8fa;">Context</th>
  <th style="padding:6px 13px; border:1px solid #d0d7de; background:#f6f8fa;">What you can observe</th>
  <th style="padding:6px 13px; border:1px solid #d0d7de; background:#f6f8fa;">What to do now</th>
  <th style="padding:6px 13px; border:1px solid #d0d7de; background:#f6f8fa;">⚠️ Risk if you act too soon</th>
</tr>
</thead>
<tbody>
<tr>
  <td bgcolor="#86efac" style="background:#86efac; padding:6px 13px; border:1px solid #d0d7de;"><strong>🟢 Proceed</strong></td>
  <td bgcolor="#bbf7d0" style="background:#bbf7d0; padding:6px 13px; border:1px solid #d0d7de;">Stakeholders describe the issue similarly; decisions stick; frontline signals and metrics point the same way; outcomes are repeatable across teams.</td>
  <td bgcolor="#bbf7d0" style="background:#bbf7d0; padding:6px 13px; border:1px solid #d0d7de;">Move to Layer 2 action-fit selection. Preserve shared understanding while scaling deliberately. Validate edge cases as you expand.</td>
  <td bgcolor="#bbf7d0" style="background:#bbf7d0; padding:6px 13px; border:1px solid #d0d7de;">Overconfidence. Early gains fail when local constraints were ignored.</td>
</tr>
<tr>
  <td bgcolor="#fde047" style="background:#fde047; padding:6px 13px; border:1px solid #d0d7de;"><strong>🟡 Align</strong></td>
  <td bgcolor="#fef9c3" style="background:#fef9c3; padding:6px 13px; border:1px solid #d0d7de;">Different groups frame different problems; decisions are reinterpreted in execution; side conversations and workarounds continue; progress depends on specific leaders.</td>
  <td bgcolor="#fef9c3" style="background:#fef9c3; padding:6px 13px; border:1px solid #d0d7de;">Build one shared problem statement, shared outcomes, and explicit trade-off rules. Surface incentive conflicts before standardising.</td>
  <td bgcolor="#fef9c3" style="background:#fef9c3; padding:6px 13px; border:1px solid #d0d7de;">Fragmented execution. Formal agreement with practical divergence.</td>
</tr>
<tr>
  <td bgcolor="#93c5fd" style="background:#93c5fd; padding:6px 13px; border:1px solid #d0d7de;"><strong>🔍 Probe</strong></td>
  <td bgcolor="#dbeafe" style="background:#dbeafe; padding:6px 13px; border:1px solid #d0d7de;">Same action gives different outcomes; evidence is mixed; experts disagree credibly; "it depends" is frequent; root cause shifts by viewpoint.</td>
  <td bgcolor="#dbeafe" style="background:#dbeafe; padding:6px 13px; border:1px solid #d0d7de;">Run bounded experiments with short feedback loops. Use action to learn cause-effect before broad rollout.</td>
  <td bgcolor="#dbeafe" style="background:#dbeafe; padding:6px 13px; border:1px solid #d0d7de;">Scaling the wrong intervention. False confidence gets amplified.</td>
</tr>
<tr>
  <td bgcolor="#fca5a5" style="background:#fca5a5; padding:6px 13px; border:1px solid #d0d7de;"><strong>⛔ Stop</strong></td>
  <td bgcolor="#fee2e2" style="background:#fee2e2; padding:6px 13px; border:1px solid #d0d7de;">Work persists by habit; ownership is unclear; outputs are weakly used; effort is high with little visible impact; value is hard to explain.</td>
  <td bgcolor="#fee2e2" style="background:#fee2e2; padding:6px 13px; border:1px solid #d0d7de;">Challenge whether to continue at all. Pause, reduce, or stop investment and redeploy capacity.</td>
  <td bgcolor="#fee2e2" style="background:#fee2e2; padding:6px 13px; border:1px solid #d0d7de;">Cost and attention drain. Activity replaces value.</td>
</tr>
</tbody>
</table>

## Fast interpretation rules

- 🟢 If understanding is shared and outcomes are consistent: **Proceed**.
- 🟡 If behaviour diverges after agreement: **Align** first.
- 🔍 If causality is unclear: **Probe** before scaling.
- ⛔ If value is unclear: **Stop** or reduce.

## Mixed-state handling

If two states are close, choose the safer path:

- 🟡🔍 `Align + Probe`: Align on the question, then probe.
- 🟢🔍 `Proceed + Probe`: Proceed only with bounded scaling.
- 🟡⛔ `Align + Stop`: Resolve value first, then decide whether to continue.
- 🔍⛔ `Probe + Stop`: Test whether value exists before further diagnosis.
- 🟢🟡 `Proceed + Align`: Reconfirm shared interpretation before scaling.

## Confidence prompt

Rate confidence as High, Medium, or Low based on signal quality.

If confidence is Low, default to probing or small-scale action rather than full rollout.

Do not treat this matrix as a diagnosis engine. Use it to sharpen judgement from observations.