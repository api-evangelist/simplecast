# Simplecast (simplecast)

Simplecast is a podcast hosting, distribution, and analytics platform for creators, networks, and brands, owned by SiriusXM Media (SiriusXM acquired Simplecast in 2020). It provides podcast and episode management, distribution to Apple Podcasts, Spotify, and other channels, embeddable players, and IAB-certified audience analytics.

Simplecast exposes a documented REST API at `https://api.simplecast.com` covering podcasts, episodes, analytics, and distribution channels. The API is self-describing - each response returns the actions available to the authenticated user - and is authenticated with a bearer token generated from the **Private Apps** page in the Simplecast dashboard (`authorization: Bearer {token}`). List endpoints paginate with `limit` and `offset` query parameters.

**Access model:** The API documentation at [apidocs.simplecast.com](https://apidocs.simplecast.com/) is publicly readable, but calling the API requires a Simplecast account and a token. Simplecast's pricing page lists "API integration" as an Enterprise-tier feature, so full/production API access appears gated to higher tiers even though the docs are open. The endpoint list in this catalog is confirmed from Simplecast's official public Postman collection; OpenAPI request/response schemas are lightly modeled because Simplecast does not publish a formal schema. The API is predominantly read-only (HTTP GET); the one documented write is uploading episode audio.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/simplecast/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/simplecast/refs/heads/main/apis.yml)

## Tags

- Podcasting
- Podcast Hosting
- Podcast Distribution
- Podcast Analytics
- Audio
- Media
- SiriusXM Media

## Timestamps

- **Created:** 2026-07-05
- **Modified:** 2026-07-05

## APIs

### Simplecast Podcasts API

List and retrieve podcasts (shows) in the authenticated account and read their related metadata - authors, categories and subcategories, keywords, seasons, distribution channels, and the generated RSS feed.

- **Human URL:** [https://apidocs.simplecast.com/](https://apidocs.simplecast.com/)
- **Base URL:** `https://api.simplecast.com`

#### Tags

- Podcasts
- Shows
- Metadata

#### Properties

- [Documentation](https://apidocs.simplecast.com/)
- [API Reference](https://apidocs.simplecast.com/)
- [OpenAPI](openapi/simplecast-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/simplecast.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/simplecast.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Simplecast Episodes API

List a podcast's episodes and retrieve individual episodes with their authors, keywords, and chapter markers, plus the seasons an episode belongs to. Supports uploading episode audio via a POST to the episode audio endpoint.

- **Human URL:** [https://apidocs.simplecast.com/](https://apidocs.simplecast.com/)
- **Base URL:** `https://api.simplecast.com`

#### Tags

- Episodes
- Audio
- Markers

#### Properties

- [Documentation](https://apidocs.simplecast.com/)
- [API Reference](https://apidocs.simplecast.com/)
- [OpenAPI](openapi/simplecast-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/simplecast.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/simplecast.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Simplecast Analytics API

Read audience analytics for podcasts and episodes - downloads, listeners, hours listened, top episodes, geographic location, time of week, listening technology (applications, browsers, devices, operating systems, web players, network types), campaigns, and embeddable-player analytics such as listens, locations, speeds, heatmap, and average completion.

- **Human URL:** [https://apidocs.simplecast.com/](https://apidocs.simplecast.com/)
- **Base URL:** `https://api.simplecast.com`

#### Tags

- Analytics
- Downloads
- Listeners

#### Properties

- [Documentation](https://apidocs.simplecast.com/)
- [API Reference](https://apidocs.simplecast.com/)
- [OpenAPI](openapi/simplecast-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/simplecast.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/simplecast.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Simplecast Distribution API

List distribution channels and retrieve a specific channel, and read the distribution channels a given podcast is syndicated to (Apple Podcasts, Spotify, and other destinations).

- **Human URL:** [https://apidocs.simplecast.com/](https://apidocs.simplecast.com/)
- **Base URL:** `https://api.simplecast.com`

#### Tags

- Distribution
- Channels
- Syndication

#### Properties

- [Documentation](https://apidocs.simplecast.com/)
- [API Reference](https://apidocs.simplecast.com/)
- [OpenAPI](openapi/simplecast-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/simplecast.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/simplecast.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/simplecast)
- [Website](https://www.simplecast.com)
- [Documentation](https://apidocs.simplecast.com/)
- [Plans](plans/simplecast-plans-pricing.yml)
- [Rate Limits](rate-limits/simplecast-rate-limits.yml)
- [Fin Ops](finops/simplecast-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
