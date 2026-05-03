# The New York Times

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
