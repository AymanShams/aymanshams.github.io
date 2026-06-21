# TDD: Ayman Shams personal site

## status

Draft for approval.

## source lock

This TDD is derived from the approved controlled docs:

- `docs/project-documentation/project-brief.md`
- `docs/project-documentation/decision-register.md`
- `docs/project-documentation/controlled-docs/prd-ayman-shams-personal-site.md`
- `docs/project-documentation/controlled-docs/app-flow.md`
- `docs/project-documentation/controlled-docs/tech-stack.md`
- `docs/project-documentation/controlled-docs/frontend-guidelines.md`
- `docs/project-documentation/controlled-docs/backend-structure.md`
- `docs/project-documentation/controlled-docs/security-guidelines.md`
- `docs/project-documentation/controlled-docs/implementation-plan.md`

No external TDD was provided or merged.

## technical decision

Build a static GitHub Pages user site in `AymanShams/aymanshams.github.io`, with the repository named `aymanshams.github.io`, published from the root of `main`.

Use plain HTML and CSS for v1. Do not add a build system, frontend framework, backend, database, forms, analytics, tracking, cookies, or custom domain.

## architecture

```text
Visitor browser
  |
  | HTTPS
  v
GitHub Pages
  |
  | Serves static files from root of main
  v
aymanshams.github.io repository
```

## target file structure

```text
/
  index.html
  404.html
  .nojekyll
  README.md
  AGENTS.md
  assets/
    css/
      styles.css
  codex-coding-os/
    index.html
  healthcare-operations/
    index.html
  notes/
    index.html
  docs/
    index.md
    delivery/
      current-state.md
    architecture/
      adr/
        0001-static-github-pages-site.md
    project-documentation/
      project-documentation-manifest.json
```

## routes

| Route | File | Purpose |
|---|---|---|
| `/` | `index.html` | Personal umbrella homepage |
| `/codex-coding-os/` | `codex-coding-os/index.html` | Codex Coding OS overview |
| `/healthcare-operations/` | `healthcare-operations/index.html` | Healthcare and insurance operations overview |
| `/notes/` | `notes/index.html` | Writing and operating notes index |
| `/404.html` | `404.html` | Not-found page |

## content requirements

### homepage

The homepage must make Ayman Shams the first visible identity. It must present the site as a personal umbrella for:

- Codex Coding OS.
- Healthcare operations and digital health work.
- Medical insurance operations work.
- Writing and operating notes.

The homepage must avoid sales-heavy sections, exaggerated claims, and generic founder positioning.

### Codex Coding OS page

The page must include this exact sentence:

> Codex Coding OS is an independent open-source project and is not affiliated with, endorsed by, or sponsored by OpenAI.

The page should link to the public GitHub repository only after the URL is verified.

### healthcare operations page

The page may reference HealPath and SiriusShield only as work areas under Ayman's personal umbrella. It must not expose patient, client, payer, financial, internal operating, or PHI details.

### notes page

The page should start as a simple index of concise public working principles. It does not need a blog engine in v1 and should not include coming-soon placeholder copy.

## frontend design

Use a text-only, serious layout.

Required properties:

- Responsive layout.
- Semantic HTML.
- One `h1` per page.
- Clear focus states.
- Strong color contrast.
- No decorative image dependency.
- No JavaScript required for navigation.

Suggested visual system:

- Neutral background.
- Dark readable text.
- One restrained accent color for links and focus states.
- Content width capped for readability.
- Compact page sections, not large marketing bands.

## security and privacy design

V1 should not collect visitor data.

Do not include:

- Forms.
- Cookies.
- Analytics.
- Third-party scripts.
- API keys.
- Secrets.
- Tracking pixels.
- Client or patient data.

If external links open in a new tab, use `rel="noopener noreferrer"`.

If JavaScript is added later, do not use dangerous DOM sinks such as `innerHTML` for untrusted content, string-based code execution, or unreviewed third-party scripts.

## deployment model

1. Commit static files to `main`.
2. Configure GitHub Pages to deploy from `main` root.
3. Wait for Pages deployment.
4. Verify the public URL loads.

The expected v1 URL is:

```text
https://aymanshams.github.io/
```

## validation plan

Before launch:

1. Verify all internal links.
2. Check approved external GitHub, LinkedIn, booking, and project website URLs, documenting any platform verification limitation.
3. Confirm OpenAI disclaimer appears exactly on the Codex Coding OS page.
4. Check desktop and mobile rendering.
5. Check keyboard focus visibility.
6. Check that no sensitive healthcare or insurance detail is present.
7. Check that no third-party scripts, analytics, forms, cookies, secrets, or API keys are present.
8. Confirm GitHub Pages publishes from `main` root.

## implementation slices

### slice 1: repo and documentation foundation

Outputs:

- Clone or create `AymanShams/aymanshams.github.io`.
- Add `README.md`, `AGENTS.md`, `docs/index.md`, current state, ADR, and workflow manifest.

Exit criteria:

- Repo exists locally.
- Remote origin is correct.
- Manifest and docs are present.
- Coding permission is recorded before site files are created.

### slice 2: static site shell

Outputs:

- `index.html`
- `404.html`
- `.nojekyll`
- `assets/css/styles.css`
- Subpage directories and entry files.

Exit criteria:

- Files open locally.
- Navigation works.
- No build process is required.

### slice 3: approved content

Outputs:

- Homepage copy.
- Codex Coding OS page copy.
- Healthcare operations page copy.
- Notes page copy.

Exit criteria:

- OpenAI disclaimer is exact.
- No sensitive detail is present.
- Links are verified or omitted.

### slice 4: local validation

Outputs:

- Link check.
- Visual check.
- Accessibility basics check.
- Sensitive-content check.

Exit criteria:

- No blocking defects.

### slice 5: publish and verify

Outputs:

- GitHub Pages configuration.
- Published site verification.
- Updated current state and handoff.

Exit criteria:

- Live URL loads.
- Repository state is clean.
- Handoff records actual status.

## open issues

| Issue | Status | Blocking |
|---|---|---|
| Exact GitHub, LinkedIn, booking, and project website URLs | Resolved for current published links | No |
| Custom domain availability and price are not checked | Deferred | No |
| Public email address is not supplied | Deferred | No |

## approval gate

This TDD must be approved before repo documentation and agent instructions become the next phase. Coding remains blocked until the full documentation workflow passes and `coding_start` approval is recorded in the manifest.
