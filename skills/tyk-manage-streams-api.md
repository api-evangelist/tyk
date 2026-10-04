---
name: tyk-manage-streams-api
description: Create, view, modify, and delete a Streams API.
api: openapi/tyk-streams-apis-api-openapi.yml
operations:
- createStreamsApi
- getStreamsAPIDetails
- updateStreamsApi
- patchApiStreams
- deleteStreamsApi
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/tyk-streams-apis-api-openapi.yml ; every operationId checked against the contract
---

# tyk-manage-streams-api

Create, view, modify, and delete a Streams API.

## Steps

1. 1. `createStreamsApi` – fields: [], headers: []
2. 2. `getStreamsAPIDetails` – fields: [], headers: []
3. 3. `updateStreamsApi` – fields: [], headers: []
4. 4. `patchApiStreams` – fields: [], headers: []
5. 5. `deleteStreamsApi` – fields: [], headers: []

## Rules

- Include an authentication header: either Admin-Auth (ApiKeyAuth), X-Tyk-Authorization (api_key), or a Bearer token (bearerAuth).
- No rate limit is defined; exhaustion returns no specific HTTP status.
