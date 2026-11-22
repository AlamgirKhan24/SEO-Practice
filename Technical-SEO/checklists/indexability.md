# Checklist: Indexability

Check whether important, canonical pages can be indexed and whether duplicate or low-value URLs are handled intentionally. A single signal does not always determine Google's selected canonical or indexing outcome.

- [ ] Important URLs return the expected status and are not unintentionally marked `noindex` in HTML or `X-Robots-Tag`
- [ ] Canonical signals (HTML, redirects, sitemap, and internal links) are consistent for important pages
- [ ] Canonical targets are valid, indexable, and representative of duplicate or equivalent content
- [ ] HTTP/HTTPS, hostname, trailing-slash, and parameter variants resolve consistently where appropriate
- [ ] Search Console indexing reports and URL Inspection are reviewed when access and data are available
- [ ] Reported exclusions are compared with the site's intended indexing strategy before being treated as defects
- [ ] Thin, duplicate, expired, or internal-search pages have an intentional indexation strategy
- [ ] Paginated, faceted, and filtered URLs are reviewed for crawl and indexation impact
- [ ] Soft 404s and error pages that return a successful status are identified
- [ ] Important content is present in rendered HTML when client-side rendering is used
- [ ] Internal links and XML sitemaps point to the preferred canonical URLs

Do not treat a missing self-referencing canonical, an SEO plugin score, or a search-engine exclusion as an issue without checking the page purpose and other canonicalization signals.

**Related fix guides:** `fixes/indexability/`
