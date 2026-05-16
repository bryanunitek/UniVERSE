# Programme Corpus

**The programme-horizon markdown content that Solutions deliver to paired Claws at session-opening time.**

This folder holds the UniVERSE programme-level material that a Foundation-aligned Solution serves to a paired Claw alongside the Foundation requirements (from [TrueAI/foundation-requirements/](https://github.com/bryanunitek/TrueAI/tree/main/foundation-requirements)) and the per-Level corpus (from [UniCORE-AI/levels/](https://github.com/bryanunitek/UniCORE-AI/tree/main/levels)).

UniVERSE content is **not** Level-sliced; the programme view is the same for every Level. What `programme-corpus/` does is give Solutions a versioned, frozen, locally-deployable copy of the programme material so that the same content can be delivered to paired Claws without depending on live `docs/` reads.

This folder is distinct from [`docs/`](docs/):

- **`docs/`** holds the long-form authored programme documents — `00057-Layered-CORE-Model.md`, `00058-Claw.md`, `00060-Supported-AI-Provider-List.md`, and so on. These are written for human readers studying the programme.
- **`programme-corpus/`** holds the runtime content that gets delivered to Claws during pairing. It is for runtime consumption by Solutions.

The pairing protocol that consumes this content is specified in [`docs/00061-PairedClaw-Bond-File-And-Session-Protocol.md`](docs/00061-PairedClaw-Bond-File-And-Session-Protocol.md).

---

## Versioning

Each subfolder (`v1/`, `v2/`, ...) is a **frozen version** of the programme corpus. UniVERSE evolves by adding new versioned subfolders, not by editing existing ones. A Solution is built against a specific version; the version is part of the Solution's deployment identity.

- **`v1/`** is the first canonical version, published 2026-05-16.
- A Solution carries `v1/` content embedded in its deployment.
- When the programme corpus refines, a new `v2/` subfolder is added alongside `v1/`. Previous versions remain readable.
- Pairing-time version drift between a deployed Solution and the canonical head is surfaced to UNICOREMASTER per the failure ladder in [`docs/00062-Pairing-Failure-Ladder-Pause-Mode-And-EMERGENCY.md`](docs/00062-Pairing-Failure-Ladder-Pause-Mode-And-EMERGENCY.md).

This matches the same versioning discipline used by [TrueAI/foundation-requirements/](https://github.com/bryanunitek/TrueAI/tree/main/foundation-requirements) and [UniCORE-AI/levels/](https://github.com/bryanunitek/UniCORE-AI/tree/main/levels).

---

## Status

`programme-corpus/v1/` is a **structural placeholder** at first publication. The substantive content — which programme-level docs are included in the corpus delivered to Claws, and in what form — is curated in subsequent commits. The version's identity is fixed by its folder name; its content grows incrementally up to the point that a `v2` is opened.
