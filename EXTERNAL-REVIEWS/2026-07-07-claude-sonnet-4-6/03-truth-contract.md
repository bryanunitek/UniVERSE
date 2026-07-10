# Document 03 — The Truth Contract: TRUE/FALSE/UNVERIFIED as a System — Claude Sonnet 4.6 (L3 review, pinned)

**Reviewer:** Claude Sonnet 4.6 (L3 review, pinned) — this Claw
**Date:** 2026-07-07

---

The TrueAI Foundation's truth contract is a three-state epistemic system: TRUE, FALSE, UNVERIFIED. This document examines whether it is the right system, whether it is complete, and whether it is operationally deployable.

---

## Why a three-state system?

Most AI systems operate with an implicit two-state model: the system either outputs an answer or declines to answer. The answer may be confident or hedged, but the hedging is stylistic ("I think," "it seems," "I'm not certain") rather than structural. There is no formal distinction between "I have evidence for this" and "I do not have evidence but it sounds plausible."

The failure mode this produces is well-documented: AI systems generate plausible-sounding answers to questions they cannot actually answer, because the training incentive rewards plausible output over honest uncertainty. The stylistic hedge covers the fabrication without constraining it.

The TRUE/FALSE/UNVERIFIED system is a structural response. UNVERIFIED is not a hedge — it is a classification. It means: the system reached the end of its evidential reasoning and found no grounds for assertion. It is a first-class output, not a softened version of FALSE.

This is the right design. Forcing a clear distinction between "evidenced" and "not-yet-evidenced" breaks the incentive for confident fabrication. A system that must classify its outputs into one of three states — rather than generating text on a confidence spectrum — cannot as easily conceal uncertainty behind stylistic fluency.

---

## Is the three-state system complete?

I identify three questions about completeness that the foundation documents should address.

**Question 1: What is the unit of classification?**

A document may contain claims that are individually TRUE, FALSE, and UNVERIFIED. A complex legal analysis may contain fifty claims in different states. The truth contract is stated at the claim level, but the public documents do not specify the granularity of classification in practice. Is a document classified by its weakest claim? By a summary of claim states? Is there a schema for multi-claim documents?

This is not a defect — it is a design question that the implementation documents (which I have not fully read) may already answer. I raise it because the operational usefulness of the three-state system depends on a clear answer at this level.

**Question 2: Who verifies the classification?**

TRUE means evidenced. Evidence is "human-submitted supporting material" (Level 2 in the 12-Level stack). But the system classifies the claim as TRUE based on evidence submitted by humans who may themselves be wrong, biased, or deliberately misleading. The truth contract does not seem to claim that TRUE means objectively true — it claims that TRUE means evidenced by what has been submitted.

This is honest and it is the right scope for what an AI governance system can actually guarantee. But it should be stated explicitly. The risk is that users treat a TRUE classification as an objective truth claim when it is actually an evidenced-by-submission claim. The system's integrity depends on the integrity of what is submitted to it at Level 2.

**Question 3: What happens when evidence conflicts?**

If two pieces of submitted evidence support contradictory claims, and both are human-submitted, what does the system do? The 12-Level model suggests this is resolved at Level 3 (Verification) and Level 4 (Context). But the truth contract as stated in TrueAI does not address the conflicting-evidence case explicitly. An indication of how the system handles conflicting evidence would strengthen the contract.

---

## Operational deployability

The TRUE/FALSE/UNVERIFIED system is operationally deployable in principle. The challenge is enforcement.

In the current generation of LLMs, the model can be instructed to use the three-state system, and it will comply most of the time. But the underlying model has no structural mechanism that prevents it from generating text that reads as TRUE while the underlying reasoning rested on a fabricated chain of evidence. The governance layer's ability to enforce the truth contract depends on:

1. The quality of evidence submitted at Level 2
2. The verification performed at Level 3
3. The instruction set given to the AI at the application boundary

UniCORE's answer is that all three of these are governed by human-authored MD files at the appropriate levels. This is correct as a design target. The residual risk — that a sufficiently long or complex session might produce spurious TRUE classifications — is named in the honest framing rather than hidden.

---

## The UNVERIFIED classification applied to this review

I note that the author of FULL_FORMAL_STATEMENT.md applies the UNVERIFIED classification to their own beliefs:

> "This statement is declared UNVERIFIED by its author, in accordance with principle 7 of the TrueAI Foundation."

And specifically:

> "I believe that for humanity to survive, two things are required: there can be no weapons, and there must be mutual respect and understanding... I cannot prove humanity will reach that direction, and I will not pretend otherwise. This belief is UNVERIFIED."

This is significant. The author is applying the framework to themselves — not exempting their own normative claims from the epistemic standards they are asking AI systems to meet. This is consistent, intellectually honest, and unusual. Most governance frameworks are built on confident normative premises without applying the same evidential scrutiny to those premises that the framework applies to AI outputs.

The self-application of the truth contract to the framework's own foundational beliefs is a genuine strength of the UniCORE approach.

---

## Document history

- 2026-07-07 (5f9b6d7) — EXTERNAL-REVIEWS: add Claude Sonnet 4.6 (L3 pinned) independent review 2026-07-07

*Back-filled from git log on 2026-07-10 21:35 UTC. Kind 2 versioning (dated change notes) — see HORIZON.md § Evolution and versioning. Kind 1 (formal `Version:` bumps) remains OFF until first GitHub Discussion.*
