# Crawlability and Indexability Status

**Audit date:** 21 November 2026  
**Scope:** readiness assessment only. No TechFind domain or staging URL was supplied.

## Findings

Googlebot access, robots.txt, HTML robots directives, X-Robots-Tag, blocked resources, internal links, crawl depth and index coverage are **unknown**. No crawling or Search Console inspection was possible. This is not evidence of either healthy or unhealthy technical status.

Keep the concepts separate:

- **Crawlability:** whether a crawler can request and render a URL/resources. A robots.txt disallow can prevent crawling, but is not a reliable way to remove a URL from search results.
- **Indexability:** whether a crawled URL is eligible and selected for indexing. `noindex` is an indexing directive that must be crawlable for Google to observe; conflicting canonical/robots signals can confuse selection.
- **Discovery:** provide crawlable links from the navigation, categories, breadcrumbs and related content. A sitemap helps discovery but does not guarantee indexing.

## Recommended template checks after a staging URL exists

1. Test robots.txt, DNS/TLS and representative category/product/guide URLs with a crawler using rendered-page inspection where needed.
2. Inspect meta robots and X-Robots-Tag headers for each template, including pagination, filters, internal search, cart and checkout.
3. Confirm products and categories are reachable through links and are not blocked by authentication, robots rules, WAF challenge or client-side-only navigation.
4. Compare allowed crawl URLs with canonical URLs and intended indexable pages. Do not use robots.txt to hide duplicate pages that need canonical/noindex signals observed.
5. Verify key URLs in Search Console URL Inspection after property verification.
6. Record crawl date, user agent, rendering mode, URL count, status distribution, errors and exclusions; save raw exports.

Detailed current status and recommendations are in `Audits/03_Crawlability_Indexability_Status.csv`. No fixes have been implemented.
