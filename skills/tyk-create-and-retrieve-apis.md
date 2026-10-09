---
name: tyk-create-and-retrieve-apis
description: Create a new OAS API, retrieve its definition, and download it in OAS format.
api: openapi/tyk-tyk-oas-apis-api-openapi.yml
operations:
- createApiOAS
- getOASApi
- downloadApiOASPublic
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/tyk-tyk-oas-apis-api-openapi.yml ; every operationId checked against the contract
---

# tyk-create-and-retrieve-apis

Create a new OAS API, retrieve its definition, and download it in OAS format.

## Steps

1. 1. Use `createApiOAS` with the request body containing the OAS API definition.
2. 2. Use `getOASApi` with the path parameter `apiID` returned from the create step to fetch the API definition.
3. 3. Use `downloadApiOASPublic` with the same `apiID` to download the API in OAS format.

## Rules

- Auth: Include either the `Admin-Auth` header (ApiKeyAuth) or the `X-Tyk-Authorization` header (api_key) with a valid API key.
- Idempotency: The `createApiOAS` operation is not idempotent; repeated calls will create duplicate APIs.
- Errors: On failure, the API returns standard HTTP error codes (e.g., 4xx for client errors, 5xx for server errors).
