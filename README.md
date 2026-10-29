# Discogs

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

Discogs is a community-built music database and marketplace for physical music releases (vinyl, CD, cassette, and more). The Discogs API gives developers programmatic read/write access to artists, releases, masters, labels, search, user collections and wantlists, marketplace listings, orders, and inventory management — using Discogs Auth tokens, key+secret credentials, or full OAuth 1.0a on behalf of other users.

**Areas:** Music · Marketplace · Catalog · Community · Vinyl · Public APIs

## Discogs on APIs.io

Everything profiled for Discogs is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/discogs/](https://apis.io/providers/discogs/)** — or go straight to one of the APIs or properties below.

### APIs (8)

- [Discogs Database API](https://apis.io/apis/discogs/discogs-database-api/) — Access Discogs database: artists, releases, masters, labels, and search.
- [Discogs Image API](https://apis.io/apis/discogs/discogs-image-api/) — Image asset retrieval (proxied via OAuth).
- [Discogs Inventory Management API](https://apis.io/apis/discogs/discogs-inventory-management-api/) — Bulk inventory export and CSV upload management.
- [Discogs Marketplace API](https://apis.io/apis/discogs/discogs-marketplace-api/) — Marketplace listings, orders, fees, price suggestions, and release stats.
- [Discogs User Collection API](https://apis.io/apis/discogs/discogs-user-collection-api/) — Manage a user's record collection.
- [Discogs User Identity API](https://apis.io/apis/discogs/discogs-user-identity-api/) — Authenticated user identity, profile, submissions, and contributions.
- [Discogs User Lists API](https://apis.io/apis/discogs/discogs-user-lists-api/) — Browse and manage user-created lists of releases, artists, and labels.
- [Discogs User Wantlist API](https://apis.io/apis/discogs/discogs-user-wantlist-api/) — Manage a user's wantlist.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### GraphQL (1)

GraphQL schemas.

- [Moved to /providers/discogs/](https://apis.io/graphqls/discogs/discogs-graphql/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Discogs Agentic Access](https://apis.io/agentic-access/discogs/discogs-agentic-access/)

#### JSON Schema (55)

The data models the API reads and writes.

- [Artist](https://apis.io/schemas/discogs/discogs-artist/)
- [ArtistRelease](https://apis.io/schemas/discogs/discogs-artist-release/)
- [ArtistSummary](https://apis.io/schemas/discogs/discogs-artist-summary/)
- [CollectionFolder](https://apis.io/schemas/discogs/discogs-collection-folder/)
- [CollectionRelease](https://apis.io/schemas/discogs/discogs-collection-release/)
- [Community](https://apis.io/schemas/discogs/discogs-community/)
- [Contribution](https://apis.io/schemas/discogs/discogs-contribution/)
- [Currency](https://apis.io/schemas/discogs/discogs-currency/)
- [Fee](https://apis.io/schemas/discogs/discogs-fee/)
- [Identifier](https://apis.io/schemas/discogs/discogs-identifier/)
- [Identity](https://apis.io/schemas/discogs/discogs-identity/)
- [Image](https://apis.io/schemas/discogs/discogs-image/)
- [InventoryExport](https://apis.io/schemas/discogs/discogs-inventory-export/)
- [InventoryExportsResponse](https://apis.io/schemas/discogs/discogs-inventory-exports-response/)
- [InventoryUpload](https://apis.io/schemas/discogs/discogs-inventory-upload/)
- [InventoryUploadsResponse](https://apis.io/schemas/discogs/discogs-inventory-uploads-response/)
- [Label](https://apis.io/schemas/discogs/discogs-label/)
- [LabelRelease](https://apis.io/schemas/discogs/discogs-label-release/)
- [LabelSummary](https://apis.io/schemas/discogs/discogs-label-summary/)
- [List](https://apis.io/schemas/discogs/discogs-list/)
- [ListItem](https://apis.io/schemas/discogs/discogs-list-item/)
- [Listing](https://apis.io/schemas/discogs/discogs-listing/)
- [ListingNew](https://apis.io/schemas/discogs/discogs-listing-new/)
- [ListingRelease](https://apis.io/schemas/discogs/discogs-listing-release/)
- [ListingUpdate](https://apis.io/schemas/discogs/discogs-listing-update/)
- …and 30 more published on APIs.io

#### JSON Structure (55)

Data models expressed in JSON Structure.

- [Discogs Artist Release Structure](https://apis.io/json-structure/discogs/discogs-artist-release-structure/)
- [Discogs Artist Structure](https://apis.io/json-structure/discogs/discogs-artist-structure/)
- [Discogs Artist Summary Structure](https://apis.io/json-structure/discogs/discogs-artist-summary-structure/)
- [Discogs Collection Folder Structure](https://apis.io/json-structure/discogs/discogs-collection-folder-structure/)
- [Discogs Collection Release Structure](https://apis.io/json-structure/discogs/discogs-collection-release-structure/)
- [Discogs Community Structure](https://apis.io/json-structure/discogs/discogs-community-structure/)
- [Discogs Contribution Structure](https://apis.io/json-structure/discogs/discogs-contribution-structure/)
- [Discogs Currency Structure](https://apis.io/json-structure/discogs/discogs-currency-structure/)
- [Discogs Fee Structure](https://apis.io/json-structure/discogs/discogs-fee-structure/)
- [Discogs Identifier Structure](https://apis.io/json-structure/discogs/discogs-identifier-structure/)
- [Discogs Identity Structure](https://apis.io/json-structure/discogs/discogs-identity-structure/)
- [Discogs Image Structure](https://apis.io/json-structure/discogs/discogs-image-structure/)
- [Discogs Inventory Export Structure](https://apis.io/json-structure/discogs/discogs-inventory-export-structure/)
- [Discogs Inventory Exports Response Structure](https://apis.io/json-structure/discogs/discogs-inventory-exports-response-structure/)
- [Discogs Inventory Upload Structure](https://apis.io/json-structure/discogs/discogs-inventory-upload-structure/)
- [Discogs Inventory Uploads Response Structure](https://apis.io/json-structure/discogs/discogs-inventory-uploads-response-structure/)
- [Discogs Label Release Structure](https://apis.io/json-structure/discogs/discogs-label-release-structure/)
- [Discogs Label Structure](https://apis.io/json-structure/discogs/discogs-label-structure/)
- [Discogs Label Summary Structure](https://apis.io/json-structure/discogs/discogs-label-summary-structure/)
- [Discogs List Item Structure](https://apis.io/json-structure/discogs/discogs-list-item-structure/)
- [Discogs List Structure](https://apis.io/json-structure/discogs/discogs-list-structure/)
- [Discogs Listing New Structure](https://apis.io/json-structure/discogs/discogs-listing-new-structure/)
- [Discogs Listing Release Structure](https://apis.io/json-structure/discogs/discogs-listing-release-structure/)
- [Discogs Listing Structure](https://apis.io/json-structure/discogs/discogs-listing-structure/)
- [Discogs Listing Update Structure](https://apis.io/json-structure/discogs/discogs-listing-update-structure/)
- …and 30 more published on APIs.io

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Discogs Context](https://apis.io/jsonld/discogs/discogs-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Discogs Vocabulary](https://apis.io/vocabularies/discogs/discogs-vocabulary/)

#### Examples (49)

Example requests and responses.

- [Discogs Artist Example](https://apis.io/examples/discogs/discogs-artist-example/)
- [Discogs Artist Release Example](https://apis.io/examples/discogs/discogs-artist-release-example/)
- [Discogs Artist Summary Example](https://apis.io/examples/discogs/discogs-artist-summary-example/)
- [Discogs Collection Folder Example](https://apis.io/examples/discogs/discogs-collection-folder-example/)
- [Discogs Collection Release Example](https://apis.io/examples/discogs/discogs-collection-release-example/)
- [Discogs Community Example](https://apis.io/examples/discogs/discogs-community-example/)
- [Discogs Contribution Example](https://apis.io/examples/discogs/discogs-contribution-example/)
- [Discogs Fee Example](https://apis.io/examples/discogs/discogs-fee-example/)
- [Discogs Identifier Example](https://apis.io/examples/discogs/discogs-identifier-example/)
- [Discogs Identity Example](https://apis.io/examples/discogs/discogs-identity-example/)
- [Discogs Image Example](https://apis.io/examples/discogs/discogs-image-example/)
- [Discogs Inventory Export Example](https://apis.io/examples/discogs/discogs-inventory-export-example/)
- [Discogs Inventory Exports Response Example](https://apis.io/examples/discogs/discogs-inventory-exports-response-example/)
- [Discogs Inventory Upload Example](https://apis.io/examples/discogs/discogs-inventory-upload-example/)
- [Discogs Inventory Uploads Response Example](https://apis.io/examples/discogs/discogs-inventory-uploads-response-example/)
- [Discogs Label Example](https://apis.io/examples/discogs/discogs-label-example/)
- [Discogs Label Release Example](https://apis.io/examples/discogs/discogs-label-release-example/)
- [Discogs Label Summary Example](https://apis.io/examples/discogs/discogs-label-summary-example/)
- [Discogs List Example](https://apis.io/examples/discogs/discogs-list-example/)
- [Discogs List Item Example](https://apis.io/examples/discogs/discogs-list-item-example/)
- [Discogs Listing Example](https://apis.io/examples/discogs/discogs-listing-example/)
- [Discogs Listing New Example](https://apis.io/examples/discogs/discogs-listing-new-example/)
- [Discogs Listing Release Example](https://apis.io/examples/discogs/discogs-listing-release-example/)
- [Discogs Listing Update Example](https://apis.io/examples/discogs/discogs-listing-update-example/)
- [Discogs Lists Response Example](https://apis.io/examples/discogs/discogs-lists-response-example/)
- …and 24 more published on APIs.io

#### Collections (8)

Postman and Open Collection request collections.

- [Discogs Database API](https://apis.io/collections/discogs/open-discogs-database-api/)
- [Discogs Database Image API](https://apis.io/collections/discogs/open-discogs-image-api/)
- [Discogs Database Inventory Management API](https://apis.io/collections/discogs/open-discogs-inventory-management-api/)
- [Discogs Database Marketplace API](https://apis.io/collections/discogs/open-discogs-marketplace-api/)
- [Discogs Database User Collection API](https://apis.io/collections/discogs/open-discogs-user-collection-api/)
- [Discogs Database User Identity API](https://apis.io/collections/discogs/open-discogs-user-identity-api/)
- [Discogs Database User Lists API](https://apis.io/collections/discogs/open-discogs-user-lists-api/)
- [Discogs Database User Wantlist API](https://apis.io/collections/discogs/open-discogs-user-wantlist-api/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Discogs — jsonschema rules](https://apis.io/rules/discogs/discogs-jsonschema-spectral-rules/)
- [Discogs API Rules](https://apis.io/rules/discogs/discogs-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Discogs Authentication](https://apis.io/security/discogs/discogs-authentication/)
- [Discogs Domain Security](https://apis.io/security/discogs/discogs-domain-security/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Discogs Scopes](https://apis.io/scopes/discogs/discogs-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Discogs Plans Pricing](https://apis.io/plans/discogs/discogs-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Discogs Rate Limits](https://apis.io/rate-limits/discogs/discogs-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.discogs.com)
- [Documentation](https://www.discogs.com/developers)
- [API reference](https://www.discogs.com/developers)
- [Support](https://support.discogs.com)
- [Blog](https://blog.discogs.com)
- [Terms of service](https://support.discogs.com/hc/articles/360009334593-API-Terms-of-Use)
- [GitHub](https://github.com/discogs)

## API Evangelist rating

**Kin Score 36.6** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 78.6 |
| Contract quality | 24.4 |
| Contract governance | 27.3 |
| Operational transparency | 10.5 |
| Developer ergonomics | 52.4 |
| Access clarity | 15.8 |

**Agent readiness 30.8** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | verified |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | documented (partial credit) |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 30.4** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/discogs/](https://apis.io/providers/discogs/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Discogs: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/discogs/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
