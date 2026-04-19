# Tyk (tyk)
Tyk is an open-source API gateway and management platform supporting REST, GraphQL, gRPC, and Async APIs with a developer portal, analytics, and flexible deployment across cloud, on-premise, and hybrid environments.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - API Gateway, API Management, GraphQL, Open Source

## Timestamps

- **Created:** 2026-03-18
- **Modified:** 2026-04-19

## APIs

### Tyk Gateway API
The Tyk Gateway API provides a RESTful interface for managing API definitions, keys, certificates, and health checks directly on a Tyk Gateway node. It is used to configure and operate the gateway programmatically in self-managed and open-source deployments.

**Human URL:** [https://tyk.io/docs/tyk-apis/](https://tyk.io/docs/tyk-apis/)

#### Tags:

 - Administration, Gateway, Open Source, REST API

#### Properties

- [Documentation](https://tyk.io/docs/tyk-apis/)
- [OpenAPI](openapi/tyk-gateway-api-openapi.yml)
- [JSONSchema](json-schema/tyk-gateway-access-definition-schema.json)
- [JSONLD](json-ld/tyk-gateway-context.jsonld)
- [GitHubRepository](https://github.com/TykTechnologies/tyk)

### Tyk Dashboard API
The Tyk Dashboard API is a superset of the Gateway API providing programmatic access to a centralized database of API definitions, keys, policies, users, and organizations. It is the primary integration point for managing multi-team Tyk deployments and is authenticated via an access credentials header.

**Human URL:** [https://tyk.io/docs/tyk-dashboard-api](https://tyk.io/docs/tyk-dashboard-api)

#### Tags:

 - Administration, Dashboard, Management, REST API

#### Properties

- [Documentation](https://tyk.io/docs/tyk-dashboard-api)
- [OpenAPI](openapi/tyk-dashboard-api-openapi.yml)
- [ChangeLog](https://tyk.io/docs/developer-support/release-notes/dashboard)
- [GitHubRepository](https://github.com/TykTechnologies/tyk-analytics)

### Tyk Dashboard Admin API
The Tyk Dashboard Admin API provides super-administrative access to the Tyk Dashboard, enabling management of organizations and system-level configuration. It is used for bootstrapping and managing multi-organization Tyk deployments.

**Human URL:** [https://tyk.io/docs/tyk-dashboard-api](https://tyk.io/docs/tyk-dashboard-api)

#### Tags:

 - Admin, Dashboard, Multi-Tenant, REST API

#### Properties

- [Documentation](https://tyk.io/docs/tyk-dashboard-api)
- [OpenAPI](openapi/tyk-dashboard-admin-api-openapi.yml)
- [GitHubRepository](https://github.com/TykTechnologies/tyk-analytics)

### Tyk MDCB API
The Tyk Multi Data Centre Bridge (MDCB) API enables synchronization of API configurations, keys, and policies across geographically distributed Tyk Gateway clusters. It provides a control plane for managing multiple data center deployments from a single Tyk Dashboard.

**Human URL:** [https://tyk.io/docs/](https://tyk.io/docs/)

#### Tags:

 - MDCB, Multi-Data Center, REST API, Synchronization

#### Properties

- [Documentation](https://tyk.io/docs/)
- [OpenAPI](openapi/tyk-mdcb-api-openapi.yml)
- [JSONSchema](json-schema/tyk-mdcb-data-plane-config-schema.json)
- [JSONLD](json-ld/tyk-mdcb-context.jsonld)
- [GitHubRepository](https://github.com/TykTechnologies/tyk-sink)

## Common Properties

- [Portal](https://tyk.io/)
- [Documentation](https://tyk.io/docs/)
- [GettingStarted](https://tyk.io/docs/getting-started/)
- [Authentication](https://tyk.io/docs/basic-config-and-security/security/authentication-authorization/)
- [Blog](https://tyk.io/blog/)
- [ChangeLog](https://tyk.io/docs/developer-support/release-notes/dashboard)
- [GitHubOrganization](https://github.com/TykTechnologies)
- [GitHubRepository](https://github.com/TykTechnologies/tyk)
- [Support](https://community.tyk.io/)
- [FAQ](https://tyk.io/docs/frequently-asked-questions/)
- [Pricing](https://tyk.io/price-comparison/)
- [CLI](https://github.com/TykTechnologies/tyk-cli)
- [SDK - Go Gateway SDK](https://github.com/TykTechnologies/tyk)

## Features

| Name | Description |
|------|-------------|
| API Gateway | High-performance, open-source API gateway supporting REST, GraphQL, gRPC, TCP, and async APIs with low-latency request proxying. |
| Rate Limiting | Configurable rate limiting and throttling policies to protect backend services from traffic spikes and abuse. |
| Authentication | Multiple authentication methods including API keys, JWT, OAuth 2.0, mutual TLS, OpenID Connect, and basic auth. |
| Analytics and Monitoring | Real-time API analytics, traffic monitoring, and detailed logging with export to multiple backend stores. |
| Developer Portal | Customizable developer portal for API documentation, key management, and developer onboarding. |
| GraphQL Support | Native GraphQL proxy and Universal Data Graph for federating REST and GraphQL APIs into a single graph endpoint. |
| API Versioning | Built-in support for API versioning with URL, header, and query parameter-based version routing. |
| Policy Management | Centralized access control policies for managing rate limits, quotas, and access rights across multiple APIs. |
| Multi Data Center | MDCB enables synchronization of API configurations and keys across geographically distributed gateway clusters. |
| Plugin System | Extensible middleware plugin system supporting Go, Python, JavaScript, Lua, and gRPC-based custom plugins. |
| AI Gateway | Tyk AI Studio provides an AI gateway for managing, governing, and interacting with AI models across your organization. |

## Use Cases

| Name | Description |
|------|-------------|
| API Monetization | Enable API-as-a-product strategies with tiered plans, usage tracking, and developer self-service through the portal. |
| Microservices Gateway | Centralize traffic management, authentication, and observability for microservices architectures. |
| Multi-Cloud API Management | Deploy gateways across cloud, on-premise, and hybrid environments with centralized management. |
| Legacy API Modernization | Wrap legacy SOAP and XML APIs with modern REST or GraphQL interfaces using Tyk's transformation middleware. |
| Partner API Program | Manage third-party developer access with fine-grained policies, quota management, and analytics per consumer. |
| AI API Management | Govern and manage AI model APIs with rate limiting, access control, and usage analytics through Tyk AI Studio. |

## Integrations

| Name | Description |
|------|-------------|
| Kubernetes | Tyk Operator provides native Kubernetes integration for managing API definitions and policies as custom resources. |
| Terraform | Infrastructure-as-code provider for managing Tyk configurations through Terraform. |
| Keycloak | Integration with Keycloak for OAuth 2.0 and OpenID Connect authentication flows. |
| Auth0 | Support for Auth0 as an identity provider for JWT validation and OAuth 2.0 token management. |
| Prometheus | Export gateway metrics to Prometheus for monitoring and alerting with Grafana dashboards. |
| OpenTelemetry | Distributed tracing integration with OpenTelemetry for end-to-end request visibility. |
| Backstage | Backstage plugin for viewing and managing Tyk API definitions from within the Backstage developer portal. |
| Jenkins | CI/CD integration for automated API deployment and configuration updates through Jenkins pipelines. |
| Ansible | Ansible playbooks for automated Tyk gateway and dashboard provisioning and configuration. |
| Helm Charts | Official Helm charts for deploying Tyk components on Kubernetes clusters. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Tyk Gateway API](openapi/tyk-gateway-api-openapi.yml)
- [Tyk Dashboard API](openapi/tyk-dashboard-api-openapi.yml)
- [Tyk Dashboard Admin API](openapi/tyk-dashboard-admin-api-openapi.yml)
- [Tyk MDCB API](openapi/tyk-mdcb-api-openapi.yml)

### JSON Schema

- 213 schema files in [json-schema/](json-schema/)

### JSON Structure

- 213 structure files in [json-structure/](json-structure/)

### JSON-LD

- [Tyk Gateway Context](json-ld/tyk-gateway-context.jsonld)
- [Tyk MDCB Context](json-ld/tyk-mdcb-context.jsonld)

### Examples

- 213 example files in [examples/](examples/)

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [Tyk Gateway](capabilities/shared/gateway.yaml) -- 16 operations for API definition, key, policy, and certificate management
- [Tyk Dashboard](capabilities/shared/dashboard.yaml) -- 12 operations for centralized API management
- [Tyk Dashboard Admin](capabilities/shared/dashboard-admin.yaml) -- 8 operations for organization and system administration
- [Tyk MDCB](capabilities/shared/mdcb.yaml) -- 4 operations for data plane monitoring and diagnostics

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [API Management](capabilities/api-management.yaml) | Gateway + Dashboard | 16 | API Developer / Platform Engineer |
| [Platform Administration](capabilities/platform-administration.yaml) | Dashboard Admin + MDCB | 12 | Platform Administrator |

## Vocabulary

- [Tyk Vocabulary](vocabulary/tyk-vocabulary.yaml)

## Rules

- [Tyk Spectral Rules](rules/tyk-spectral-rules.yml)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
