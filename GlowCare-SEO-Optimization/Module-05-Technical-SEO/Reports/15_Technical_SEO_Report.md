# Module 05 — Technical SEO Report

**Date prepared:** 21 November 2026  
**Project:** GlowCare, proposed portfolio ecommerce concept for Pakistan  
**Status:** Technical baseline plan. No live domain or staging site was provided; no live technical audit or implementation is claimed.

## Baseline and crawl analysis
All actual test fields are unassessed. The baseline workbook lists checks, evidence needed, methods, priority and recommended action. The crawl workbook is a repeatable crawl protocol covering response codes, internal/external links, redirects, metadata, headings, canonicals, directives and orphan discovery. Recommended tool chain: Screaming Frog for crawl, Search Console for Google-side indexing/CWV, browser/device review, PSI/Lighthouse for performance. Run only after the domain and access are confirmed.

## Crawlability, indexability, sitemap and robots
Keep public product/category/brand/guide pages crawlable and linked. Use an automatically generated sitemap containing only canonical, indexable, successful URLs. Reference it in robots.txt and submit via GSC; inclusion does not guarantee indexing. The sample sitemap intentionally uses `example.com` placeholders. The sample robots file blocks likely private/search areas; validate actual platform routes before deployment. Robots.txt is not access control and does not reliably remove URLs from results.

## Canonicals and duplicates
Normalize HTTP/HTTPS and host with one-hop permanent redirects. Use self-referencing canonicals on indexable pages and clean canonical product/category URLs. Control sort/filter parameters; index only distinct valuable facets. Keep pagination URLs distinct and crawlable with their own canonicals. Redirect permanent moves; use canonical hints for duplicate/alternate versions that remain available.

## Performance and mobile
No PSI, Lighthouse, CrUX or field data was available. Measure representative home/category/product/guide templates after launch, separating lab diagnostics from field data. Google’s current good CWV thresholds at the 75th percentile are LCP ≤2.5s, INP <200ms, CLS <0.1. Optimize only after measuring. Mobile test list covers navigation, readability, media, product selection and checkout parity.

## Structured data
Use Organization/WebSite/BreadcrumbList and Product/Offer/Article only with accurate information visible on the corresponding pages. Examples are templates with placeholders; do not publish until product data, price, stock, brand, author and business details are real. Do not add fake reviews/ratings. Validate markup and keep it synchronized with page content. Eligibility does not guarantee rich results.

## HTTPS, redirects, regional SEO
Use valid TLS, one-hop HTTPS redirects, no mixed content, and carefully tested security headers; this is not a penetration test. Maintain a redirect map for changed/deleted URLs; do not blanket-redirect removed products to the home page. Begin with Pakistan-focused English pages. Add Urdu alternatives only when high-quality translations/support exist; use reciprocal hreflang only for true equivalent page variants.

## Issue and implementation plans
Issue tracker entries are potential risks/recommendations, not detected defects. Roadmap begins with domain/platform/access confirmation, then crawl and indexation foundations, mobile QA, measured performance work, structured data and ongoing monitoring. Priorities and estimates are preliminary pending platform and developer review.

## Limitations and inferred deliverables
The supplied Module 05 prompt cuts off after the sixth deliverable filename (`06_R...`). I completed every visible task and inferred additional deliverable names from the task list: crawlability report, sample sitemap, robots recommendation, canonical strategy, performance/mobile, schema, redirects/regional, workbooks, and final report. No actual site testing is possible until a live URL is provided.

## Files
See folders `Audits/`, `Analysis/`, `Configuration/`, `Spreadsheets/`, and `Reports/`. Module 06 and later work has not begun.

### Sources
[Google Search Central: Core Web Vitals](https://developers.google.com/search/docs/appearance/core-web-vitals) · [PageSpeed Insights](https://developers.google.com/speed/docs/insights/v5/about) · [Sitemaps](https://developers.google.com/search/docs/crawling-indexing/sitemaps/overview) · [Ecommerce site structure](https://developers.google.com/search/docs/specialty/ecommerce/help-google-understand-your-ecommerce-site-structure) · [Ecommerce URL structure](https://developers.google.com/search/docs/specialty/ecommerce/designing-a-url-structure-for-ecommerce-sites) · [Faceted navigation](https://developers.google.com/crawling/docs/faceted-navigation) · [Robots.txt](https://developers.google.com/search/docs/crawling-indexing/robots/intro) · [Product structured data](https://developers.google.com/search/docs/appearance/structured-data/product) · [Article structured data](https://developers.google.com/search/docs/appearance/structured-data/article).
