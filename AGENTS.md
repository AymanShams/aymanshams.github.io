# Project Agent Instructions

## required reading order

1. Read this file.
2. Read `CLAUDE.md` if using Claude Code.
3. Read `docs/project-documentation/project-documentation-manifest.json`.
4. Run the workflow manifest validator.
5. Run `python scripts/agent/session_continuity.py start` when available.
6. Read `docs/delivery/current-state.md`.
7. Read `docs/index.md`.
8. Read the latest handoff referenced by current state.
9. Read `docs/project-documentation/tdd-ayman-shams-personal-site.md` before coding.

## source of truth

Use this order:

1. Explicit user decisions in the current task.
2. `docs/project-documentation/project-documentation-manifest.json`.
3. Controlled product documentation under `docs/project-documentation/controlled-docs/`.
4. `docs/project-documentation/tdd-ayman-shams-personal-site.md`.
5. Repo documentation under `docs/`.
6. Current state and handoff notes as coordination records only.

## project rules

- Do not start coding unless the workflow manifest permits coding.
- Do not treat current state or handoff notes as permission to code.
- Keep Ayman Shams as the umbrella identity.
- Do not use HealPath or SiriusShield as the umbrella brand.
- Keep Codex Coding OS clearly independent from OpenAI.
- Do not change architecture without updating the TDD and ADRs.
- Do not add a framework, backend, database, forms, analytics, cookies, tracking, or third-party scripts without an approved documentation update.
- Do not commit secrets, PHI, client records, patient records, payer details, financial details, generated credentials, or local tool metadata.
- Update docs in the same change when site scope, content boundaries, deployment, security, or validation behavior changes.

## required disclaimer

The Codex Coding OS page must include this exact sentence:

> Codex Coding OS is an independent open-source project and is not affiliated with, endorsed by, or sponsored by OpenAI.

## validation before completion

Run the relevant checks before claiming completion:

1. Workflow manifest validator.
2. Filled artifact validator when documentation changes.
3. Session continuity validation when current state or handoff changes.
4. Link, responsive layout, accessibility, and sensitive-content checks after site files exist.

Report any unavailable check honestly.
