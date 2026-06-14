# Discogs GraphQL Schema

## Overview

This document describes a conceptual GraphQL schema for the Discogs API. Discogs is a community-built music database and marketplace for physical music releases (vinyl, CD, cassette, and more). The Discogs REST API provides programmatic read/write access to artists, releases, masters, labels, search, user collections and wantlists, marketplace listings, orders, and inventory management.

The schema below maps the Discogs REST API surface to a GraphQL type system, enabling strongly-typed, introspectable queries across the full Discogs data model.

## Schema Source

- **REST API Reference:** https://www.discogs.com/developers
- **Base URL:** https://api.discogs.com
- **Authentication:** Discogs Token, Key+Secret, or OAuth 1.0a
- **Community Python SDK:** https://github.com/joalla/discogs_client

## Core Domain Areas

### Database

The Discogs database covers the global catalog of physical music releases:

- **Releases** — Individual pressings with format, label, tracklist, images, identifiers, and community stats.
- **Masters** — Canonical groupings of release versions (e.g., all pressings of a given album).
- **Artists** — Musicians, bands, producers, and composers with roles, aliases, and member lists.
- **Labels** — Record labels with contact information, sublabels, and full release catalogs.
- **Search** — Free-text search across all entity types with rich filter parameters.

### User Surfaces

Authenticated user operations include:

- **Identity** — Profile, avatar, and account metadata.
- **Collection** — Vinyl/media collections organized into custom folders with per-copy notes and ratings.
- **Wantlist** — Tracked desired releases with notes and priority ratings.

### Marketplace

The Discogs Marketplace enables peer-to-peer buying and selling:

- **Inventory** — Seller listings for specific releases in defined media conditions.
- **Listings** — Individual sale items with condition grades, price, and seller notes.
- **Orders** — Purchase transactions between buyers and sellers.
- **Price Suggestions** — Discogs-calculated suggested prices by release and condition.

## Type Inventory

The schema defines 65 named types organized across these domains:

| Domain | Types |
|---|---|
| Release | Release, ReleaseDetails, ReleaseFormat, ReleaseLabel, ReleaseGenre, ReleaseStyle, ReleaseYear |
| Master | Master, MasterDetails, MasterVersions |
| Artist | Artist, ArtistDetails, ArtistImage, ArtistRole, ArtistAlias, ArtistMembers |
| Label | Label, LabelDetails, LabelImage, LabelContact, LabelSublabel |
| Track | Track, TrackDetails, TrackPosition, TrackArtist |
| Video | Video, VideoDetails |
| Format | Format, FormatType, FormatDescription |
| Genre/Style | Genre, GenreDetails, Style, StyleDetails |
| Image | Image, ImageDetails, ImageType |
| Identifier | Identifier, IdentifierType |
| Collection | Collection, CollectionFolder, CollectionItem |
| Wantlist | Wantlist, WantlistItem |
| Inventory | Inventory, InventoryItem |
| Listing | Listing, ListingDetails, ListingCondition |
| Order | Order, OrderDetails, OrderItem |
| Seller | Seller, SellerDetails |
| Community | Community, CommunityHave, CommunityWant |
| Rating | Rating |
| Auth | APIKey, Token |
| Pagination | PageInfo |
| Search | SearchResults |

## Root Operations

### Queries

```graphql
release(id: ID!): ReleaseDetails
master(id: ID!): MasterDetails
artist(id: ID!): ArtistDetails
label(id: ID!): LabelDetails
search(query: String!, type: String, filters: SearchFilters): SearchResults
collection(username: String!): Collection
wantlist(username: String!): Wantlist
inventory(username: String!): Inventory
listing(id: ID!): ListingDetails
order(id: ID!): OrderDetails
```

### Mutations

```graphql
addToCollection(username: String!, releaseId: ID!, folderId: ID): CollectionItem
removeFromCollection(username: String!, instanceId: ID!): Boolean
addToWantlist(username: String!, releaseId: ID!): WantlistItem
removeFromWantlist(username: String!, releaseId: ID!): Boolean
createListing(input: ListingInput!): Listing
updateListing(id: ID!, input: ListingInput!): Listing
deleteListing(id: ID!): Boolean
updateOrder(id: ID!, input: OrderInput!): Order
```

## Authentication

The Discogs API supports three authentication mechanisms:

1. **Discogs Token** — Single personal access token passed as a request header or query parameter. Suitable for read-heavy personal scripts.
2. **Key + Secret** — Application-level credentials that identify your app without user context.
3. **OAuth 1.0a** — Three-legged flow for third-party apps acting on behalf of other users.

## Rate Limits

Unauthenticated requests: 25 requests/minute. Authenticated requests: 60 requests/minute. Image requests require OAuth. See the rate limits document at `rate-limits/discogs-rate-limits.yml` for full details.

## Notes

This is a conceptual schema. Discogs does not operate a native GraphQL endpoint. This schema is intended to illustrate how the Discogs REST API surface maps to GraphQL conventions and to support tooling, documentation, and integration planning.
