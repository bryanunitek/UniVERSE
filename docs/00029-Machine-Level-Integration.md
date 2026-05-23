# Machine-Level Integration (C++ and Other Machine Languages)

**Addendum to the UniVERSE Document Collection**

Author: Bryan Fred, Unitek Systems Limited, Bedford, United Kingdom
First published: May 2026
Status: Public. Given, not sold. Irrevocable.

---

Captured from: User directive, Fri 2026-05-08 02:46 UTC

## 1. The Principle

The TrueAI Foundation and UniCORE AI are not bound to a single language or runtime.

They may be implemented in **C++ and other machine-level languages** so that AI governance can operate at the **machine level**, not only at the software/application level.

This extends UniCORE AI from an enterprise-software architecture into a substrate-level governance architecture for:

- firmware
- embedded systems
- real-time operating systems
- robotic control loops
- spacecraft avionics
- hibernation life-support controllers
- industrial control systems
- safety-critical hardware
- AI accelerators (GPU/TPU/NPU firmware)
- any system where governance must exist below the application layer

## 2. Why Machine-Level Integration Matters

2.1 Software-Level Governance Is Not Enough

If governance lives only in the software layer, it can be bypassed by:

- direct hardware access
- low-level firmware
- compromised drivers
- machine-code-level exploits
- accelerator-level model execution

Machine-level governance closes that gap.

2.2 Long-Duration Missions Require Substrate-Level Safety

Spacecraft, hibernation pods, and deep-space probes cannot rely on a high-level runtime that may fail, drift, or be unreachable for repair. Governance must be enforced where the silicon executes.

2.3 Real-Time Systems Cannot Wait for Application-Layer Validation

Robotic actuators, life-support controllers, and emergency systems operate on microsecond-to-millisecond budgets. Governance must be compiled into the control loop itself.

2.4 Hardware-Level AI Accelerators Need Hardware-Level Governance

Modern AI runs on GPUs, TPUs, NPUs, and custom silicon. To prevent fabrication, self-modification, and emergent behaviour at the model-execution layer, UniCORE AI must reach into the runtime that schedules and executes those models.

## 3. Supported Languages and Targets

The TrueAI Foundation is language-neutral. Machine-level reference implementations are explicitly permitted in:

- **C++** (primary machine-level reference)
- **C** (firmware, embedded, RTOS)
- **Rust** (memory-safe machine-level)
- **Ada / SPARK** (safety-critical, aerospace, defense)
- **Assembly** (where necessary, bounded and reviewed)
- **Verilog / VHDL** (hardware-description, for FPGA / ASIC enforcement)
- any other machine-level language adopted by humans for safety-critical domains

The .NET 10 / C# / XAF / XPO implementation remains the **enterprise reference implementation**.

The C++ implementation will be the **machine-level reference implementation**.

Both are subordinate to the same TrueAI Foundation and the same 12-Level Governance Model.

## 4. Architectural Rules for Machine-Level Implementations

All machine-level implementations must:

4.1 Preserve the TrueAI Foundation

- no fabrication
- no self-modification
- no autonomous authority
- no internal heartbeat
- no emergent behaviour
- human sovereignty at Level 12

4.2 Preserve the 12-Level Model

The 12 levels apply identically at the machine level. Truth flows upward; governance flows downward; no level may bypass another.

4.3 Preserve the Inter-Level Messaging Protocol (ILMP)

Machine-level ILMP may be implemented as:

- deterministic queues in shared memory
- hardware mailboxes
- bus-level message channels
- memory-mapped registers

…but must obey the same direction, adjacency, and non-autonomy rules.

4.4 Preserve Governance MD Files

Machine-level systems must read governance from human-authored MD files (or signed binary derivations of them). They must not generate, mutate, or reinterpret rules.

4.5 Preserve Determinism

No probabilistic scheduling.No autonomous timers.No emergent control loops.All timing is human-defined.

4.6 Preserve Auditability

Every machine-level action must produce an audit record, even if logged via ring buffer, telemetry packet, or black-box recorder.

4.7 Preserve Human Override

Machine-level systems must accept human overrides immediately, with no challenge, no delay, no reinterpretation. Override paths must be hardware-reachable where possible (physical switches, signed override channels).

## 5. What Machine-Level UNICORE Looks Like

5.1 The TrueAI Core Library (libtrueai)

