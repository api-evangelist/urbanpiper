# UrbanPiper (urbanpiper)

UrbanPiper is a restaurant commerce platform whose POS-integration API connects a restaurant's POS/ERP to online ordering aggregators (Swiggy, Zomato, UberEats, DoorDash, Deliveroo, Talabat, Amazon, Careem and more). The REST API covers catalogue/menu management, store and item/option availability, order relay and order status updates, and outbound webhooks, powering the Prime, Hub and Atlas products.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/urbanpiper/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/urbanpiper/refs/heads/main/apis.yml)

## Tags

- Restaurants
- Food Delivery
- Ordering
- POS
- Aggregators
- Commerce

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### UrbanPiper Catalog & Menu API

Create and update the full restaurant catalogue (categories, items, option groups, options, taxes and charges) for a brand and push it to the connected aggregator platforms, with flush operations for resetting catalogue data per brand or store.

- **Human URL:** [https://api-docs.urbanpiper.com/downstream/](https://api-docs.urbanpiper.com/downstream/)
- **Base URL:** `https://pos-int.urbanpiper.com`

#### Tags

- Catalog
- Menu
- Categories
- Items
- Options

#### Properties

- [Documentation](https://api-docs.urbanpiper.com/downstream/)
- [API Reference](https://api-docs.urbanpiper.com/downstream/v/api-documentation/endpoints/menu/add-update-menu)
- [OpenAPI](openapi/urbanpiper-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/urbanpiper.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/urbanpiper.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### UrbanPiper Orders API

Receive aggregator orders relayed to the POS via webhook and push order status updates (Acknowledged, Food Ready, Dispatched, Completed, Cancelled) back to UrbanPiper, including self-delivery rider details and webhook retry.

- **Human URL:** [https://api-docs.urbanpiper.com/downstream/](https://api-docs.urbanpiper.com/downstream/)
- **Base URL:** `https://pos-int.urbanpiper.com`

#### Tags

- Orders
- Order Relay
- Order Status
- Webhooks

#### Properties

- [Documentation](https://api-docs.urbanpiper.com/downstream/)
- [API Reference](https://api-docs.urbanpiper.com/downstream/v/api-documentation/endpoints/order-management/order-status-update)
- [OpenAPI](openapi/urbanpiper-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/urbanpiper.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/urbanpiper.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### UrbanPiper Stores & Locations API

Create and update store/location records and map each location to a brand using the POS/ERP reference ID, so that menus and orders can be synced per location across aggregator platforms.

- **Human URL:** [https://api-docs.urbanpiper.com/downstream/](https://api-docs.urbanpiper.com/downstream/)
- **Base URL:** `https://pos-int.urbanpiper.com`

#### Tags

- Stores
- Locations
- Onboarding

#### Properties

- [Documentation](https://api-docs.urbanpiper.com/downstream/)
- [API Reference](https://api-docs.urbanpiper.com/downstream/v/api-documentation/endpoints/stores/store-toggle)
- [OpenAPI](openapi/urbanpiper-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/urbanpiper.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/urbanpiper.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### UrbanPiper Item Availability API

Toggle stores on and off and mark items and options in or out of stock in real time during operational hours, including marking items out-of-stock on an active order, with availability changes propagated to the aggregator platforms.

- **Human URL:** [https://api-docs.urbanpiper.com/downstream/](https://api-docs.urbanpiper.com/downstream/)
- **Base URL:** `https://pos-int.urbanpiper.com`

#### Tags

- Availability
- Stock Out
- Item Toggle
- Store Toggle

#### Properties

- [Documentation](https://api-docs.urbanpiper.com/downstream/)
- [API Reference](https://api-docs.urbanpiper.com/downstream/v/api-documentation/endpoints/menu/menu-toggle)
- [OpenAPI](openapi/urbanpiper-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/urbanpiper.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/urbanpiper.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### UrbanPiper Webhooks API

Register and manage webhook endpoints that UrbanPiper calls to relay orders, item-action callbacks and rider status updates to the POS, with an X-UPR-Biz-Id header identifying the brand and a webhook retry endpoint.

- **Human URL:** [https://api-docs.urbanpiper.com/downstream/](https://api-docs.urbanpiper.com/downstream/)
- **Base URL:** `https://pos-int.urbanpiper.com`

#### Tags

- Webhooks
- Callbacks
- Order Relay
- Rider Status

#### Properties

- [Documentation](https://api-docs.urbanpiper.com/downstream/)
- [API Reference](https://api-docs.urbanpiper.com/downstream/v/api-documentation/endpoints/getting-started/webhooks-callbacks)
- [OpenAPI](openapi/urbanpiper-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/urbanpiper.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/urbanpiper.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/urbanpiper)
- [LinkedIn](https://www.linkedin.com/company/urbanpiper)
- [Website](https://www.urbanpiper.com)
- [Documentation](https://api-docs.urbanpiper.com/downstream/)
- [Plans](plans/urbanpiper-plans-pricing.yml)
- [Rate Limits](rate-limits/urbanpiper-rate-limits.yml)
- [Fin Ops](finops/urbanpiper-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
