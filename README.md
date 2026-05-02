# Revert

Revert is an open-source unified API platform that makes it easy to build product integrations 10x faster. It provides a single standardized API to integrate with CRMs, ticketing systems, chat platforms, and accounting software, with built-in OAuth management, token refresh, and retry logic.

**Website:** https://www.revert.dev/  
**GitHub:** https://github.com/revertinc/revert  
**Documentation:** https://docs.revert.dev  
**Type:** company  
**License:** AGPL-3.0

## APIs

### Revert Unified API

Single API surface normalizing operations across multiple third-party platforms:

- **CRM:** Salesforce, HubSpot, Zoho CRM, Pipedrive, Close CRM
- **Ticketing:** Jira, Asana
- **Chat:** Slack, Microsoft Teams, Discord
- **Accounting:** Xero, QuickBooks

**Base URL:** https://api.revert.dev  
**Authentication:** API Key (`x-revert-api-token` header) + Tenant ID (`x-revert-t-id` header)

## Artifacts

### OpenAPI Specs

| File | Description |
|------|-------------|
| [revert-unified-api-openapi.yml](openapi/revert-unified-api-openapi.yml) | Full Revert Unified API including CRM, Tickets, Chat, and Accounting endpoints |

### Rules

| File | Description |
|------|-------------|
| [revert-rules.yml](rules/revert-rules.yml) | Spectral ruleset enforcing Revert API conventions |

### Capabilities

| File | Description |
|------|-------------|
| [crm-integration.yaml](capabilities/crm-integration.yaml) | Unified CRM workflow: contacts, companies, deals, leads |
| [shared/revert-unified-api.yaml](capabilities/shared/revert-unified-api.yaml) | Shared per-API capability definition |

### JSON Schema

| File | Description |
|------|-------------|
| [revert-contact-schema.json](json-schema/revert-contact-schema.json) | Normalized CRM Contact entity schema |
| [revert-deal-schema.json](json-schema/revert-deal-schema.json) | Normalized CRM Deal/Opportunity entity schema |

### JSON Structure

| File | Description |
|------|-------------|
| [revert-contact-structure.json](json-structure/revert-contact-structure.json) | Contact entity field documentation |

### JSON-LD

| File | Description |
|------|-------------|
| [revert-context.jsonld](json-ld/revert-context.jsonld) | JSON-LD context mapping Revert vocabulary to schema.org |

### Examples

| File | Description |
|------|-------------|
| [revert-get-contacts-example.json](examples/revert-get-contacts-example.json) | List CRM contacts request/response example |
| [revert-create-deal-example.json](examples/revert-create-deal-example.json) | Create CRM deal request/response example |

### Vocabulary

| File | Description |
|------|-------------|
| [revert-vocabulary.yml](vocabulary/revert-vocabulary.yml) | Domain vocabulary for Revert integration platform concepts |

## Key Features

- **Unified CRM API** — One interface for Salesforce, HubSpot, Zoho, Pipedrive, and Close
- **OAuth Management** — Automatic token lifecycle with refresh and failure handling
- **Self-Hosting** — Full Docker Compose deployment for data sovereignty
- **Drop-in UI SDKs** — React, Vue, and JavaScript components for OAuth connection flows
- **Field Mapping** — Provider-native fields normalized plus raw `additional` fields preserved

## Maintainers

- Kin Lane — kin@apievangelist.com
