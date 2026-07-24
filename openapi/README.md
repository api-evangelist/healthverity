# OpenAPI / FHIR specs

No machine-readable API contract was harvested for HealthVerity.

As of the 2026-07-24 bootstrap review, HealthVerity publishes:

- **No public developer portal** (developer/docs/fhir/api subdomains do not resolve; `/developers`, `/api`, `/interoperability` return 404).
- **No FHIR CapabilityStatement** (HealthVerity is a real-world-data / de-identification / tokenization platform, not a FHIR server or EHR/FHIR-network participant). No `/metadata` or `/.well-known/smart-configuration` exists.
- **No downloadable OpenAPI/Swagger.**

The only vendor-named programmatic surface is the gated, enterprise **HealthVerity Identity API** (real-time de-identification), described conceptually on the Identity Manager product page (https://healthverity.com/identity-manager/) but with no reference documentation, base URL, endpoints, or authentication scheme published. Access is via commercial/partner agreement.

Nothing was fabricated. This directory will hold verbatim specs if HealthVerity publishes them in the future.
