# ADR-0001: static GitHub Pages site

## status

Accepted.

## context

Ayman Shams needs a lean personal umbrella site for technical reviewers, founders, healthcare operators, partners, and people checking his work from GitHub or LinkedIn.

The site must not become a marketing-heavy landing page. It must be easy to ship and maintain.

## decision

Use a static GitHub Pages user site in `AymanShams/aymanshams.github.io`, published from the root of `main`.

Use plain HTML and CSS for v1.

## alternatives considered

| Alternative | Why rejected for v1 |
|---|---|
| Next.js | Too much framework and deployment overhead for a small static site |
| React or Vite | Adds a build step without enough v1 benefit |
| Jekyll | Useful for a blog, but v1 does not need a theme engine |
| CMS | Adds maintenance, accounts, and security concerns |
| Forms or analytics | Adds data collection and privacy questions |

## consequences

Positive:
- Minimal cost.
- Easy to inspect.
- Easy to maintain.
- Good fit for a GitHub-linked personal site.

Negative:
- Manual content updates.
- No dynamic content.
- No built-in blog engine.

Follow-up required:
- Check custom domain availability after v1 launch.
- Add public writing pages only when content is approved.

## notes

Owner: Ayman Shams.  
Date: 2026-06-15.  
Related docs: `docs/project-documentation/controlled-docs/tech-stack.md`, `docs/project-documentation/tdd-ayman-shams-personal-site.md`.
