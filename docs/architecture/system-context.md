# system context

## context

The site is a public static website hosted on GitHub Pages.

```text
Visitor
  |
  | HTTPS
  v
GitHub Pages
  |
  | Static files from root of main
  v
AymanShams/aymanshams.github.io
```

## components

| Component | Responsibility |
|---|---|
| Browser | Renders static HTML and CSS |
| GitHub Pages | Hosts static files |
| Repository | Stores pages, styles, documentation, and source history |
| DNS | Deferred for v1 |

## trust boundaries

| Boundary | Risk | Control |
|---|---|---|
| Public internet to static site | Public readers can see all published content | Publish only reviewed content |
| Repo to GitHub Pages | Published files become public | Review before push |
| External profile links | Wrong link can misroute readers | Verify URLs before launch |

## excluded systems

- Backend server.
- Database.
- API.
- Authentication.
- Forms.
- Analytics.
- Custom domain in v1.
