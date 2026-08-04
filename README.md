# Tyk (tyk)

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

Tyk is an open-source API gateway and management platform supporting REST, GraphQL, gRPC, and Async APIs with a developer portal, analytics, and flexible deployment across cloud, on-premise, and hybrid environments.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- API Gateway
- API Management
- GraphQL
- Open Source

## Timestamps

- **Created:** 2026-03-18
- **Modified:** 2026-05-19

## APIs

### Tyk Gateway API

The Tyk Gateway API provides a RESTful interface for managing API definitions, keys, certificates, and health checks directly on a Tyk Gateway node. It is used to configure and operate the gateway programmatically in self-managed and open-source deployments.

- **Human URL:** [https://tyk.io/docs/tyk-apis/](https://tyk.io/docs/tyk-apis/)
- **Base URL:** `https://tyk.io/`

#### Tags

- Administration
- Gateway
- Open Source
- REST API

#### Properties

- [Documentation](https://tyk.io/docs/tyk-apis/)
- [OpenAPI](openapi/tyk-gateway-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tyk-gateway-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tyk-gateway-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/tyk-gateway-access-definition-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/tyk-gateway-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [GitHub Repository](https://github.com/TykTechnologies/tyk)

### Tyk Dashboard API

The Tyk Dashboard API is a superset of the Gateway API providing programmatic access to a centralized database of API definitions, keys, policies, users, and organizations. It is the primary integration point for managing multi-team Tyk deployments and is authenticated via an access credentials header.

- **Human URL:** [https://tyk.io/docs/tyk-dashboard-api](https://tyk.io/docs/tyk-dashboard-api)
- **Base URL:** `https://tyk.io/`

#### Tags

- Administration
- Dashboard
- Management
- REST API

#### Properties

- [Documentation](https://tyk.io/docs/tyk-dashboard-api)
- [OpenAPI](openapi/tyk-dashboard-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tyk-dashboard-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tyk-dashboard-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Changelog](https://tyk.io/docs/developer-support/release-notes/dashboard)
- [GitHub Repository](https://github.com/TykTechnologies/tyk-analytics)

### Tyk Dashboard Admin API

The Tyk Dashboard Admin API provides super-administrative access to the Tyk Dashboard, enabling management of organizations and system-level configuration. It is used for bootstrapping and managing multi-organization Tyk deployments.

- **Human URL:** [https://tyk.io/docs/tyk-dashboard-api](https://tyk.io/docs/tyk-dashboard-api)
- **Base URL:** `https://tyk.io/`

#### Tags

- Admin
- Dashboard
- Multi-Tenant
- REST API

#### Properties

- [Documentation](https://tyk.io/docs/tyk-dashboard-api)
- [OpenAPI](openapi/tyk-dashboard-admin-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tyk-dashboard-admin-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tyk-dashboard-admin-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [GitHub Repository](https://github.com/TykTechnologies/tyk-analytics)

### Tyk MDCB API

The Tyk Multi Data Centre Bridge (MDCB) API enables synchronization of API configurations, keys, and policies across geographically distributed Tyk Gateway clusters. It provides a control plane for managing multiple data center deployments from a single Tyk Dashboard.

- **Human URL:** [https://tyk.io/docs/](https://tyk.io/docs/)
- **Base URL:** `https://tyk.io/`

#### Tags

- MDCB
- Multi-Data Center
- REST API
- Synchronization

#### Properties

- [Documentation](https://tyk.io/docs/)
- [OpenAPI](openapi/tyk-mdcb-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tyk-mdcb-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tyk-mdcb-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/tyk-mdcb-data-plane-config-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/tyk-mdcb-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [GitHub Repository](https://github.com/TykTechnologies/tyk-sink)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/tyk)
- [Portal](https://tyk.io/)
- [Documentation](https://tyk.io/docs/)
- [Getting Started](https://tyk.io/docs/getting-started/)
- [Authentication](https://tyk.io/docs/basic-config-and-security/security/authentication-authorization/)
- [Blog](https://tyk.io/blog/)
- [Changelog](https://tyk.io/docs/developer-support/release-notes/dashboard)
- [GitHub Organization](https://github.com/TykTechnologies)
- [GitHub Repository](https://github.com/TykTechnologies/tyk)
- [Support](https://community.tyk.io/)
- [F A Q](https://tyk.io/docs/frequently-asked-questions/)
- [Pricing](https://tyk.io/price-comparison/)
- [C L I](https://github.com/TykTechnologies/tyk-cli)
- [SDK](https://github.com/TykTechnologies/tyk)
- [Spectral Rules](rules/tyk-spectral-rules.yml)
- [Vocabulary](vocabulary/tyk-vocabulary.yaml)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [M C P Server](https://github.com/TykTechnologies/tyk-dashboard-mcp)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
