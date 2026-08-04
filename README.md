# HealthVerity (healthverity)

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

HealthVerity is a United States life-sciences data platform (Philadelphia, PA) operating what it calls the nation's largest real-world data (RWD) ecosystem: 150 billion-plus de-identified transactions across 330 million-plus U.S. patients from 75-plus data sources (medical and pharmacy claims, labs, and EHR, following its integration of Symphony Health). Its products sit on the IPGE framework - Identity, Privacy, Governance, Exchange - and include HealthVerity Marketplace, Identity Manager and Census (privacy-safe identity resolution to a universal HealthVerity ID / HVID), Governance Manager, HealthVerity FLOW, and eXOs (an AI-native real-world-evidence agent).

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/healthverity/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/healthverity/refs/heads/main/apis.yml)

## API Posture

HealthVerity is a RWD / tokenization / de-identification company, not a standards-based clinical interoperability vendor. As of this review it publishes **no public developer portal, no FHIR CapabilityStatement, and no downloadable OpenAPI**. The only vendor-named programmatic surface is the gated, enterprise **HealthVerity Identity API** for real-time de-identification, described conceptually on the Identity Manager product page but without public reference documentation, base URL, or self-serve onboarding. All products are accessed under commercial/partner agreements (request a demo, contact sales).

## Tags

- Healthcare
- United States
- Life Sciences
- Real-World Data
- Identity Resolution
- De-Identification
- Tokenization
- Data Marketplace
- HIPAA
- Claims

## Timestamps

- **Created:** 2026-07-24
- **Modified:** 2026-07-24

## APIs

### HealthVerity Identity API

Gated, enterprise real-time de-identification API named on the HealthVerity Identity Manager product page. Under the "sync on demand" modality, customers write records to the HealthVerity Identity API and records are processed in real time, replacing PII with a universal HealthVerity ID (HVID) while all PII remains with the data owner. No public reference documentation, base URL, or authentication details are published.

- **Human URL:** [https://healthverity.com/identity-manager/](https://healthverity.com/identity-manager/)

#### Properties

- [Documentation](https://healthverity.com/identity-manager/)

## Common Properties

- [Website](https://healthverity.com/)
- [Blog](https://blog.healthverity.com/)
- [GitHub Organization](https://github.com/healthverity)
- [LinkedIn](https://www.linkedin.com/company/healthverity)
- [Support](https://healthverity.com/contact/)
- [Privacy Policy](https://healthverity.com/privacy-policy/)
- [Terms of Service](https://healthverity.com/terms-and-conditions/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
