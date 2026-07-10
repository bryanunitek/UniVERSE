# Layered CORE Model

**The four-tier architecture of UniVERSE / TrueAI / UniCORE AI**

Author: Bryan Fred, Unitek Systems Limited, Bedford, United Kingdom
First published: May 2026
Status: Public. Given, not sold. Irrevocable.

---

## 1. Purpose

This document specifies the layered architecture of the UniVERSE
programme. It names four tiers — three of CORE (gifted, not sellable)
and one of Solutions (services-built, sellable). It states the
derivation rule that decides whether new work joins a CORE tier or
the Solutions tier. It names the attribution requirements that
accompany each origin.

It is the architectural reference for any party building on the
Foundation. Programme materials in UniVERSE, TrueAI, and UniCORE-AI
that touch on Solutions, derivation, or commercial conduct refer
back to this document.

A companion treatment of the same model, at the scale of
civilisational and inter-body governance, is in
[HORIZON.md](../HORIZON.md) under "Long horizon."

---

## 2. The four tiers

### Level 1 CORE — TrueAI Foundation

The Nine Invariants and the governance principles that any AI system
in a critical decision path must satisfy. Universal. Vertical-agnostic.
Jurisdiction-agnostic. Body-agnostic.

Gift. Not sellable. Not licensable beyond CC BY 4.0.

### Level 2 CORE — UniCORE AI

The 12-level reference architecture that implements the TrueAI
Foundation in working form. Inter-level messaging protocol, reasonable
governance threshold, human override protocol. Universal.

Gift. Not sellable. Not licensable beyond CC BY 4.0.

### Level 3 CORE — Scope-Domain CORE

A reference library specific to a particular scope domain. A scope
domain may be:

- A **vertical** — an industry sector (Law, Medical, Accountancy, etc.).
- A **jurisdiction** — a sovereign entity at any level (federal, state,
  county, city, parish) that chooses to anchor to the Foundation.
- A **body** — an inhabited body (Earth, Moon, Mars, etc.).
- A **network fabric** — a communication-bound scope such as an
  inter-body fabric or a detached craft in transit.

Multiple peer COREs may exist for any single scope domain. Two
different organisations may produce two different Vertical COREs for
the Law sector; both are L3 CORE, both gifted, both sit at the same
tier.

UniCORE.Law-Claw is the first L3 Scope-Domain CORE — the Vertical CORE
for the Law sector, produced by Unitek.

Gift. Not sellable. Not licensable beyond CC BY 4.0.

#### When a Vertical CORE prototype is required to be public

