# University of Auckland (university-of-auckland)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
