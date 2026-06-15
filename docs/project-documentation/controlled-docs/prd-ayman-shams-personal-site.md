# PRD: Ayman Shams personal site

## 1. summary

Ayman Shams needs a lean personal site that acts as the umbrella for his public work. The first release should help serious readers understand the main work areas, then route them to the right project or profile without marketing bloat.

## 2. contacts

| Name | Role | Comment |
|---|---|---|
| Ayman Shams | Owner and final approver | Owns identity, content, links, and approval to code |
| Codex | Documentation and implementation assistant | May draft docs and code only inside approved gates |

## 3. background

Ayman's public work spans AI-assisted coding workflows, digital health operations, insurance operations, and writing about operating systems for work. These areas should be connected under the personal name rather than under HealPath or SiriusShield.

The site should serve people who arrive from GitHub or LinkedIn. They likely want quick orientation, proof of seriousness, and a path to the relevant work. They do not need a large marketing homepage.

## 4. objective

Create a public personal landing page that makes the umbrella identity clear and sends each reader to the right next page.

Key results for v1:

| Objective | Key result | Measurement |
|---|---|---|
| Clear positioning | A first-time reader can state the four work areas after one homepage scan | Manual review |
| Technical trust | Codex Coding OS has a visible GitHub route and OpenAI non-affiliation disclaimer | Page review |
| Professional restraint | Homepage has no inflated claims, sales funnel, popups, or generic founder language | Content review |
| Maintainability | Site can be edited with plain HTML and CSS | Repo review |
| Safe publishing | No sensitive healthcare, insurance, client, patient, or internal operations data is published | Content review |

## 5. market segments

| Segment | Job to be done | Site need |
|---|---|---|
| Technical reviewers | Evaluate Codex Coding OS and Ayman's work discipline | Clear project page, disclaimer, GitHub link |
| Founders and partners | Understand where Ayman can contribute | Short, serious overview of work areas |
| Healthcare operators | See healthcare operations and process-design relevance | Healthcare operations page without sensitive details |
| Insurance operations partners | Understand SiriusShield as a work area | Short mention under operations scope |
| LinkedIn readers | Find public notes and project links | Writing page and contact links |

## 6. value propositions

- Ayman has one stable public home for serious reviewers.
- Codex Coding OS is presented as an independent open-source project with correct boundaries.
- HealPath and SiriusShield are visible without becoming the umbrella brand.
- Writing and operating notes have a place to grow without forcing a blog engine into v1.
- The site stays simple enough to maintain.

## 7. solution

### 7.1 routes

| Route | Purpose |
|---|---|
| `/` | Personal umbrella homepage |
| `/codex-coding-os/` | Codex Coding OS overview and disclaimer |
| `/healthcare-operations/` | HealPath, digital health, primary care, chronic care, and insurance operations overview |
| `/notes/` | Writing and operating notes index |
| `/404.html` | Simple not-found page |

### 7.2 homepage content

The homepage should include:

1. Name and short positioning line.
2. Four work areas in a compact layout:
   - Codex Coding OS
   - Healthcare operations and digital health
   - Medical insurance operations
   - Writing and operating notes
3. Short "current focus" section.
4. Links to GitHub and LinkedIn when verified.

### 7.3 Codex Coding OS page

The page must include this exact disclaimer:

> Codex Coding OS is an independent open-source project and is not affiliated with, endorsed by, or sponsored by OpenAI.

The page should explain the project in plain language:

- A workflow system for disciplined AI-assisted coding.
- Focus areas: manifests, gates, repo instructions, handoffs, review, and validation.
- Link to the GitHub repository when verified.

### 7.4 healthcare operations page

The page should describe the work area without over-claiming:

- Digital health operations.
- Primary care and chronic care management.
- Workflow design, quality, process controls, and implementation discipline.
- SiriusShield as medical insurance operations BPO work.
- Links to the public HealPath and SiriusShield websites when verified.

No patient details, client details, performance claims, financial metrics, or internal operating procedures should be included.

### 7.5 notes page

The page should start as a simple index with concise public working principles. It should not publish empty coming-soon or placeholder copy.

- Healthcare operations.
- AI governance.
- Process design.
- Operational excellence.
- AI-assisted coding workflows.

### 7.6 technology

Use static HTML and CSS. Add a `.nojekyll` file so GitHub Pages serves files directly without Jekyll processing. Use minimal JavaScript only if a later approved feature requires it.

### 7.7 assumptions

- The site will be public.
- The GitHub account is `AymanShams`.
- Actual GitHub, project website, and LinkedIn URLs will be verified before publishing.
- Email will be omitted until a public address is approved.
- Custom domain will be deferred.

## 8. release

v1 should be one small implementation slice:

- Create the repo or use the existing `aymanshams.github.io` repo.
- Add static pages.
- Enable GitHub Pages from root on `main`.
- Verify links, responsive layout, accessibility basics, and published URL.

Later releases can add a custom domain, selected writing pages, and curated case notes.
