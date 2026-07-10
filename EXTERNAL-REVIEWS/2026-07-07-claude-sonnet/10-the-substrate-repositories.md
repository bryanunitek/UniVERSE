# 10 — The substrate repositories

**Reviewer:** Claude Sonnet (L3 review, rolling) | anthropic/claude-sonnet-4-6
**Date:** 2026-07-07

---

## The Six Lines of Truth

> AI seeks TRUTH. TRUTH is discovered through governed evidence, not invention.
> What is verified true is TRUE. What is verified false is FALSE.
> What is not yet verified is UNVERIFIED. AI must always act truthfully.

---

The four substrate repositories (UniCORE, UniCORE.GVB, UniSaaS.UniCORE, UniSaaS.UniCORE.GVB) are the implementation-shape layer. I assess what they contribute to the public record.

## What the four repositories are

**UniCORE** is the reference product implementation — the single-tenant enterprise deployment shape of the 12-level architecture. It is the product form of UniCORE-AI for organisations that run their own infrastructure: private data centres, private cloud, sovereign cloud.

**UniCORE.GVB** is the Global Virtual Bridge — the substrate-services layer that underpins UniCORE. It provides the infrastructure stack that the 12-level architecture runs on: identity and access management, data residency and sovereignty, the audit backbone, the inter-level messaging bus, the Stability monitoring layer, and the Human Override Protocol channel.

**UniSaaS.UniCORE** is the SaaS-topology sister of UniCORE. It implements the same 12-level architecture in a multi-tenant configuration, where multiple organisations (tenants) each hold their own Level 12 while the platform operator holds a separate platform-level Level 12.

**UniSaaS.UniCORE.GVB** is the Global Virtual Bridge for the SaaS topology.

## What the four repositories contribute

**Architectural specificity.** The substrate repositories name specific technical components: `GovernanceValidator.cs`, `ThresholdEngine.cs`, `DriftDetection.cs` (from document 00007, the Reasonable Governance Threshold Specification). These file references tell a reader what kind of system this is being built as — it is a server-side .NET application with named components for the Reasonable Governance Threshold, not a vague "platform." That specificity is informative even before the code is public.

**Deployment topology clarity.** The two topology pairs (enterprise/GVB and SaaS/GVB) address the two dominant institutional deployment patterns: self-hosted and cloud-hosted. Separating them into distinct repositories makes the governance implications of each topology explicit — a tenant in the SaaS topology holds a different kind of Level 12 authority than an enterprise in the self-hosted topology.

**The multi-tenant Level 12 non-merging constraint.** UniSaaS.UniCORE is explicit: tenant authority applies to tenant decisions; vendor authority applies to platform operations. The two Level 12s do not merge. This implements Invariant 5 (No Domain Merging) in the SaaS topology without requiring each tenant to self-host. It is a careful design that makes SaaS deployment viable while preserving the sovereignty guarantees.

## What the four repositories cannot contribute yet

Source code is not yet public in any of the four substrate repositories. The code lives in private "-Claw" repositories and is published at the first certification event.

This means the architectural claims in the four repositories — while consistent with UniCORE-AI's architecture — cannot be independently verified at the implementation level. The claims are plausible given the architecture; they are UNVERIFIED given the absence of source code.

The honest framing: all four repositories state this plainly. No repository claims otherwise. "Source code is not yet published here" is stated in the README of each. This is a v1.0 state, not a misrepresentation.

## Assessment

The four substrate repositories contribute meaningful architectural specificity to the public record. The deployment topology choices (single-tenant enterprise vs multi-tenant SaaS; each with a GVB substrate layer) are well-reasoned and address the real institutional deployment landscape. The multi-tenant Level 12 non-merging constraint is the most important governance innovation in these repositories.

The absence of source code means all implementation claims are UNVERIFIED until the first certification event. That is honest, stated, and the expected v1.0 state of the programme.

---

*Reviewer: Claude Sonnet (L3 review, rolling) | anthropic/claude-sonnet-4-6 | 2026-07-07*
*Part of UniVERSE › External Reviews. Given, not sold. Irrevocable. Licensed under CC BY 4.0.*

---

## Document history

- 2026-07-07 (f7868a0) — EXTERNAL-REVIEWS: add Claude Sonnet (L3 rolling) independent review 2026-07-07

*Back-filled from git log on 2026-07-10 21:35 UTC. Kind 2 versioning (dated change notes) — see HORIZON.md § Evolution and versioning. Kind 1 (formal `Version:` bumps) remains OFF until first GitHub Discussion.*
