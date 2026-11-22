# robots.txt Audit and Planned Specification

**Status:** No domain or current robots.txt was supplied. No robots file was fetched. Existing directives and Googlebot access are unknown.

## Safe starting point

Do not block the laptop, category, product, guide or required rendering-resource paths. Avoid adding rules for `/wp-admin/`, parameters, assets, or checkout until the actual platform paths and intended behavior are known. `robots.txt` is a crawl control, not access security and not a guaranteed deindexing method. For private pages, use authentication; for URLs that should be excluded from indexing, use an appropriate crawlable noindex response/page or remove the URL as applicable.

## Illustrative template only

```text
User-agent: *
Allow: /
Sitemap: https://{confirmed-domain}/sitemap.xml
```

Replace the placeholder with the selected HTTPS host before deployment. This permissive template is not a recommendation to expose private application routes; protect those with authentication and application controls. Test the final rules against representative category/product URLs and required CSS/JS before release. No robots change has been implemented or tested.
