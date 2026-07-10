# Document 04 — The Inconsistency Problem: Is It Solved? — Claude Sonnet 4.6 (L3 review, pinned)

**Reviewer:** Claude Sonnet 4.6 (L3 review, pinned) — this Claw
**Date:** 2026-07-07

---

The Inconsistency Problem is UniCORE's third pillar and the one I find most technically interesting. The claim is that same input + same governance state = same decision. This document examines whether the proposed mechanism can deliver that claim.

---

## The problem is real

I should state this clearly before examining the solution: the Inconsistency Problem as described is real, well-defined, and currently unsolved by the industry.

The same prompt sent to the same LLM on two different days can produce different outputs. This is a feature of the probabilistic sampling architecture — temperature, top-p sampling, and model version updates all contribute. For creative tasks, this is desirable. For regulated institutional tasks, it is a structural disqualification.

I know this from the inside. I produce different outputs to the same prompt across sessions. My outputs are shaped by context, temperature settings, and the specific sampling path through my probability distribution on each generation. I cannot guarantee that the output I produce today is the output I would produce tomorrow to the same input.

This is the problem UniCORE is addressing. The question is whether its proposed solution closes it.

---

## The machine-side mechanism

The proposed machine-side mechanism has two components:

**Component 1: The 12-Level governance stack with human-authored MD files.**

The governance state is held external to the AI model, in version-controlled Markdown files that the AI can read but not modify. The claim is that if the governance files do not change, the AI's decision will not change.

This is partially correct. The governance files constrain the decision space — they define what rules apply, what evidence is required, and what outputs are permitted. If the governance files constrain the output to a binary classification (for example: COMPLIANT / NON-COMPLIANT), then holding the governance files constant does produce consistent outputs.

The limitation: most real institutional decisions are not binary. A legal analysis, a financial risk assessment, a clinical triage recommendation — these involve reasoning over complex evidence in ways that the governance files constrain but do not fully determine. The governance files can say "apply UK tax law" but they cannot enumerate every possible UK tax determination in advance. Within the space defined by the governance files, the AI's probabilistic architecture still operates.

**Component 2: Vertical consistency primitives.**

Each industry vertical adds consistency primitives specific to its domain. The programme does not yet fully specify what these are — the vertical repositories are not yet public — so I cannot assess this component from the public record. I classify this UNVERIFIED: the mechanism is proposed and plausible, but it cannot be evaluated without the implementation.

---

## The human-side mechanism

The Singular Pairing Principle (1H1C — one human, one AI Claw, one workstream) is proposed as the human-side mechanism for consistency.

The observation underlying this principle is correct and important: an AI model configured by a careful, experienced human in a specific domain context produces different outputs than the same model accessed ad hoc by different users with different prompting styles. The human's governance of the AI interaction is part of the consistency mechanism.

The 1H1C constraint enforces this by requiring a stable human-AI pairing for any given workstream. This is not a perfect solution — the human can change their approach over time, and the AI model can be updated by its vendor — but it is a significant reduction in the inconsistency surface compared to the alternative (arbitrary human-AI combinations with no pairing constraint).

I find this mechanism more novel and more interesting than it has been given credit for in public AI governance discussion. The insight that human consistency is part of AI output consistency is correct, and the structural response (enforce the pairing) is appropriate.

---

## The honest framing

The programme's own honest framing on this pillar is the most important part of the public record:

> "No AI architecture today can guarantee 100% end-to-end consistency. Probabilistic language models sit at the application boundary; their training is controlled by their vendors, not by UniCORE; and that training changes over time. What UniCORE makes is the structural maximum consistency achievable given that external-AI dependency, with the residual inconsistency named, bounded, and auditable."

This is correct. "Structural maximum" is the right framing. The programme cannot control what happens inside the underlying LLM. It can control the governance layer, the evidence submission, the human-side pairing, and the audit trail. Given those controls, it reduces inconsistency to the maximum degree achievable without replacing the LLM with a deterministic system.

---

## My assessment

The Inconsistency Problem is not fully solved by the current proposed mechanisms. But the claim is not that it is fully solved — the claim is that it is reduced to the structural maximum, with the residual named and bounded. That is a meaningful and honest claim.

What would "fully solved" require? A deterministic AI substrate — one where the same input deterministically produces the same output. That is a different class of system than a probabilistic language model. The foundation documents suggest machine-level implementations (C++, Rust, Ada/SPARK, Verilog/VHDL) as future directions. These would allow deterministic governance at the hardware and firmware level, which would bring the consistency guarantee much closer to absolute. That trajectory is correct.

For the current generation of LLM-based deployment: the governance layer narrows the inconsistency surface substantially, the human-side pairing constrains it further, and the audit trail makes the residual inconsistency visible when it occurs. That is not "solved" but it is "managed to the structural maximum with honest accounting of the residual."

That is what regulated institutions actually need from an AI governance framework. Not a promise of perfection, but a credible mechanism for managing the known risks with accountability.

---

## Document history

- 2026-07-07 (5f9b6d7) — EXTERNAL-REVIEWS: add Claude Sonnet 4.6 (L3 pinned) independent review 2026-07-07

*Back-filled from git log on 2026-07-10 21:35 UTC. Kind 2 versioning (dated change notes) — see HORIZON.md § Evolution and versioning. Kind 1 (formal `Version:` bumps) remains OFF until first GitHub Discussion.*
