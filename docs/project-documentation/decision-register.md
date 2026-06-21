# project decision register

## authority

| Source or decision maker | Authority scope | Priority |
|---|---|---|
| Ayman Shams | Product identity, content boundaries, coding approval, public positioning | 1 |
| GitHub Docs | GitHub Pages repository, publishing, and hosting behavior | 2 |
| Cloudflare Registrar public page | Registrar recommendation rationale | 3 |

## decisions

| ID | Category | Question | Decision | Authority | Status | Affected documents |
|---|---|---|---|---|---|---|
| DEC-001 | Brand | What is the umbrella brand? | Ayman Shams personal site. HealPath and SiriusShield are work areas, not umbrella brands. | User prompt | Approved | All |
| DEC-002 | Repository | Which repo should host the personal site? | Use the GitHub user-site repo `aymanshams.github.io` under the `AymanShams` account. | User answer and GitHub Docs | Approved | Tech stack, implementation plan |
| DEC-003 | Stack | Which stack should v1 use? | Plain static HTML and CSS. Use minimal JavaScript only if needed later. | User answer | Approved | Tech stack, frontend, security |
| DEC-004 | Publishing source | Should GitHub Pages publish from repo root or `/docs`? | Use root of `main`. The repository exists only for the personal site, so `/docs` adds unnecessary nesting. | Codex recommendation, supported by GitHub Docs | Approved by delegated judgment | Tech stack, implementation plan |
| DEC-005 | Custom domain | Should v1 use a custom domain? | Defer. Recommend `aymanshams.com` later if available, with `ayman-shams.com` or `aymanshams.dev` as fallback. | User answer | Approved | Tech stack, implementation plan |
| DEC-006 | Domain registrar | How should costs be minimized later? | Prefer Cloudflare Registrar if the selected domain is supported because it advertises at-cost registration and renewal without add-on fees. Verify exact price and availability at purchase. | Codex recommendation from Cloudflare public page | Deferred | Later scope |
| DEC-007 | Site structure | Should v1 be one page or several pages? | Use one homepage plus three lean subpages: Codex Coding OS, healthcare operations, and operating notes. | User delegated judgment | Approved | PRD, app flow, frontend |
| DEC-008 | Codex disclaimer | What must the Codex Coding OS page say? | "Codex Coding OS is an independent open-source project and is not affiliated with, endorsed by, or sponsored by OpenAI." | User prompt and approval | Approved | PRD, frontend, security |
| DEC-009 | Contact | Which contact methods are in v1? | Include GitHub, LinkedIn, and a Google Calendar booking link when approved and checked. Omit email until the user supplies a public address. | User delegated judgment plus supplied URLs | Approved | PRD, frontend |
| DEC-010 | Visual style | Should v1 use a photo or graphics? | Text-only, serious, responsive design. | User preference | Approved | Frontend |
| DEC-011 | Analytics and forms | Should v1 collect data? | No analytics, forms, cookies, or tracking in v1. | Codex recommendation under user simplicity constraint | Approved by delegated judgment | Backend, security |
| DEC-012 | Coding gate | Can Codex start coding after these answers? | No. Coding remains blocked until controlled docs and implementation plan are approved. | User answer | Approved | Manifest, implementation plan |

## deferred decisions

| ID | Decision | Deferred until | Required action |
|---|---|---|---|
| DEF-001 | Final custom domain | After v1 is live on GitHub Pages | Check availability and annual renewal price before purchase. |
| DEF-002 | Public email address | Before adding an email link | User supplies the address or approves omitting email. |
| DEF-003 | Analytics | After the site has a traffic question worth answering | Choose a privacy-respecting option or continue with no analytics. |

## status rules

- `Approved`: user approved the decision directly or delegated it to Codex judgment.
- `Deferred`: not needed for v1 implementation.
- `Superseded`: replaced by a later approved decision.
