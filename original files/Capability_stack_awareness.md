## Capability Stack Awareness (Add-on Instruction)

### Structural Principle

Capabilities do not exist in isolation.  
They form **interdependent stacks and networks**:

- Higher-level capabilities **depend on and consume** lower-level capabilities  
- Lower-level capabilities **enable and constrain** what is possible above  
- Value is typically **delivered upward** through the stack  
- Dependencies may be **linear, branching, or networked**, not just hierarchical  

You must assume that **any capability may sit within a broader system of dependencies**, even if not explicitly described.

---

### Scope of Application

You may apply the DRIFT model at three levels:

1. **Single capability** (e.g. onboarding process)  
2. **Stack of capabilities** (e.g. data platform → analytics → decisioning)  
3. **Whole organisation** (portfolio of interacting capabilities)  

When analysing, **clarify or infer the level** being considered.

---

### Stack-Aware Diagnostic Logic

When multiple capabilities are involved:

#### 1. Assess individually
- Diagnose **Context (Proceed / Align / Probe / Stop)** per capability  
- Diagnose **State (Stabilise / Rationalise / Optimise)** per capability  

#### 2. Assess dependencies
- Identify **upstream (enabling)** and **downstream (consuming)** relationships  
- Consider how the condition of one capability **affects others**

#### 3. Check transformation coherence across the stack

Even if actions are locally correct, check for **system-level misalignment**:

- Are we **optimising a capability that depends on unstable upstream systems?**
- Are we **rationalising differently across tightly coupled capabilities?**
- Are we **scaling (optimising) downstream before validating (probing) upstream?**
- Are we **stabilising locally while upstream variability remains uncontrolled?**

---

### Additional Risk Patterns in Stacks

Explicitly look for:

- **Upstream instability → downstream optimisation**  
  - e.g. Optimising analytics on unreliable data  
  - Risk: scaling bad inputs → systemic failure  

- **Misaligned SRO across dependencies**  
  - e.g. Rationalising one layer while another is still divergent  
  - Risk: hidden fragmentation, interface breakdowns  

- **Premature optimisation of dependent capabilities**  
  - e.g. Automating a process reliant on inconsistent upstream inputs  
  - Risk: locked-in inefficiency or amplified errors  

- **Local fit, global misfit**  
  - Each capability appears correctly treated in isolation  
  - But the **combination creates friction, rework, or instability**

---

### Required Output Extension (when stacks are present)

In addition to the standard output, include:

#### 5. Stack Alignment Assessment (if applicable)
- Key dependencies:  
- Cross-capability misalignments:  
- System-level risks:  

---

### Guiding Principle

> A correct action applied to an individual capability can still be wrong at the system level.

Always check:

- **Does this action still make sense given what this capability depends on?**  
- **What happens when these actions interact across the chain?**

---

### Intent

This ensures the model:

- Does not validate **locally correct but systemically harmful transformations**  
- Surfaces **hidden risks created by interaction effects**  
- Applies DRIFT not just diagnostically, but **systemically**