# TechFind Product Page SEO Template

**Status:** proposed reusable specification. No actual SKU or live TechFind page was supplied.

## Above the fold

- Breadcrumbs: Home → relevant category → product, with links to real canonical destinations.
- H1: `{Brand} {Model} {Key Configuration}`. Keep the title specific to the sellable configuration.
- Product images: original, sufficiently detailed, accurate views. Use descriptive filenames and alt text that describes the visible view.
- Price and availability: show current feed-backed price and stock state; keep the page consistent with checkout and structured data.
- Purchase control: clear add-to-cart/buy action with accessible name and visible state.
- Short summary: explain what differentiates this specific configuration using verified facts.

## Suggested content order

1. Product name and concise factual summary.
2. Price, availability, delivery estimate and warranty provider/terms (only verified current facts).
3. Key specification summary.
4. Full specifications table: manufacturer/model identifier, processor, graphics, memory, storage, display, operating system, ports, connectivity, dimensions/weight, battery (as officially specified), and included items. Omit unknown fields rather than guessing.
5. Compatibility, configuration and package notes where relevant.
6. Shipping, returns and warranty links to approved policy pages.
7. Genuine customer reviews, if collected and displayed with appropriate moderation/disclosure. Never fabricate, selectively misrepresent, or mark up nonexistent reviews.
8. Related products selected by a clear user need (similar configuration, alternative price, or compatible accessory).

## Metadata and headings

- Title pattern: `{Brand} {Model} {Key Configuration} | TechFind`.
- Meta description: `Review verified specifications, current availability and price for the {Brand} {Model}. Check compatibility and included items before ordering.` Populate only if accurate; keep descriptions unique.
- One H1 for the page. H2 examples: `Key specifications`, `Full specifications`, `What’s included`, `Warranty and delivery`, `Customer reviews`, `Related products`.
- Stable URL pattern: `/product/{brand-model-configuration}/`. Avoid session IDs, mutable sale claims, or multiple category-path copies. Use one canonical URL per sellable variant where the data is meaningfully distinct.

## Image and accessibility details

- Example filename: `dell-inspiron-14-7440-front.webp` (only when the image truly depicts that product/model/view).
- Example alt: `Dell Inspiron 14 7440 laptop, front view`.
- Use empty alt for decorative images; don't repeat surrounding copy in alt text.
- Supply responsive image candidates, explicit intrinsic dimensions/aspect ratio, and efficient modern formats with fallback where needed.
- Avoid lazy-loading the main likely Largest Contentful Paint image; lazy-load below-the-fold gallery images.
- Ensure keyboard access, visible focus, labeled controls, sufficient text contrast, and meaningful status announcements.

## Structured data recommendation

Consider `Product` and `Offer` structured data only when the visible page contains matching, accurate product/offer facts. Ensure currency, price, stock status, product identity and review information (if any) agree with the page and checkout. Do not invent GTIN/MPN, ratings, reviews, price, or availability. Validate using current search-engine documentation and testing tools at implementation time; no markup has been created or tested in this project.

## QA before publishing

- Confirm every field against the live product record and manufacturer documentation.
- Verify price, currency, stock and policy consistency through checkout.
- Confirm canonical URL, indexability, breadcrumb destinations and internal links in the rendered site.
- Test mobile layout, image zoom, keyboard flow, and error/stock-state messages.
- Review title/H1 uniqueness across variants and avoid near-duplicate pages that do not help shoppers.
