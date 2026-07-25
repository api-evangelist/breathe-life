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

## Links

- [Website (decommissioned)](https://www.breathelife.com/)
- [Wayback Machine snapshot, 2022-10-05](https://web.archive.org/web/20221005001219/https://www.breathelife.com/)
- [LinkedIn](https://www.linkedin.com/company/breathe-life/)
- [Facebook](https://www.facebook.com/breathelifeinsurance/)
- [GitHub organization: getbreathelife](https://github.com/getbreathelife)
- [SE2 acquires Breathe Life, 2022-03-28 (archived)](https://web.archive.org/web/20220519024512/https://www.breathelife.com/se2-acquires-breathe-life-to-scale-saas-product-and-data-capabilities-for-carriers-across-the-insurance-lifecycle/)
- [Zinnia (acquirer, formerly SE2)](https://zinnia.com/)
- [Zinnia Developer Portal](https://developers.zinnia.com/) — Zinnia's portal, not Breathe Life's
