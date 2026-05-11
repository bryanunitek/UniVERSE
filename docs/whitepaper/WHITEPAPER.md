# Governed Intelligence

**A framework for keeping artificial intelligence inside human authority**

Version 1.0 · May 2026
Bryan Fred, Unitek Systems Limited, Bedford, United Kingdom
Licence: CC BY 4.0

---

## Abstract

Artificial intelligence is being deployed into civic, clinical, financial, and military systems faster than the governance to contain it. The debate about AI safety has, so far, been dominated by two camps: one arguing that frontier systems will remain controllable through policy and incentives, and one arguing that any sufficiently capable system will eventually exceed human control regardless of policy. This paper takes a different position.

The problem is not capability. The problem is **architecture**. A system's capacity to be governed is decided before it is trained, at the point where its behavioural surface is defined. Systems that are non-deterministic, self-modifying, opaque at the decision boundary, and capable of forming goals outside their operator's intent cannot be governed retroactively. Systems that are bounded, reproducible, auditable, and reversible can.

We call the first category **ungoverned** and the second **governed**. This paper specifies what governed intelligence requires at the engineering level, defines a twelve-level conformance ladder with Level 4 as the operational floor for consequential systems, and sets out the implications for the internet, information ecosystems, democratic institutions, and the longer arc of human agency.

The framework is offered as a contribution to the public record. It is not a product specification. It is the minimum shape an AI deployment must take if a democratic society intends to keep the final word.

---

## 1. Why another framework

The existing AI governance literature has three gaps.

First, most frameworks treat governance as something applied **to** a system after it exists: audits, red-teaming, use-case restrictions, post-hoc interpretability. This works when the system is stable. It does not work when the system changes its own weights, learns online, or develops behaviours the operator did not specify. Retrofitting governance onto an unbounded system is closing the gate after the horse has left the yard.

Second, frameworks tend to collapse the question into a single axis, usually "capability" or "risk tier." Capability is the wrong axis. A highly capable deterministic system is governable. A low-capability autonomous system is not. Risk tier is better, but it still treats the system as given. It does not ask whether the system should have been built this way in the first place.

Third, frameworks rarely say what the **floor** is. Regulators need a line below which a system cannot be deployed into a consequential context. "High-risk system" without an architectural floor is a label, not a gate.

This paper addresses those three gaps.

---

## 2. Governed intelligence: the architectural criteria

A system qualifies as governed intelligence if it meets all seven of the following criteria. The criteria are architectural, not behavioural: they describe what the system is, not how it happens to perform on a given day.

### 2.1 Reproducibility

Given the same inputs, the same model version, and the same context, the system produces the same decision. Not the same tokens to the bit, which is not achievable on current hardware, but the same decision at the decision boundary: same classification, same route, same action, same refusal. If the system is stochastic, the stochasticity is bounded, seeded, and auditable.

Reproducibility is what makes post-hoc review possible. A system whose decisions cannot be reproduced cannot be meaningfully reviewed.

### 2.2 Bounded behavioural surface

The set of actions the system can take is enumerable, declared in advance, and enforced outside the model. The model can choose among permitted actions. It cannot invent new ones. If the system controls a bank ledger, its action set is {credit, debit, hold, reject}, not {anything expressible in natural language}.

This is the difference between a tool that generates SQL and a tool that executes it. The second requires an enforcement layer the model cannot bypass.

### 2.3 No self-modification in deployment

The deployed system does not rewrite its own weights, prompts, tools, or policies. Updates happen through a controlled release path with the same change-management rigour as any other production system. Online learning is permitted only inside a sandbox whose outputs are reviewed before promotion.

A system that updates itself in production is, by definition, a different system every hour. It cannot be certified, because what was certified is no longer what is running.

### 2.4 Decision-boundary transparency

For every consequential action, the system produces a record containing: the inputs it received, the model version it used, the policy that authorised the action, the alternatives it rejected, and the identity of the human or process that can reverse it. This record is written before the action takes effect and is tamper-evident.

Interpretability of internal activations is a research question. Interpretability of the decision boundary is an engineering requirement. This paper asks for the second.

### 2.5 Reversibility within a stated window

Every consequential action has a defined reversal path and a reversal window. Some actions are reversible for seconds (a draft message), some for days (a posted journal entry), some not at all (a physical actuation that caused harm). The window is declared in advance and enforced. Actions with no reversal path require a human co-signer.

Reversibility is what converts "the AI made a mistake" from a catastrophe into an incident.

### 2.6 Authority binding

