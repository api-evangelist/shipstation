# ShipStation GraphQL Schema

## Overview

This document describes a conceptual GraphQL schema for the ShipStation multi-carrier shipping platform. ShipStation exposes a REST API (V1 at `ssapi.shipstation.com` and V2 at `docs.shipstation.com`), and this schema represents those capabilities in GraphQL terms to support tooling, documentation, and integration design.

The schema covers order management, shipment creation, label generation, carrier rate shopping, warehouse management, product management, return handling, and store integrations.

## Authentication

ShipStation V1 uses HTTP Basic authentication with an API key and API secret. V2 uses bearer token authentication. A GraphQL gateway would need to forward credentials via request headers.

## Core Domain Areas

### Orders

Orders represent ecommerce transactions imported from connected stores or created via API. Each order carries line items, addresses, payment details, and shipping preferences. Orders progress through statuses such as `awaiting_payment`, `awaiting_shipment`, `shipped`, `cancelled`, and `on_hold`.

Types: `Order`, `OrderDetail`, `OrderStatus`, `OrderTag`, `OrderItem`, `ItemDetail`, `ItemSKU`, `ItemWeight`, `ItemDimension`, `OrderAddress`, `ShipTo`, `BillTo`, `CustomField`, `PaymentMethod`, `PaymentAmount`, `ConfirmationType`

### Shipments and Labels

Shipments are created from orders and represent the physical dispatch of goods. Labels are generated per shipment and encode carrier-specific tracking and barcode data.

Types: `Shipment`, `ShipmentDetail`, `ShipmentStatus`, `ShipmentTag`, `Label`, `LabelData`, `ShipmentItems`, `ShipmentWeight`, `ShipmentDimension`

### Carriers and Rates

ShipStation connects to multiple carriers (USPS, UPS, FedEx, DHL, Canada Post, etc.) and provides rate shopping across services. Each carrier exposes available services and package codes.

Types: `Carrier`, `CarrierService`, `CarrierShipment`, `CarrierCode`, `Rate`, `RateDetail`, `ServiceCode`, `PackageCode`

### International Shipping

International shipments require customs declarations including contents type, non-delivery instructions, and insurance options.

Types: `InternationalOptions`, `ContentsType`, `NonDeliveryOption`, `InsuranceOptions`, `InsuredValue`

### Advanced Options and Gifts

Orders and shipments may carry advanced routing options, gift messaging, and merchant reference data.

Types: `AdvancedOptions`, `StoreID`, `SourceStore`, `MerchantRef`, `GiftOptions`, `Gift`, `GiftMessage`

### Fulfillment and Warehouses

Fulfillment centers and warehouses define where inventory is held and from where shipments originate. Warehouse origin addresses appear on labels.

Types: `Fulfillment`, `FulfillmentCenter`, `Warehouse`, `WarehouseDetails`, `WarehouseOrigin`

### Returns

Returns represent reverse logistics flows where customers send goods back. Return approvals and statuses are tracked separately.

Types: `Return`, `ReturnApproval`, `ReturnStatus`

### Users, Stores, and Accounts

ShipStation accounts contain users with role-based permissions and connected stores from ecommerce platforms (Shopify, WooCommerce, Amazon, eBay, Etsy, etc.).

Types: `User`, `UserDetails`, `Store`, `StoreDetails`, `Account`, `APIKey`, `Token`, `Webhook`

## Query Surface

The schema exposes queries for listing and fetching individual resources:

- `orders` — paginated list with filters for status, store, date range, tag
- `order(orderId)` — single order by ID
- `shipments` — paginated list with filters
- `shipment(shipmentId)` — single shipment
- `carriers` — list of connected carriers
- `rates(input)` — rate shop across carriers for a given package and addresses
- `warehouses` — list of warehouses
- `stores` — list of connected stores
- `returns` — list of returns

## Mutation Surface

- `createOrder` — create a new order
- `updateOrder` — update order fields
- `deleteOrder` — delete a draft order
- `createShipment` — create shipment and generate label
- `voidLabel` — void an existing label
- `createReturn` — initiate a return
- `addTag` / `removeTag` — manage order tags
- `holdOrder` / `releaseOrder` — manage order hold status
- `createWebhook` / `deleteWebhook` — manage event subscriptions

## Schema File

See `shipstation-schema.graphql` in this directory for the full type definitions.

## References

- ShipStation V1 API Docs: https://www.shipstation.com/docs/api/
- ShipStation V2 API Docs: https://docs.shipstation.com/
- GitHub Organization: https://github.com/shipstation
