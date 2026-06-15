# backend structure

## decision

There is no backend in v1.

## static architecture

| Component | Purpose |
|---|---|
| HTML files | Page structure and content |
| CSS file | Layout, typography, colors, responsive behavior |
| `.nojekyll` | Prevent GitHub Pages from applying Jekyll processing |
| `404.html` | Simple not-found page |
| GitHub Pages | Static hosting |

## not included

- No server.
- No database.
- No authentication.
- No admin panel.
- No content management system.
- No API.
- No form submission.
- No analytics script.
- No cookies.
- No storage of visitor data.

## file structure target

```text
/
  index.html
  404.html
  .nojekyll
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
    project-documentation/
```

## update model

Updates happen through Git commits. Ayman or an approved coding agent edits static files, previews locally, then pushes to GitHub. GitHub Pages publishes the updated files.

## operational limits

Because v1 has no backend:

- The site cannot collect messages.
- The site cannot manage subscriptions.
- The site cannot personalize content.
- The site cannot store visitor activity.

These limits are intentional for v1.
