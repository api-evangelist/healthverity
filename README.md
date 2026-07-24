# HealthVerity (healthverity)

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
