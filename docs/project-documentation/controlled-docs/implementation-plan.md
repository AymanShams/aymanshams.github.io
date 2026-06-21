# implementation plan

## direct answer

Build the first release as a static GitHub Pages site in `aymanshams.github.io`, published from the root of `main`. Do not start implementation until these controlled docs are approved and the TDD phase passes.

## assumptions

- The repository is or will be available under the `AymanShams` GitHub account.
- The public site URL will be `https://aymanshams.github.io/` for v1.
- Approved external URLs will be checked before publishing, with platform verification limitations documented when applicable.
- No email link will be added unless a public email address is supplied.
- No custom domain will be added in v1.

## WBS tree

| WBS | Node | Purpose | Status | Depends on |
|---|---|---|---|---|
| 0 | Project control | Keep gates, docs, and approvals accurate | In progress | None |
| 1 | Site requirements | Lock page scope, wording, and exclusions | For review | 0 |
| 2 | Repo setup | Create or clone `aymanshams.github.io` | Blocked until approval | 1 |
| 3 | Static site foundation | Add HTML, CSS, routing, and 404 page | Blocked until approval | 2 |
| 4 | Content implementation | Add homepage and subpage copy | Blocked until approval | 3 |
| 5 | Review and validation | Check links, responsiveness, accessibility, and sensitive content | Blocked until approval | 4 |
| 6 | GitHub Pages launch | Configure Pages and verify published URL | Blocked until approval | 5 |
| 7 | Handoff | Record current state and next maintenance rules | Blocked until approval | 6 |

## node contracts

### WBS 0 project control

Objective:
Maintain the workflow manifest and prevent coding before approval.

Outputs:
- Updated manifest.
- Controlled docs for approval.

Validation:
- Manifest validator passes.
- `code_allowed` remains `false` until approval.

### WBS 1 site requirements

Objective:
Approve page scope, wording boundaries, stack, and launch rules.

Outputs:
- PRD.
- App flow.
- Tech stack.
- Frontend guidelines.
- Backend structure.
- Security guidelines.
- Implementation plan.

Validation:
- User approves controlled docs or requests revisions.

### WBS 2 repo setup

Objective:
Prepare the GitHub Pages repo without adding unnecessary tooling.

Outputs:
- Local clone of `AymanShams/aymanshams.github.io`.
- Root `README.md`.
- Root `AGENTS.md`.

Validation:
- `git status -sb` is clean before implementation.
- Remote origin points to the approved repo.

### WBS 3 static site foundation

Objective:
Create the static file structure.

Outputs:
- `index.html`.
- `404.html`.
- `.nojekyll`.
- `assets/css/styles.css`.
- Subpage directories.

Validation:
- Pages open locally as files.
- No build command required.

### WBS 4 content implementation

Objective:
Add approved copy and links.

Outputs:
- Homepage.
- Codex Coding OS page with exact disclaimer.
- Healthcare operations page.
- Notes page.

Validation:
- No placeholder links.
- No sensitive healthcare or insurance details.
- OpenAI disclaimer present exactly.

### WBS 5 review and validation

Objective:
Check quality before publish.

Outputs:
- Link check.
- Responsive layout check.
- Accessibility basics check.
- Sensitive-content review.

Validation:
- No broken internal links.
- Layout works on desktop and mobile.
- Keyboard focus is visible.
- Content review passes.

### WBS 6 GitHub Pages launch

Objective:
Publish v1.

Outputs:
- GitHub Pages configured from root on `main`.
- Published URL verified.

Validation:
- Public URL loads.
- GitHub Pages deployment is green.

### WBS 7 handoff

Objective:
Record actual launch state and maintenance rules.

Outputs:
- Current-state update.
- Handoff note.
- Next maintenance steps.

Validation:
- Handoff points to actual files and live URL.

## dependency order

1. Approve controlled docs.
2. Draft and approve TDD.
3. Create repo docs and agent instructions.
4. Clone or create the approved GitHub repo.
5. Build static site.
6. Validate locally.
7. Publish through GitHub Pages.
8. Verify live site.

## validation gates

| Gate | Required evidence | Owner | Pass condition |
|---|---|---|---|
| Controlled-doc approval | User approval in chat | Ayman | Docs accepted or revisions completed |
| TDD approval | TDD approved after alignment review | Ayman | No unresolved drift |
| Coding permission | Manifest `coding_start` approval | Ayman | `code_allowed` true |
| Local validation | Local file preview and checks | Codex | Pages render and links work |
| Launch validation | Published GitHub Pages URL | Codex | Live page loads correctly |

## risks and failure modes

| Risk | Why it matters | Control |
|---|---|---|
| Overbuilding | Slows launch and creates maintenance burden | Plain static v1 |
| Brand confusion | HealPath or SiriusShield could look like umbrella brand | Use Ayman Shams as first-page signal |
| OpenAI affiliation confusion | Codex name can be misread | Exact disclaimer on Codex page |
| Sensitive healthcare detail | Public site can expose wrong information | Portfolio-level descriptions only |
| Domain distraction | Custom domain setup can slow v1 | Defer domain |

## next action

Approve or revise these controlled docs. Coding remains blocked.
