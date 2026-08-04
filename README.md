# Simplecast (simplecast)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
