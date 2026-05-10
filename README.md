# Causal Explanation Protocol

**Language:** [English](SKILL.md) | [简体中文](zh-CN/README.md)

A structured protocol for rigorous causal explanation. Classify first, then explain. Audit the driving force, then build the chain.

## What It Does

When explaining *why* something happens, it's easy to fall into circular reasoning, false analogies, or pseudo-root-causes. This protocol provides:

- **Pre-flight checks** — pitfall identification + driving force audit, executed before any explanation begins
- **A 4-mode decision tree** — classifies every phenomenon into one of four causal structures before building the explanation
- **Per-mode templates** — each mode has a specific explanatory form, starting-cause definition, and analogy requirement
- **Empirically tested** — built via TDD: baseline agents were tested without the skill, failures were documented, and the protocol was written to address those specific failures

## The Four Modes

| Mode | Applies to | Core operation |
|------|-----------|----------------|
| **A: Necessity Transmission** | Passive physical/engineering systems | Build unidirectional, unbranched chain from an independent conservation law |
| **B: Steady-State Equilibrium** | Negative-feedback systems, rule-locked games | Package the cycle as a steady-state module (don't unpack it) |
| **C: Path-Dependent Evolution** | Historical lock-in, sensitive to initial conditions | Separate contingency (don't explain "why B was chosen") from necessity (explain "why lock-in is inevitable") |
| **D: Emergence & Self-Organization** | Many individuals following simple rules | Enforce micro→macro causal unidirectionality |

## Usage

This protocol is implemented as a Claude Code skill. See [SKILL.md](SKILL.md) for the full reference.

To install:

```bash
# Copy to your Claude Code skills directory
cp SKILL.md ~/.claude/skills/causal-explanation-protocol/SKILL.md
```

Or use the [Chinese edition](zh-CN/SKILL.md) if your working language is Chinese.

## License

MIT
