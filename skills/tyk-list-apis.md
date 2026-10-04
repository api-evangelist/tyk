---
name: tyk-list-apis
description: Retrieve a list of APIs and then fetch details for a selected API.
api: openapi/tyk-apis-api-openapi.yml
operations:
- getApis
- getApi
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/tyk-apis-api-openapi.yml ; every operationId checked against the contract
---

# tyk-list-apis

Retrieve a list of APIs and then fetch details for a selected API.

## Steps

1. 1. Call `getApis` – no required query parameters; include an authentication header (e.g., `Admin-Auth`, `X-Tyk-Authorization`, or Bearer token).
2. 2. Call `getApi` – path parameter `apiId` required; include the same authentication header.

## Rules

- Authentication: Provide one of the supported auth headers – `Admin-Auth`, `X-Tyk-Authorization`, or a Bearer token.
- Idempotency: GET operations are safe and idempotent.
