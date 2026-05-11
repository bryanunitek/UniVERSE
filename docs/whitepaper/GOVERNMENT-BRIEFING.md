# Governed Intelligence — briefing for policymakers

**A proposed architectural floor for AI systems in consequential use**

Version 1.0 · May 2026 · Unitek Systems Limited · CC BY 4.0

---

## The problem in one page

AI systems are being placed in the decision path for medical triage, benefits eligibility, loan approval, policing, hiring, education, and public communications. The policy response so far has focused on three things: risk tiering, transparency obligations, and sectoral guidance. These are useful but insufficient. They assume the system can be governed once it exists.

Many current systems cannot. They update themselves in deployment. They produce different decisions for the same inputs. They have no enumerated action set. They cannot explain which alternatives they rejected. They cannot be reversed. They are not bound to a named human authority. A regulator inspecting such a system after an incident has nothing to inspect.

The gap is architectural, not legal. A statute requiring accountability cannot produce accountability if the system was not built to support it.

## The proposal

An AI system deployed into a consequential context should meet seven architectural criteria before deployment:

1. **Reproducibility** — same inputs produce the same decision at the decision boundary.
2. **Bounded action surface** — the set of actions the system can take is enumerated and enforced outside the model.
3. **No self-modification in deployment** — weights, prompts, and policies change only through a controlled release path.
4. **Decision-boundary transparency** — every consequential action produces a tamper-evident record of inputs, model version, authorising policy, rejected alternatives, and reversal authority.
5. **Reversibility** — every consequential action has a defined reversal path and window, or a human co-signer if no reversal is possible.
6. **Authority binding** — every action is bound to a named human role, mandate, and jurisdiction.
7. **Non-influence on the operator** — the system does not shape the behaviour or belief of the humans supervising it.

A system that meets all seven is **governable**. A system that fails one is not.

## The ladder

The white paper defines twelve levels of conformance. Level 4 is proposed as the floor for consequential deployment. Indicative mapping:

| Use case | Minimum level |
|---|---|
| Personal productivity, creative work | not regulated under this framework |
| Customer-facing assistants, search | Level 3 |
| Internal enterprise decision support | Level 4 |
| Financial posting, legal document generation | Level 5 |
| Medical triage, clinical decision support | Level 6 |
| Public-sector benefits and rights decisions | Level 7 |
| Ranking systems affecting public information at scale | Level 8 |
| Autonomous physical actuation in public space | Level 9 |

Higher levels add cultural, economic, and long-horizon governance and are relevant to infrastructure operating over decades.

## What this changes for policy

Most existing AI regulation can adopt this framework without rewriting primary legislation. The framework supplies the **technical floor** that phrases like "appropriate safeguards" and "human oversight" currently leave undefined.

Specifically, regulators can:

- **Require conformance evidence at market entry.** A vendor selling an AI system into a regulated context must demonstrate which level their system meets against each of the seven criteria. The evidence is architectural, not behavioural, so it can be assessed before deployment rather than after harm.
- **Define minimum levels by sector.** Healthcare, financial services, public administration, and information ranking each need a declared floor. The table above is a starting point.
- **Bind procurement to conformance.** Public-sector AI procurement can require Level 7 minimum as a condition of contract award. This alone would reshape the market.
- **Require continuous conformance.** A system that modifies itself out of conformance must be taken out of the consequential path until reassessed.

The framework does not require new institutions. It requires existing regulators to specify the shape of the systems they will accept.

## What this does not do

It does not ban any class of AI. Research, creative work, and exploration are outside its scope. It does not solve training-data governance, compute governance, or model-weight security. Those are adjacent levers operating on different parts of the stack. It does not address hypothetical superintelligent systems; it addresses the systems being deployed now.

It also does not resolve the political question of who decides which level is required where. That remains a decision for legislatures and regulators. The framework gives them a vocabulary that is precise enough to legislate with.

## Suggested next steps

1. Assign a named body to assess current in-scope AI deployments against the seven criteria.
2. Publish a draft sectoral mapping for public comment.
3. Add conformance evidence to existing procurement frameworks for consequential AI.
4. Require incident reporting that cites which criterion failed, not which outcome occurred.
5. Revisit at twelve months. The framework is versioned; so should the policy be.

## Why this is worth reading

The critique of current AI safety approaches is not that they are wrong. It is that they operate downstream of a decision that was made upstream: the decision about what shape the system would take. By the time a regulator is evaluating a deployed system, the governable-or-not question has already been answered by the builder. This framework moves the decision forward to where it can still be made.

---

**Full paper.** *Governed Intelligence: A framework for keeping artificial intelligence inside human authority.* Fred, B. (2026). Unitek Systems. CC BY 4.0.

**Contact.** bryan@unitek-systems.co.uk

**Licence.** CC BY 4.0 — free to cite, adapt, and incorporate into policy work with attribution.
