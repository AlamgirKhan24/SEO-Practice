# XML Sitemap Strategy

Generate sitemap(s) from the production CMS/catalog. Include only absolute, canonical, indexable URLs returning 200: homepage, useful categories, in-stock or otherwise valid product pages, approved brand pages, published articles/guides and important public information pages. Exclude redirects, noindex URLs, internal search, cart, checkout, account, filters/sort variations and error pages.

Use a sitemap index when there are multiple sitemaps, e.g. products, categories/pages, and articles. Google accepts up to 50,000 URLs or 50MB uncompressed per sitemap. Keep `<lastmod>` accurate and based on significant page changes; don't update every URL every day without an actual change. Submit the index in Search Console and reference it in robots.txt. Sitemap discovery doesn't guarantee crawl or indexation.

The supplied XML is illustrative and uses `https://www.example.com` because GlowCare has no domain yet. Replace the origin only after canonical hostname selection. [Google sitemap overview](https://developers.google.com/search/docs/crawling-indexing/sitemaps/overview) · [Build and submit](https://developers.google.com/search/docs/crawling-indexing/sitemaps/build-sitemap).
