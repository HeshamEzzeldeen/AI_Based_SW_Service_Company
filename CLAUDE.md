# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this workspace is

This is not a code repository. There is nothing to build, lint or test. It holds the Markdown output of one StartupKit ideation session (`ai-automotive-sw`): two founders (Hesham and his brother Waled, both embedded automotive SW engineers in Cairo) are designing an AI-native AUTOSAR Classic BSW engineering-services startup. The work is driven by the user-level StartupKit skills (`/startupkit` orchestrator plus `/sk-diverge`, `/sk-niche`, `/sk-competitors`, `/sk-positioning`, `/sk-offer`, `/sk-validate`, `/sk-money`, `/sk-leads`, `/sk-skills`, `/sk-pitch`, `/sk-export`), which live in `~/.claude/skills/` along with their `references/` templates. Each skill reads earlier phase files and writes its own.

## Layout and state

- The session files sit at the **repository root** (not under `workspace/sessions/...`, even if a skill expects that path).
- `00-session.md` is the source of truth for progress. Its YAML front matter (`activePhase`, `nextPhase`, per-phase `status`/`file`, `goldNiche`) and the Progress Tracker table must be kept in sync whenever a phase starts, pauses or completes. Cross-phase decisions go in **Session Notes** as dated bullets, and each finished phase fills its summary block at the bottom (Gold Niche, Competitive Intelligence, Positioning, Core Offer, ...).
- Phase output file names come from the front matter `file:` field; they are not always `NN-<key>.md` (e.g. `06-validation.md`, `07-money-model.md`, `08-lead-strategy.md`, `11-one-pager.md`).
- Deep-tier phases also get a folder named after the phase file (e.g. `03-competitors/`) containing:
  - `raw/`: one file per research agent (the evidence base), plus `raw/_agent-brief.md`, the shared brief given to every agent (product summary, prior findings not to re-research, search cap, labelling rules),
  - synthesized deliverables (reports, battle cards, dossiers, matrix),
  - `verification-report.md`: a verifier pass that treats `raw/` as the source of truth and logs Critical/Warning/Info issues,
  - `PROGRESS.md` with agent states and resume steps when a phase is paused (kept after completion as a record).
- `05-offer/pricing-model.xlsx` is the hours-based pricing model behind the offer price; yellow cells are inputs the founders will replace with timesheet data. Use the xlsx skill to read or change it, and keep `05-offer.md` / `00-session.md` prices consistent with its outputs.

## Current state (2026-10-25)

Phases 1-5 complete; next is Phase 6 (`/sk-validate`). Positioning: "AUTOSAR security integration", claims scoped to Vector MICROSAR + ETAS RTA on Infineon AURIX/TRAVEO (see `04-positioning/raw/founder-input.md`). Offer: "Secure ECU Package" (EUR 85k new ECU / EUR 35k derivative, provisional model outputs). The long-term "AI-generated AUTOSAR stack" idea is recorded in Session Notes and must stay out of buyer-facing messaging.

## Content conventions to keep

- Claims carry evidence labels and confidence: `[Data, H]`, `[Opinion, M]`, `[Estimate, L-M]`, `[Est.]`, with source URL and date for Data. Write `DATA GAP:` instead of guessing. Keep labelling new claims this way, and don't upgrade an Opinion/Estimate to Data without a source.
- Corrections are visible and attributed (e.g. "V1 correction" notes) instead of silently rewriting numbers.
- Decisions already made by the founders are recorded in Session Notes and phase intakes. Treat them as settled: Gold niche I (AUTOSAR BSW delivery for Tier 1/OEM BSW managers), Silver H (cybersecurity BSW integration + ISO 21434 evidence) as the entry wedge, ISO 21434 evidence conditional on a named 21434/TARA hire or partner, and the "half the cost" promise held back until a baseline exists (founders' effort data: 3-6 PM per ECU without AI).

## Operational constraints

- A shared web-search budget ran out in Phase 3, and Phase 4 agents hit the usage limit before writing. Cap each research agent at about 25 searches, give them a shared `_agent-brief.md`, and have them write their raw file early/incrementally (with a `Status:` line at the top) so partial work survives.
- Open gates noted in the session: check the founders' current-employer non-compete / non-solicit / IP clauses before any customer contact (Hesham is at Avelabs, also a listed competitor; Waled at Luxoft), get legal review before naming any past programme, and confirm Vector/ETAS/EB licence terms for third-party AI automation ("Gate 0") before building.
