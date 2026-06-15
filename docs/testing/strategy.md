# testing strategy

## scope

V1 testing is static-site validation.

## checks before launch

| Check | Pass condition |
|---|---|
| Internal links | All internal links resolve |
| External links | GitHub and LinkedIn URLs are verified |
| OpenAI disclaimer | Exact approved sentence appears on Codex Coding OS page |
| Responsive layout | Pages are readable on desktop and mobile |
| Keyboard navigation | Links can be reached and focus is visible |
| Sensitive content | No PHI, client, patient, payer, or internal operations detail |
| Static-only rule | No backend, forms, analytics, cookies, or third-party scripts |
| GitHub Pages | Live URL loads after publish |

## manual review

Manual review is sufficient for v1 because there is no application logic, data model, API, or build step.

If JavaScript or build tooling is added later, testing must be expanded before implementation.
