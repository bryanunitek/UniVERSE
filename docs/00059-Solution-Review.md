# Solution Review

**Onboarding an existing solution onto a Foundation-aligned CORE: one human, one Claw, begin**

Author: Bryan Fred, Unitek Systems Limited, Bedford, United Kingdom
First published: May 2026
Status: Public. Given, not sold. Irrevocable.
Version: 1.0 — May 2026

---

## 1. Purpose

This document is operational guidance for the owner of an existing
solution who intends to bring that solution onto a Foundation-aligned
CORE. It states the smallest viable starting shape, names who the
first human in the pairing should be, and explains why the choice of
that first human determines what knowledge survives the first
generation of the Solution.

It is a companion to
[00057 Layered CORE Model](00057-Layered-CORE-Model.md) (which
defines the Solutions tier and its time horizon) and
[00058 Claw](00058-Claw.md) (which defines the governed channel the
human pairs with).

---

## 2. The process

The operational shape of a Solution Review, end to end, is five steps:

### A. One human

The person on the human side of the pairing is the one with the most experience and knowledge of the solution being reviewed. Not the most senior by job title; not the most recently joined; not a committee. The single human who carries the deepest lived context of the solution. (Why this person, in detail: [§6](#6-why-the-most-experienced-human).)

### B. One Claw

The AI side of the pairing is one **Claw** — a governed human-AI channel as defined in
[00058 §2.1](00058-Claw.md#21-claw). Not a **MyClaw**
([00058 §2.3](00058-Claw.md#23-myclaw)) — a personal, ungoverned AI connection cannot carry the governance the review output needs to inherit. One Claw, one Solution, one review.

### C. Give the Claw access to the three programme repositories

Give the Claw read access to the three public repositories that together publish the Foundation, the architecture, and the programme:

- [https://github.com/bryanunitek/UniVERSE](https://github.com/bryanunitek/UniVERSE)
- [https://github.com/bryanunitek/TrueAI](https://github.com/bryanunitek/TrueAI)
- [https://github.com/bryanunitek/UniCORE-AI](https://github.com/bryanunitek/UniCORE-AI)

These three repositories are the source-of-truth set the Claw needs in order to evaluate the solution against the Foundation, the Layered CORE Model, and the programme's published commitments. All three are public and all three are gifted under CC BY 4.0; the Claw needs no special permission to read them.

### D. Upload a trimmed archive of the solution

The human prepares a **trimmed ZIP** of their existing solution and uploads it to the Claw. "Trimmed" means: enough of the solution for the Claw to understand its structure, decisions, and content, without binaries, build artefacts, third-party dependency dumps, or material the human is not authorised to share. As a starting list:

- source code,
- schema and data-model definitions,
- configuration files,
- internal documentation, design notes, decision records,
- where they exist: architecture diagrams, integration maps, threat models.

The upload is the input the Claw works against in step E. The size and shape of the trim is the human's call; the test is whether the Claw has enough material to make a substantive judgement.

### E. Ask the Claw to review and advise

The human asks the Claw, in their own words, to review the uploaded solution and advise on how it fits into the UniVERSE programme — specifically into the **TrueAI Foundation**, **UniCORE AI**, and any relevant **L3 Scope-Domain CORE** (for Law-sector solutions, that means UniCORE-Claw — see [00057 §2](00057-Layered-CORE-Model.md#2-the-four-tiers)).

The Claw's first response is the start of the review, not the end of it. From step E onward, **the rest is between the human and the Claw** — to discuss, to refine, to argue with, to push back on, and to move toward the future together. The programme provides the Foundation, the architecture, and the Layered CORE Model as the framing material; the human and the Claw produce the review output ([§7](#7-what-the-review-produces)) inside that framing, on their own working rhythm.

### If the solution owner cannot operate the Claw directly

The five-step process assumes the solution owner — the human with the deepest experience and knowledge of the solution — sits in the pairing themselves. That is the preferred shape, and it is what the rule in [§3](#3-the-rule-behind-the-process) names.

In practice, the most experienced human in a Solution is also frequently the busiest. Senior partners, founding architects, long-tenured heads of practice — the people who carry the institutional memory the review needs ([§6.2](#62-the-undocumented-is-what-matters)) — do not always have the working hours to sit with a Claw across the weeks a review takes.

In that case, the work may be done on the solution owner's behalf by a **certified UniVERSE / TrueAI / UniCORE-AI expert** — an external practitioner who is fluent in the Foundation, the Layered CORE Model, and the programme's published commitments, who **holds a current Solution Review certificate issued by Unitek Systems Limited**, and who provides Solution Review as a service. The five-step process does not change. What changes is who sits on the human side of the pairing, and what the solution owner must still supply.

**What the expert does**

- Holds a **current Solution Review certificate issued by Unitek Systems Limited**, which names them as authorised to operate the Claw side of a delegated Solution Review on the programme's behalf. Uncertified practitioners may not offer Solution Review as a delegated service; an uncertified review is not a Solution Review in the programme's sense.
- Operates the Claw across steps B, C, D, and E.
- Carries the Foundation, the Layered CORE Model, and the Singular Pairing Principle into the session as the framing material the review must satisfy.
- Acts as the named operator-of-record in the review output, alongside (not in place of) the solution owner.
- Declares the delegation explicitly in the review's attribution couplet, so the audit trail records both the human-of-record and the operator who ran the pairing on their behalf.

**What the solution owner must still supply, directly**

The expert is a conduit, not a substitute. The institutional memory the review depends on lives in the solution owner, not in the expert, and the review collapses to a surface read if the owner does not put themselves into the loop at the points where their knowledge is the only knowledge that exists. At minimum, the solution owner must:

- Authorise the trimmed archive (step D) and confirm what may and may not be shared.
- Answer the questions that surface during the pairing — in person, on a call, in writing, asynchronously — in their own words, so the material entering the Claw is the owner's institutional memory and not the expert's reconstruction of it.
- Be available for clarifications across the working period of the review. A review that proceeds for days without any direct input from the owner is, in this document's terms, not a Solution Review of *their* solution — it is the expert's reading of it.
- Sign off on the review output as the human-of-record before it is published or relied on internally.

**What the expert must not do**

- Operate as a Solution Review provider without a current Unitek Systems Limited certificate. The certificate is the marker that distinguishes a programme-recognised expert from a practitioner who has merely read the public repositories.
- Invent institutional memory the solution owner has not supplied. If the owner has not answered a question, the answer is *unknown to this review*; it is not the expert's guess.
- Operate the pairing as a MyClaw ([00058 §2.3](00058-Claw.md#23-myclaw)). The Claw used in a delegated review is still a governed Claw, bound by the same governance the direct case is bound by.
- Claim the review as their own work. The output is the solution owner's review of their solution, conducted with expert assistance. The attribution couplet ([§7](#7-what-the-review-produces)) reflects that.

A delegated review honours [§6](#6-why-the-most-experienced-human) — the principle that the most experienced human matters — rather than working around it. It says: when the most experienced human cannot also be the most available one, the programme provides a way to bring their knowledge into the pairing through an expert who carries the governance in on their behalf.

**About the certificate**

The Solution Review certificate is issued by **Unitek Systems Limited** (UK company 04228041), as the originating organisation of UniVERSE, TrueAI, and UniCORE-AI. The certificate names the practitioner, the period for which it is current, and the L3 Scope-Domain CORE (or COREs) under which the practitioner is authorised to provide Solution Review services. The certificate is revocable. A revoked certificate ends the practitioner's authorisation to provide delegated Solution Review under the programme name, although it does not affect work already completed, published, and certified under a previously-current certificate.

**Bryan Fred, as Author and Creator of UniVERSE, TrueAI, and UniCORE-AI, holds this certificate by default.** The default-held certificate is a structural property of the Author/Creator role, not an issuance: it does not require nomination, application, examination, or external authorisation, because the certifying authority and the certificate-holder are, in this case, the same originating identity. The default certificate passes to any successor named under the [TrueAI whitepaper succession statement](https://github.com/bryanunitek/TrueAI/blob/main/docs/whitepaper/WHITEPAPER.md#8-succession-and-stewardship), on the same default-held basis, for as long as the succession process remains active. Successors do not need to be re-certified; they inherit the certificate as part of inheriting the role.

The full Solution Review certification scheme — criteria, examination, renewal, revocation, and the relationship between the certifying body and the L3 CORE governance layer — will be published as a separate programme document. Until that document is published, certificates other than the default-held certificate are issued by direct nomination by Bryan Fred and Unitek Systems Limited; the scheme will replace nomination with a public process once defined.

---

## 3. The rule behind the process

> **Get one human. Get one Claw. Begin.**
> **Choose the person with the most experience and knowledge of the
> solution.**

Three sentences. Each one is doing work. The five-step process in [§2](#2-the-process) is the operational expression of this rule. The sections below explain why each part of the rule is load-bearing.

---

## 4. Why one human

Solution review is production work. Production work under the
Foundation is bound by the
[Singular Pairing Principle](https://github.com/bryanunitek/TrueAI/blob/main/docs/10001-Singular-Pairing-Principle.md):
one human, one AI Claw per workstream. A committee at the session
level is ruled out by 10001 directly. This document is 10001 applied
to onboarding rather than to greenfield production.

A committee dilutes the pairing into a group dynamic the protocol
was never built for. A Claw receiving conflicting authority signals
from multiple humans cannot reconcile them without assuming
authority it does not have, which violates No Authority Assumption
and No Emergent Behaviour. The pairing breaks before any work has
been done.

The single human is the named author and certifier of the review
output. They are responsible for the decisions the Claw helps them
formulate. They are accountable to whichever governance layer the
Solution sits under.

---

## 5. Why one Claw

A Claw carries the governance of the layer it serves
([00058 §2.1](00058-Claw.md#21-claw)). A review of an existing solution
needs to happen *inside* that governance envelope, because the
output of the review will be claimed as Foundation-aligned work and
will be audited as such.

A MyClaw is the wrong tool for this work
([00058 §2.3](00058-Claw.md#23-myclaw)). A MyClaw carries no governance, no
attribution couplet, no audit trail against programme rules. Output
from a MyClaw cannot be claimed as Foundation-aligned. Using a
MyClaw to review an existing solution that the owner intends to
bring onto a CORE creates a provenance break at the most important
moment.

A separate Claw should be used for each distinct Solution being
reviewed ([TrueAI 10001](https://github.com/bryanunitek/TrueAI/blob/main/docs/10001-Singular-Pairing-Principle.md)).
A single Claw running multiple parallel solution reviews carries
context and assumptions across reviews and breaks traceability.

---

## 6. Why the most experienced human

This is the load-bearing choice. Three reasons.

### 6.1 The deepest knowledge goes in first

The Claw's initial understanding of the solution is shaped by
whoever teaches it. If the first human carries twenty years of
context about the solution, the Claw begins from twenty years. If
the first human carries six months, the Claw begins from six
months. Corrections later in the pairing cost time, trust, and —
most importantly — they leave a record that the foundation was
laid wrong and had to be rebuilt.

This is not a question of intelligence or skill. It is a question
of starting capital. The Claw starts with the knowledge the first
human brings. The right opening is the maximum.

### 6.2 The undocumented is what matters

Every long-running solution carries knowledge that is not in any
document. The workarounds adopted in 2014 because of a vendor bug
that has since been fixed but whose fix never propagated. The
configuration that looks wrong but is right because of an integration
the new team is not aware of. The decision not to adopt a feature
because of a regulatory question that was answered ten years ago and
has been quietly true ever since.

The most experienced human is the carrier of this material. They are
also frequently the only carrier — most of it has never been written
down because writing it down was nobody's job.

A Claw, well used, asks questions the human has not thought to
write. The pairing surfaces the undocumented and turns it into
material the Solution can audit, govern, and carry forward across
generations. That surfacing is the point of the review.

### 6.3 Institutional memory across the time horizon

A Foundation-aligned Solution is meant to last one hundred years,
one thousand years
([00057 §2 Time horizon of a Solution](00057-Layered-CORE-Model.md#time-horizon-of-a-solution)).
Across a horizon of that length, the institutional memory entering
the system at the first pairing is the seed of everything the
Solution will know about itself in century three.

The senior human will retire. They will not be the human at the
Claw in five years, in fifteen, in forty. What they teach the Claw
in the review is the bridge between their lived knowledge and the
Solution's continuing operation after they are gone.

This is not a metaphor. The Generation IT Succession charter
([TrueAI 10003](https://github.com/bryanunitek/TrueAI/blob/main/docs/10003-Generation-IT-Succession.md))
treats producer hand-off as a load-bearing mechanism. Solution
Review is the same mechanism applied to the existing solution
itself: the first pairing is the first generation. Whoever sits in
that pairing seeds the chain.

---

## 7. What the review produces

A Solution Review produces, at minimum:

- a **named Solution** with explicit attribution
  ([00057 §4 Attribution](00057-Layered-CORE-Model.md#4-attribution));
- a **declared CORE alignment** — which L3 CORE (if any) the
  Solution derives from, and which Foundation layers it builds on;
- a **content provenance map** — what is taken from CORE (and
  therefore propagates the gift), what is built fresh, and which
  pieces require explicit decisions
  ([00057 §3.2](00057-Layered-CORE-Model.md#32-what-take-content-from-core-means));
- a **human-of-record** — the senior human in the pairing, named
  as Solution author and certifier;
- a **Claw-of-record** — the specific Claw used for the review,
  identified for audit purposes.

Subsequent work on the Solution proceeds from the review output as
a starting baseline. The same human-Claw pairing may continue, or a
fresh pairing may take over under Generation IT Succession; either
way, the review output is what is handed over.

---

## 8. What the review is not

- It is not a deliverable that produces selling material. The output
  of a review is governance and provenance, not marketing. Sales
  and client-facing material derive from the Solution itself, not
  from the review.
- It is not a single sitting. A Solution worth reviewing will
  generally take many pairing sessions over weeks or months. The
  rule is that all of those sessions occur inside the same
  human-Claw pairing.
- It is not an excuse to skip
  [Certification Before Layered Governance](https://github.com/bryanunitek/TrueAI/blob/main/docs/10002-Certification-Before-Layered-Governance.md).
  A review brings a Solution into Foundation alignment; the
  Foundation's certification posture still applies before per-level
  governance documents are authored against the Solution.
- It is not a substitute for a CORE. If the Solution belongs in a
  vertical that does not yet have an L3 CORE, the review may
  identify content that should be lifted into a new CORE rather
  than retained in the Solution. That decision is a separate
  workstream and follows
  [00057 §3.1 Gift propagation](00057-Layered-CORE-Model.md#31-gift-propagation).

---

## 9. Relationship to other programme commitments

- The **Singular Pairing Principle**
  ([TrueAI 10001](https://github.com/bryanunitek/TrueAI/blob/main/docs/10001-Singular-Pairing-Principle.md))
  is the production rule this document specialises to onboarding.
- The **Layered CORE Model**
  ([00057](00057-Layered-CORE-Model.md))
  names the tier the reviewed Solution will sit in (Solutions tier)
  and the COREs the Solution may attribute against.
- **Claw vocabulary**
  ([00058](00058-Claw.md))
  defines the channel the human pairs with and distinguishes a Claw
  from a MyClaw.
- **Generation IT Succession**
  ([TrueAI 10003](https://github.com/bryanunitek/TrueAI/blob/main/docs/10003-Generation-IT-Succession.md))
  governs the human side of the pairing across the Solution's
  hundred-year horizon.

---

## 10. Status

This document, like all programme documents, is evolving. The
five-step process ([§2](#2-the-process)) and the three sentences of the rule ([§3](#3-the-rule-behind-the-process))
are settled. Future revisions may elaborate on review outputs
([§7](#7-what-the-review-produces)) and on the relationship to Certification ([§8](#8-what-the-review-is-not)) as more
Solutions are reviewed and the practical shape becomes clearer.

Public-facing changes to the Solution Review guidance will be
flagged in [HORIZON.md](../HORIZON.md).

---

— Bryan Fred, Unitek Systems Limited, Bedford, United Kingdom
