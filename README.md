# Breathe Life (breathe-life)

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

Breathe Life is a Montreal, Quebec based life insurance technology company — an enterprise SaaS core-systems vendor rather than a carrier or a broker — founded in 2018 to sell life insurers a modern new-business origination and distribution platform. Its product was the Breathe Life Hybrid Origination (Hybrid Distribution) Platform, sold either end-to-end or as four separately licensable modules: Quoter, Hybrid e-App, Advisor Tools and Data Dashboards, supporting advisor-driven, consumer self-serve, or blended selling of individual life products. Its home market is Canada. SE2, an Eldridge business, announced its acquisition of Breathe Life on 2022-03-28; SE2 subsequently rebranded as Zinnia, and breathelife.com has since been decommissioned.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/breathe-life/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/breathe-life/refs/heads/main/apis.yml)

## Tags

- Insurance
- Canada
- Life Insurance
- Insurtech
- Core Systems
- Policy Origination
- Quoting
- Underwriting
- Agent Tools
- SaaS
- Acquired

## Timestamps

- **Created:** 2026-07-25
- **Modified:** 2026-07-25

## APIs

Breathe Life publishes no public API.

This is the honest and expected outcome for this company. Every first-party developer hostname and path probed on 2026-07-25 either failed to resolve or returned 404, and the company's primary domain no longer serves a website at all:

- `breathelife.com` — HTTP 404, nginx "Site Not Configured"
- `www.breathelife.com` — HTTP 404, WP Engine "Site is not available"
- `developer.breathelife.com`, `developers.breathelife.com`, `docs.breathelife.com`, `api.breathelife.com` — DNS does not resolve
- `status.breathelife.com` — dangling CNAME to Atlassian Statuspage; HTTP 302 to statuspage.io

The full Wayback Machine index of the site (1,164 archived URLs, 2018–2023) contains no `/developers`, `/api`, `/docs`, `/swagger`, `/openapi` or `/integrations` path — only two blog tag pages, `/tag/developer/` and `/tag/software-developer/`. No OpenAPI, Swagger, AsyncAPI, GraphQL SDL, `.proto` or Postman collection was ever published, so the `openapi/` directory is intentionally omitted from this repo.

Quote, bind, issue and FNOL all existed as real product capability inside the Hybrid Origination Platform — the Quoter and Hybrid e-App modules are literally quote and application capture — but they were delivered as a carrier-licensed, login-gated SaaS application, never as an addressable public API.

**ACORD posture: no ACORD reference found.** No occurrence of ACORD, AL3, ACORD XML, NGDS, IVANS, Applied Epic or Vertafore appears on any archived Breathe Life page, in the GitHub organization, or in any published npm package.

## Artifacts

Enrichment round 2026-07-25. With no API to ground spec-derived artifacts in, the only artifacts that can honestly exist here are registry, probe and lifecycle records:

- [`packages/breathe-life-packages.yml`](packages/breathe-life-packages.yml) — six first-party npm packages (`@breathelife/prettier-plugin-sort-imports`, three `eslint-config-breathelife-*`, two `cls-hooked` forks) plus the `getbreathelife/onespansign` Terraform provider (0.1.1-beta, 3,863 downloads). All internal tooling or third-party API clients; no product SDK, so no `SDKs` pointer is claimed.
- [`well-known/breathe-life-well-known.yml`](well-known/breathe-life-well-known.yml) — every `/.well-known/` path probed on both surviving hosts returned HTTP 404.
- [`conformance/breathe-life-conformance.yml`](conformance/breathe-life-conformance.yml) — the historical PCI DSS / SOC 2 Type II / SOC 3 attestations from the archived Security page, plus API-standard conformance (all false by absence).
- [`lifecycle/breathe-life-lifecycle.yml`](lifecycle/breathe-life-lifecycle.yml) — terminal lifecycle record: acquisition, decommissioning, the deleted Atlassian status page, and the company timeline.
- [`security/breathe-life-domain-security.yml`](security/breathe-life-domain-security.yml) — TLS/HSTS/DNSSEC/CAA/SPF/DMARC probe. No DNSSEC, CAA limited to Let's Encrypt, SPF and DMARC present with `p=none`, and the presented certificate does not match the hostname.
- [`llms/breathe-life-llms.txt`](llms/breathe-life-llms.txt) — generated llms.txt (`/llms.txt` on the live host returns 404).

Deliberately absent, because the underlying thing does not exist: `openapi/`, `asyncapi/`, `graphql/`, `mcp/`, `skills/`, `scopes/`, `authentication/`, `conventions/`, `errors/`, `sandbox/`, `cli/`, `components/`, `data-model/`, `changelog/`, `overlays/`, `grpc/`. No `StatusPage`, `Compliance`, `PrivacyPolicy`, `WellKnown` or `Security` pointer is wired either — each of those checks asserts a live public surface, and Breathe Life has none.

## Links

- [Website (decommissioned)](https://www.breathelife.com/)
- [Wayback Machine snapshot, 2022-10-05](https://web.archive.org/web/20221005001219/https://www.breathelife.com/)
- [LinkedIn](https://www.linkedin.com/company/breathe-life/)
- [Facebook](https://www.facebook.com/breathelifeinsurance/)
- [GitHub organization: getbreathelife](https://github.com/getbreathelife)
- [SE2 acquires Breathe Life, 2022-03-28 (archived)](https://web.archive.org/web/20220519024512/https://www.breathelife.com/se2-acquires-breathe-life-to-scale-saas-product-and-data-capabilities-for-carriers-across-the-insurance-lifecycle/)
- [Zinnia (acquirer, formerly SE2)](https://zinnia.com/)
- [Zinnia Developer Portal](https://developers.zinnia.com/) — Zinnia's portal, not Breathe Life's
