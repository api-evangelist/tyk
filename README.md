# Tyk (tyk)

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
