# app flow

## scope

The site is a static personal website. The primary flow is reader orientation, not account creation, lead capture, or content management.

## roles

| Role | Goal |
|---|---|
| Visitor | Understand Ayman's work and choose the relevant next page |
| Technical reviewer | Reach Codex Coding OS and GitHub quickly |
| Healthcare or operations reader | Understand healthcare and insurance operations work without reading code |
| Ayman | Update static content safely |

## primary flow

1. Visitor opens `https://aymanshams.github.io/`.
2. Visitor sees Ayman Shams as the umbrella identity.
3. Visitor scans the work areas.
4. Visitor chooses one route:
   - Codex Coding OS.
   - Healthcare operations.
   - Operating notes.
   - Public profile link.
5. Visitor reaches the selected page.
6. Visitor exits through GitHub, LinkedIn, or another approved external link.

## page flow

| Page | Entry point | Main action | Exit |
|---|---|---|---|
| Homepage | Direct visit, GitHub profile, LinkedIn profile | Choose a work area | Subpage or external profile |
| Codex Coding OS | Homepage or GitHub | Understand project and disclaimer | GitHub repository |
| Healthcare operations | Homepage or LinkedIn | Understand healthcare and insurance operating focus | LinkedIn or homepage |
| Notes | Homepage or LinkedIn | Browse writing themes | Future note page or homepage |
| 404 | Broken link | Return to homepage | Homepage |

## alternate paths

| Situation | Expected behavior |
|---|---|
| Visitor lands directly on subpage | Subpage includes top navigation and link back to homepage. |
| External link is not ready | Omit the link rather than publishing a placeholder. |
| No notes are published yet | Notes page lists themes and says public notes will be added when ready. |
| Custom domain is not configured | Site uses the default GitHub Pages URL. |
| Visitor uses mobile | Layout stacks cleanly with readable text and no horizontal scrolling. |

## failure states

| Failure | User-facing behavior | Fix |
|---|---|---|
| Broken internal link | 404 page offers a return to homepage | Fix route path |
| Missing external URL | Link is omitted | Add verified URL in a later edit |
| GitHub Pages build delay | Site may take up to several minutes to update after push | Check Pages deployment status |
| Sensitive wording found before launch | Content is blocked from publish | Revise wording and re-review |

## approval and publishing flow

1. Controlled docs approved.
2. TDD and repo documentation created.
3. Implementation plan approved for coding.
4. Static files created.
5. Local file preview checked.
6. GitHub Pages setup checked.
7. Published site reviewed.
8. Final launch state recorded.
