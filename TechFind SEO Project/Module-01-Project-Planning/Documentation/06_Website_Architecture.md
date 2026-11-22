# Proposed Website Architecture and URL Plan

**Status:** proposed structure; domain, platform, catalog depth, filters, and operational service facts are unconfirmed. No URL is live or implemented.

## Principles

- One indexable canonical landing page per useful category, supported brand, and product.
- Create a brand/use-case landing page only when it has a stable selection of products and unique utility; avoid near-duplicate thin pages.
- Keep faceted/filter URLs from generating uncontrolled indexable combinations. Decide crawl/index rules with actual platform behavior in Module 05.
- Product URLs should be stable across category paths where practical. Use a single canonical product URL; don't duplicate it under multiple folders.
- Preserve useful discontinued pages when they have ongoing demand/links, with alternatives; otherwise retire them using appropriate redirects or status codes after review.
- Keep policy and service information easy to find; policy wording must match the actual business and receive appropriate review.

## Proposed sitemap and page roles

| Level / page | Example URL pattern | Purpose and SEO role | Indexing / quality condition |
|---|---|---|---|
| Homepage | `/` | Brand introduction, main categories, trust/service facts, featured in-stock inventory | Unique, fast, clear links to primary catalog paths |
| Laptop hub | `/laptops/` | Broad laptop category and selection routes | Substantial useful assortment and category intro |
| Brand category | `/laptops/hp/`, `/laptops/dell/`, `/laptops/lenovo/` | Browse brand inventory | Publish only for stocked/maintained brand assortment; avoid brand pages with no unique product value |
| Use-case category | `/laptops/gaming/`, `/laptops/student/` | Help shoppers browse by a genuinely supported use case | Use objective criteria; only index if useful, sufficiently populated, and distinct |
| Accessories | `/laptop-accessories/` | Browse relevant accessories | Split into subcategories only when catalog supports it |
| Product detail | `/product/{brand-model-or-stable-slug}/` | Exact model/configuration, price, availability, specs, delivery and warranty facts | One canonical page per sellable variant when content and stock handling justify separate URLs |
| Buying guide | `/guides/how-to-choose-a-laptop/` | Explain selection and route to relevant categories/products | Original, maintained, knowledgeable guidance; disclose review methodology where applicable |
| Comparison guide | `/guides/{model-or-use-case}-comparison/` | Support considered purchases | Avoid speculative/unsupported product claims; update when models change |
| Blog index | `/guides/` or `/blog/` | Organize editorial resources | Prefer a useful guide hub; blog naming is a product decision, not an SEO requirement |
| About | `/about/` | Explain seller identity, expertise, sourcing/service practices | Only publish verifiable company/team claims |
| Contact | `/contact/` | Provide support/contact routes and service hours | Match active channels; protect personal contact data where appropriate |
| Delivery | `/delivery/` | Coverage, fees and timing | Publish only operationally approved details |
| Returns/refunds | `/returns/` | Explain return eligibility/process | Must match actual policy and applicable law; obtain business/legal review |
| Warranty | `/warranty/` | Explain warranty scope and claim path | Distinguish manufacturer and seller coverage precisely |
| Payment | `/payment/` | Explain accepted methods and process | Publish only supported methods |
| Privacy | `/privacy/` | Explain data processing | Business/legal review required |
| Terms | `/terms/` | Purchase terms | Business/legal review required |
| Cart/checkout/account | `/cart/`, `/checkout/`, `/account/` | Complete purchase and manage account | Usually no search landing value; control indexation appropriately after technical review |

## Navigation and internal links

Primary navigation: Laptops, Accessories, Buying Guides, About, Contact. Use breadcrumbs from home → category → product. Guides link to relevant categories/products; product pages link to comparable products and relevant guides. Use crawlable HTML links and descriptive anchors. Do not force every product into multiple indexable path variants.

## Pakistan language/region handling

Begin with one Pakistan-serving English experience if that matches audience and support capability. Add Urdu only after validating demand and committing to full-quality translation, language-specific URLs, localized content, and correct alternate-language annotations. Avoid mixing languages in a way that creates duplicate or confusing versions. Do not geotarget city pages without distinct service evidence.

## URL examples

Examples are illustrative only, not keyword research or exact SEO targets. Keep slugs lowercase, concise, stable, and understandable. Product page slug should include an unambiguous brand/model identifier rather than a mutable promotional phrase.
