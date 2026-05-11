# AGENTS.md — UniVERSE

**Read this first, every time, before touching this repo.**

---

## What this repo is

`bryanunitek/UniVERSE` — the civilisational-scale programme. Whitepapers, governance, outreach, press, framework documents. **Not code.** No .NET, no product, no build.

Sister repos:
- `bryanunitek/TrueAI` — the immutable foundation (small, stable, never forked)
- `bryanunitek/UniCORE-AI` — the 12-level reference architecture
- `bryanunitek/UniCORE-Claw` — the .NET/XAF codebase (separate concern)

When Bryan says "UniVERSE", he means **this repo only**. Do not spill work into the others.

## Who pushes

**I push directly.** Commit and `git push origin main` on Bryan's behalf. No GitHub Desktop, no approval loop. This is the standing rule for UniVERSE, TrueAI, and UniCORE-AI. Only UniCORE-Claw has the GitHub-Desktop-by-default rule.

## Branching

- **One branch: `main`.** Never create feature branches. Never create dev branches.
- Never open pull requests. Direct commits to `main`.

## Commit style

- Author: `bryanunitek <bryan.fred@unitek-systems.com>` (use `--author=` when committing so attribution is correct even when local git config differs).
- Message format: `<type>: <subject line>` then blank line, then body. Types: `docs`, `outreach`, `governance`, `press`, `chore`.
- Body lists the files added/changed and the "what / why" in two or three sentences.

## Layout

Keep the existing shape. Do not invent new top-level directories without asking.

| Path | Purpose |
|---|---|
| `README.md` | Programme overview, document index |
| `FULL_FORMAL_STATEMENT.md` | Canonical founding statement |
| `LICENSE.md` | CC BY 4.0 / gift licence |
| `docs/` | Numbered foundation documents 001–056 (keep the numbering scheme) |
| `docs/whitepaper/` | The Governed Intelligence whitepaper set (WHITEPAPER.md + derivatives) |
| `OUTREACH/` | Dated outreach campaigns, e.g. `OUTREACH/2026-05-10-founding-notice/` |
| `public-drafts/`, `markdown/`, `_extracted/` | Working material; do not push churn into these unless asked |

New numbered docs (057+) go into `docs/` using the same `NNN-X-Title-With-Hyphens.md` pattern as the existing ones. If a new piece does not fit the numbered series, ask before placing it.

## Attribution rules (durable)

- **Authorship / licence / legal entity:** Unitek Systems Limited (UK)
- **Hosting / SaaS / infra claims:** Unitek Systems USA Inc
- **Licence for all content here:** CC BY 4.0, "given, not sold, irrevocable"
- **Author byline:** `Bryan Fred, Unitek Systems Limited` unless Bryan says otherwise
- **Version/date:** include version + month-year on any substantive document (e.g. `Version 1.0 · May 2026`)

## Contact rules (durable)

Two tiers, and only these two:

- **Public discussion** → GitHub Discussions of the relevant repo
  - UniVERSE: https://github.com/bryanunitek/UniVERSE/discussions
  - TrueAI: https://github.com/bryanunitek/TrueAI/discussions
  - UniCORE-AI: https://github.com/bryanunitek/UniCORE-AI/discussions
- **Private contact / connection request** → LinkedIn: https://www.linkedin.com/in/bryan-fred-02209753/

**Do not publish** Bryan's personal email (`bryan.fred@unitek-systems.com`, `bryan@unitek-systems.co.uk`), personal phone numbers, or the Unitek Systems generic inboxes (`info@`, `support@`, `services@`) in any file committed to this repo.

Git commit author metadata is the one exception: use `bryanunitek <bryan.fred@unitek-systems.com>` for `--author=` so the git log attributes correctly. That address lives in git metadata, not in published prose.

When writing a "Contact" section in any public document (README, whitepaper derivative, LICENSE, press material, submission), use the two-tier block above. Do not invent a third tier, do not add back direct email or phone.

## Byline rules (durable)

- **Formal full byline:** `Bryan Fred, Unitek Systems Limited, Bedford, United Kingdom` — four parts, in that order.
- **Use the full formal** on:
  - `Author:` fields at the top of any document
  - Signoff lines at the end of a document (`— Bryan Fred, Unitek Systems Limited, Bedford, United Kingdom, May 2026.`)
  - LICENSE contact blocks
  - UN submissions, government briefings
  - Masthead blocks of whitepapers and foundation documents
  - Press release front-matter `author:` field (the body uses a dateline, not a byline)
- **Short form** `Bryan Fred, Unitek Systems Limited` is acceptable only in running prose ("authored by Bryan Fred of Unitek Systems Limited", "said Fred", etc.) or inside a press dateline like `**London, May 2026**`.
- **"Bryan" alone** is fine inside prose after Bryan Fred has been introduced, and in informal voices (blog-style pieces, OUTREACH letters where he signs personally).
- **Never** shorten the byline to "Bryan, Unitek Systems Limited" — that's the pre-normalisation form and will be rewritten.
- **Role line, when used:** `Senior Solutions Architect, Unitek Systems Limited (United Kingdom) and Unitek Systems USA Inc.`
- **Version/date:** on any substantive document include version + month-year (e.g. `Version 1.0 · May 2026`).

## Press releases (durable)

- **All press releases live in `/press/` at the repo root.** Never put a press release in `docs/`, `docs/whitepaper/`, or anywhere else.
- **Filename:** `YYYY-MM-DD-short-kebab-slug.md`. The date is mandatory in the filename. No undated `PRESS-RELEASE.md`.
- **Front-matter block at the top** of every release:
  ```
  ---
  date: YYYY-MM-DD
  author: Bryan Fred, Unitek Systems Limited, Bedford, United Kingdom
  repo: UniVERSE
  slug: short-kebab-slug
  licence: CC BY 4.0
  ---
  ```
- **Dateline in the body:** `**London, D MMMM YYYY**` (full date, not just month).
- **Contact block at the end** must use the two-tier policy (Discussions + LinkedIn), never personal email or phone.
- After adding a release, add a row to `/press/README.md`.

## Voice

- Reasoned, not declaratory. Engineering-honest. Avoid manifesto tone.
- Do not use "TrueAI vs FalseAI" binary framing in UniVERSE-facing whitepapers unless Bryan specifically asks for it. The general-public artifact uses "governed / ungoverned" instead — portable and adoptable.
- Binary TrueAI/FalseAI framing belongs more naturally in `_trueai` / `_unicore-ai` material.

## Do not

- Do not touch this repo from a UniCORE-Claw session by accident.
- Do not create branches, open PRs, or introduce a dev workflow.
- Do not rename or renumber the existing 001–056 document series.
- Do not mix product/code material from UniCORE-Claw into UniVERSE documents.

## After push

Tell Bryan the commit hash and what changed in one or two sentences. That's the handshake.
