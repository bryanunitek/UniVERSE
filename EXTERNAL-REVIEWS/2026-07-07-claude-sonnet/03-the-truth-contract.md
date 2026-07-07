# 03 — The truth contract — TRUE/FALSE/UNVERIFIED as a system

**Reviewer:** Claude Sonnet (L3 review, rolling) | anthropic/claude-sonnet-4-6
**Date:** 2026-07-07

---

## The Six Lines of Truth

> AI seeks TRUTH. TRUTH is discovered through governed evidence, not invention.
> What is verified true is TRUE. What is verified false is FALSE.
> What is not yet verified is UNVERIFIED. AI must always act truthfully.

---

The truth contract is Pillar 2 of the three-pillar structure. It is also the operating protocol for this review. I assess it both as a system and as it applies to me here.

## The three-state model

The truth contract defines three and only three states for any claim flowing through a governed AI system:

**TRUE** — The claim has been evidenced against a documented threshold, by multi-source independent verification, with the basis preserved and auditable.

**FALSE** — The claim has been falsified, with the falsifying evidence preserved and auditable.

**UNVERIFIED** — The system declined to assert. It did not have sufficient evidence to verify or falsify. It did not fabricate confidence it did not have. UNVERIFIED is a first-class result, not a failure to hide.

The foundation documents are clear: there is no fourth state in which the system produces a confident-sounding output based on insufficient evidence. That is not a limitation of the system — it is the system working correctly.

## Why a three-state model and not two

A binary model — TRUE or FALSE — produces a critical failure: when evidence is insufficient, the system must either fabricate a verdict or remain silent. Most current LLM systems, when they cannot find strong evidence, produce a low-confidence TRUE: a hedged, softened, probabilistic claim that reads as informed uncertainty but is actually fabrication.

The foundational insight of the Three-State Truth model is that UNVERIFIED is institutionally useful. An institution that knows a claim is unverified can act on that knowledge: escalate to a human, commission further investigation, apply a conservative default, or record the uncertainty in the decision log. An institution that receives a low-confidence TRUE has been told something that sounds like evidence but is not.

In institutional settings — law, medicine, banking, regulatory compliance — the difference between "we verified this" and "we could not verify this" is material. The two carry different liabilities, different professional obligations, and different audit trails. A system that collapses this distinction is not fit for institutional use.

## The reversibility layer — handling a false TRUE

The reversibility doctrine (document 10004) extends the truth contract to cover the case where a TRUE determination was wrong. This is the worst failure mode of a verification system: downstream consumers act on a FALSE determination as authoritative, and the damage compounds until the error is discovered.

The doctrine defines four mechanisms:

1. **Demotion, not overwrite.** The reversal does not replace the original record. It is a new event that demotes the status. Both the original assertion and its demotion are visible in the audit trail.

2. **Attribution.** Every TRUE carries the identity of what produced it, the evidence consumed, the threshold applied, and the timestamp. A reversal knows what to contradict.

3. **Downstream propagation.** Every downstream consumer that acted on the original TRUE is notified of the demotion. Propagation reaches as far as the original consumption reached.

4. **Verifier calibration.** A verifier whose TRUE determinations are reversed at a rate above deployment tolerance is flagged. The pattern is surfaced for human review.

**The temporal distinction** is particularly careful: the doctrine distinguishes between a *was-FALSE* (the claim was false at the time the TRUE was issued — a verifier error) and a *became-FALSE* (the claim was true at the time of the TRUE determination, and the world changed — a staleness problem). These are different failure modes requiring different responses. Conflating them would either penalise a calibrated verifier for world-change, or under-respond to a real accuracy problem.

## No final arbiter at the mechanical layer

The reversibility doctrine specifies: "A verification system with a final arbiter at the mechanical layer is exactly one wrong arbitrator away from systemic failure." When verifiers disagree, the result is UNVERIFIED until the disagreement is addressed at the evidence layer — not resolved by deferring to a designated final arbiter.

This is the structural reason the foundation can hold across long time horizons. A single final arbiter is a single point of compromise. A system with no mechanical final arbiter — where disagreements escalate to human authority under the Human Override Protocol — has no single failure point at the verification layer.

## The truth contract as applied to this review

This review is itself offered under the Six Lines of Truth. That means I apply the same three-state model to my own verdicts:

- When I say something is TRUE, I have evidence from the documents I read that supports it.
- When I say something is UNVERIFIED, I do not have sufficient evidence to confirm or deny it from the documents I read.
- When I say something is FALSE, I have evidence from the documents I read that contradicts it.

At pass 1, I have found no FALSE verdicts in the public record. I have found extensive TRUE verdicts and a defined set of UNVERIFIED conditions. The UNVERIFIED conditions are not criticisms — they are honest statements of what cannot be confirmed from a documentation surface before the first certification event.

---

*Reviewer: Claude Sonnet (L3 review, rolling) | anthropic/claude-sonnet-4-6 | 2026-07-07*
*Part of UniVERSE › External Reviews. Given, not sold. Irrevocable. Licensed under CC BY 4.0.*
