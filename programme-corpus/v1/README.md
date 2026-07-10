# Programme Corpus — v1

**First canonical version of the UniVERSE programme corpus for Solutions to deliver to paired Claws.**

Published: 2026-05-16

This is the version that the first generation of Foundation-aligned Solutions — beginning with `UniCORE.Law-Claw` — is built against.

## Manifest

The set of programme docs that comprise `v1` is curated incrementally. The starting manifest is:

- [`docs/00057-Layered-CORE-Model.md`](../../docs/00057-Layered-CORE-Model.md) — the Layered CORE model
- [`docs/00058-Claw.md`](../../docs/00058-Claw.md) — the Claw vocabulary
- [`docs/00060-Supported-AI-Provider-List.md`](../../docs/00060-Supported-AI-Provider-List.md) — the supported AI provider list
- [`docs/00061-PairedClaw-Bond-File-And-Session-Protocol.md`](../../docs/00061-PairedClaw-Bond-File-And-Session-Protocol.md) — the pairing protocol
- [`docs/00062-Pairing-Failure-Ladder-Pause-Mode-And-EMERGENCY.md`](../../docs/00062-Pairing-Failure-Ladder-Pause-Mode-And-EMERGENCY.md) — the failure ladder
- [`HORIZON.md`](../../HORIZON.md) — programme horizon and timescale

These are the docs a Solution embeds for the programme-corpus delivery. The set may expand as additional programme docs become canonical; the set does not shrink within `v1`.

## Status

`v1` is **frozen** with respect to its identity. Once a Solution has been built against `v1` with the manifest above, the meaning of `v1` is fixed.

The decision of whether a programme-corpus refinement requires a new `v2` (versus a within-`v1` content expansion) is made at the time of refinement, on a case-by-case basis. The discipline is: if a refinement changes what a deployed Solution would surface to a paired Claw, it gets a `v2`. If a refinement only adds new material that older deployments would not have used anyway, it can stay within `v1`.

See the parent [`README.md`](../README.md) for the versioning discipline.

---

## Document history

- 2026-05-16 (0193331) — docs(00061+00062): PairedClaw pairing protocol and failure ladder; programme-corpus/v1 stub
- 2026-05-22 (96a956a) — fix(public-corpus): repository enumerations updated 3 -> 5 (Foundation triad + gift-layer extension)

*Back-filled from git log on 2026-07-10 21:35 UTC. Kind 2 versioning (dated change notes) — see HORIZON.md § Evolution and versioning. Kind 1 (formal `Version:` bumps) remains OFF until first GitHub Discussion.*