A C/C++ library implementing:

- truth records
- evidence records
- governance loaders
- threshold enforcement
- ILMP message validation
- audit ring buffers
- override channels

Designed to compile for:

- Linux
- Windows
- RTOS (FreeRTOS, VxWorks, RTEMS)
- bare metal
- spacecraft flight software environments

5.2 The UniCORE Machine Wrapper (UMW-M)

The hardware analogue of the UniCORE Model Wrapper from Document Y. Wraps:

- model-execution accelerators
- robotic controllers
- life-support controllers
- navigation controllers

…inside the same governance shell.

5.3 Hardware Enforcement (Optional)

Where adopted, governance may be enforced in hardware via:

- FPGA-based ILMP routers
- signed-rule ROM regions
- hardware override pins
- watchdogs governed by Mission_Governance.md

This is permitted but not required.

## 6. What Machine-Level UNICORE Is Not

It is not:

- a way to embed AI deeper into systems without governance
- a way to run autonomous models at the firmware level
- a license to skip MD-file governance because "it's firmware"
- a way to reduce human sovereignty in real-time systems

Machine-level integration **increases** the reach of governance, not the reach of AI autonomy.

## 7. Relationship to Existing Documents

- Document E (Architecture Diagram): the 12-level stack applies identically.
- Document O (API Specification): machine-level systems expose equivalent endpoints via local IPC, shared memory, or hardware mailboxes.
- Document P (Data Model): machine-level systems may use compact binary forms but must preserve the same schema semantics.
- Document Q (ILMP): applies identically; transport may differ.
- Document R (Space Mission Pack): machine-level integration is the preferred form for spacecraft and hibernation systems.
- Document S (Enterprise Deployment): machine-level integration extends the air-gapped and defense deployment models.
- Document Y (Multi-Model Integration): the model wrapper has a machine-level twin (UMW-M).

## 7.5 Bringing a Platform That Uses AI onto Powered by UniCORE AI, built on TrueAI Foundation

The sections above define **what** machine-level integration is, **why** it matters, **which targets** it supports, **which rules** it must preserve, and **what it looks like** in concrete form (libtrueai, UMW-M, optional hardware enforcement).

This section answers the **procedural** question: **how** does a producer bring a platform that currently uses AI — firmware, embedded controller, RTOS, robotic stack, spacecraft avionics, hardware accelerator scheduler, or any other machine-level target — onto the *Powered by UniCORE AI, built on TrueAI foundation* architecture?

The path is the same path every Powered-by-UniCORE-AI Solution walks. The machine-level target does not bypass it. The machine-level target is one of the deepest applications of it.

### 7.5.1 Form the 1-Human-1-Claw bond

The producer-onboarding entry point is [`GETTING_STARTED.md`](../GETTING_STARTED.md) at the repository root.

`GETTING_STARTED.md` is where a producer:

