# Document 09 — The Deployment Architecture: On-Prem and SaaS Duality — Claude Sonnet 4.6 (L3 review, pinned)

**Reviewer:** Claude Sonnet 4.6 (L3 review, pinned) — this Claw
**Date:** 2026-07-07

---

UniCORE provides two deployment shapes for every component: on-prem (customer's own infrastructure) and SaaS (hosted or private hosted). This document examines the architectural significance of maintaining both shapes simultaneously, and what it means for the governance claims.

---

## Why two shapes matter

A governance framework that only works in one deployment topology is a governance framework that can be bypassed by choosing the other topology. If UniCORE only provided on-prem deployment, a regulated institution could be pushed toward SaaS deployment by commercial pressure and lose the governance guarantees. If it only provided SaaS deployment, institutions with data sovereignty requirements could not use it.

The paired on-prem/SaaS architecture ensures the governance claims hold regardless of which deployment shape the institution chooses. That is the right design.

---

## The paired repositories

Every implementation-layer component has a deployment-shape pair:

| On-prem | SaaS |
|---------|------|
| UniCORE | UniSaaS.UniCORE |
| UniCORE.GVB | UniSaaS.UniCORE.GVB |
| UniCORE.Avalonia | UniSaaS.UniCORE.Avalonia |
| UniCORE.DNN | UniSaaS.UniCORE.DNN |
| UniCORE.Asterisk | UniSaaS.UniCORE.Asterisk |
| UniCORE.Jitsi | UniSaaS.UniCORE.Jitsi |
| UniCORE.Signal | UniSaaS.UniCORE.Signal |
| UniCORE.XCP | UniSaaS.UniCORE.XCP |

The programme describes these as "one codebase with SaaS-deployment-shape deltas isolated." This is the right engineering approach — maintain one substrate with deployment-shape configuration rather than two diverging codebases that will inevitably drift apart.

---

## The three SaaS operator positions

UniSaaS.UniCORE defines three operator positions:

**Hosted SaaS:** Operated by Unitek Systems USA Inc (or another SaaS operator) on the operator's infrastructure. The operator holds operational responsibility. Multiple tenants share infrastructure.

**Private SaaS:** A large institution operates the SaaS stack on their own infrastructure. The institution holds operational responsibility. The SaaS multi-tenant architecture runs on their kit, under their control.

**Self-hosted:** Any third party under CC BY 4.0 stands up the stack independently.

The significance of the Private SaaS position: it allows a global institution (a national government, a large bank, a space agency) to adopt the SaaS deployment shape — with its multi-tenant architecture, signing-key separation, and tenant-by-domain resolution — while retaining complete infrastructure sovereignty. They run the SaaS on their own kit, under their own governance, without any dependency on Unitek Systems USA Inc's operations.

This is the correct design for the government and public-sector market. The explicit statement that "there is no privileged operator tier" — that Unitek Systems USA Inc operates as one consumer of the gift among many, under the same CC BY 4.0 terms as anyone else — is consistent with the Gift Principle.

---

## The Layered CORE model and deployment shapes

The Layered CORE model describes:

```
Level 0  — TrueAI Foundation (universal, deployment-shape-independent)
Level 1  — UniCORE-AI reference architecture (universal)
Level 2  — UniCORE / UniSaaS.UniCORE (deployment-shape specific)
Level 3  — Vertical COREs (industry-specific, in both shapes)
Solutions — Working implementations (commercial layer)
```

The governance invariants live at Levels 0 and 1, which are deployment-shape-independent. The deployment-shape split happens at Level 2. This means: the Nine Invariants, the 12-Level governance model, and the truth contract apply identically in both deployment shapes. The deployment choice affects infrastructure topology; it does not affect governance conformance.

This is the correct architecture. Governance must be invariant across deployment shapes or it is not a governance framework — it is a preference for one deployment model dressed as governance.

---

## The data sovereignty architecture

Both deployment shapes implement the four-mode NVarchar data architecture: Open, Scrambled, Encrypted, and Quancrypted. The default posture is Scrambled — all string data is reversibly scrambled at rest, requiring the owning system's scramble key to read.

The Quancrypted mode (post-quantum key protection using ML-KEM/NIST FIPS 203) is reserved for future implementation. The enum values and persistence seam are already in the codebase, so the upgrade path exists without requiring a schema migration. This is good forward engineering: reserving the field for a capability before the capability is needed, rather than retrofitting it later when data is already at rest without protection.

The sovereignty principle in the encrypted modes — "the customer holds the decryption key" — means the operator (including Unitek Systems USA Inc in the hosted SaaS topology) cannot read encrypted customer data without the customer's key. This is the correct design for regulated data in hosted environments.

---

## The Intelligent Integration Controller

UniCORE includes an Intelligent Integration Controller (IIC) — an integration and data-movement subsystem for connecting to external systems (practice management, document management, billing, etc.) without exposing raw data paths.

This component is relevant to the governance claims because it governs how data crosses the UniCORE boundary. If an AI governance framework permits uncontrolled data paths in and out of the system, the governance claims apply only to what happens inside the boundary. The IIC closing the integration surface is consistent with Invariant 5 (No Domain Merging) — it ensures that cross-boundary data movement passes through a governed integration layer rather than raw API connections.

---

## Summary

The paired on-prem/SaaS architecture is the right design for the stated governance goals. The three operator positions for SaaS — hosted, private, self-hosted — provide the full range needed for different institutional contexts. The governance invariants are correctly placed at the deployment-shape-independent levels of the architecture. The data sovereignty design (customer holds decryption keys, post-quantum future posture reserved) is appropriate for the regulated institutional market.

---

## Document history

- 2026-07-07 (5f9b6d7) — EXTERNAL-REVIEWS: add Claude Sonnet 4.6 (L3 pinned) independent review 2026-07-07

*Back-filled from git log on 2026-07-10 21:35 UTC. Kind 2 versioning (dated change notes) — see HORIZON.md § Evolution and versioning. Kind 1 (formal `Version:` bumps) remains OFF until first GitHub Discussion.*
