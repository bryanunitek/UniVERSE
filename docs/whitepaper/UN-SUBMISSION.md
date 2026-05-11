# Stakeholder submission on the governance of artificial intelligence

**Submitted by:** Bryan Fred, Unitek Systems Limited (United Kingdom)
**Date:** May 2026
**Licence:** CC BY 4.0
**Route:** General stakeholder contribution, adaptable to UNESCO Recommendation on the Ethics of Artificial Intelligence follow-up, the Global Digital Compact implementation track, and ITU AI for Good stakeholder processes.

---

## Purpose of this submission

This submission proposes an **architectural floor** for artificial intelligence systems deployed into consequential decision contexts. The floor is intended to complement, not replace, existing normative instruments, in particular the UNESCO Recommendation on the Ethics of Artificial Intelligence (2021) and the commitments under the Global Digital Compact. It provides the technical specificity that those instruments, by design, do not contain.

The submission is offered freely, under a Creative Commons Attribution licence, with no commercial interest in its adoption.

## The gap addressed

Current international instruments on AI ethics articulate principles — human oversight, accountability, transparency, fairness, safety — that States and operators are expected to implement. The principles are sound. The implementation gap is that most deployed AI systems are architecturally incapable of supporting them.

A system whose decisions cannot be reproduced cannot be audited. A system whose action set is not enumerated cannot be bounded. A system that modifies itself in production cannot be certified, because what was certified is not what is running. A system that cannot be reversed cannot be held accountable in any operational sense.

Principle-level commitments, without an architectural floor, produce compliance on paper and failure in practice. This submission proposes the missing floor.

## The proposed criteria

A system deployed into a consequential context — defined as one where its outputs affect a person's rights, livelihood, health, liberty, or access to public services — should meet seven architectural criteria:

1. **Reproducibility of decisions at the decision boundary.**
2. **An enumerated and externally enforced action surface.**
3. **No self-modification in deployment outside a controlled release path.**
4. **A tamper-evident record, produced before each consequential action, containing inputs, model version, authorising policy, rejected alternatives, and reversal authority.**
5. **A declared reversal path and window for each action, or a named human co-signer where reversal is not possible.**
6. **Binding of every action to a named human role, mandate, and jurisdiction.**
7. **A prohibition on the system shaping the behaviour or belief of the humans who operate it.**

A conformance ladder of twelve levels is described in the accompanying white paper. Level 4 is proposed as the minimum for any consequential deployment. Higher levels are proposed for medical, public-administration, information-ranking, and long-horizon infrastructure uses.

## Relation to existing instruments

**UNESCO Recommendation on the Ethics of Artificial Intelligence (2021).** The seven criteria operationalise the Recommendation's principles of human oversight and determination, transparency and explainability, responsibility and accountability, and safety and security. They do not add new principles. They specify what a system must be, architecturally, for those principles to be enforceable.

**Global Digital Compact.** The framework supports the Compact's objective of promoting a safe, secure, and trustworthy digital future. It offers a testable specification that Member States and platforms can reference in national implementation plans.

**OECD AI Principles (2019, updated 2024).** The criteria are consistent with the principles of robustness, security and safety, and accountability, and provide a shared vocabulary for cross-border assessment.

**ISO/IEC 42001 (AI management systems).** Level 5 of the conformance ladder corresponds approximately to the management-system posture required by ISO/IEC 42001. The framework is offered as compatible with, not competing against, that standard.

## Suggested actions

For the consideration of Member States, UN entities, and stakeholders:

1. **Reference an architectural floor in national AI strategies.** Principle-level language remains appropriate at the international level. An architectural floor is appropriate at the national implementation level.
2. **Attach conformance evidence to public-sector AI procurement.** A vendor supplying AI into a public-sector consequential-decision path should demonstrate which level of conformance the system meets, assessed before deployment.
3. **Include architectural criteria in capacity-building programmes.** Regulators in jurisdictions that are building AI oversight for the first time benefit more from a concrete specification than from a principle restated.
4. **Align incident reporting.** Post-incident reporting should name the criterion that failed — reproducibility, reversibility, authority binding — rather than only the outcome. This converts incidents into evidence about architectural gaps.
5. **Review periodically.** The framework is versioned and is offered on the understanding that it will be revised as practice develops. International instruments might benefit from the same discipline.

## Scope, limits, and invitations

This submission does not address training-data governance, compute governance, model-weight security, or the long-term question of systems that may exceed current capability envelopes. Those are adjacent questions operating on different parts of the stack. The framework here is a necessary contribution, not a sufficient one.

The framework is offered as a contribution to the public record. Member States, UN entities, regional bodies, national regulators, and civil-society organisations are invited to adopt, adapt, translate, and extend it, with attribution, under the terms of CC BY 4.0.

## Author and contact

Bryan Fred
Senior Solutions Architect, Unitek Systems Limited (United Kingdom) and Unitek Systems USA Inc.

All contact via GitHub Discussions: https://github.com/bryanunitek/UniVERSE/discussions

The full framework is set out in: Fred, B. (2026). *Governed Intelligence: A framework for keeping artificial intelligence inside human authority.* Unitek Systems. CC BY 4.0.

---

*This submission is offered in the author's personal and professional capacity as a practitioner. It does not represent the position of any government, intergovernmental body, or standards organisation.*