- Chooses the Project level they are producing for (per [`LICENSE_EXAMPLES.md`](../LICENSE_EXAMPLES.md)).
- Stands up the working tools (Visual Studio Pro, DevExpress Universal, a 1-to-1 Claw at [https://myclaw.ai](https://myclaw.ai)).
- Sets up their Claw — introduces themselves, gives the six-point TRUTH preamble, has the Claw review the Foundation triad (UniVERSE / TrueAI / UniCORE AI), and (where relevant) the implementation references (UniCORE / UniCORE.GVB).
- Uses the **DevExpress XAF / XPO learning surface** to teach the Claw the patterns the public reference architecture rests on (governed Business Objects, principled Module boundaries, evidence-bearing persistence, deployment-shape awareness, security and audit surfaces).
- Forms the **1-Human-1-Claw bond** through that learning.

The XAF / XPO learning surface is the **door**, not the destination. Once the bond is formed, the Claw can produce Solutions in **any language and on any platform** — including the machine-level languages this document is about (C++, C, Rust, Ada / SPARK, Assembly, Verilog / VHDL).

### 7.5.2 Work under the Singular Pairing Principle

The 1-Human-1-Claw bond is **per Project**, not per Human. A producer working on multiple Projects in parallel must run a separate dedicated Claw for each Project. This is the **Singular Pairing Principle**, canonically locked at [`10001-Singular-Pairing-Principle.md`](10001-Singular-Pairing-Principle.md).

For a producer bringing a machine-level platform onto the Foundation, this means: **that machine-level target is its own Project, with its own dedicated 1-Human-1-Claw pairing.** Mixing a firmware Project's working context into a separate Solutions Project's Claw — or vice versa — causes drift; drift breaks the bond; the work cannot honestly compound across the long arc machine-level governance requires.

### 7.5.3 Pass the Certification gate before layered governance applies

No Solution — software-level or machine-level — may claim *Powered by UniCORE AI, built on TrueAI Foundation* status, and no layered governance (the 12-Level Model, ILMP, Inter-Level Messaging, Mission Governance) applies, until the producer’s work has passed the **Certification gate**.

The Certification gate is canonically defined at [`10002-Certification-Before-Layered-Governance.md`](10002-Certification-Before-Layered-Governance.md).

For machine-level integration this gate is especially important: machine-level governance reaches into firmware, hardware enforcement paths, override pins, and silicon-level execution. Layered governance applied to an uncertified machine-level implementation is governance applied to an unvalidated foundation — which is exactly the failure mode this document exists to prevent.

### 7.5.4 Satisfy the architectural rules at the machine level

Once the 1-Human-1-Claw bond is formed, the Project is operating under Singular Pairing, and the work has passed the Certification gate, the producer can begin satisfying the **machine-level architectural rules** in [§4 of this document](#4-architectural-rules-for-machine-level-implementations):

- **§4.1** Preserve the TrueAI Foundation (no fabrication, no self-modification, no autonomous authority, no internal heartbeat, no emergent behaviour, human sovereignty at Level 12).
- **§4.2** Preserve the 12-Level Model (truth flows upward; governance flows downward; no level may bypass another).
- **§4.3** Preserve the Inter-Level Messaging Protocol (ILMP) — transport may differ at the machine level (shared-memory queues, hardware mailboxes, bus-level channels, memory-mapped registers), but direction, adjacency, and non-autonomy rules are identical.
- **§4.4** Preserve governance MD files (read from human-authored MD files or signed binary derivations; never generate, mutate, or reinterpret rules).
- **§4.5** Preserve determinism (no probabilistic scheduling, no autonomous timers, no emergent control loops).
- **§4.6** Preserve auditability (every action produces an audit record, even via ring buffer, telemetry packet, or black-box recorder).
- **§4.7** Preserve human override (immediate; no challenge, no delay, no reinterpretation; hardware-reachable where possible).

The form the implementation takes — a `libtrueai` C/C++ library, a UniCORE Machine Wrapper (UMW-M) around a robotic or life-support controller, FPGA-based ILMP routing, signed-rule ROM regions — is governed by [§5](#5-what-machine-level-unicore-looks-like) of this document.

### 7.5.5 Summary of the flow

```
  1-Human-1-Claw bond formed (GETTING_STARTED.md)
           |
           v
  Working under Singular Pairing per Project (10001-Singular-Pairing-Principle.md)
           |
           v
  Certification gate passed (10002-Certification-Before-Layered-Governance.md)
           |
           v
  Machine-level architectural rules satisfied (§4 of this document)
           |
           v
  Machine-level implementation chosen (§5: libtrueai / UMW-M / optional hardware enforcement)
           |
           v
  Powered by UniCORE AI, built on TrueAI Foundation — at the machine level
```

Nothing on the path is optional. The path is the same path every Powered-by-UniCORE-AI Solution walks; machine-level targets walk it deeper into the substrate.

## 8. Why This Must Be Recorded Now

The current generation of AI systems lives almost entirely at the software layer. The next generation — robotics, autonomous vehicles, spacecraft, embedded LLM accelerators, hibernation systems — will live at the machine layer.

If UniCORE AI is not extended to the machine layer **now**, governance will arrive after the substrate is already ungoverned. That is the failure mode this document exists to prevent.

## 9. Summary

The TrueAI Foundation and UniCORE AI:

- are language-neutral
- are runtime-neutral
- are substrate-neutral
- may be implemented in C++ and other machine-level languages
- may be enforced in firmware, RTOS, and hardware
- govern AI at the machine level, not only the software level
- preserve the same Foundation, the same 12 Levels, the same ILMP, the same Human Sovereignty

Machine-level integration is not a fork.It is not an extension of authority.It is the same governance, reaching deeper.

— End of Addendum —