A Vertical CORE prototype — any L3 Scope-Domain CORE under
development, intended for use by more than one client, or intended
as a reusable reference library for a sector — is required to be
published publicly **at the point it qualifies to display the
attribution couplet defined in [§4](#4-attribution).** Until it
qualifies, it may remain private; private during prototype phase is
the correct posture, because the prototype has not yet demonstrated
conformance to the Foundation and to UniCORE AI.

This applies to any producer, not only to Unitek. The trigger is
**scope** (multi-client / reusable-vertical intent), not identity.

A single-client deliverable, by contrast, sits in the Solutions tier
below. It is not a Vertical CORE, regardless of who builds it. It
may remain private indefinitely. The line that separates a Vertical
CORE from a Solution is the line that separates mandatory-public
from optional-private.

### Solutions tier (not CORE)

A specific client's working implementation, built by a
Generation IT producer pair on top of the relevant CORE layers. A
Law Firm's Solution, derived from the UniCORE.Law-Claw L3 CORE, powered
by UniCORE AI, built on the TrueAI Foundation, is in the Solutions
tier.

Services-built. Sellable as services-delivered work. Required to
attribute its CORE origins (see [§4](#4-attribution)).

The Solutions tier is where commercial value lives. The CORE tiers
above it are explicitly outside the commercial layer.

#### Time horizon of a Solution

The time horizon of an Enterprise Solution built on this stack is
**not** today's ten-to-twenty year enterprise software lifecycle.
That is the beginning. An Enterprise Solution produced by a
Generation IT pair, on Foundation-aligned CORE, is meant to last
**one hundred years, one thousand years.**

This is a deliberate break from the replace-every-decade pattern of
today's enterprise software. Foundation-aligned Solutions are
expected to carry the same critical decision work across many human
generations. The CORE tiers above (L1, L2, L3) are themselves
gifted and perpetual; the Solution built on them is expected to
sustain the same time horizon as the CORE it rests on.

#### How the time horizon is sustained

A Solution with a hundred-year or thousand-year horizon outlasts
its original producer pair by many human generations. Two mechanisms
carry it forward.

The **Generation IT Succession charter**
([TrueAI 10003](https://github.com/bryanunitek/TrueAI/blob/main/docs/10003-Generation-IT-Succession.md))
is the producer hand-off mechanism. It is not only a quality floor
for initial production; it is the explicit path by which producer
authority transfers from one generation of Generation IT producers
to the next, without breaking continuity of the Solution.

**Harmony, mutual respect, and peace** are the relational substrate
on which the Solution rests. At a timespan of ten-plus human
generations, no volume of compliance, authority, or coercion can
sustain a working system. Only genuine harmony scales that far. At
this horizon harmony is not aspirational language; it is the
material out of which the Solution is built. The Foundation's
commitment to harmony is therefore a structural requirement of
Solutions built on it, not a values statement bolted on to a
technical project.

#### How model-window saturation is handled at this horizon

A Solution with a hundred-year or thousand-year horizon will run
through many generations of model technology. No model's context
window survives that span. The mechanism that lets governance
survive the gap is that the model's context window is not the
governed context.

The **governed substrate** — the active corpus references, the
principal identity surface, the pending decision graph, the
attestation snapshot, the audit trail — lives in durable storage,
independent of any model's window. When a window saturates, the
deployment compacts according to a fixed rule: a documented pinned
set stays in the active window, everything else is summarised with
hash-anchored references back to the durable record. Compaction
itself is a recorded governed event.

A future model with a different window size reads the same governed
substrate that today's model reads. This is the system-side analogue
of Generation IT Succession: the producer side carries forward across
human generations, the substrate side carries forward across model
generations. Both are required for the time horizon to hold.

Full treatment in
[UniCORE-AI 20002 — Compaction and Durable Continuity](https://github.com/bryanunitek/UniCORE-AI/blob/main/docs/20002-Compaction-And-Durable-Continuity.md).

---

## 3. The derivation rule

Whether new work joins a CORE tier or the Solutions tier is decided
by a single rule:

> **If new work takes content from an existing CORE, the new work is
> CORE.**
> **If new work builds fresh on the layer above without taking CORE
> content, the new work is a Solution.**

Take-from-CORE → the new work is CORE → gifted, not sellable.
Build-fresh-on-layer-above → the new work is a Solution → sellable as
services output, with required attribution.

This is the line that decides whether a piece of work belongs in the
CORE layers (L1, L2, or L3) or in the Solutions tier.

### 3.1 Gift propagation

A derivative of CORE is itself CORE, and is itself gifted. Every
chain of derivation stays collectively free. CORE cannot be converted
to private property at any link in any chain.

If `<3rd Party 1>` takes content from UniCORE.Law-Claw and produces
`<3rd Party 1>-Law-Claw`, then `<3rd Party 1>-Law-Claw` is itself L3 CORE.
`<3rd Party 1>` may not sell it. If `<3rd Party 2>` then takes
content from either `<3rd Party 1>-Law-Claw` or UniCORE.Law-Claw to produce
`<3rd Party 2>-Law-Claw`, then `<3rd Party 2>-Law-Claw` is itself L3 CORE.
And so on, forward through every chain.

Gift propagation is the architectural mechanism that prevents
anyone — including the original producer — from converting shared
CORE into private property.

### 3.2 What "take content from CORE" means

Taking content from CORE includes, without limit:

- copying Business Objects or Business Logic from the CORE,
- copying schema or data structures from the CORE,
- copying configuration, rules, or workflow definitions from the CORE,
- adapting any of the above with modifications.

Building fresh on the layer above means writing new Business Objects,
new Business Logic, new schemas, new configurations — without taking
content from any CORE layer below.

A Solution that uses UniCORE AI (L2) as substrate but writes its own
domain content from scratch is a Solution. A Solution that copies
content from a Vertical CORE (L3) into itself absorbs CORE status
through that copying and itself becomes CORE.

---

## 4. Attribution

All work that depends on the Foundation, whether CORE or Solution,
must attribute its origins. Three forms cover the cases.

For a Vertical CORE, the right to display this attribution is also
the public quality gate. A Vertical CORE earns the right to display
the couplet by demonstrating conformance to everything published
in the TrueAI and UniCORE AI repositories, by mutual agreement
between its producer pair and the Foundation stewards. The Solutions
tier inherits the right by deriving from a Vertical CORE that
already holds it, or by building directly on TrueAI + UniCORE AI
without L3 CORE content.

Three forms cover the cases:

### 4.1 Solution built on TrueAI + UniCORE AI, no L3 CORE used

> Powered by UniCORE AI · Built on the TrueAI Foundation

### 4.2 Solution built using L3 CORE content

> Powered by UniCORE AI · Built on the TrueAI Foundation
> · Derived from `<L3 CORE name>`

Example: a Law Firm Solution that takes Business Objects from
UniCORE.Law-Claw would carry:

> Powered by UniCORE AI · Built on the TrueAI Foundation
> · Derived from UniCORE.Law-Claw

This Solution is itself CORE under the gift propagation rule (because
it took content from L3 CORE). It cannot be sold. The attribution
makes the gift-chain participation visible.

### 4.3 L3-peer CORE derived from another L3 CORE

> `<3rd Party N>-Law-Claw` · Derived from UniCORE.Law-Claw
> · Powered by UniCORE AI · Built on the TrueAI Foundation

Example: `<3rd Party 1>-Law-Claw`, an L3 Vertical CORE for the Law
sector produced by a third party who took content from
UniCORE.Law-Claw, would carry:

> `<3rd Party 1>-Law-Claw` · Derived from UniCORE.Law-Claw
> · Powered by UniCORE AI · Built on the TrueAI Foundation

The "Derived from" line marks gift-chain participation. It also
marks that the derived work is itself CORE and unsellable, which
is the legal-mechanical signal a Client or competitor needs.

---

## 5. Naming conventions

- **L3 Vertical COREs** use the `UniCORE-<vertical>-Claw` naming
  pattern, where `<vertical>` is the scope domain. Examples:
  `UniCORE.Law-Claw` (the Law-sector reference Vertical CORE),
  `UniCORE-Medical-Claw`, `UniCORE-Banking-Claw`, etc. The `-Claw`
  suffix marks the channel as a governed Claw
  (see [00058 §2.1](00058-Claw.md#21-claw)); the vertical token
  narrows the scope domain. Third-party L3 Vertical COREs follow the
  same pattern: `<3rd Party 1>-<vertical>-Claw`.
- **L3 Body COREs** use the `Uni-` prefix with the body name
  (UniEARTH, UniLUNA, UniMARS, etc.).
- **L3 Jurisdiction COREs and L3 Fabric COREs** do not yet have
  fixed naming conventions; these are reserved for future
  specification when adopted.

UniVERSE is the umbrella programme that publishes L1 + L2 as a
coherent whole. It is not itself a CORE tier.

---

## 6. Enforcement

Gift propagation is a norm until it is enforced. CC BY 4.0 alone
does not enforce it — under CC BY 4.0 a third party may modify a
CORE work and sell the derivative, provided they preserve attribution
and do not misrepresent authorship.

Enforcement comes from three layers operating together:

1. **CC BY 4.0** on the source content of each CORE — preserves the
   gift at the level of the source itself.
2. **Trademark** on naming conventions (the `-Claw` suffix, the
   `Uni-` prefix for body COREs, and the names of specific COREs
   such as UniCORE.Law-Claw, UniEARTH, etc.) — prevents derivatives
   passing themselves off as originals.
3. **Certification mark** on TrueAI / UniCORE AI with regulations
   that include gift propagation as a binding requirement on
   mark users. A derivative-seller loses access to the mark, and
   therefore loses Foundation-aligned status and the public trust
   anchor that accompanies it.

The Foundation does not prevent a third party from forking a CORE
work and selling the derivative under their own un-attributed name.
It prevents them from doing so under the marks and naming conventions
that signal Foundation alignment.

---

## 7. Relationship to other programme commitments

The Layered CORE model is the structural architecture of the
programme. Several programme commitments depend on it:

- The **Gift Principle**
  ([00028](../docs/00028-TrueAI-Foundation-Gift-Principle.md))
  is the value-statement that motivates the CORE tiers being
  gifted. The Layered CORE model is the operational expression of
  that principle across multiple tiers and scope domains.
- The **Singular Pairing Principle**
  ([TrueAI 10001](https://github.com/bryanunitek/TrueAI/blob/main/docs/10001-Singular-Pairing-Principle.md))
  binds production of Solutions and Scope-Domain COREs to one
  human + one AI per workstream. The Layered CORE model names the
  output tiers; Singular Pairing names the production unit.
- **Certification Before Layered Governance**
  ([TrueAI 10002](https://github.com/bryanunitek/TrueAI/blob/main/docs/10002-Certification-Before-Layered-Governance.md))
  requires the Foundation to be in place before per-level
  governance documents are applied. This applies to every tier of
  CORE: a Vertical CORE may not have Region/Country/State/
  Organisation governance documents authored against it until that
  CORE itself has passed Certification.
- **Generation IT Succession**
  ([TrueAI 10003](https://github.com/bryanunitek/TrueAI/blob/main/docs/10003-Generation-IT-Succession.md))
  binds the human side of the production pair to the Generation IT
  qualification standard. The first Vertical CORE in a vertical
  requires full-vertical-experience Generation IT; subsequent
  Solutions and COREs in the same vertical have a wider eligible
  producer pool.

The Layered CORE model does not replace any of those documents. It
sits alongside them as the structural reference.

---

## 8. What this document is not

- It is not a licence. The licence is CC BY 4.0, in
  [LICENSE.md](../LICENSE.md).
- It is not a delivery plan. Delivery is governed by working
  practice in each repo's `AGENTS.md`.
- It is not an exhaustive specification of every scope domain.
  Vertical, jurisdiction, body, and fabric scope domains are
  named; future scope domains may exist that are not yet specified.
- It is not a claim that the model is the only architecture
  compatible with the TrueAI Foundation. Other architectures may
  be developed by other producers. The Foundation does not require
  them to use the Layered CORE model; it requires them to satisfy
  the Nine Invariants.

---

## 9. Status

This document, like all programme documents, is evolving. Its
`Version` line is a statement revision number, not a programme
release version. The architectural envelope — three tiers of CORE,
one tier of Solutions, gift propagation as the derivation rule —
is stable. Specific naming conventions and attribution forms may
be refined.

Public-facing changes to the Layered CORE model itself will be
flagged in [HORIZON.md](../HORIZON.md).

---

— Bryan Fred, Unitek Systems Limited, Bedford, United Kingdom

---

## Document history

- 2026-05-13 (65dc967) — docs/00057: Layered CORE Model
- 2026-05-13 (6bd9ba1) — docs: Solution time horizon is 100/1000 years, not 10-20
- 2026-05-13 (ece9c77) — docs: lock versioning at 1.0 until first GitHub Discussion
- 2026-05-13 (8201f00) — docs: wrap every section sign (§) reference inside a markdown link
- 2026-05-15 (3bf96df) — docs: 00057 + 00058 — forward-link to 20001/20002
- 2026-05-15 (51903df) — docs(rename): UniCORE-Claw → UniCORE-Law-Claw under new naming pattern
- 2026-05-15 (82fb73a) — docs: surface multi-client mandatory-public rule, Badge as quality gate, and reserved UniCORE-Claw name
- 2026-05-22 (96a956a) — fix(public-corpus): repository enumerations updated 3 -> 5 (Foundation triad + gift-layer extension)
- 2026-05-22 (9bcde37) — docs: complete version-marker sweep across public corpus

*Back-filled from git log on 2026-07-10 21:35 UTC. Kind 2 versioning (dated change notes) — see HORIZON.md § Evolution and versioning. Kind 1 (formal `Version:` bumps) remains OFF until first GitHub Discussion.*
