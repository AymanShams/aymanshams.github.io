# source inventory and authority map

## controlling sources

| Source | Authority scope | Status |
|---|---|---|
| User prompt dated 2026-06-15 | Project goal, brand boundaries, audience, no-code gate, OpenAI disclaimer requirement | Controlling |
| User answers dated 2026-06-15 | Repo approval, static-site flexibility, domain deferral, text-only preference, coding approval gate | Controlling |
| GitHub Docs, Creating a GitHub Pages site | GitHub Pages repo naming, publishing source, static file support, public-site warning | Verified external source |
| GitHub Docs, About custom domains and GitHub Pages | Custom-domain options, www recommendation, verification and takeover warning | Verified external source |
| Cloudflare Registrar page | Low-cost registrar recommendation, at-cost renewal positioning, DNS and WHOIS privacy features | Verified external source |

## source authority

| Decision area | Controlling source | Rule |
|---|---|---|
| Umbrella brand | User prompt | The personal site is the umbrella. HealPath and SiriusShield must not become the umbrella brand. |
| Repository | User answer plus GitHub Docs | Use the GitHub user-site repository, named `aymanshams.github.io` if created under account `AymanShams`. |
| Coding permission | User prompt and user answer | Coding is blocked until project docs and implementation plan are approved. |
| Stack | User answer plus GitHub Docs | Use a lean static site. Avoid a framework unless a later requirement makes it necessary. |
| Domain | User answer plus GitHub Docs | Defer custom domain for v1. Recommend a low-cost custom domain later. |
| OpenAI disclaimer | User prompt and user approval | Codex Coding OS must state that it is independent and not affiliated with, endorsed by, or sponsored by OpenAI. |

## sensitivity flags

| Data or content | Sensitivity | Rule |
|---|---|---|
| Personal bio and public work summary | Public once published | Keep accurate, restrained, and non-promotional. |
| GitHub, LinkedIn, booking, and project links | Public | Check links before publishing and document platform verification limitations. |
| Email address | Personal contact data | Omit unless user supplies a public address for the site. |
| HealPath and SiriusShield details | Business sensitive if too specific | Describe at portfolio level only in v1. Do not publish client, patient, PHI, financial, or internal operating details. |
| Healthcare operations notes | Potentially sensitive depending on examples | Use generalized, non-client, non-patient examples only. |

## source conflicts

No source conflicts are currently known.

## sources

- User prompt and answers in this Codex session, 2026-06-15.
- GitHub Docs, Creating a GitHub Pages site: https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
- GitHub Docs, About custom domains and GitHub Pages: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/about-custom-domains-and-github-pages
- Cloudflare Registrar: https://www.cloudflare.com/products/registrar/
