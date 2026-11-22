# Checklist: Crawlability

Can search engines discover and fetch the site's important URLs reliably?

- [ ] `robots.txt` is available at `/robots.txt` and returns an expected response
- [ ] Important pages and required resources are not unintentionally blocked by `robots.txt`
- [ ] The sitemap is referenced from `robots.txt` when appropriate
- [ ] XML sitemaps are reachable and submitted to relevant webmaster tools when available
- [ ] Sitemaps contain preferred, canonical URLs that return successful responses and are intended for indexing
- [ ] Each sitemap respects the limit of 50,000 URLs or 50 MB uncompressed; larger sets use a sitemap index
- [ ] Sitemaps are segmented meaningfully when that helps monitoring and maintenance
- [ ] Important pages are reachable through crawlable internal links
- [ ] Low-value URL spaces, filters, and parameters do not create uncontrolled crawl paths
- [ ] Important pages return consistent responses to users and search-engine crawlers
- [ ] Redirect chains, loops, and recurring server errors are investigated
- [ ] Crawl depth and orphan URL checks are reviewed against the site's intended architecture
- [ ] Staging and non-production environments are protected from unintended public indexing

A robots.txt block can prevent crawling but does not, by itself, guarantee that a URL will be excluded from search results. Check indexing controls and the actual URL signals separately.

**Related fix guides:** `fixes/crawlability/`
