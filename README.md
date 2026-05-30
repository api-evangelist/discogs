# Discogs (discogs)

Discogs is a community-built music database and marketplace for physical music releases (vinyl, CD, cassette, and more). The Discogs API gives developers programmatic
read/write access to artists, releases, masters, labels, search, user collections and wantlists, marketplace listings, orders, and inventory management — using Discogs
Auth tokens, key+secret credentials, or full OAuth 1.0a on behalf of other users.

**URL:** [Visit APIs.json URL](https://www.discogs.com/developers/)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Music
 - Marketplace
 - Catalog
 - Community
 - Vinyl
 - Public APIs

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-29

## APIs

### Discogs API

RESTful API to the Discogs music catalog and marketplace. Covers the Database (artist, release, master, label, search), authenticated User surfaces
(identity, profile, collection, wantlist, lists, contributions, submissions, ratings), Marketplace (inventory, orders, listings, fees, price suggestions,
release stats), bulk Inventory Management (CSV export/upload), and OAuth-signed Image retrieval.

**Human URL:** [https://www.discogs.com/developers](https://www.discogs.com/developers)

**Base URL:** `https://api.discogs.com`

#### Tags:

 - Database
 - Marketplace
 - User Identity
 - User Collection
 - User Wantlist
 - User Lists
 - Inventory Management
 - Image

#### Properties

- [Documentation](https://www.discogs.com/developers)
- [APIReference](https://www.discogs.com/developers)
- [Authentication](https://www.discogs.com/developers#page:authentication)
- [TermsOfService](https://support.discogs.com/hc/articles/360009334593-API-Terms-of-Use)
- [OpenAPI](openapi/discogs-openapi-original.yml)
- [Python SDK (Joalla Community Continuation)](https://github.com/joalla/discogs_client)
- [Python SDK (Modern Reimplementation)](https://github.com/jmfontaine/discogs-sdk)
- [Java SDK (Community)](https://github.com/andy-miles/discogs-java-client)
- [Swift Service (Community)](https://github.com/rock-n-code/discogs-service)
- [PHP SDK (Discogs Client - Deprecated Official)](https://github.com/discogs/discogs_client)
- [Monthly XML Data Dumps](https://discogs-data-dumps.s3.us-west-2.amazonaws.com/index.html)
- [NaftikoCapability](capabilities/discogs-database.yaml)
- [NaftikoCapability](capabilities/discogs-image.yaml)
- [NaftikoCapability](capabilities/discogs-inventory-management.yaml)
- [NaftikoCapability](capabilities/discogs-marketplace.yaml)
- [NaftikoCapability](capabilities/discogs-user-collection.yaml)
- [NaftikoCapability](capabilities/discogs-user-identity.yaml)
- [NaftikoCapability](capabilities/discogs-user-lists.yaml)
- [NaftikoCapability](capabilities/discogs-user-wantlist.yaml)

## Common Properties

- [Website](https://www.discogs.com)
- [Documentation](https://www.discogs.com/developers)
- [APIReference](https://www.discogs.com/developers)
- [TermsOfService](https://support.discogs.com/hc/articles/360009334593-API-Terms-of-Use)
- [Authentication](https://www.discogs.com/developers#page:authentication)
- [Support](https://support.discogs.com)
- [Forum](https://www.discogs.com/forum/topic/1082)
- [Status](https://status.discogs.com)
- [Blog](https://blog.discogs.com)
- [Plans](plans/discogs-plans-pricing.yml)
- [RateLimits](rate-limits/discogs-rate-limits.yml)
- [GitHubOrganization](https://github.com/discogs)
- [PublicAPIsListing](https://github.com/public-apis/public-apis)
- [Monthly XML Data Dumps](https://discogs-data-dumps.s3.us-west-2.amazonaws.com/index.html)
- [MCP Server (cswkim)](https://github.com/cswkim/discogs-mcp-server)
- [MCP Server (rianvdm OAuth)](https://github.com/rianvdm/discogs-mcp)
- [MCP Server (pipeworx-io)](https://github.com/pipeworx-io/mcp-discogs)
- [MCP Server (andylobban Self-hostable)](https://github.com/andylobban/discogs-mcp-server)
- [MCP Server (leosakharoff)](https://github.com/leosakharoff/discogs-mcp)
- [Vocabulary](vocabulary/discogs-vocabulary.yml)
- [SpectralRuleset](rules/discogs-rules.yml)
- [JSONLDContext](json-ld/discogs-context.jsonld)

## Features

| Name | Description |
|------|------|
| Database Search | Free-text search across releases, masters, artists, and labels with rich filters (year, country, format, label, genre, style, barcode, catno). |
| Release Catalog | Detailed release records including tracks, formats, labels, artists, videos, identifiers, community stats, and marketplace stats. |
| User Collection Management | Read and modify user record collections, organized into custom folders with notes and rating per copy. |
| User Wantlist | Track wanted releases, with notes and ratings; add and remove releases programmatically. |
| Marketplace Listings | List, update, and delete records for sale; query inventory by username; integrate with checkout flows via the Listing endpoints. |
| Marketplace Orders | Inspect, update, and message on orders the authenticated seller has received. |
| Price Suggestions | Get Discogs-calculated suggested marketplace prices by release and media condition. |
| Bulk Inventory Management | CSV-driven bulk add, change, and delete of inventory listings via asynchronous upload jobs; full inventory export to CSV. |
| OAuth 1.0a | Three-legged OAuth 1.0a flow for building third-party apps that act on behalf of other Discogs users. |
| Monthly XML Data Dumps | Discogs publishes a monthly snapshot of the full database (artists, labels, masters, releases) as XML on S3 for bulk analysis. |

## Use Cases

| Name | Description |
|------|------|
| Music Discovery Apps | Build apps that surface release metadata, cover art, video links, community ratings, and label discographies. |
| Vinyl Reseller Tools | Power inventory management, pricing, and order workflows for vinyl resellers selling on the Discogs Marketplace. |
| Collection Trackers | Mobile and desktop apps that sync a collector's Discogs collection and wantlist offline. |
| Catalog Enrichment | Enrich third-party music libraries (DJ tools, archive systems, streaming metadata) with Discogs identifiers, formats, and release dates. |
| AI Music Agents | Power LLM-driven shopping, discovery, and collection-management agents via the Discogs MCP server ecosystem. |
| Research and Analytics | Use the monthly XML data dumps for population-level analysis of pressing variants, label catalogs, and marketplace pricing. |

## Integrations

| Name | Description |
|------|------|
| OAuth 1.0a | Standards-compliant OAuth 1.0a for delegated user authorization. |
| CSV | Bulk inventory imports and exports use CSV files. |
| Microcks | OpenAPI spec is annotated with x-microcks-operation extensions for mock-server compatibility. |
| Model Context Protocol | Five plus community MCP servers expose Discogs surfaces (search, collection, wantlist, marketplace) as MCP tools for LLM agents. |

## Solutions

| Name | Description |
|------|------|
| Marketplace Storefront Sync | Combine inventory upload, order management, and price suggestions to operate a multi-channel record store with Discogs as inventory of record. |
| Collector Mobile Companion | Combine identity, collection, wantlist, and search to build a fully-featured mobile companion for record collectors. |
| Catalog Resolution Service | Use search and release endpoints to resolve fuzzy track metadata into canonical Discogs IDs and master release versions. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [discogs-openapi-original.yml](openapi/discogs-openapi-original.yml)

### JSON Schema (55 files)

See [json-schema/](json-schema/) — 55 schema files extracted from the OpenAPI components.

### JSON Structure (55 files)

See [json-structure/](json-structure/) — 55 JSON Structure files (json-structure.org meta).

### JSON-LD Contexts

- [discogs-context.jsonld](json-ld/discogs-context.jsonld)

### Examples (55 files)

See [examples/](examples/) — 55 representative example payloads.

## Capabilities

Self-contained Naftiko capability files (one per OpenAPI tag) with inline REST and MCP adapters.

| Capability | Consumed Operations | MCP Tools | File |
|------------|---------------------|-----------|------|
| Discogs API — Database | 12 | 12 | [discogs-database.yaml](capabilities/discogs-database.yaml) |
| Discogs API — Image | 1 | 1 | [discogs-image.yaml](capabilities/discogs-image.yaml) |
| Discogs API — Inventory Management | 9 | 9 | [discogs-inventory-management.yaml](capabilities/discogs-inventory-management.yaml) |
| Discogs API — Marketplace | 14 | 14 | [discogs-marketplace.yaml](capabilities/discogs-marketplace.yaml) |
| Discogs API — User Collection | 4 | 4 | [discogs-user-collection.yaml](capabilities/discogs-user-collection.yaml) |
| Discogs API — User Identity | 5 | 5 | [discogs-user-identity.yaml](capabilities/discogs-user-identity.yaml) |
| Discogs API — User Lists | 2 | 2 | [discogs-user-lists.yaml](capabilities/discogs-user-lists.yaml) |
| Discogs API — User Wantlist | 3 | 3 | [discogs-user-wantlist.yaml](capabilities/discogs-user-wantlist.yaml) |

## Vocabulary

- [discogs-vocabulary.yml](vocabulary/discogs-vocabulary.yml) — Unified taxonomy mapping operational (OpenAPI) and capability (Naftiko) dimensions.

## Rules

- [discogs-rules.yml](rules/discogs-rules.yml) — 35 Spectral rules enforcing Discogs API conventions.

## Plans & Pricing

- [discogs-plans-pricing.yml](plans/discogs-plans-pricing.yml)

## Rate Limits

- [discogs-rate-limits.yml](rate-limits/discogs-rate-limits.yml)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
