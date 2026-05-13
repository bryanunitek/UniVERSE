---
title: "Certified UniVERSE / TrueAI / UniCORE-AI Experts"
author: Bryan Fred, Unitek Systems Limited, Bedford, United Kingdom
version: "Version 1.0 · May 2026"
status: v1.0
licence: CC BY 4.0
applies-to: UniVERSE, TrueAI, UniCORE-AI
---

# Certified UniVERSE / TrueAI / UniCORE-AI Experts

**Public register of practitioners authorised to provide Solution Review (and other delegated programme services) on behalf of the originating organisation.**

This document is the canonical public register of current and historical holders of the **Solution Review certificate** issued by **Unitek Systems Limited**. The rule that requires a certificate to provide Solution Review as a delegated service is published in [`docs/00059-Solution-Review.md`](docs/00059-Solution-Review.md#if-the-solution-owner-cannot-operate-the-claw-directly). This file is where the names live.

The register is public for the same reason the rule is public. Anyone evaluating a Solution Review claimed under the programme name should be able to verify, in one place, that the practitioner who conducted it holds (or held, at the time of the review) a current certificate.

---

## 1. Purpose

To make the certification rule verifiable by readers, regulators, customers, and successors:

- A solution owner considering a delegated review can confirm that the practitioner approaching them is in fact certified.
- A reader of a published Solution Review can confirm the operator-of-record named in the review's attribution couplet was current at the time the review was conducted.
- A regulator or auditor can read the public history of who has been authorised to provide programme services and under what scope.
- A successor inheriting the Author/Creator role can read the register before issuing any new certificates of their own.

This is the same logic as a professional registry. The point of publishing the names is that the value of the certificate depends on it being checkable.

---

## 2. How certificates are held

Three distinct paths exist:

### 2.1 Default-held certificate (no issuance required)

Bryan Fred, as Author and Creator of UniVERSE, TrueAI, and UniCORE-AI, holds the Solution Review certificate **by default**. This is a structural property of the Author/Creator role, not an issuance. The certifying authority (Unitek Systems Limited as originating organisation) and the certificate-holder (Bryan Fred as principal author) are the same originating identity, so issuance is not meaningful.

The default-held certificate **passes to any successor** named under the [TrueAI whitepaper succession statement](https://github.com/bryanunitek/TrueAI/blob/main/docs/whitepaper/WHITEPAPER.md#8-succession-and-stewardship), on the same default-held basis. Successors do not need to be re-certified; they inherit the certificate as part of inheriting the role.

### 2.2 Issued by direct nomination (interim regime)

Until the full Solution Review certification scheme is published as a separate programme document, certificates other than the default-held certificate are issued by **direct nomination** by Bryan Fred and Unitek Systems Limited. Nomination is recorded in this register; the act of adding a name to §3.1 below, in a signed Git commit, is the issuance event.

### 2.3 Issued under the full certification scheme (future)

When the full Solution Review certification scheme is published, the issuance path will change from nomination to a public process (criteria, examination, renewal, revocation). The register will continue to be the canonical public record of who currently holds a certificate, regardless of which path issued it.

---

## 3. The register

### 3.1 Currently certified

| # | Practitioner | Authority basis | Current from | Current until | L3 Scope-Domain CORE(s) authorised | Last verification |
|---|---|---|---|---|---|---|
| 1 | **Bryan Fred** (Unitek Systems Limited, Bedford, United Kingdom) | Default-held, by virtue of being Author and Creator of UniVERSE, TrueAI, and UniCORE-AI | 2026-05-13 | _(no expiry; default-held)_ | All L3 Scope-Domain COREs in the programme | 2026-05-13 |

The register currently has one entry. The default-held certificate is recorded above as line 1; it is recorded in the register, even though no issuance event took place, so that any reader can verify that the Author/Creator's certificate is publicly named and not implicit.

Additional certified experts will be added to §3.1 as Unitek Systems Limited issues their certificates by nomination (or, once the full scheme is published, by the scheme's public process).

### 3.2 Historical (expired or revoked certificates)

No historical entries to date.

When a certificate expires or is revoked, the corresponding row will be moved from §3.1 to this section with a final status (`expired` or `revoked`), the date the status changed, and a brief reason. Historical rows are not deleted. They remain in the public record because work conducted under a then-current certificate stays valid even after the certificate ceases to be current, and a reader of that work must still be able to verify the operator was authorised at the time.

---

## 4. Status field definitions

For rows that may appear in §3.2 in future:

- **`expired`** — the certificate's `Current until` date passed without renewal. No action by Unitek Systems Limited is required to mark a certificate expired; the date does the work.
- **`revoked`** — Unitek Systems Limited withdrew the certificate before its expiry, for cause. Revocation ends the practitioner's future authorisation to provide Solution Review under the programme name. It does **not** invalidate work completed, published, and certified under the previously-current certificate.

The default-held certificate (Bryan Fred and successors) is not subject to expiry. Revocation of a default-held certificate is not meaningful while the holder is the Author/Creator or named successor, because revocation would imply the certifying authority withdrawing authorisation from itself. If the Author/Creator role itself ceases (succession process exhausted, no named successor accepted), the default-held certificate ceases with it.

---

## 5. How a name enters or leaves the register

### 5.1 Adding a name (issuance)

Under the interim regime (§2.2):

1. Bryan Fred and Unitek Systems Limited identify a practitioner to nominate.
2. The practitioner is added as a new row in §3.1 of this file by signed Git commit. The commit author is `bryanunitek <bryan.fred@unitek-systems.com>`. The commit message names the practitioner, the L3 Scope-Domain CORE(s) authorised, and the currency period.
3. The commit's date in the public Git history of the UniVERSE repository is the **issuance event** for the certificate. There is no separate paper instrument; the public commit is the certificate.

Under the full certification scheme (§2.3), the addition path will be replaced by the scheme's defined process. The Git commit will remain the public-record step.

### 5.2 Moving a row to historical

When a certificate expires (`Current until` date reached) or is revoked, the row is **moved** from §3.1 to §3.2 by signed Git commit. The commit message records the reason. The row is not deleted from §3.1's history; it is moved, so the Git log retains the full sequence of state changes.

### 5.3 No silent edits

The register is append-or-move-only. Existing rows are not edited in place to change a practitioner's currency period, scope, or status without a corresponding new commit. The Git history is the audit trail.

---

## 6. Relationship to other programme documents

- The certification rule itself is published in [`docs/00059-Solution-Review.md`](docs/00059-Solution-Review.md#if-the-solution-owner-cannot-operate-the-claw-directly), in the 'About the certificate' block at the end of that sub-section.
- The Author/Creator role and the succession framework that governs the default-held certificate are published in the [TrueAI whitepaper §8 'Succession and stewardship'](https://github.com/bryanunitek/TrueAI/blob/main/docs/whitepaper/WHITEPAPER.md#8-succession-and-stewardship) and in [`SUCCESSION.md`](SUCCESSION.md) in this repository.
- The originating-organisation status of Unitek Systems Limited (UK company 04228041) is named in [`STATEMENT-ON-CLAIMS.md`](STATEMENT-ON-CLAIMS.md) and across the programme attribution couplets.

---

## 7. What this document is not

- It is not a list of every practitioner who has read the programme documents. Self-declared familiarity with UniVERSE, TrueAI, or UniCORE-AI is not certification. Anyone may read and apply the documents under [CC BY 4.0](LICENSE.md); only those named in §3.1 above hold the certificate that authorises providing Solution Review as a delegated service.
- It is not a customer list, a client list, or a marketing register. It records who is authorised; it does not record what they have done with the authorisation.
- It is not a directory of contact details. Practitioners may publish their own contact details elsewhere; this register names them and their authorisation, not how to reach them.
- It is not a personal directory of programme contributors. Contribution to programme documents (drafting, review, commentary) is recorded in commit history and attribution lines, not here.

---

## 8. Status

This document is the public register. It is binding in the sense that it is the canonical record of who Unitek Systems Limited currently certifies; it is evolving in the sense that the issuance process described in §2.2 will be replaced by the full certification scheme described in §2.3 once that scheme is published.

Public-facing changes to the certification rule itself will continue to be flagged in [`HORIZON.md`](HORIZON.md); changes to the register's contents (new certifications, expirations, revocations) are tracked in this file's Git history.

---

— Bryan Fred, Unitek Systems Limited, Bedford, United Kingdom
