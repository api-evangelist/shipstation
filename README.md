# ShipStation (shipstation)

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

ShipStation is a leading shipping platform for ecommerce businesses providing APIs to integrate shipping workflows into applications. The ShipStation API enables developers to automate order management, create shipments, generate labels, track packages, manage warehouses, and connect to multiple carriers. ShipStation offers both V1 (ssapi.shipstation.com) and V2 (ShipEngine-powered) API versions.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/shipstation/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/shipstation/refs/heads/main/apis.yml)

## Scope

- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

- Ecommerce
- Labels
- Logistics
- Order Management
- Shipping
- Warehousing

## Timestamps

- **Created:** 2025-03-01
- **Modified:** 2026-05-30

## APIs

### ShipStation V1 API

The ShipStation V1 API provides programmatic access to ShipStation's shipping platform for ecommerce businesses. Endpoints cover order management, shipment creation, label generation, carrier rate shopping, package tracking, warehouse management, product management, and store integrations. Authentication uses HTTP Basic auth with API key and secret. Base URL is https://ssapi.shipstation.com with a rate limit of 40 requests per minute.

- **Human URL:** [https://www.shipstation.com/docs/api/](https://www.shipstation.com/docs/api/)

#### Tags

- Ecommerce
- Labels
- Order Management
- Shipping

#### Properties

- [Documentation](https://www.shipstation.com/docs/api/)
- [OpenAPI](openapi/shipstation-v1-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/shipstation-v1.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/shipstation-v1.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/shipstation-webhooks-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [JSON Schema](json-schema/shipstation-order-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/shipstation-shipment-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/shipstation-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Spectral Rules](rules/shipstation-rules.yml)
- [Vocabulary](vocabulary/shipstation-vocabulary.yml)

### ShipStation V2 API

The ShipStation V2 API is the next-generation shipping and inventory API built on ShipEngine technology. It provides improved endpoints for creating orders, managing customers, querying order and shipping data, and integrating with ShipStation's multi-carrier shipping platform. Available to Standard plan and higher accounts with the API add-on.

- **Human URL:** [https://docs.shipstation.com/](https://docs.shipstation.com/)

#### Tags

- Ecommerce
- Labels
- Order Management
- Shipping

#### Properties

- [Documentation](https://docs.shipstation.com/)
- [API Reference](https://docs.shipstation.com/rest)
- [Postman Collection](collections/shipstation-v1.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/shipstation-v1.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/shipstation)
- [LinkedIn](https://www.linkedin.com/company/shipstation)
- [Documentation](https://www.shipstation.com/docs/api/)
- [API Reference](https://docs.shipstation.com/)
- [Getting Started](https://docs.shipstation.com/getting-started)
- [Authentication](https://www.shipstation.com/docs/api/requirements/)
- [OpenAPI](https://docs.shipstation.com/openapi/downloads) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Support](https://help.shipstation.com/hc/en-us/articles/360025856212-ShipStation-API)
- [Terms of Service](https://www.shipstation.com/legal/terms-of-service/)
- [Privacy Policy](https://www.shipstation.com/legal/privacy-policy/)
- [Website](https://www.shipstation.com)
- [Features](undefined)
- [Integrations](https://www.shipstation.com/partners/)
- [L L Ms Txt](https://docs.shipstation.com/llms.txt)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
