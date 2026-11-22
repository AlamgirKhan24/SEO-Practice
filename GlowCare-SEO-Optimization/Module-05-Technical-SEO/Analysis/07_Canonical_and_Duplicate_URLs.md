# Canonical and Duplicate URL Strategy

Choose one HTTPS host (www or non-www), one trailing-slash convention, and one consistent product/category URL format. Enforce host/protocol normalization with a single-hop permanent redirect. Use self-referencing canonicals on preferred indexable URLs.

- HTTP and alternate host: redirect permanently to chosen HTTPS canonical host.
- Trailing slash: redirect inconsistent variants if the platform supports stable normalization.
- Product variant routes: if content is substantially the same, canonicalize variants to the main product URL; retain distinct indexable variants only when users need them and the content differs meaningfully.
- Tracking parameters: canonical to clean URL when the page content is the same.
- Sort parameters: canonical to clean category if only ordering changes.
- Filters: index a facet landing page only if it has distinct search/user value and unique content; otherwise prevent duplicate indexation with a consistent canonical/noindex strategy. Avoid robots blocking before Google can see noindex/canonical signals; choose crawl-control based on platform and crawl budget needs.
- Pagination: each page gets its own URL and canonical; link sequentially. Don't canonicalize page 2+ to page 1.
- Similar categories: consolidate only if intent/content overlap is genuine. Keep separate useful categories with distinct inventory and purpose.
- Duplicate product copy: use accurate manufacturer facts plus useful unique store information; do not create boilerplate keyword text.

Canonical example: `<link rel="canonical" href="https://www.example.com/skincare/moisturizers/">`.

A permanent redirect is appropriate when retiring or permanently moving a URL and users/bots should resolve to one destination. Canonical is a signal for duplicate/alternate content that should remain accessible. [Google ecommerce URL guidance](https://developers.google.com/search/docs/specialty/ecommerce/designing-a-url-structure-for-ecommerce-sites).
