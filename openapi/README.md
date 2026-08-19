# OpenAPI / FHIR specs

No machine-readable API contract was harvested for HealthVerity.

## Round 2 — contract discovery, 2026-08-15

A full STEP 0b contract-discovery pass was run against **every** resolving HealthVerity
host, not just the docs host. Nothing was found.

**Hosts resolved:** `healthverity.com`, `blog.healthverity.com`,
`marketplace.healthverity.com` (new this round), `info.healthverity.com`,
`symphonyhealth.com` / `www.symphonyhealth.com` (acquired 2026-05-08).

**Hosts that do not resolve (NXDOMAIN):** `api.healthverity.com`,
`docs.healthverity.com`, `developer.healthverity.com`, `developers.healthverity.com`,
`app.healthverity.com`, `portal.healthverity.com`, `platform.healthverity.com`,
`identity.healthverity.com`, `exos.healthverity.com`, `console.healthverity.com`,
`mcp.healthverity.com`, `status.healthverity.com`, `api.symphonyhealth.com`.

**Paths probed on every resolving host** — all 404 (or 403 for
`healthverity.com/openapi.yaml`, a WAF response, not a document):
`/openapi.json`, `/openapi.yaml`, `/swagger.json`, `/v1/openapi.json`,
`/api/openapi.json`, `/swagger/v1/swagger.json`, `/api-docs`, `/docs`, `/redoc`,
`/spec`, `/graphql`, `/llms.txt`, `/.well-known/agent-card.json`,
`/.well-known/agent.json`, `/.well-known/api-catalog`, `/.well-known/mcp.json`,
`/.well-known/oauth-authorization-server`, `/.well-known/oauth-protected-resource`,
`/.well-known/openid-configuration`.

**One false positive was rejected.** `symphonyhealth.com` returns **HTTP 200 with the
same WordPress homepage HTML for every path**, including `/openapi.json` and
`/.well-known/agent-card.json`. These are soft-404s. Nothing was saved from them.

**`marketplace.healthverity.com` is real but gated.** It is a genuine
HealthVerity-owned Django application (`<meta name="is_hv_env" content="True">`,
`/static/hv_favicon.png`) and it is the sign-in portal the eXOs page points existing
users at. Every request redirects to `/login/?next=...`, `/api`, `/api/v1`,
`/api/docs`, `/api/schema` and `/api/swagger.json` all return the app's 404 page, and
its `robots.txt` is `User-agent: * / Disallow: /`. There is a real application behind
that login; there is no public contract in front of it.

## What HealthVerity publishes

- **No public developer portal.**
- **No FHIR CapabilityStatement.** HealthVerity is a real-world-data /
  de-identification / tokenization platform, not a FHIR server or EHR/FHIR-network
  participant. No `/metadata`, no `/.well-known/smart-configuration`.
- **No downloadable OpenAPI/Swagger, GraphQL SDL, AsyncAPI or Postman collection.**
  (A `healthverity.com` Postman *team* exists with 0 collections and 0 workspaces —
  not a published surface.)
- **No client SDK.** The GitHub org has 9 repos, all infrastructure utilities or
  forks; none wraps a HealthVerity API. See `packages/`.

The only vendor-named programmatic surface is the gated, enterprise **HealthVerity
Identity API** (real-time de-identification), described conceptually on the Identity
Manager product page (https://healthverity.com/identity-manager/): *"Customers write
to the HealthVerity Identity API and records are processed in real time"*, activated by
*"a pre-configured java application or API"*. No reference documentation, base URL,
endpoints, or authentication scheme is published, and the Java application is not on
any public registry. Access is via commercial/partner agreement.

**HealthVerity eXOs** (announced 2025-09-30, "powered by Medeloop") is an agentic-AI
evidence platform — but an end-user one. Its published Terms of Use grant access
*"exclusively within the Platform"* and state *"Customer will not copy, extract, export
or download any Content from the Platform"*. That is the opposite of a programmatic
surface, and it is why no MCP or agent-card artifact exists here.

Nothing was fabricated. This directory will hold verbatim specs if HealthVerity
publishes them in the future.
