# security guidelines

## decision

Keep v1 static and data-minimal. The safest first version is a public site that does not collect, store, or process user data.

## data classification

| Data | Classification | Rule |
|---|---|---|
| Public page copy | Public | Publish only after review |
| GitHub, LinkedIn, booking, and project URLs | Public | Check before publishing and document platform verification limitations |
| Email address | Personal contact data | Omit until approved |
| HealPath details | Business sensitive if detailed | Keep portfolio-level only |
| SiriusShield details | Business sensitive if detailed | Keep portfolio-level only |
| Patient, client, payer, or PHI content | Restricted | Never publish |

PHI means protected health information.

## controls

- No forms.
- No cookies.
- No analytics.
- No third-party scripts.
- No inline JavaScript.
- No secrets in the repository.
- No API keys in frontend code.
- No patient, client, payer, or internal operating data.
- External links should use safe link attributes when opening a new tab.

## frontend security requirements

If JavaScript is added later:

- Do not use `innerHTML` for untrusted content.
- Do not use `eval`, `new Function`, or string-based timers.
- Do not inject third-party scripts without review.
- Do not store secrets in `localStorage` or `sessionStorage`.
- Validate URLs before assigning them to `href`, `src`, or navigation targets.

## content review rules

Before publishing, review every page for:

- OpenAI affiliation risk.
- Unsupported claims about Codex Coding OS.
- Healthcare service claims that need legal or regulatory review.
- Patient, client, payer, payment, contract, or internal operations details.
- Business details that belong in private HealPath or SiriusShield materials.

## OpenAI disclaimer rule

The Codex Coding OS page must include this exact sentence:

> Codex Coding OS is an independent open-source project and is not affiliated with, endorsed by, or sponsored by OpenAI.

## domain security later

If a custom domain is added later:

- Verify the domain in GitHub before attaching it to the Pages site.
- Prefer a `www` subdomain configuration.
- Keep DNS records aligned with the active GitHub Pages site.
- Remove stale DNS records if the Pages site is disabled or moved.

## sources

- GitHub Docs, About custom domains and GitHub Pages: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/about-custom-domains-and-github-pages
- Security Best Practices skill, JavaScript general web frontend security reference.
