# Breathe Life (breathe-life)

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
