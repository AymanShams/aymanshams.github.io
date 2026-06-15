# release process

## release gate

Do not release until the workflow manifest permits coding and launch validation passes.

## release sequence

1. Confirm workflow manifest approval.
2. Confirm exact implementation slice.
3. Build static files.
4. Preview locally.
5. Run validation checks.
6. Commit changes.
7. Push to `main`.
8. Confirm GitHub Pages deployment.
9. Verify the live URL.
10. Update `docs/delivery/current-state.md`.
11. Write a handoff note.

## launch validation

- Homepage loads.
- Subpages load.
- 404 page works.
- Internal links work.
- External links are correct.
- Codex Coding OS disclaimer is exact.
- No sensitive healthcare or insurance detail is present.
- No analytics, forms, cookies, or third-party scripts are present.
