# University of Auckland (university-of-auckland)

The University of Auckland is New Zealand's largest and highest-ranked university, placed #92 in the QS World University Rankings 2025. This repository catalogs its public developer and API footprint as an [APIs.json](https://apisjson.org) provider profile. The footprint is modest and decentralized — there is no single unified developer portal — and is anchored by the institution's Figshare research data repository (REST + OAI-PMH), a public University Directory staff API, and a domain-verified GitHub organization.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/university-of-auckland/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=university-of-auckland-api-evangelist&utm_content=repo

## Type

- Index / Consumer / 3rd-Party

## Tags

Education, Higher Education, University, Research Data, Open Data, New Zealand

## APIs

- **University of Auckland Figshare Research Repository API** — Figshare v2 REST API exposing public articles, datasets, and collections (filter `institution=12`). Docs: https://docs.figshare.com/ · Repository: https://auckland.figshare.com/
- **University of Auckland Figshare OAI-PMH Service** — OAI-PMH metadata harvesting for the institutional research repository. Docs: https://docs.figshare.com/old_docs/OAI-PMH/
- **University Directory API** — Public staff search, summary-profile, and full-profile APIs. Docs: https://unidirectory.auckland.ac.nz/apidocs (documented public; host did not resolve from the verification environment)

## Plans / Rate Limits / FinOps

- Plans & Pricing: [plans/university-of-auckland-plans-pricing.yml](plans/university-of-auckland-plans-pricing.yml)
- Rate Limits: [rate-limits/university-of-auckland-rate-limits.yml](rate-limits/university-of-auckland-rate-limits.yml)
- FinOps: [finops/university-of-auckland-finops.yml](finops/university-of-auckland-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.auckland.ac.nz/
- GitHub: https://github.com/university-of-auckland
- LinkedIn: https://www.linkedin.com/school/university-of-auckland/
- Review: [review.yml](review.yml)

## Notes

This profile reflects only confirmed or clearly documented public resources — no endpoints were fabricated. The Figshare REST API, OAI-PMH service, documentation, official website, GitHub org, and staff profiles site were probed live and returned successful responses; Figshare's `institution=12` mapping was confirmed via `k6.auckland` DOIs. The University Directory API is documented as publicly accessible, but `unidirectory.auckland.ac.nz` did not resolve from the verification environment, so it is cataloged from documentation references with a caveat. See [review.yml](review.yml) for per-URL HTTP statuses.

## Maintainers

- Kin Lane — kin@apievangelist.com
