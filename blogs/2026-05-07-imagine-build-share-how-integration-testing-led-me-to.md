---
title: "Imagine, build, share – how integration testing led me to create the Tyk mock MCP server"
url: "https://tyk.io/blog/imagine-build-share-how-integration-testing-led-me-to-create-the-tyk-mock-mcp-server/"
date: "2026-05-07"
author: "Laurentiu Ghiur"
feed_url: "https://tyk.io/feed/"
---
If you had to sum up the Tyk approach in three sentences, the above would be spot on. Working at Tyk means being encouraged to create and collaborate, and the pace of AI evolution right now means there are plenty of opportunities to do so. This is how the Tyk MCP mock server and mock client were born… I needed a mock server for integration testing. When you’re building an API gateway that proxies MCP traffic, you need to test the full round-trip: client → gateway → upstream server.
