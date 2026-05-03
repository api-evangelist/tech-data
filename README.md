# Tech Data (TD SYNNEX)

Tech Data (now TD SYNNEX) is one of the world's largest IT distributors and solutions
aggregators, serving as an intermediary between technology vendors and resellers. The
company merged with SYNNEX in 2021 to form TD SYNNEX. TD SYNNEX exposes the StreamOne
Ion API platform for reseller partners to manage customers, products, orders, subscriptions,
and cloud services programmatically.

**Website:** https://www.tdsynnex.com  
**StreamOne Ion API Docs:** https://docs.streamone.cloud/  
**Digital Bridge Platform:** https://www.tdsynnex.com/na/us/digital-bridge/

## Tags

Cloud, Distribution, Information Technology, Partner

## Timestamps

- **Created:** 2026-03-24
- **Modified:** 2026-05-03

## APIs

### TD SYNNEX StreamOne Ion API

The StreamOne Ion API provides reseller partners with programmatic access to TD SYNNEX's
cloud distribution platform. Partners can manage end customers, browse product catalogs,
create and manage orders, handle subscriptions, configure cloud provider accounts, and
access billing reports. Supports multi-vendor cloud management across Microsoft, Google,
and AWS through a unified interface. Authentication uses OAuth 2.0.

**Base URL:** `https://ion.tdsynnex.com/api/v3`  
**Documentation:** https://docs.streamone.cloud/

**Endpoints:**
- Authentication: `POST /oauth/token`
- Customers: `GET/POST /v3/accounts/{accountId}/customers`
- Products: `GET /v3/accounts/{accountId}/products`
- Orders: `GET/POST/PUT/DELETE /v3/accounts/{accountId}/orders`
- Subscriptions: `GET /v3/accounts/{accountId}/customers/{customerId}/subscriptions`
- Carts: `GET/POST/PUT /v3/accounts/{accountId}/carts`
- Reports: `GET /v3/accounts/{accountId}/reports`

### TD SYNNEX Digital Bridge API

Digital Bridge is TD SYNNEX's integration platform providing enterprise-grade REST APIs
and pre-built connectors for products, pricing, orders, renewals, and cloud services.

**Documentation:** https://www.tdsynnex.com/na/us/digital-bridge/

## Artifacts

| Type | File |
|---|---|
| OpenAPI | [streamone-ion-openapi.yml](openapi/streamone-ion-openapi.yml) |
| Spectral Rules | [streamone-ion-rules.yml](rules/streamone-ion-rules.yml) |
| Capabilities (Shared) | [shared/streamone-ion.yaml](capabilities/shared/streamone-ion.yaml) |
| Workflow Capability | [cloud-distribution.yaml](capabilities/cloud-distribution.yaml) |
| JSON Schema (Customer) | [streamone-ion-customer-schema.json](json-schema/streamone-ion-customer-schema.json) |
| JSON Schema (Order) | [streamone-ion-order-schema.json](json-schema/streamone-ion-order-schema.json) |
| JSON Schema (Subscription) | [streamone-ion-subscription-schema.json](json-schema/streamone-ion-subscription-schema.json) |
| JSON Structure (Customer) | [streamone-ion-customer-structure.json](json-structure/streamone-ion-customer-structure.json) |
| JSON Structure (Order) | [streamone-ion-order-structure.json](json-structure/streamone-ion-order-structure.json) |
| JSON-LD Context | [tech-data-context.jsonld](json-ld/tech-data-context.jsonld) |
| Examples | [streamone-ion-list-customers-example.json](examples/streamone-ion-list-customers-example.json) |
| Examples | [streamone-ion-create-order-example.json](examples/streamone-ion-create-order-example.json) |
| Vocabulary | [tech-data-vocabulary.yml](vocabulary/tech-data-vocabulary.yml) |

## Capabilities

### Workflow Capabilities

- **[Cloud Distribution](capabilities/cloud-distribution.yaml)** - Unified REST + MCP capability for partner customer management, product catalog browsing, order processing, subscription management, and billing reports (15 tools).

### Shared Per-API Definitions

- **[StreamOne Ion](capabilities/shared/streamone-ion.yaml)** - Complete consumed definition for the StreamOne Ion API.

## Common Properties

- [Website](https://www.tdsynnex.com)
- [Login](https://ion.tdsynnex.com/)
- [LinkedIn](https://www.linkedin.com/company/td-synnex/)
- [Terms of Service](https://www.tdsynnex.com/na/us/legal/terms-of-use/)
- [Privacy Policy](https://www.tdsynnex.com/na/us/legal/privacy-notice/)

## Maintainers

- Kin Lane (kin@apievangelist.com)
