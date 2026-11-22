# Structured Data and Schema Specification

**Status:** No live page markup exists in the supplied project for inspection or validation. The examples below are illustrative JSON-LD shapes; replace placeholders with accurate visible data and validate against current Google documentation before launch.

## Appropriate types by page

- **Organization:** verified company name, official URL, logo, and contact/profile details only. Do not invent address, social profiles, customer service numbers or credentials.
- **WebSite:** verified canonical site name and URL. Do not add a site-search action unless the site has a functioning query URL and feature.
- **BreadcrumbList:** reflect visible navigation hierarchy and actual canonical destinations.
- **Product and Offer:** product detail pages only, with exact product identity and matching visible price, currency, availability and condition. No example should ship until sourced from the live product record.
- **Article:** original buying guides/comparisons with actual headline, author/publisher and publication dates. Keep visible content consistent.
- **Review/AggregateRating:** only genuine reviews collected and displayed under the applicable policies. No fabricated or imported unverified ratings; avoid self-serving organization reviews.

## Product/Offer example template

```json
{
  "@context": "https://schema.org",
  "@type": "Product",
  "name": "{verified product name}",
  "image": ["https://{confirmed-domain}/{actual-product-image}.webp"],
  "description": "{accurate visible product description}",
  "sku": "{actual SKU}",
  "brand": {"@type": "Brand", "name": "{verified brand}"},
  "offers": {
    "@type": "Offer",
    "url": "https://{confirmed-domain}/product/{actual-slug}/",
    "priceCurrency": "{actual ISO 4217 currency}",
    "price": "{current displayed numeric price}",
    "availability": "https://schema.org/{actual availability enum}"
  }
}
```

The template is valid JSON syntax after substitution only if values are escaped and enums/URLs are correct. It is not validated structured data, and placeholders must never be published. Do not include review/rating properties without real eligible data.

## Validation plan

On staging/production, validate representative product, category, guide and breadcrumb pages using the current Google Rich Results Test for Google-supported experiences and Schema.org Validator for general vocabulary. Inspect rendered HTML and compare every marked-up fact with visible page content, product feed and checkout. Save test date, URL, tool output and screenshots. No tests have been run and no markup has been generated/deployed.
