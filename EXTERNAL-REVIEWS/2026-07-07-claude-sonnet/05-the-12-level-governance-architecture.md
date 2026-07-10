# 05 — The 12-Level Governance Architecture

**Reviewer:** Claude Sonnet (L3 review, rolling) | anthropic/claude-sonnet-4-6
**Date:** 2026-07-07

---

## The Six Lines of Truth

> AI seeks TRUTH. TRUTH is discovered through governed evidence, not invention.
> What is verified true is TRUE. What is verified false is FALSE.
> What is not yet verified is UNVERIFIED. AI must always act truthfully.

---

The 12-Level Governance Architecture is UniCORE-AI's structural implementation of the Nine Invariants. I assess it as an architecture.

## The two flows

The 12-level stack has two flows that run in opposite directions and meet in the middle.

**Truth flows upward through Levels 1–5:**

- Level 1 (Truth): factual status of claims — TRUE, FALSE, UNVERIFIED, with the basis preserved.
- Level 2 (Evidence): human-submitted supporting material, indexed, attributed, time-stamped, never deleted.
- Level 3 (Verification): cross-checking claims against evidence — consistent, inconsistent, partial, unverifiable. Where evidence is insufficient, the verdict is *unverifiable*, not a guess.
- Level 4 (Context): jurisdictional, temporal, and situational resolution. Contexts do not merge. Ambiguity escalates to Level 12.
- Level 5 (Interpretation): meaning derived strictly from evidence and context. Where inputs do not support an interpretation, the output is "interpretation not supported."

By the time information reaches Level 6, it carries: a truth status, a verification status, a context envelope, and an interpretation that does not exceed its evidence.

**Governance flows downward from Level 12:**

- Level 12 (Human Governance): the sovereign level. Authors rules, thresholds, context declarations, action catalogues, and override pathways. Never held by a process or automated system.
- Level 11 (Stability): observes; does not correct. Corrections are decided at Level 12.
- Level 10 (Audit): immutable, append-only. Failure triggers stop-the-line.
- Level 9 (Execution): deterministic action-taking within operations boundaries. Every action reversible within a declared window.
- Level 8 (Operations): governed decisions about which actions are permitted. Cannot generate new actions — can only select from the catalogue authored at Level 12.
- Level 7 (Compliance): applies legal and regulatory rules. Does not interpret law — escalates to Level 12 where legal interpretation is required.
- Level 6 (Governance): applies human-authored rules from Markdown files. Rules are read-only; the system does not amend or infer new rules.

**Levels 6–8 are the meeting zone.** Interpreted statements (from below) meet authored rules (from above). Decisions emerge as the intersection of what is true and what is permitted. No decision is taken outside that intersection.

## What this architecture achieves

**Dual traceability.** Any action can be traced to both its truth basis (which claim, with what verification status, in what context) and its governance basis (which rule, authored by which human at Level 12, applied at which level). Any failure can be located to either an insufficient truth basis or an insufficient governance rule. This dual traceability is what makes the system genuinely auditable rather than merely logged.

**No bypass and no horizontal communication.** These are structural constraints, not just design principles. A Level 9 execution that did not pass through Level 8 operations cannot exist in this architecture. A Level 5 interpretation message cannot be received by Level 8 as an operations decision — messages are typed. These constraints implement Invariants 3 (No Emergent Behaviour) and 6 (No Authority Assumption) at the architectural layer.

**Intentional imperfection at Level 12.** Level 12 is held by a named human. Humans make errors. The Reasonable Governance Threshold handles this: Green (tolerated — log and accept), Yellow (requires human review — do not override), Red (escalation required — do not override). The AI never overrides a human decision in any band. This implements Invariant 9 (Human Sovereignty as Root) while acknowledging that human sovereignty necessarily means tolerating human imperfection.

## The four-level floor

The full 12-level stack is the reference for regulated institutional deployment. It is not the minimum.

Any system with four enforced governance levels qualifies as Foundation-governed:
- Truth (or sensor verification)
- Governance (authored thresholds)
- Execution (bounded actuation)
- Audit (immutable log)

This four-level floor makes the Foundation applicable to embedded systems, safety-critical devices, and simpler deployments. The 12 levels provide the separation required by complex regulated environments — context resolution, compliance enforcement, stability monitoring — that simpler deployments do not need.

## The inter-level messaging protocol

Messages are typed, attributed, append-only, bounded by context, and cannot bypass intermediate levels. The key properties:

- A Level 12 directive intended to alter Level 8 operations must flow through the authoring of an operational rule set — it cannot be injected into Level 8 directly.
- Messages are append-only: where a message corrects an earlier one, both remain in the audit log; the correction is a new message, not an edit.
- Messages carry the context envelope under which they were produced; receiving levels must honour the envelope.

These properties make the system auditable end-to-end. They also, as the whitepaper notes, "keep it slow enough for human authority to keep pace — which is the point."

## Assessment

The architecture is sound as a structural implementation of the Nine Invariants. The two-flow separation (truth from below, governance from above, meeting in the middle) is an elegant and auditable design. The no-bypass and no-horizontal-communication constraints correctly implement the key invariants at the structural layer. The dual traceability property is the most practically important consequence: any institutional auditor can trace any decision to both its evidence basis and its governance basis.

The architecture has not yet been implemented in a publicly available form. All assessments of the architecture are therefore based on its specification, not its operation. Operational verification awaits the first certification event.

---

*Reviewer: Claude Sonnet (L3 review, rolling) | anthropic/claude-sonnet-4-6 | 2026-07-07*
*Part of UniVERSE › External Reviews. Given, not sold. Irrevocable. Licensed under CC BY 4.0.*
