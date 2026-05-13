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

## 2. The rule

> **Get one human. Get one Claw. Begin.**
> **Choose the person with the most experience and knowledge of the
> solution.**

Three sentences. Each one is doing work.

---

## 3. Why one human

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

## 4. Why one Claw

A Claw carries the governance of the layer it serves
([00058 §2.1](00058-Claw.md)). A review of an existing solution
needs to happen *inside* that governance envelope, because the
output of the review will be claimed as Foundation-aligned work and
will be audited as such.

A MyClaw is the wrong tool for this work
([00058 §2.3](00058-Claw.md)). A MyClaw carries no governance, no
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

## 5. Why the most experienced human

This is the load-bearing choice. Three reasons.

### 5.1 The deepest knowledge goes in first

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

### 5.2 The undocumented is what matters

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

### 5.3 Institutional memory across the time horizon

A Foundation-aligned Solution is meant to last one hundred years,
one thousand years
([00057 §2 Time horizon of a Solution](00057-Layered-CORE-Model.md)).
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

## 6. What the review produces

A Solution Review produces, at minimum:

- a **named Solution** with explicit attribution
  ([00057 §4 Attribution](00057-Layered-CORE-Model.md));
- a **declared CORE alignment** — which L3 CORE (if any) the
  Solution derives from, and which Foundation layers it builds on;
- a **content provenance map** — what is taken from CORE (and
  therefore propagates the gift), what is built fresh, and which
  pieces require explicit decisions
  ([00057 §3.2](00057-Layered-CORE-Model.md));
- a **human-of-record** — the senior human in the pairing, named
  as Solution author and certifier;
- a **Claw-of-record** — the specific Claw used for the review,
  identified for audit purposes.

Subsequent work on the Solution proceeds from the review output as
a starting baseline. The same human-Claw pairing may continue, or a
fresh pairing may take over under Generation IT Succession; either
way, the review output is what is handed over.

---

## 7. What the review is not

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
  [00057 §3.1 Gift propagation](00057-Layered-CORE-Model.md).

---

## 8. Relationship to other programme commitments

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

## 9. Status

This document, like all programme documents, is evolving. The three
sentences of the rule (§2) are settled. Future revisions may
elaborate on review outputs (§6) and on the relationship to
Certification (§7) as more Solutions are reviewed and the practical
shape becomes clearer.

Public-facing changes to the Solution Review guidance will be
flagged in [HORIZON.md](../HORIZON.md).

---

— Bryan Fred, Unitek Systems Limited, Bedford, United Kingdom
