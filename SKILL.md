---
name: causal-explanation-protocol
description: Use when explaining causal relationships, justifying why phenomena occur, or answering "why" questions about complex systems. Trigger especially when the system involves feedback loops, path dependence, emergence, equilibrium, or when circular reasoning and false analogies are risks. Also use when the user asks for root-cause analysis or critiques an existing explanation.
---

# Universal Causal Explanation Protocol

## Overview

This protocol does not teach causal reasoning — it provides a **pre-classification + structured template** that ensures the same pre-flight checks run before every explanation, the correct explanatory form is selected based on phenomenon type, and circular reasoning and false analogies are systematically avoided.

Core principle: **Classify first, then explain. Audit the driving force, then build the chain.**

## When to Use

- User asks "Why does X happen?"
- Explaining a phenomenon's causal mechanism to someone
- Reviewing or refuting an existing causal explanation
- System involves feedback loops, path dependence, emergence, or equilibrium
- Suspecting circular reasoning or pseudo-analogies in an explanation

## Pre-Flight Check Layer (Mandatory)

Must execute both steps before building any explanation. **Do not skip.**

### Step 1: Pitfall Identification

Scan the explanation space for the following fallacies:

| Fallacy Type | Detection Question | Red Flag |
|-------------|-------------------|----------|
| Circular reasoning | Does the "cause" need the "effect" to define itself? | Two variables define each other |
| False analogy | Is the analogy's causal structure isomorphic to the target system? | Superficial similarity, different mechanism |
| Pseudo root cause | Does the claimed "cause" itself have a deeper driving force? | "Why" can be asked indefinitely |

### Step 2: Driving Force Audit

For any claimed "cause," ask:

```
What is the driving force behind this "cause"?
  ├── Active intent (design, decision, purposeful action)
  ├── Passive constraint (physical law, conservation law, external boundary condition)
  └── Emergent regularity (statistical inevitability of large numbers of individuals)
```

Only when you reach one of the three categories above can you claim to have found the **root cause**. If you can still ask "why," you haven't reached the bottom.

## Mode Classification

After completing pre-flight checks, classify the phenomenon into one of four modes using the decision tree:

```
Does the system contain a negative-feedback loop (steady-state maintenance)?
  ├── Yes → Mode B: Constrained Steady-State Equilibrium Chain
  └── No  → Is the outcome strongly sensitive to initial conditions, with positive-feedback lock-in?
            ├── Yes → Mode C: Path-Dependent Evolution / Historical Chain
            └── No  → Does the macro pattern emerge from many individuals following simple rules?
                      ├── Yes → Mode D: Emergence & Self-Organization Chain
                      └── No  → Mode A: Necessity Transmission Chain
```

## Four Explanatory Modes

### Mode A: Necessity Transmission Chain

**Applies to**: Steady-state, passive, strongly-constrained, non-intentional systems (physics, engineering).

**Nature of starting cause**: Absolutely external, immutable physical boundary or conservation law.

**Explanatory form**:
```
Cause A (independent physical boundary / conservation law) → passively causes B → necessarily causes C
```

Hard requirements:
- Chain is unidirectional, unbranched, non-cyclic
- Each step must necessarily follow from the previous
- No form of circular reference allowed

**Analogy requirement**: Must use a system with an isomorphic physical mechanism (e.g., rowing paddle pushing water → wing pushing air), not superficial similarity.

---

### Mode B: Constrained Steady-State Equilibrium Chain

**Applies to**: Steady-state systems with negative feedback; games where agents have intent but are locked in by rules.

