# Crawlability and Indexability — Proposed Configuration

No live domain was supplied; these are configuration principles, not tested directives.

- Allow public, useful category, product, brand, guide, and policy pages to be crawled. Use real crawlable `<a href>` links from navigation/category/pagination; don't rely on search forms or button-only navigation.
- Keep admin, cart, checkout, account and internal search out of search results via application authentication where needed and `noindex` for crawlable pages that should not appear. Do not treat robots.txt as security.
- Use robots.txt only to manage crawling of known URL patterns/resources. A blocked URL may still appear as a URL-only result if linked elsewhere. Don't block CSS/JS needed to render pages.
- Use self-referencing canonical tags on indexable pages. For truly duplicate or alternate URLs, canonicalize consistently; use redirects for permanent URL moves/host normalization.
- Keep faceted combinations controlled. Index only facets with distinct demand and unique value; otherwise use a consistent parameter strategy, canonical/noindex as appropriate, and consider crawl controls after ensuring important product links remain discoverable.
- Product pages should be linked from categories and sitemap; do not make search-box discovery the only route.
- Pagination needs distinct crawlable URLs and sequential links; each page should have its own canonical when it represents distinct products. Don't canonicalize every page to page one.
- Monitor URL Inspection, Page indexing, sitemap processing and server logs once verified Search Console/site access exists.

Example directives are in `06_Robots_txt_Recommendation.txt`. Validate them against actual platform routes before deployment.

Sources: [Google ecommerce navigation](https://developers.google.com/search/docs/specialty/ecommerce/help-google-understand-your-ecommerce-site-structure), [faceted navigation](https://developers.google.com/crawling/docs/faceted-navigation), [robots.txt introduction](https://developers.google.com/search/docs/crawling-indexing/robots/intro).
