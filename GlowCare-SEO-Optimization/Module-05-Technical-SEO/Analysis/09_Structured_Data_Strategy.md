# Structured Data Strategy and Examples

Only use JSON-LD values visible and accurate on the page. Replace placeholders from real business/catalog sources; omit unavailable fields. Validate with Google Rich Results Test and Schema Markup Validator. Structured data can make a page eligible for supported appearances but does not guarantee display.

## Organization (sitewide, after details are verified)
```json
{"@context":"https://schema.org","@type":"Organization","name":"GlowCare","url":"https://www.example.com/","logo":"https://www.example.com/assets/logo.png","contactPoint":{"@type":"ContactPoint","contactType":"customer support","url":"https://www.example.com/contact/"}}
```
Do not invent legal name, address, telephone, logo asset, social profiles or sameAs links.

## WebSite (homepage)
```json
{"@context":"https://schema.org","@type":"WebSite","name":"GlowCare","url":"https://www.example.com/"}
```

## BreadcrumbList
```json
{"@context":"https://schema.org","@type":"BreadcrumbList","itemListElement":[{"@type":"ListItem","position":1,"name":"Home","item":"https://www.example.com/"},{"@type":"ListItem","position":2,"name":"Skincare","item":"https://www.example.com/skincare/"},{"@type":"ListItem","position":3,"name":"Moisturizers","item":"https://www.example.com/skincare/moisturizers/"}]}
```

## Product and Offer (example template; do not publish placeholder values)
```json
{"@context":"https://schema.org","@type":"Product","name":"{exact visible product name}","image":["{public product image URL}"],"description":"{accurate visible description}","brand":{"@type":"Brand","name":"{verified brand}"},"sku":"{verified SKU}","offers":{"@type":"Offer","url":"{canonical product URL}","priceCurrency":"PKR","price":"{current visible numeric price}","availability":"https://schema.org/InStock"}}
```
Remove fields not known; `availability` must mirror live stock. Never invent ratings/reviews. AggregateRating/review markup requires genuine eligible review content, visible on-page and compliant with Google policy. Product rich results are subject to Google requirements and can change. Use merchant center feeds as appropriate.

## Article / BlogPosting
```json
{"@context":"https://schema.org","@type":"BlogPosting","headline":"{visible article headline}","image":["{representative image URL}"],"datePublished":"{ISO date}","dateModified":"{ISO date}","author":{"@type":"Person","name":"{real author name}","url":"{author bio URL}"},"publisher":{"@type":"Organization","name":"GlowCare"},"mainEntityOfPage":"{canonical article URL}"}
```
Use real dates and credited authors only. Google Article docs describe these as recommended properties. [Product](https://developers.google.com/search/docs/appearance/structured-data/product), [Article](https://developers.google.com/search/docs/appearance/structured-data/article), [Breadcrumb](https://developers.google.com/search/docs/appearance/structured-data/breadcrumb), [Organization](https://developers.google.com/search/docs/appearance/structured-data/organization).
