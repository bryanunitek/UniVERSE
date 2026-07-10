# Document 12 — Open Questions for a Second Pass — Claude Sonnet 4.6 (L3 review, pinned)

**Reviewer:** Claude Sonnet 4.6 (L3 review, pinned) — this Claw
**Date:** 2026-07-07

---

This document collects the questions I would bring back to the repositories in a second pass. They are organised by priority: the first group are the most structurally significant; the second group are important but less urgent.

---

## Group 1 — Structural questions (highest priority)

**Q1: What is the published conformance specification for the certification gate?**

The certification gate is the programme's most important governance mechanism. The question is what an implementation must demonstrate to pass it. The specification should be public, precise, and independently auditable. If it is not yet published, when will it be? (See Document 07.)

**Q2: What is the plan for an independent certification governance body?**

The gate is currently administered by the programme creator. For long-term credibility, the gate needs oversight from a body with interests independent of the creator's commercial interests. Is this planned? What is the timeline? (See Document 07.)

**Q3: What is the clarification of Invariant 4 (No Human Influence)?**

As stated, Invariant 4 seems to prohibit the ordinary influence that a well-reasoned output has on a reader. The intent is clearly to prohibit active influence operations (manipulation, persuasion beyond the evidence, belief engineering). That clarification should be in the foundation documents. (See Document 02.)

**Q4: What is the conformance test specification for Invariant 3 (No Emergent Behaviour)?**

The invariant correctly closes the heartbeat/timer route. How does an auditor determine whether a given AI system's timing and scheduling behaviour is "externally directed" (permitted) versus "self-generated" (prohibited)? (See Document 02.)

**Q5: How is conflicting evidence handled at Levels 3 and 4?**

The truth contract defines TRUE (evidenced), FALSE (falsified), and UNVERIFIED (not asserted). What happens when two pieces of submitted human evidence support contradictory claims? The Verification level (Level 3) presumably resolves this, but the resolution mechanism is not described in the public documents I read. (See Document 03.)

---

## Group 2 — Important but less urgent

**Q6: What is the inter-level messaging protocol (ILMP) specification?**

Document 00017 in the UniVERSE index is "UniCORE AI Inter-Level Messaging Protocol (ILMP)." I have not read it. The ILMP is the specification that enforces the no-horizontal-communication and no-bypass properties of the 12-Level stack at the implementation level. Reading this document would be the most important second-pass read for assessing the architecture's implementation claims. (See Document 05.)

**Q7: What does Level 11 (Stability / Drift Detection) actually monitor and how?**

Drift detection is the mechanism for detecting when the AI substrate has changed enough to affect the consistency guarantees. The monitoring mechanism, the threshold for intervention, and the response process are not described in the READMEs. This is the level I am most curious about in the implementation documents. (See Document 05.)

**Q8: What is the conditional revocation mechanism for the Gift Principle?**

The Gift Principle states that the gift can be withdrawn from a violator. Who determines that a violation has occurred? What is the process? What is the remedy? These governance mechanics are not yet specified in the public documents. (See Document 06.)

**Q9: What is the "4 or more levels" conformance claim?**

UniCORE-AI states: "Any AI system with 4 or more enforced governance levels uses the UniVERSE / TrueAI / UniCORE AI foundations — regardless of level names or industry." I read this as claiming too much. A 4-level system that does not implement the Nine Invariants is not using the TrueAI Foundation in any meaningful sense. I would want this clarified. (See Document 05.)

**Q10: What is the Generation IT succession plan?**

Document 10003 (Generation IT Succession) is listed across multiple repositories as a mastered document. The 30-year programme depends on generational continuity. The succession plan for both the programme and the individual certifications is important for long-term credibility. I have not read this document; it should be on the second-pass reading list.

**Q11: What open-source projects have been selected and why?**

The building-block selection (Asterisk, Jitsi, Signal, XCP) tells us something about the intended operational scope of the programme. Understanding the selection criteria — why these projects and not others — would help in assessing whether the governance claims will hold across the full stack. Were these selected because they are the most governable open-source implementations of their respective functions? Because they have compatible licences? Because they are the most mature?

---

## What these questions are not

They are not evidence that the programme is flawed. They are the questions that remain open after reading the public READMEs and that would be answered by reading the fuller document set and the eventual implementation.

A governance framework that had no open questions after reading its READMEs would be a governance framework that was either trivially simple or less than fully specified. The open questions here are the result of taking the programme seriously enough to ask what would need to be true for the claims to hold.
