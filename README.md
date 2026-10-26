# UrbanPiper (urbanpiper)

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
