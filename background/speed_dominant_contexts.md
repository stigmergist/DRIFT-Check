# Background: Speed-Dominant Exception Handling

## Overview

DRIFT is designed to improve judgement by slowing action until context and capability are sufficiently understood. This works well in most organisational situations, where premature action leads to wasted effort, misalignment, or instability.

However, there is a distinct class of situations where **delay itself reduces the probability of success**. These are **speed-dominant (power-law) contexts**, and they require an explicit exception.

Without this exception, DRIFT can be over-applied — leading to unnecessary caution, delayed decisions, and missed opportunities.

This document defines:

* how to recognise speed-dominant contexts
* how DRIFT application should adjust
* what risks emerge when the exception is overused

---

## Core Idea

The distinction is not simply “uncertain vs unclear”.

It is:

> **Does waiting improve the outcome — or reduce the chance of success?**

This creates two different modes:

| Context type       | Effect of waiting                           | Appropriate behaviour                 |
| ------------------ | ------------------------------------------- | ------------------------------------- |
| Normal uncertainty | Improves understanding and decision quality | Probe, align, stabilise before acting |
| Speed-dominant     | Reduces ability to compete or succeed       | Act earlier with partial fit          |

The key interaction is between:

* **uncertainty (lack of clarity)**
* **time sensitivity (cost of delay)**

---

## Signals of a Speed-Dominant Context

Speed-dominant contexts are not defined by urgency alone. They show **structural signals** where speed directly creates advantage.

Look for combinations of:

* **Position matters early**

  * First movers gain durable advantage (distribution, share, access)
  * Late entrants struggle to catch up regardless of quality

* **Scale changes behaviour**

  * Learning, performance, or value only emerges at scale
  * Small experiments are not representative

* **Power-law outcomes**

  * A small number of winners capture most value
  * Being “good” is insufficient without being early or large

* **Time-bound opportunity**

  * Windows are closing (market formation, funding runway, regulatory shift)
  * Delay reduces viability, not just speed

* **High tolerance for inefficiency**

  * The system can absorb instability in exchange for growth
  * Imperfection is accepted if it enables movement

---

## Signals of Normal Uncertainty (Non-Speed Context)

In contrast, most organisational situations show:

* Waiting **clarifies cause and effect**
* Small-scale tests are **representative**
* Outcomes are **recoverable if delayed**
* Value can be assessed **before scaling**
* Missteps are **correctable without losing position**

Here, DRIFT should be applied normally.

---

## DRIFT Adjustment in Speed-Dominant Contexts

The goal is not to bypass DRIFT, but to **shift what is enforced vs what is relaxed**.

### Elements to Relax

These checks may be intentionally incomplete:

* **Alignment**

  * Accept directional coherence rather than full agreement
  * Avoid extended alignment cycles that delay movement

* **Stability**

  * Tolerate known instability if it enables scale or position
  * Accept reactive behaviour temporarily

* **Small-scale probing**

  * Replace controlled experiments with **learning at scale**
  * Use real-world exposure rather than isolated testing

---

### Elements to Keep Mandatory

These remain critical even under speed pressure:

* **Value (Stop check)**

  * Still test whether the opportunity is worth pursuing
  * Avoid scaling activity with unclear or weak value

* **Irreversibility awareness**

  * Identify decisions that cannot be undone
  * Protect against irreversible downside

* **Basic viability**

  * Ensure the system can function at a minimal level
  * Avoid scaling something fundamentally unusable

---

### Reframed Question

Instead of:

> “Are we clear enough to act?”

Use:

> “Does waiting improve our chance of success — or reduce it?”

---

## Failure Modes When Overused

When the speed exception is applied too broadly, it creates a different class of failure.

### 1. False race conditions

* Situations are treated as urgent when they are not
* “Speed” becomes a default justification for action

**Consequence:** unnecessary risk-taking without strategic benefit

---

### 2. Fragility accumulation

* Instability is tolerated without a path to stabilisation
* Technical, operational, or organisational debt compounds

**Consequence:** system becomes harder to control over time

---

### 3. Loss of recovery ability

* Continuous movement prevents consolidation
* The system never returns to stabilise or rationalise

**Consequence:** inability to transition from growth to sustainable operation

---

### 4. Misreading pressure as necessity

* Internal urgency (targets, expectations) is mistaken for external necessity
* Behaviour optimises for pace, not advantage

**Consequence:** effort increases without improving competitive position

---

## Diagnostic Tension

The most important distinction to maintain:

> **Are we early in a real race — or reacting to pressure to move?**

These produce similar behaviours (speed, reduced checks), but differ in outcome:

| Situation                   | Outcome                                          |
| --------------------------- | ------------------------------------------------ |
| Real speed-dominant context | Faster movement increases chance of success      |
| Misapplied speed exception  | Faster movement increases risk without advantage |

---

## Practical Guardrail

Before relaxing DRIFT checks, test:

* Does delay measurably reduce our ability to compete?
* Does scale meaningfully change learning or outcomes?
* Are we trading control for advantage — or just losing control?

If these are unclear, default back to normal DRIFT application.

---

## Implication for DRIFT Coverage

This represents a **missing grouped-set** in the current system:

* DRIFT_CHECK → emphasises fit before action
* Decision thresholds → emphasise clarity before commitment
* Judgement → emphasises grounded understanding

None explicitly cover:

> **When reduced fit is acceptable because speed is the advantage**

This creates a systematic bias toward caution.

---

## Summary

Speed-dominant contexts are defined by a simple but critical shift:

> **In most situations, better understanding improves outcomes.**
> **In these situations, delay reduces the chance of success.**

DRIFT should not be removed — but **selectively relaxed**.

The risk is not just moving too fast.

It is **moving fast when it doesn’t actually matter**.
