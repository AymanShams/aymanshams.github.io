# project brief

## decision

Create a lean personal GitHub Pages site for Ayman Shams. The site will be the umbrella for public work across Codex Coding OS, healthcare operations, insurance operations, and operating notes.

Use the GitHub user-site repository `aymanshams.github.io` under the `AymanShams` account. Build the first version as static HTML and CSS, with no framework, no backend, no forms, no analytics, and no custom domain at launch.

## problem

People who find Ayman through GitHub, LinkedIn, healthcare work, or operating notes need one credible place to understand what he works on and where to go next. Without a personal umbrella site, each project risks looking disconnected, overexplained, or incorrectly positioned as the parent brand.

## users

| User type | Need | Priority |
|---|---|---|
| Technical reviewer | Understand Codex Coding OS quickly, see the independence disclaimer, and reach the GitHub project | High |
| Founder or partner | Understand Ayman's operating focus without a sales-heavy page | High |
| Healthcare operator | See the connection between digital health, primary care, chronic care, and process design | High |
| Insurance operations partner | Understand that SiriusShield is one work area, not the umbrella identity | Medium |
| Reader from LinkedIn | Find concise operating notes and public writing | Medium |

## goals

- Make Ayman Shams the clear umbrella identity.
- Give each work area a short, credible landing point.
- Keep v1 simple enough to ship and maintain.
- Avoid marketing-heavy sections, exaggerated claims, and generic personal-brand language.
- Keep healthcare and insurance wording accurate without exposing sensitive operational details.

## non-goals

- No HealPath or SiriusShield umbrella brand.
- No database, authentication, backend, forms, payments, CMS, newsletter engine, or analytics in v1.
- No detailed case studies with client, patient, payer, financial, PHI, or internal workflow data.
- No claim that Codex Coding OS is connected to OpenAI.
- No custom domain during the first launch.

## first release scope

- Homepage at `https://aymanshams.github.io/`.
- Codex Coding OS page with the approved OpenAI non-affiliation disclaimer.
- Healthcare operations page covering HealPath, primary care, chronic care, and digital health work at a high level.
- Operating notes page for writing on AI governance, healthcare operations, process design, and operational excellence.
- Minimal navigation, text-only layout, responsive design, and accessible HTML.
- GitHub, LinkedIn, and booking links when approved and checked. Omit email until a public address is supplied.

## later scope

- Custom domain, preferably `aymanshams.com` if available.
- Public writing index with dated notes.
- Selected project case notes after sensitive details are removed.
- Optional RSS feed if writing becomes active.
- Optional privacy-respecting analytics only if there is a specific decision need.

## data involved

| Data type | Example | Sensitivity | Source of truth | Owner |
|---|---|---|---|---|
| Public profile copy | Name, role summary, work areas | Public | Approved site copy | Ayman Shams |
| Project and contact links | GitHub repositories, LinkedIn profile, Google Calendar booking page, project websites | Public | Approved and checked public URLs | Ayman Shams |
| Business descriptions | HealPath and SiriusShield summaries | Business sensitive if over-detailed | Approved portfolio wording | Ayman Shams |
| Writing topics | AI governance, operating notes | Public after approval | Approved pages | Ayman Shams |

## integrations

| Integration | Purpose | Required for first release | Source authority |
|---|---|---|---|
| GitHub Pages | Static site hosting | Yes | GitHub Docs |
| GitHub repository | Site source and public deployment | Yes | User answer |
| Custom domain | Personal URL | No | User answer |
| Cloudflare Registrar or similar low-cost registrar | Future domain purchase and DNS | No | Cloudflare public registrar page |

## constraints

- Budget: keep v1 at zero hosting cost and defer domain spend.
- Deployment: GitHub Pages from the root of `main`.
- Privacy and compliance: do not publish PHI, client names, patient details, internal operating details, or unsupported performance claims.
- Maintenance: plain static files only so future updates can be done without a build chain.

## open material decisions

No material decisions block controlled-doc approval.

## safe assumptions

- Use text-only v1 unless the user later supplies a preferred headshot or visual identity.
- Use a serious, restrained voice.
- Use subpages instead of one long homepage because the audience includes technical and healthcare readers with different intent.