**Nature of starting cause**: A set of mutually constraining rules or forces that together define a stable attractor. At least one element must be exogenous (not determined by the system's internal state).

**Core operation — Package, don't unpack**:

❌ **Wrong approach** (unpacking the cycle):
> "Temperature drops → heater on → temperature rises → heater off → temperature drops → back to the start... each step is temporally one-directional so it's not circular."

This is logically defensible but wastes explanatory power. What the listener wants is not "why each step is reasonable" but "why the whole system necessarily stabilizes around a certain value."

✅ **Correct approach** (package as a steady-state module):
> "The system is jointly defined by two mutually constraining forces/rules, X and Y. X drives the system in one direction; Y's strength increases with the magnitude of deviation. Their intersection is the steady state Z. Whenever the system deviates from Z, Y's constraining force automatically strengthens to pull it back. Z is therefore the inevitable steady-state outcome."

**Explanatory form**:
```
Rule set {X, Y} defines steady state Z → mathematically/physically Z is the unique intersection → system necessarily fluctuates around Z
```

**Analogy requirement**: Must use a system with the same "conflict-in-equilibrium" structure (e.g., spring with hanging weight: gravity and elastic force contend, system automatically stabilizes at a certain length). Do not use a unidirectional chain analogy.

---

### Mode C: Path-Dependent Evolution / Historical Chain

**Applies to**: Forms/institutions that are the cumulative result of history, with sensitivity to initial conditions.

**Nature of starting cause**: A small difference at a bifurcation point + a positive-feedback amplification mechanism. Both parts are required.

**Critical boundary to maintain**:

| What to explain (necessity) | What NOT to explain (contingency) |
|---------------------------|----------------------------------|
| Once on a given trajectory, why it's hard to turn back and outcome C becomes inevitable | Why B was selected rather than A at the fork |

**Explanatory form**:
```
Bifurcation point: small difference / random fluctuation → B is selected (this is contingency; do not explain "why B")
Lock-in mechanism: B → triggers positive feedback M (scale effects / network effects / acquired investment) → possibility space rapidly narrows → necessarily leads to C
```

**Analogy requirement**: Must use a system with the same "bifurcation + lock-in" structure (e.g., a snowball rolling downhill: a tiny initial bump determines its final path). Do not use a system with only lock-in but no bifurcation.

---

### Mode D: Emergence & Self-Organization Chain

**Applies to**: Large numbers of simple individuals following simple rules, producing complex macro patterns.

**Nature of starting cause**: The bottom-level individual rules (algorithm). These rules are fixed and exogenous.

**Core constraint — causal arrow is irreversible**:
```
Micro rule R → countless parallel interactions → macro statistical regularity P
```
P cannot in turn explain R. Macro patterns are descriptive, not causal.

**Explanatory form**:
```
All individuals independently follow rule R → collective behavior mathematically/physically necessarily produces macro pattern P → no central coordination needed
```

**Violation check**: If the explanation contains "because the congestion wave exists, drivers brake" — a macro→micro causal arrow — it is circular reasoning. The correct statement is "each driver brakes because the car ahead braked; the collective set of these local decisions forms the congestion wave."

**Analogy requirement**: Must use a system that also emerges from parallel rules (e.g., sandpile avalanches, magnetic needles collectively pointing in one direction). Do not use systems with leaders or central coordination.

---

## Common Mistakes (from empirical testing)

| Mistake | Correct approach |
|---------|-----------------|
| Skipping pre-flight checks and jumping straight to explanation | Must execute pitfall identification + driving force audit first; cannot be skipped |
| Explaining without classifying | Must use the decision tree to determine the mode, then build the explanation using the corresponding template |
| Unpacking the cycle in Mode B instead of packaging it | Stop defending each step sequentially. Find the exogenous anchor + constraining relationship; package as a steady-state module |
| Trying to explain "why B instead of A" in Mode C | Explicitly declare this as contingency; explanatory power applies to "why lock-in" not "why selection" |
| Using macro patterns to explain micro behavior in Mode D | Check every causal arrow's direction; ensure micro→macro, never the reverse |
| Providing analogies without isomorphism check | Compare the causal structure (feedback type, driving force origin) of target and analogy, not surface features |

## Quick Reference

| Phenomenon | Mode | Starting cause form | Core operation |
|-----------|------|-------------------|----------------|
| No feedback, passive physical process | A: Necessity Transmission | Independent physical boundary / conservation law | Build unidirectional, unbranched chain |
| Negative feedback, steady-state maintenance | B: Steady-State Equilibrium | Mutually constraining rule set (with exogenous anchor) | Package cycle as steady-state module |
| Positive feedback, historical lock-in | C: Path-Dependent Evolution | Bifurcation difference + amplification mechanism | Separate contingency (don't explain) from necessity (explain) |
| Many individuals, simple rules | D: Emergence & Self-Organization | Bottom-level individual rules | Enforce micro→macro causal unidirectionality |

## Domain-Specific Enhancements (Optional)

### For Computing / Networking / Distributed Systems: Layered Causal Scoping

A unique risk in computer systems: the same observable symptom (e.g., "service is down") has a completely different causal structure depending on which abstraction layer you lock into. Using the wrong mode for a layer is a **category error**, not an explanation quality issue.

Before entering the decision tree, declare the analysis layer:

```
"This explanation is scoped to the [physical / kernel / protocol / application / business] layer,
and only discusses causal mechanisms internal to that layer, without cross-layer confusion of driving-force types."
```

**Why this is necessary**:

| Same symptom: "service unavailable" | Scoped layer | Corresponding mode |
|-------------------------------------|-------------|-------------------|
| Fiber cut | Physical | A: Necessity Transmission (signal loss → link down → route unreachable) |
| Network partition; CP system under CAP rejects writes | Protocol | B: Steady-State Equilibrium (consistency vs. availability constrain each other; Paxos/Raft maintains steady state with quorum) |
| Deadlock (two transactions each waiting for the other's lock) | Kernel / Application | B: Steady-State Equilibrium (circular lock-wait as "attractor"; never resolves without external intervention) |
| Retry storm (timeout → retry → more timeouts → more retries) | Application | D: Emergence & Self-Organization (each client independently follows retry rule; avalanche emerges) |

Entering the decision tree without declaring the layer → risk of using Mode D to explain a fiber cut, or Mode A to explain CAP split-brain. Both are wrong.

### For Highly Complex Phenomena: Mode Superposition (Strictly Guarded)

Rare phenomena span the boundary of two causal structures. In such cases, mode superposition is permitted, but **all of the following conditions must be met; none can be waived**:

```
1. Each mode explains exactly [one independent facet] of the phenomenon; no overlap.
   Example: Mode C explains "how lock-in occurred"; Mode B explains "why the locked-in equilibrium self-maintains."

2. The causal scope and temporal boundary of each mode must be explicitly declared.
   Example: "[Mode C covers 1870–1930: how the path was selected and locked in]
             [Mode B covers 1930–present: how the Nash equilibrium self-maintains post-lock-in]"

3. Under superposition, each mode's "starting cause" must be independently defined; no sharing.
   Violation: "Starting cause is both historical contingency and market equilibrium forces" ← not allowed.

4. If the two facets cannot be cleanly separated → fall back to the decision tree and pick the dominant mode.
   When in doubt, default to a single mode.
```

**If any of the above conditions are unmet, superposition is forbidden. When in doubt, superposition is forbidden.**
