# contributing

## project rule

This repository is a personal site. Keep changes small, source-aligned, and easy to review.

## before editing

1. Read `AGENTS.md`.
2. Read `docs/project-documentation/project-documentation-manifest.json`.
3. Read `docs/delivery/current-state.md`.
4. Read `docs/index.md`.
5. Read the controlled TDD at `docs/project-documentation/tdd-ayman-shams-personal-site.md`.

## content rules

- Keep Ayman Shams as the umbrella identity.
- Do not make HealPath or SiriusShield the umbrella brand.
- Keep Codex Coding OS clearly independent from OpenAI.
- Do not publish PHI, patient details, client details, payer details, financial details, or internal operating procedures.
- Do not add unsupported claims.
- Do not add marketing-heavy sections.

PHI means protected health information.

## technical rules

- Keep v1 static.
- Do not add a framework, backend, database, forms, cookies, analytics, tracking, or third-party scripts without an approved doc update.
- If architecture changes, add or update an ADR.
- If content scope changes, update the PRD or relevant product docs.

## review checklist

Before a change is complete:

1. Internal links work.
2. External links are verified.
3. The Codex Coding OS disclaimer is exact if that page is touched.
4. The site works without JavaScript.
5. No sensitive healthcare or insurance content is present.
6. No secrets or API keys are present.
7. Documentation is updated when behavior changes.
