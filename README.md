# The New York Times

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

The New York Times is one of the world's most respected news organizations, providing comprehensive journalism across politics, culture, business, science, health, and the arts since 1851. The NYT Developer Network exposes a suite of RESTful APIs enabling developers to search and access NYT articles, best-seller book lists, movie reviews, semantic metadata, top stories, and popular content. All APIs require an API key obtained from the NYT Developer Portal.

**Website:** [nytimes.com](https://nytimes.com)  
**Developer Portal:** [developer.nytimes.com](https://developer.nytimes.com)  
**GitHub:** [github.com/nytimes](https://github.com/nytimes)

---

## APIs

| API | Description | Base URL |
|-----|-------------|----------|
| [Archive API](https://developer.nytimes.com/docs/archive-product/1/overview) | Articles by month going back to 1851 | `https://api.nytimes.com/svc/archive/v1` |
| [Article Search API](https://developer.nytimes.com/docs/articlesearch-product/1/overview) | Full-text article search with facets | `https://api.nytimes.com/svc/search/v2` |
| [Books API](https://developer.nytimes.com/docs/books-product/1/overview) | Best Sellers lists and book reviews | `https://api.nytimes.com/svc/books/v3` |
| [Most Popular API](https://developer.nytimes.com/docs/most-popular-product/1/overview) | Most emailed, shared, and viewed articles | `https://api.nytimes.com/svc/mostpopular/v2` |
| [Movie Reviews API](https://developer.nytimes.com/docs/movie-reviews-api/1/overview) | Movie reviews and critics' picks | `https://api.nytimes.com/svc/movies/v2` |
| [Semantic API](https://developer.nytimes.com/docs/semantic-api-product/1/overview) | Controlled vocabulary of entities and concepts | `https://api.nytimes.com/svc/semantic/v2` |
| [TimesTags API](https://developer.nytimes.com/docs/timestags-product/1/overview) | Tag autocomplete (deprecated, use Semantic API) | `https://api.nytimes.com/svc/suggest/v1` |
| [Times Newswire API](https://developer.nytimes.com/docs/timeswire-product/1/overview) | Real-time article stream as articles are published | `https://api.nytimes.com/svc/news/v3` |
| [Top Stories API](https://developer.nytimes.com/docs/top-stories-product/1/overview) | Articles currently featured on section pages | `https://api.nytimes.com/svc/topstories/v2` |

---

## OpenAPI Specifications

| Spec | File |
|------|------|
| Archive API | [openapi/new-york-times-archive-openapi-original.yml](openapi/new-york-times-archive-openapi-original.yml) |
| Article Search API | [openapi/new-york-times-article-search-openapi-original.yml](openapi/new-york-times-article-search-openapi-original.yml) |
| Books API | [openapi/new-york-times-books-openapi-original.yml](openapi/new-york-times-books-openapi-original.yml) |
| Most Popular API | [openapi/new-york-times-most-popular-openapi-original.yml](openapi/new-york-times-most-popular-openapi-original.yml) |
| Movie Reviews API | [openapi/new-york-times-movie-review-openapi-original.yml](openapi/new-york-times-movie-review-openapi-original.yml) |
| Semantic API | [openapi/new-york-times-semantic-openapi-original.yml](openapi/new-york-times-semantic-openapi-original.yml) |
| TimesTags API | [openapi/new-york-times-times-tags-openapi-original.yml](openapi/new-york-times-times-tags-openapi-original.yml) |
| Times Newswire API | [openapi/new-york-times-times-newswire-openapi-original.yml](openapi/new-york-times-times-newswire-openapi-original.yml) |
| Top Stories API | [openapi/new-york-times-top-stories-openapi-original.yml](openapi/new-york-times-top-stories-openapi-original.yml) |

---

## Naftiko Capabilities

Capabilities are organized in two layers: shared per-API definitions and workflow-oriented compositions.

### Workflow Capabilities

| Workflow | File | Description |
|----------|------|-------------|
| Article Research | [capabilities/article-research.yaml](capabilities/article-research.yaml) | Article search + archive + top stories + newswire for journalists and researchers |
| Content Discovery | [capabilities/content-discovery.yaml](capabilities/content-discovery.yaml) | Most popular articles + books best sellers + movie reviews for media analysis |
| Metadata Enrichment | [capabilities/metadata-enrichment.yaml](capabilities/metadata-enrichment.yaml) | Semantic concept lookup and search for entity resolution and knowledge graphs |

### Shared Per-API Definitions

| API | File |
|-----|------|
| Archive API | [capabilities/shared/archive.yaml](capabilities/shared/archive.yaml) |
| Article Search API | [capabilities/shared/article-search.yaml](capabilities/shared/article-search.yaml) |
| Books API | [capabilities/shared/books.yaml](capabilities/shared/books.yaml) |
| Most Popular API | [capabilities/shared/most-popular.yaml](capabilities/shared/most-popular.yaml) |
| Movie Reviews API | [capabilities/shared/movie-reviews.yaml](capabilities/shared/movie-reviews.yaml) |
| Semantic API | [capabilities/shared/semantic.yaml](capabilities/shared/semantic.yaml) |
| Top Stories API | [capabilities/shared/top-stories.yaml](capabilities/shared/top-stories.yaml) |
| Times Newswire API | [capabilities/shared/times-newswire.yaml](capabilities/shared/times-newswire.yaml) |

---

## Spectral Rules

| Ruleset | File |
|---------|------|
| NYT API Rules | [rules/new-york-times-rules.yml](rules/new-york-times-rules.yml) |

---

## JSON Schemas

| Schema | File |
|--------|------|
| Article | [json-schema/new-york-times-article-schema.json](json-schema/new-york-times-article-schema.json) |
| Best Seller Book | [json-schema/new-york-times-book-schema.json](json-schema/new-york-times-book-schema.json) |

---

## JSON Structure

| Structure | File |
|-----------|------|
| Article | [json-structure/new-york-times-article-structure.json](json-structure/new-york-times-article-structure.json) |

---

## JSON-LD

| Context | File |
|---------|------|
| NYT Context | [json-ld/the-new-york-times-context.jsonld](json-ld/the-new-york-times-context.jsonld) |

---

## Examples

| Example | File |
|---------|------|
| Search Articles | [examples/new-york-times-search-articles-example.json](examples/new-york-times-search-articles-example.json) |
| Top Stories | [examples/new-york-times-top-stories-example.json](examples/new-york-times-top-stories-example.json) |

---

## Vocabulary

| Vocabulary | File |
|------------|------|
| NYT Vocabulary | [vocabulary/the-new-york-times-vocabulary.yml](vocabulary/the-new-york-times-vocabulary.yml) |

---

## Authentication

All NYT APIs use API key authentication passed as a query parameter:

```
?api-key=YOUR_API_KEY
```

Get your API key at [developer.nytimes.com/accounts/create](https://developer.nytimes.com/accounts/create).

---

## SDKs and Clients

- [Times Wire Ruby Client](https://github.com/nytimes/times_wire) — Ruby client for the Times Newswire API
- [NYT Campaign Finance Python Client](https://github.com/nytimes/nytcampfin) — Python client for the Campaign Finance API
- [Public API Specs](https://github.com/nytimes/public_api_specs) — Official OpenAPI specifications from NYT

---

## Maintainers

**FN:** Kin Lane  
**Email:** kin@apievangelist.com

---

*Profile generated 2026-05-03*
