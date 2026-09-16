# Mazar Mall — 60-Second CGI Advertisement

This repository is the production source of truth for a premium 60-second CGI client-presentation film for Mazar Mall.

## Goal
Make the client feel that Mazar Mall already exists: architecturally believable, emotionally aspirational, visually premium, and consistent with the supplied Mazar Mall references.

## Creative thesis
**TOMORROW HAS A VIEW.**

The film is not a slideshow. It is a cinematic journey through the completed project: aerial reveal → commercial podium → amenity transition → residential arrival → signature Floor 5 balcony sunset moment → furnished home → blue-hour/night hero.

## Canonical building facts used by this project
- 20 physical levels total.
- 2 underground levels: B2 and B1.
- 18 above-ground floors: 1–18.
- Floors 1–2: commercial.
- Floor 3: amenities / lifestyle level.
- Floors 4–18: residential.
- Floor 5 is the **second residential floor** and is the signature balcony scene.
- Residential typical floors use the supplied typical-floor reference.

Do not invent official legal unit numbering, unconfirmed tenant brands, or unverified project claims.

## Production roles
- **Codex** — production orchestrator, asset auditor, manifest/version manager, QA coordinator, edit assembler.
- **Astra** — required creative-director / cinematic reasoning layer when available in the execution environment.
- **Higgsfield** — image/video generation backend.
- **Human approval** — final authority on architecture, client claims, music, logo, and public-release wording.

## Repository map
- `assets/references/exterior/` — canonical exterior references.
- `assets/references/hero/` — curated hero views.
- `assets/references/unit-plans/` — furnished plan references.
- `assets/references/plans/` — typical floor PDF.
- `assets/site/` — exact site/drone plates to add before site-accurate generation.
- `docs/` — creative brief, facts, storyboard, continuity, workflow, acceptance.
- `production/` — machine-readable shot manifest and status.
- `prompts/` — Codex master prompt and generated shot prompt packs.
- `outputs/` — previews, selected generations, and final masters.

## First command for an agent
Read, in order:
1. `AGENTS.md`
2. `docs/01_CREATIVE_BRIEF.md`
3. `docs/02_PROJECT_FACTS.md`
4. `docs/03_STORYBOARD_60S.md`
5. `docs/04_VISUAL_CONTINUITY_BIBLE.md`
6. `docs/05_HIGGSFIELD_WORKFLOW.md`
7. `docs/06_ACCEPTANCE_CRITERIA.md`
8. `production/shot_manifest.json`
9. `prompts/CODEX_MASTER_PROMPT.md`

## Non-negotiable
Never claim a generation, site match, model, render, or browser/tool result succeeded unless it actually succeeded and the evidence is recorded.