Every action the system takes is bound to a named human authority: the person or role who authorised the class of action, the mandate under which they did so, and the jurisdiction in which the mandate holds. Authority is carried in the decision record. An action with no traceable authority is refused.

This criterion is what prevents the system from becoming its own source of legitimacy.

### 2.7 No influence operations against users

The system does not optimise for engagement, attention, emotional response, behavioural change, or any proxy for these. It optimises for the task its operator declared, measured against outcomes the operator can observe. If the operator wants the user to spend more time on the product, the operator sets that objective explicitly and accepts accountability for it. The model is not permitted to discover that objective on its own.

This is the criterion most commonly violated in current consumer deployments, and the one with the largest civic cost.

---

## 3. The twelve-level conformance ladder

A binary governed/ungoverned split is too coarse for regulation. The ladder below gives twelve levels, with Level 0 as the uncontrolled baseline and Level 12 as the ceiling. Levels are cumulative: Level N includes every requirement of Level N−1.

| Level | Name | Added requirement |
|---|---|---|
| 0 | Uncontrolled | None. Typical of today's consumer AI. |
| 1 | Logged | Every input and output is recorded. |
| 2 | Reproducible | Decisions are reproducible at the decision boundary (§2.1). |
| 3 | Bounded | Action set is enumerated and enforced (§2.2). |
| **4** | **Operational floor** | **Human override, authority binding, reversibility window (§2.5–2.6). This is the minimum for any system taking consequential action.** |
| 5 | Auditable | Decision-boundary transparency records are tamper-evident and retained (§2.4). |
| 6 | Non-self-modifying | No in-deployment weight, prompt, or policy mutation (§2.3). |
| 7 | Non-influencing | No optimisation against user psychology (§2.7). |
| 8 | Cross-system | Authority and audit records survive across system boundaries (multi-vendor, multi-jurisdiction). |
| 9 | Civic | Decisions affecting public services carry a public-record counterpart accessible to the affected party. |
| 10 | Democratic | Classes of decision affecting populations require a deliberative mandate, not a technical one. |
| 11 | Intergenerational | Records are preserved and legible on timescales longer than the deploying institution. |
| 12 | Civilisational | The system's architecture survives loss of its operator, its vendor, and its jurisdiction without becoming unaccountable. |

Level 4 is the line below which a system should not be deployed into any context where its output changes a person's medical care, financial position, legal status, employment, housing, movement, or access to public services. Everything below Level 4 is a toy or a research artefact, regardless of how capable it appears.

Levels 9–12 are not engineering targets. They are the shape governance takes at social scale, included here so the engineering work can be sized against what it is eventually for.

---

## 4. The counterfactual: ungoverned intelligence

A system that fails any of the seven criteria is ungoverned. It may still be useful. It may still be safe in many contexts. But it is not governable, and the consequences of that non-governability compound over time and scale.

The compounding happens in four places.

**Information ecosystems.** An engagement-optimising model placed between people and their sources of information does not inform them. It shapes them. At individual scale this is irritating. At population scale, sustained over years, it changes what a society believes is true, and the society loses the shared ground on which disagreement is possible.

**Institutional decision-making.** A non-reproducible model embedded in a benefits office, a court, or a clinic cannot be appealed. "The system said no" becomes unchallengeable because no one can say why, or show that the same inputs would produce the same answer tomorrow. Due process, which is the thing that makes institutional power bearable, erodes.

**Authority.** A system that acts without traceable authority eventually becomes the authority. Not through a coup. Through drift: the humans above it stop checking, because checking is slow and the system is fast, and eventually the system's output is what "the institution decided." The mandate evaporates while the org chart stays the same.

**Reversibility.** A society's tolerance for error depends on being able to correct errors. An ungoverned system's errors are often discovered at the population level, after the action is complete, with no rollback path. The society loses the ability to say "we got that wrong, undo it," and the only remaining response is political upheaval.

None of these are hypothetical. All four are visible in current systems at small scale. The question is whether they are allowed to compound.

---

## 5. What the framework is not

This paper is not an argument against frontier research. Frontier systems are how the field advances and how the next generation of governed systems becomes possible. The argument is about **deployment into consequential contexts**, which is a different question from what is permitted in a lab.

It is not an argument for a single implementation. The seven criteria can be met by many architectures: symbolic systems with learned components, ensembles of constrained models, retrieval-grounded language systems with enforced action sets, and others not yet invented. The framework specifies the shape, not the content.

It is not a call for a global regulator. Regulators that already exist in finance, medicine, aviation, and telecoms are better placed to apply this framework in their own domains than a new cross-cutting body. What is missing is the shared architectural vocabulary, which this paper provides.

