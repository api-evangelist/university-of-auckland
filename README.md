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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Waipapa Taumata Rau | The University of Auckland is New Zealand's largest and highest-ranked university. This repository catalogs its public developer and API footprint as an [APIs.json](https://apisjson.org) provider profile, re-profiled on 2026-08-30 under the API Evangelist **university pipeline**, which settles **who operates each surface** before saving any contract.

Unlike most of this cohort, Auckland genuinely runs an API programme of its own: a **Kong developer portal** at `developer.auckland.ac.nz/prd` and a **Kong gateway** at `apis.auckland.ac.nz`, publishing two OpenAPI 3.1.0 contracts over its PeopleSoft Campus Solutions (CS9) student records. It also self-hosts a DSpace repository with a live OAI-PMH 2.0 service and runs its own Shibboleth/SAML 2.0 identity provider.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/university-of-auckland/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=university-of-auckland-api-evangelist&utm_content=repo

## Type

- university / Public Research University / Index / Provider / 3rd-Party

## Tags

University, Higher Education, Education, New Zealand, Public Research University, Universitas 21, Course Catalog, Student Records, Research Data, Research Repository, Identity Federation, OAI-PMH

## Surfaces, by operator

Every entry carries an `x-operator`: **institution** (Auckland runs it, on its own domain), **tenant** (Auckland's data and account, the vendor's contract), or **vendor** (not Auckland's at all — never saved here).

### institution

- **Course Catalog Api V3** — `https://apis.auckland.ac.nz/courses/v3` · 12 read-only operations over CS9 course views (courses, terms, subjects, consent/component codes, academic orgs, groups, careers). OpenAPI 3.1.0 saved. Live, HTTP 401 without a portal-issued key. Docs: https://developer.auckland.ac.nz/prd/documentation/api-course-catalog-v3
- **Classes Api V2** — `https://apis.auckland.ac.nz/classes/v2` · class search with 16 query parameters returning class records and meeting patterns. OpenAPI 3.1.0 saved. Live, HTTP 401 without a key. Docs: https://developer.auckland.ac.nz/prd/documentation/api-classes-v2
- **ResearchSpace OAI-PMH 2.0** — `https://researchspace.auckland.ac.nz/server/oai/request` · self-hosted DSpace, 13 metadata formats, institutional sets. Verified via `verb=Identify`.
- **ResearchSpace DSpace REST API** — `https://researchspace.auckland.ac.nz/server/api` · HAL+JSON, community tree readable anonymously. Contract is upstream DSpace's, so **no specification is saved here**.
- **Shibboleth Identity Provider (SAML 2.0 metadata)** — `https://iam.auckland.ac.nz/shibboleth` · entityID `http://iam.auckland.ac.nz/idp`, `shibmd:Scope` `auckland.ac.nz`.

### tenant

- **Figshare research data repository** — https://auckland.figshare.com/ · institution id 12, DOIs under `10.17608/k6.auckland`. The relationship is Auckland's; the `api.figshare.com/v2` contract is Figshare's and is **not** saved here.
- **Ex Libris Primo library discovery** — `vid=64UAUCK_INST:UOA`. No institution-published catalogue API exists.

## Artifacts

- OpenAPI (searched, saved verbatim): [openapi/](openapi/) with pristine copies in [openapi/_original/](openapi/_original/)
- JSON Schema (derived): [json-schema/](json-schema/)
- Example (derived, shape only — the live route returns 401): [examples/](examples/)
- Authentication · Errors · Lifecycle · Rules · Vocabulary (derived): [authentication/](authentication/) · [errors/](errors/) · [lifecycle/](lifecycle/) · [rules/](rules/) · [vocabulary/](vocabulary/)
- Conformance (probed): [conformance/university-of-auckland-conformance.yml](conformance/university-of-auckland-conformance.yml) — `oai-pmh`, `saml` and `shibboleth` met with evidence; `scim`, `lti`, `oneroster`, `ed-fi`, `caliper`, `qti`, `orcid`, `datacite`, `crossref` explicitly **not** claimed.
- Domain Security (probed): [security/university-of-auckland-domain-security.yml](security/university-of-auckland-domain-security.yml)
- Plans · Rate Limits · FinOps: [plans/](plans/) · [rate-limits/](rate-limits/) · [finops/](finops/)
- Per-URL HTTP statuses: [review.yml](review.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-30

## Common Properties

- Website: https://www.auckland.ac.nz/
- Developer Portal: https://developer.auckland.ac.nz/prd/
- API Reference: https://developer.auckland.ac.nz/prd/documentation
- GitHub: https://github.com/university-of-auckland · https://github.com/UoA-eResearch
- LinkedIn: https://www.linkedin.com/school/university-of-auckland/
- Review: [review.yml](review.yml)

## Notes — what changed on 2026-08-30, and why

The June 2026 profile credited this institution with **eleven APIs**. All eleven were one document: Figshare's generic `api.figshare.com/v2` REST specification (`info.title: Figshare API`, `contact: Figshare Support`), which the refine step had split by tag into ten per-tag OpenAPIs. Twenty-two vendor-attributed surfaces, and every artifact derived from them — collections, schemas, examples, JSON-LD, vocabulary, rulesets, scopes, authentication, agentic-access and a capability map — have been removed. That work is Figshare's engineering and is scored against Figshare's own profile, where it belongs.

Removed as dead, not merely unverified: `unidirectory.auckland.ac.nz` (the University Directory API) has **no DNS record**.

Confirmed absences, each probed rather than assumed: no open data portal (`data.auckland.ac.nz` redirects to a WordPress login), no `llms.txt`, no `.well-known/security.txt`, no status page, no changelog, no deprecation policy, no published scope list or token endpoint.

Defects in the University's own documents are recorded, not silently repaired: `servers[0].url` in Course Catalog Api V3 reads `httpss://…`; `info.version` reads `3.0` in both documents including the v2 API; `securitySchemes.apikey` omits `name` and `in`; and 4xx/5xx responses reuse the success schema.

**This correction lowers the apparent footprint, and that is the point.** No endpoints were fabricated. See [review.yml](review.yml) for per-URL HTTP statuses and [apis.yml](apis.yml) `x-coverage` for the coverage disclosure.

## Maintainers

- Kin Lane — kin@apievangelist.com
