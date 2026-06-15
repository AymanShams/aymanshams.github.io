# non-functional requirements

## performance

- Pages should load quickly on ordinary mobile connections.
- Avoid large images and unused assets in v1.
- Use one small CSS file.
- Do not add JavaScript unless approved.

## accessibility

- Use semantic HTML.
- Keep heading order logical.
- Use descriptive link text.
- Provide visible keyboard focus.
- Maintain strong color contrast.
- Do not rely on color alone to communicate meaning.

## reliability

- Site should work as static files.
- No runtime server dependency.
- No build step required.
- GitHub Pages is the only hosting dependency in v1.

## security and privacy

- No visitor data collection.
- No third-party scripts.
- No secrets in repo.
- No PHI, client, patient, payer, payment, contract, or internal operations details.

## maintainability

- Keep file structure simple.
- Keep content page-specific.
- Update docs when project scope or architecture changes.
- Record material architecture changes in ADRs.
