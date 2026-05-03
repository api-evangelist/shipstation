# ShipStation (shipstation)

ShipStation is a leading shipping platform for ecommerce businesses providing APIs to integrate shipping workflows into applications. The ShipStation API enables developers to automate order management, create shipments, generate labels, track packages, manage warehouses, and connect to multiple carriers.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/shipstation/refs/heads/main/apis.yml)

## Scope

- **Type:** Contract
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

- Ecommerce, Labels, Logistics, Order Management, Shipping, Warehousing

## Timestamps

- **Created:** 2025-03-01
- **Modified:** 2026-05-02

## APIs

### ShipStation V1 API

The ShipStation V1 API provides programmatic access to ShipStation's shipping platform for ecommerce businesses. Endpoints cover order management, shipment creation, label generation, carrier rate shopping, package tracking, warehouse management, product management, and store integrations. Authentication uses HTTP Basic auth with API key and secret. Base URL is https://ssapi.shipstation.com with a rate limit of 40 requests per minute.

**Human URL:** [https://www.shipstation.com/docs/api/](https://www.shipstation.com/docs/api/)

#### Tags

- Ecommerce, Labels, Order Management, Shipping

#### Properties

- [Documentation](https://www.shipstation.com/docs/api/)
- [OpenAPI](openapi/shipstation-v1-openapi.yml)
- [JSONSchema](json-schema/shipstation-order-schema.json)
- [JSONSchema](json-schema/shipstation-shipment-schema.json)
- [JSONLD](json-ld/shipstation-context.jsonld)
- [SpectralRules](rules/shipstation-rules.yml)
- [NaftikoCapabilities](capabilities/ecommerce-shipping.yaml)
- [Vocabulary](vocabulary/shipstation-vocabulary.yml)

### ShipStation V2 API

The ShipStation V2 API is the next-generation shipping and inventory API built on ShipEngine technology. It provides improved endpoints for creating orders, managing customers, querying order and shipping data, and integrating with ShipStation's multi-carrier shipping platform.

**Human URL:** [https://docs.shipstation.com/](https://docs.shipstation.com/)

#### Tags

- Ecommerce, Labels, Order Management, Shipping

#### Properties

- [Documentation](https://docs.shipstation.com/)
- [API Reference](https://docs.shipstation.com/rest)

## Capabilities

### Shared Definitions

| File | Description |
|---|---|
| [capabilities/shared/shipstation.yaml](capabilities/shared/shipstation.yaml) | ShipStation V1 API — orders, shipments, labels, carriers, warehouses, stores |

### Workflow Capabilities

| Capability | Description | Tools |
|---|---|---|
| [ecommerce-shipping.yaml](capabilities/ecommerce-shipping.yaml) | Ecommerce order fulfillment across multiple channels with multi-carrier shipping | 13 tools |

## Artifacts

| Type | File |
|---|---|
| OpenAPI | [openapi/shipstation-v1-openapi.yml](openapi/shipstation-v1-openapi.yml) |
| JSON Schema | [json-schema/shipstation-order-schema.json](json-schema/shipstation-order-schema.json) |
| JSON Schema | [json-schema/shipstation-shipment-schema.json](json-schema/shipstation-shipment-schema.json) |
| JSON Structure | [json-structure/shipstation-order-structure.json](json-structure/shipstation-order-structure.json) |
| JSON-LD | [json-ld/shipstation-context.jsonld](json-ld/shipstation-context.jsonld) |
| Examples | [examples/shipstation-create-order-example.json](examples/shipstation-create-order-example.json) |
| Examples | [examples/shipstation-create-label-example.json](examples/shipstation-create-label-example.json) |
| Spectral Rules | [rules/shipstation-rules.yml](rules/shipstation-rules.yml) |
| Vocabulary | [vocabulary/shipstation-vocabulary.yml](vocabulary/shipstation-vocabulary.yml) |

## Common Properties

- [Documentation](https://www.shipstation.com/docs/api/)
- [API Reference](https://docs.shipstation.com/)
- [Getting Started](https://docs.shipstation.com/getting-started)
- [Authentication](https://www.shipstation.com/docs/api/requirements/)
- [OpenAPI Downloads](https://docs.shipstation.com/openapi/downloads)
- [Support](https://help.shipstation.com/hc/en-us/articles/360025856212-ShipStation-API)
- [Terms of Service](https://www.shipstation.com/legal/terms-of-service/)
- [Privacy Policy](https://www.shipstation.com/legal/privacy-policy/)
- [Website](https://www.shipstation.com)

## Maintainers

**FN:** Kin Lane  
**Email:** kin@apievangelist.com
