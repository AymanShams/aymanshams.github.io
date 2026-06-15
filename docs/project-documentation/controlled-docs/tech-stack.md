# tech stack

## decision

Use plain static HTML and CSS in the `aymanshams.github.io` repository. Publish from the root of the `main` branch through GitHub Pages.

## selected stack

| Layer | Choice | Reason |
|---|---|---|
| Hosting | GitHub Pages | Free for public repos, native fit for a GitHub-linked personal site |
| Repository | `aymanshams.github.io` | GitHub user-site naming convention |
| Source branch | `main` | Simple default branch |
| Publishing folder | Repository root | The repo exists only for the site, so root is clearer than `/docs` |
| Markup | HTML | No build step and easy to inspect |
| Styling | CSS | Enough for a serious text-only site |
| JavaScript | None for v1 unless a specific need appears | Reduces security and maintenance risk |
| Build system | None | Avoids framework overhead |
| Custom domain | Deferred | Keeps v1 free and simple |

## rejected options

| Option | Why not v1 |
|---|---|
| Next.js | Too much stack for a small static personal site |
| React or Vite | Adds build tooling without enough benefit for v1 |
| Jekyll | Useful for blogs, but v1 does not need a theme engine or markdown collection |
| CMS | Too much setup for a small manually maintained site |
| Forms service | Adds privacy and spam handling work without a clear v1 need |
| Analytics | Adds tracking and privacy questions without a decision need |

## domain recommendation

Defer domain setup until the GitHub Pages site is live.

Best first domain to check:

- `aymanshams.com`

Fallbacks if unavailable or overpriced:

- `ayman-shams.com`
- `aymanshams.dev`

Benefits of a custom domain:

- More professional URL for LinkedIn, email signatures, and partner checks.
- More stable identity if the site moves away from GitHub later.
- Can support a professional email address later.

Cost control:

- Use GitHub Pages for free hosting.
- Prefer Cloudflare Registrar if the chosen domain is supported because Cloudflare advertises at-cost registration and renewal without add-on fees.
- Avoid bundled web hosting, paid site builders, premium email, and privacy upsells during v1.
- Verify exact availability and renewal price at purchase time.

## GitHub Pages setup

Recommended setup:

1. Repository: `aymanshams.github.io`.
2. Branch: `main`.
3. Source: deploy from branch.
4. Folder: root.
5. Entry file: `index.html`.
6. Add `.nojekyll` to disable Jekyll processing.

## source facts

- GitHub Docs state that a user site repository must be named `<user>.github.io` and uppercase owner names must be lowercased.
- GitHub Pages publishes static files and does not support server-side languages such as PHP, Ruby, or Python.
- GitHub Pages supports custom domains. GitHub recommends verifying custom domains and recommends using a `www` subdomain when using a custom domain.

## sources

- GitHub Docs, Creating a GitHub Pages site: https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
- GitHub Docs, About custom domains and GitHub Pages: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/about-custom-domains-and-github-pages
- Cloudflare Registrar: https://www.cloudflare.com/products/registrar/