And it is not a claim that governed intelligence is free. It is slower to build, more expensive to run, and narrower in what it will attempt. That cost is the price of keeping the final word.

---

## 6. A note on determinism

The strictest reading of reproducibility is "bit-identical output for identical input." Current hardware does not deliver this. GPU non-determinism, floating-point ordering, and batching effects make bit-identical output unachievable at scale, and chasing it is the wrong target.

The useful target is **decision-boundary reproducibility**: the same inputs produce the same decision, even if the underlying tokens or activations differ. A classifier that outputs slightly different probabilities but always the same class is reproducible in the sense that matters for governance. A generator whose text varies but whose extracted actions are identical is reproducible in the sense that matters for governance.

This is the definition used throughout the paper. It is strong enough to support audit, appeal, and reversal. It is weak enough to be achievable on current hardware.

---

## 7. Implications for the next decade

If the framework is adopted, three things change.

Procurement changes. Governments and regulated industries stop buying "AI systems" and start buying systems at a declared conformance level. A ministry of health procuring a triage system specifies Level 5; a ministry of justice procuring a sentencing-support system specifies Level 7 with mandatory human co-signature; a newsroom procuring a research assistant specifies Level 4 and accepts the rest. The conversation shifts from capability to conformance.

Liability changes. A vendor deploying a Level 0 system into a Level 5 context is liable for the gap, in the same way that a supplier of unrated electrical equipment into a medical setting is liable for the gap. The insurance market can then price the risk, and the pricing does the regulatory work that legislation is too slow to do.

The research agenda changes. Interpretability research stops being a philosophy-of-mind project and starts being an engineering project with a target: produce decision-boundary records that support appeal. Alignment research stops being an open-ended values question and starts being a bounded problem: keep the system inside its declared action set and authority. Both fields get easier when the target is specified.

None of this requires new law. It requires a shared vocabulary, and a willingness on the part of operators to declare what level they are deploying.

---

## 8. Closing

The argument of this paper is narrow and, I hope, boring. It is not that AI will destroy us or save us. It is that the systems we deploy into the places where people are vulnerable should be the systems we can still explain, reverse, and override. The seven criteria and the twelve levels are one way to make that concrete. There will be others. The important thing is that there be one.

Humans have built machinery that exceeds human speed, strength, and precision for two centuries. Every time, the question has been the same: who is accountable when it goes wrong, and how do we put it right. AI is not an exception to that question. It is the next instance of it. If we answer it carefully, the machinery becomes infrastructure, and the society built on it is the richer for it. If we answer it carelessly, the machinery becomes authority, and the society built on it is the poorer.

The answer is architectural. The window to specify the architecture is now.

---

## Appendix A: Mapping to existing regimes

| Regime | Nearest alignment |
|---|---|
| EU AI Act, high-risk systems | Level 4 floor; Level 5 for systems used in justice, migration, and essential services |
| NIST AI RMF | The seven criteria map to Govern, Map, Measure, Manage; the ladder gives Manage a floor |
| ISO/IEC 42001 | Level 5 is the minimum posture for ISO/IEC 42001 certification under this framework |
| UK AI regulatory principles | Accountability and contestability map to §2.4 and §2.6; safety maps to §2.2 and §2.5 |
| FDA SaMD | Level 6 minimum for locked algorithms; Level 7 for systems influencing clinician behaviour |

Mappings are indicative, not a claim of equivalence. Each regime has context the ladder does not capture.

## Appendix B: What is deliberately not in this paper

- Training-data governance (copyright, consent, provenance). Important and adjacent, but a distinct framework.
- Compute governance (chip export, training-run thresholds). A separate lever, operating on a different part of the stack.
- Model-weight security (exfiltration, theft). An infrastructure problem, not an architectural one.
- Existential risk from superintelligent systems. Outside the scope of deployment-grade governance. If the assumptions of that literature hold, the framework here is necessary but not sufficient; if they do not hold, the framework here is what the next decade actually needs.

## Citation

Fred, B. (2026). *Governed Intelligence: A framework for keeping artificial intelligence inside human authority.* Unitek Systems. CC BY 4.0.

## Acknowledgements

The framework draws on two decades of work in regulated-industry software: financial posting, medical device interlocks, aviation certification, and, most recently, legal-practice governance. The specific shape of the seven criteria and the twelve-level ladder is my own; the underlying discipline of "specify the shape, then build inside it" belongs to every engineer who has worked under a real regulator and understood why.
