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

This document is the canonical public register of current and revoked holders of the **Solution Review certificate** issued by **Unitek Systems Limited**. The rule that requires a certificate to provide Solution Review as a delegated service is published in [`docs/00059-Solution-Review.md`](docs/00059-Solution-Review.md#if-the-solution-owner-cannot-operate-the-claw-directly). This file is where the names live.

The register is public for the same reason the rule is public. Anyone evaluating a Solution Review claimed under the programme name should be able to verify, in one place, that the practitioner who conducted it holds a current certificate.

---

## 1. Purpose

To make the certification rule verifiable by readers, regulators, customers, and successors:

- A solution owner considering a delegated review can confirm that the practitioner approaching them is in fact certified.
- A reader of a published Solution Review can confirm the operator-of-record named in the review's attribution couplet was certified at the time the review was conducted.
- A regulator or auditor can read the public history of who has been authorised to provide programme services and under what scope.
- A successor inheriting the Author/Creator role can read the register before issuing any new certificates of their own.

This is the same logic as a professional registry. The point of publishing the names is that the value of the certificate depends on it being checkable.

---

## 2. How certificates are held

Certification is **open to practitioners at all career stages** — from university students and junior consultants through to senior engineers and partners. The [Senior-level requirement in 00059 §6](docs/00059-Solution-Review.md#6-why-the-most-experienced-human) is **role-specific**, not exclusionary: it applies to the *Solution Review* role itself, because that role depends on the deepest available institutional memory of the solution being reviewed. The certification scheme that authorises a practitioner to provide Solution Review (and other delegated programme services) is intentionally broader. It is the route by which students, junior consultants, and mid-career practitioners contribute to UniVERSE, TrueAI, and UniCORE-AI, build the public track record that the certifying body weighs, and grow into the work the AI Enterprise Solutions of the future will need them to do.

**[GitHub Discussions](DISCUSSIONS.md) is the public venue where certification work happens.** Certification steps begin in Discussions. Over time, certifications will be **given** as part of Discussions: nominations, the reasoning behind them, and the issuance event itself will be visible there. The signed Git commit that adds a row to §3.1 below remains the canonical record, but the public conversation that leads to that commit lives in Discussions. This is what makes the scheme open and visible rather than private and discretionary.

Three distinct paths to holding a certificate exist:

### 2.1 Default-held certificate (no issuance required)

Bryan Fred, as Author and Creator of UniVERSE, TrueAI, and UniCORE-AI, holds the Solution Review certificate **by default**. This is a structural property of the Author/Creator role, not an issuance. The certifying authority (Unitek Systems Limited as originating organisation) and the certificate-holder (Bryan Fred as principal author) are the same originating identity, so issuance is not meaningful.

The default-held certificate **passes to any successor** named under the [TrueAI whitepaper succession statement](https://github.com/bryanunitek/TrueAI/blob/main/docs/whitepaper/WHITEPAPER.md#8-succession-and-stewardship), on the same default-held basis. Successors do not need to be re-certified; they inherit the certificate as part of inheriting the role.

### 2.2 Issued by direct nomination (interim regime)

Until the full Solution Review certification scheme is published as a separate programme document, certificates other than the default-held certificate are issued by **direct nomination** by Bryan Fred and Unitek Systems Limited. Nominations originate in [Discussions](DISCUSSIONS.md), where practitioners contribute openly to programme threads and where the certifying body forms its view of who is ready for certification. Nomination is recorded in this register; the act of adding a name to §3.1 below, in a signed Git commit, is the issuance event.

### 2.3 Issued under the full certification scheme (future)

When the full Solution Review certification scheme is published, the issuance path will change from direct nomination to a defined public process (criteria, examination, the licence-violation revocation procedure). [Discussions](DISCUSSIONS.md) will remain the venue in which the public-facing parts of that process run. The register will continue to be the canonical public record of who holds a certificate, regardless of which path issued it.

**Candidate mechanism under consideration: Discussion Points.** One model the certifying body is considering for the full scheme is a points-based pathway, in which practitioners accumulate **Discussion Points** through their public contributions to programme threads (questions, drafts, reviews, applied work shared back), and may **request certification via Discussions** once they reach a defined threshold. Under this model, the path to a certificate becomes practitioner-initiated rather than purely nomination-initiated: a practitioner who has earned the threshold and believes themselves ready may open a Discussion thread requesting certification, the certifying body reviews the public record, and (if approved) the same signed-Git-commit issuance event applies. Points criteria, threshold values, and any examination component are deliberately not defined in this register; they belong in the separate scheme document referenced above. This paragraph names the candidate mechanism so that contributions made under the interim regime are not lost if the future scheme adopts a points-based on-ramp.

---

## 3. The register

### 3.1 Currently certified

| # | Practitioner | Status | Authority basis | Certified from | L3 Scope-Domain CORE(s) authorised |
|---|---|---|---|---|---|
| 1 | **Bryan Fred** (Unitek Systems Limited, Bedford, United Kingdom) | Active (default-held; not subject to status change, see [§3.4](#34-engagement-status)) | Default-held, by virtue of being Author and Creator of UniVERSE, TrueAI, and UniCORE-AI | 2026-05-13 | All L3 Scope-Domain COREs in the programme |

The register currently has one entry. The default-held certificate is recorded above as line 1; it is recorded in the register, even though no issuance event took place, so that any reader can verify that the Author/Creator's certificate is publicly named and not implicit.

Additional certified experts will be added to §3.1 as Unitek Systems Limited issues their certificates by nomination (or, once the full scheme is published, by the scheme's public process). New entries are added in Active status; the engagement-status mechanism is described in [§3.4](#34-engagement-status).

### 3.2 Revoked (licence violation only)

No revoked entries to date.

**Once issued, a Solution Review certificate cannot be revoked.** This follows the same gift-principle reasoning that applies to the foundation as a whole: what has been given is not subject to withdrawal. The single, narrow exception is **violation of the [programme licence](LICENSE.md)**. Examples of licence violation include treating programme materials as commercial property, removing or falsifying attribution, or using the certificate to misrepresent the programme.

When a certificate is revoked on those grounds, the corresponding row is moved from §3.1 to this section with the date of revocation and the specific licence violation that triggered it. The revocation ends the practitioner's future authorisation to provide delegated Solution Review under the programme name. It does **not** invalidate work already completed, published, and certified under the previously-active certificate.

There is no expiry mechanism. Certificates do not lapse with time and there is no renewal process.

### 3.3 How to verify a certificate

The canonical source of truth for any certificate is this file, in its **current state on the `main` branch of the [UniVERSE repository](https://github.com/bryanunitek/UniVERSE)** at the moment of verification. The Git history of this file records every issuance and every revocation as a signed commit; nothing else exists outside the public record.

For readers who want to confirm a name against the register but do not wish to work directly with Git, **two channels are provided by Unitek Systems Limited**:

- **Public verification — via [Discussions](DISCUSSIONS.md).** A reader, customer, regulator, or counterparty may open a Discussion thread in the UniVERSE repository asking whether a named practitioner is certified, and at what scope. The answer is given publicly in-thread. Public verification is suitable where there is no confidentiality concern and the asking party is content for the question and its answer to remain part of the programme's public record.
- **Private verification — via LinkedIn direct message to [Bryan Fred](https://www.linkedin.com/in/bryan-fred-02209753/).** Where the asking party prefers not to put a verification question on the public record (commercial confidentiality, regulatory privacy, client-relationship sensitivity), the same question may be sent privately. The answer is given privately, and references the same register entries that would have been quoted in a public response.

Both channels are authoritative. Neither channel can issue a certificate, change a register entry, or override what is recorded in the file; their role is to make the file's contents queryable for parties who would otherwise have to read raw Git history. Verification by either channel never invents a certification not recorded here — if the file says the practitioner is not certified, that is the answer in either channel.

### 3.4 Engagement status

The certificate is the gift. The **register** also carries an engagement status alongside each entry, so the register stays accurate as a current statement of who is actively part of the programme. The status reflects the practitioner's recent participation; it does not affect the validity of the certificate.

**Status values:**

- **Active** — the practitioner has contributed to programme [Discussions](DISCUSSIONS.md), or to programme work in another visibly recorded form, within the most recent twelve (12) months.
- **Expired** — the practitioner has not contributed within the most recent twelve (12) months. **The certificate is not revoked.** Only the engagement status has changed. Expired status is not a punishment; it is a register-accuracy statement that the practitioner is currently inactive.
- **Active (default-held)** applies to the default-held entry (Bryan Fred and any future named successor under the Author/Creator role). The default-held entry is never moved to Expired, because the Author/Creator's authority is a structural property of the role, not a function of recent participation.

**Status is a register property, not a certificate property.** An Expired status:

- does NOT revoke the certificate;
- does NOT lapse the certificate;
- does NOT engage the [§4](#4-when-a-certificate-may-be-revoked) revocation rule or its self-binding clause;
- does NOT invalidate any Solution Review work the practitioner has already completed and signed off as operator-of-record.

The §4 rule that a certificate may be revoked only for licence violation is unaffected by this section. The certificate, once given, remains given.

**Returning to Active.** A practitioner whose status is Expired returns to Active on any new contribution to programme Discussions or programme work. The date of the contribution is recorded as the status-change date. There is no application, no examination, no fee, and no renewal procedure in the certificate sense; the practitioner simply contributes again, and the register reflects it.

**Disputes about status are corrections, not appeals.** If a practitioner believes their contributions in the relevant window were missed, they raise the matter via the [verification channels in §3.3](#33-how-to-verify-a-certificate). If the contributions are confirmed, the register is corrected by signed Git commit, with the original Active status restored. No appeal procedure is engaged, because no revocation has occurred.

**Interim threshold.** The twelve-month value is the interim regime's working threshold. The full certification scheme referenced in [§2.3](#23-issued-under-the-full-certification-scheme-future) may adjust the value, may make the threshold sensitive to the certification level (if levelled certificates are adopted, per the candidate described in §2.3), or may relate the threshold to the Discussion Points mechanism described as a candidate in §2.3. Any change to the threshold is published in this file by signed Git commit.

---

## 4. When a certificate may be revoked

A certificate may be revoked **only** for violation of the [programme licence](LICENSE.md).

**This rule binds Bryan Fred, any future named successor, and Unitek Systems Limited itself.** None of them, acting individually or jointly, may revoke a certificate for any reason other than violation of the programme licence. The certifying authority is the first party constrained by the rule. A certificate that could be revoked at the certifying authority's discretion would carry only the authority's continuing willingness, not a real commitment, and would not survive a change of leadership or institutional pressure; the self-binding here is what gives a certified expert a credential they can rely on across decades, not just across the goodwill of the current office-holders.

No other ground is sufficient. Disagreement, inactivity, commercial competition, personal dispute, or change of opinion does not constitute grounds for revocation. The certificate, once given, follows the gift principle: it is not subject to withdrawal except where the recipient has violated the terms under which the gift was made.

The default-held certificate (Bryan Fred and successors) cannot be revoked because the certifying authority and the certificate-holder are the same originating identity; revocation would mean the authority withdrawing authorisation from itself. If the Author/Creator role itself ceases (succession process exhausted, no named successor accepted), the default-held certificate ceases with it.

---

## 5. How a name enters or leaves the register

### 5.1 Adding a name (issuance)

Under the interim regime (§2.2):

1. A practitioner contributes to programme [Discussions](DISCUSSIONS.md). This is the entry step. The contributions — questions, drafts, reviews, applied work shared back to the programme — form the public track record that the certifying body weighs.
2. Bryan Fred and Unitek Systems Limited identify a practitioner to nominate, on the strength of that public record.
3. The practitioner is added as a new row in §3.1 of this file by signed Git commit. The commit author is `bryanunitek <bryan.fred@unitek-systems.com>`. The commit message names the practitioner and the L3 Scope-Domain CORE(s) authorised, and links back to the Discussions thread(s) the nomination is grounded in.
4. The commit's date in the public Git history of the UniVERSE repository is the **issuance event** for the certificate. There is no separate paper instrument; the public commit is the certificate.

Under the full certification scheme (§2.3), the addition path will be replaced by the scheme's defined process. The Git commit will remain the public-record step.

### 5.2 Revoking a certificate (licence violation)

When a certificate is revoked for licence violation:

1. The row is **moved** from §3.1 to §3.2 by signed Git commit.
2. The commit message records the specific licence violation.
3. The row is not deleted from §3.1's history; it is moved, so the Git log retains the full sequence of state changes.

Revocation is the only way a row leaves §3.1. There is no expiry, no lapsing, and no voluntary surrender mechanism. A practitioner who no longer wishes to provide Solution Review services simply stops providing them; their certificate remains in §3.1 because it was given and is not subject to withdrawal.

### 5.3 No silent edits

The register is append-or-move-only. Existing rows are not edited in place to change a practitioner's scope or status without a corresponding new commit. The Git history is the audit trail.

---

## 6. Relationship to other programme documents

- The certification rule itself is published in [`docs/00059-Solution-Review.md`](docs/00059-Solution-Review.md#if-the-solution-owner-cannot-operate-the-claw-directly), in the 'About the certificate' block at the end of that sub-section.
- The programme licence under which certificates are issued (and the only ground for revocation) is [`LICENSE.md`](LICENSE.md).
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

Public-facing changes to the certification rule itself will continue to be flagged in [`HORIZON.md`](HORIZON.md); changes to the register's contents (new certifications, revocations) are tracked in this file's Git history.

---

— Bryan Fred, Unitek Systems Limited, Bedford, United Kingdom
