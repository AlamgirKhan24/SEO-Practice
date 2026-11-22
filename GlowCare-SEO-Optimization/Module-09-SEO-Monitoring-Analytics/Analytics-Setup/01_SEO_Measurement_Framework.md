# SEO Measurement Framework

**Status:** Proposed measurement design; no live GlowCare domain, verified GSC/GA4 properties, customer data or historical performance were provided.

## Objectives
Measure visibility in Google Search, qualified organic visits, useful content engagement, technical discoverability, relevant earned links and ecommerce outcomes after consent-aware tracking is implemented.

| Area | KPI | Definition / method | Source | Frequency / owner |
|---|---|---|---|---|
| Organic visibility | Clicks, impressions, CTR, average position | Search Console Performance; CTR = clicks ÷ impressions; position is a query/impression-weighted average | GSC | Monthly; SEO |
| Organic traffic | Organic sessions/users, engaged sessions, landing pages | GA4 Organic Search acquisition and landing page reports | GA4 | Monthly; analyst |
| Keyword performance | Query/page observations | GSC queries/pages; third-party rank tracker only as a separate estimate | GSC + optional tracker | Monthly; SEO |
| Content | Page clicks/impressions, CTR, sessions and content actions | Join GSC URL performance with GA4 landing page data; align canonical URL/date range | GSC + GA4 | Monthly; editor/SEO |
| Technical | Intended URL indexation, CWV status, sitemap, crawl issues | GSC indexing/CWV, crawl and PSI/CrUX where available | GSC/SF/PSI | Weekly critical checks; monthly review; SEO/dev |
| Backlinks | New/lost referring domains, relevant links, referral sessions | GSC Links and paid index exports; manual quality review | GSC/Ahrefs/Semrush/GA4 | Monthly; SEO/PR |
| Ecommerce | add_to_cart, checkout, purchase, refund, revenue | GA4 recommended events reconciled with backend orders | GA4 + backend | Weekly QA; monthly reporting; analytics/finance |
| Local | City query clicks/impressions, local pages, GBP metrics if eligible | GSC/GA4; Business Profile only if eligible/verified | GSC/GA4/GBP | Monthly; SEO |

## Reporting rules
Record date range, property, filters, source, export date, timezone, currency, and any sampling/consent limitations. Keep actual metrics separate from estimates and proposed targets. Search Console and GA4 use different attribution/definitions; do not expect exact parity. Never report zero as “no performance” if tracking is not configured; use “not available.”

Google Search Console measures clicks, impressions, CTR and average position; Google recommends trend interpretation, especially clicks/impressions rather than position alone. [GSC Performance](https://support.google.com/webmasters/answer/17010961)
