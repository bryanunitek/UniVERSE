# UniCORE AI Deep-Space Communication Protocols

**DelayAware Governance • Blackout Safety • Deterministic Messaging**

Author: Bryan Fred, Unitek Systems Limited, Bedford, United Kingdom
First published: May 2026
Status: Public. Given, not sold. Irrevocable.

---

## 1. Purpose

The Deep-Space Communication Protocols define how UniCORE AI:

handles communication delays

handles communication blackouts

maintains governance integrity

prevents autonomous decisionmaking

ensures deterministic behaviour

preserves human sovereignty

maintains mission safety during long silences

These protocols apply to:

lunar missions

Mars missions

asteroid belt missions

outerplanet probes

deep-space transit habitats

interstellar precursor missions

## 2. Communication Principles

2.1 Delay Does Not Grant Autonomy

UniCORE AI must never assume authority due to:

signal delay

signal loss

blackout

degraded bandwidth

2.2 Deterministic Behaviour Under Delay

All actions must remain:

predictable

reversible

logged

thresholdbound

2.3 No Autonomous Messaging

UniCORE AI cannot:

initiate communication

generate new message types

escalate without rules

broadcast without human instruction

2.4 Human Sovereignty

Even with a 40minute roundtrip delay, humans remain the final authority.

## 3. Communication Modes

UniCORE AI operates in four communication modes:

Mode 1 — RealTime (0–5 seconds)

Mode 2 — NearRealTime (5–60 seconds)

Mode 3 — DelayAware (1–40 minutes)

Mode 4 — Blackout Mode (40+ minutes or no signal)

Each mode has strict governance rules.

4. MODE 1 — REALTIME (0–5 seconds)

Used in:

lowEarth orbit

lunar surface

lunar orbit

UniCORE Behaviour

normal governance

normal ILMP messaging

immediate human override

Restrictions

no autonomous actions

no threshold changes

no selfgenerated messages

5. MODE 2 — NEARREALTIME (5–60 seconds)

Used in:

Earth–Moon operations

Lagrange point missions

UniCORE Behaviour

delayaware logging

preapproved safety actions only

no autonomous reconfiguration

Restrictions

cannot escalate without human confirmation

cannot initiate emergency protocols

6. MODE 3 — DELAYAWARE (1–40 minutes)

Used in:

Mars missions

asteroid belt missions

deep-space transit

UniCORE Behaviour

enters DelayAware Governance Mode

freezes noncritical operations

maintains thresholds

logs all drift events

queues outbound messages

Allowed Actions

stabilize within green/yellow bands

isolate failing subsystems

maintain life support

Prohibited Actions

autonomous maneuvers

autonomous habitat changes

autonomous hibernation actions

autonomous emergency declarations

Human Override

Overrides are queued and executed deterministically upon receipt.

7. MODE 4 — BLACKOUT MODE (40+ minutes or no signal)

Used in:

solar conjunction

radiation storms

antenna misalignment

deep-space shadow zones

UniCORE Behaviour

enters Blackout Governance Mode

freezes all noncritical operations

maintains life support

maintains environmental thresholds

prevents autonomous actions

logs all events locally

Allowed Actions

emergency stabilization

threshold enforcement

structural integrity protection

Prohibited Actions

ANY autonomous missionaltering action

ANY autonomous navigation

ANY autonomous habitat reconfiguration

ANY autonomous hibernation intervention

Blackout Exit

Upon signal restoration:

transmit full audit log

transmit drift log

await human instruction

do not resume suspended operations until authorized

## 8. Message Structure

UniCORE AI uses deterministic message packets:

MessageId

Timestamp (Mission Time)

SourceLevel

TargetLevel

PayloadHash

PayloadJson

GovernanceSignature

8.1 No SelfGenerated Messages

AI cannot create:

new message types

new routing rules

new governance signatures

## 9. Drift Detection During Delay

UniCORE AI must detect:

environmental drift

navigation drift

radiation drift

structural drift

governance drift

communication drift

RedBand Drift Behaviour

enter Safe Mode

freeze noncritical systems

log event

await human instruction

## 10. Navigation Communication Protocols

UniCORE AI must:

never initiate maneuvers

never correct course autonomously

never adjust trajectory

never fire thrusters

Allowed Actions

monitor

log

detect drift

escalate

## 11. Habitat Communication Protocols

UniCORE AI must:

maintain environmental thresholds

isolate failing subsystems

prevent cascade failures

Prohibited Actions

autonomous bulkhead control

autonomous power rerouting

autonomous atmospheric changes

## 12. Hibernation Communication Protocols

UniCORE AI must:

monitor vitals

detect anomalies

enforce thresholds

Prohibited Actions

autonomous revival

autonomous sedation

autonomous cycle changes

## 13. Emergency Communication Protocols

During emergencies:

UniCORE may stabilize

UniCORE may isolate

UniCORE may protect life support

But cannot:

declare missionlevel emergencies

alter mission parameters

override human authority

## 14. Interplanetary Law Alignment

UniCORE AI must comply with:

Outer Space Treaty

Artemis Accords

mission charters

habitat law

interplanetary governance MD files

AI cannot interpret treaties.

---

## Document history

- 2026-05-08 (7f420f6) — Initial commit: UniVERSE Foundation Documents (56 docs + Full Formal Statement)
- 2026-05-08 (189f14e) — Renumber 56 docs 001-056 for clean timeline sort order
- 2026-05-11 (6c1433f) — docs: add LinkedIn for private contact + normalise byline to Bryan Fred
- 2026-05-11 (0fe27ab) — docs: full formal byline — Bryan Fred, Unitek Systems Limited, Bedford, United Kingdom
- 2026-05-13 (fbebe5b) — docs: rename all 56 docs to 5-digit numeric codes, drop letter codes
- 2026-05-13 (c6a685b) — docs: Path-1 mechanical style pass on all numbered docs
- 2026-05-22 (9bcde37) — docs: complete version-marker sweep across public corpus

*Back-filled from git log on 2026-07-10 21:35 UTC. Kind 2 versioning (dated change notes) — see HORIZON.md § Evolution and versioning. Kind 1 (formal `Version:` bumps) remains OFF until first GitHub Discussion.*
