# Proposed Website Architecture

Architecture is conditional on the actual catalog, brand rights, platform, inventory, and query research. Build a page only when it serves a distinct user need and has stable, useful content. Avoid indexing empty, duplicate, thin, or temporary filter combinations.

| Page type | Example URL | Purpose / audience | SEO role and internal links |
|---|---|---|---|
| Home | `/` | Explain offer and guide all shoppers | Link to priority categories, trust/policy information, guides, and seasonal content where useful |
| Skincare hub | `/skincare/` | Organize face-care range | Parent hub to cleansers, moisturizers, sunscreen, serums, toners, masks |
| Cleansers | `/skincare/cleansers/` | Browse actual cleanser selection | Link to relevant products and neutral cleanser guide |
| Moisturizers | `/skincare/moisturizers/` | Browse moisturizer range | Link to products and routine/selection guide |
| Sunscreens | `/skincare/sunscreens/` | Browse sun-protection products | Link to exact product details and educational sunscreen guide; avoid unverified SPF/medical claims |
| Serums | `/skincare/serums/` | Browse serum products | Link to products and ingredient explainers after evidence review |
| Toners | `/skincare/toners/` | Browse toners if assortment merits distinct category | Link to products; omit if too few products or no distinct intent |
| Face masks | `/skincare/face-masks/` | Browse masks where useful inventory exists | Cross-link to products and related skincare categories |
| Hair care | `/hair-care/` | Separate hair-care assortment | Link to subcategories only when real assortment supports them |
| Body care | `/body-care/` | Browse body products | Link to products and appropriate guides |
| Lip care | `/lip-care/` | Browse lip-care products | Link from relevant care categories and products |
| Beauty accessories | `/beauty-accessories/` | Non-formula tools/accessories | Keep separate from skincare formulations; link to relevant use guides |
| Brand page | `/brands/{brand}/` | Browse a brand where authorized and useful | Link to all in-stock brand products; create only with sufficient unique value and permission |
| Product detail | `/products/{product-slug}/` | Evaluate and buy a specific product | Category breadcrumbs, related products, brand, accurate attributes, FAQs if supported |
| Guides hub | `/guides/` | Find educational resources | Organize reviewed evergreen guides and connect them contextually to categories/products |
| Guide article | `/guides/{topic}/` | Answer informational questions | Link to relevant categories without making medical claims or forcing sales links |
| About | `/about/` | Explain actual company and operating model | Trust and entity context; publish only verified facts |
| Contact | `/contact/` | Reach support | Clear support route; link from policies and footer |
| Shipping | `/shipping/` | Explain coverage, charges, times, tracking | Reduce uncertainty; link near checkout and product pages |
| Returns | `/returns/` | Explain eligible returns/refunds | State actual terms and local legal review; link in footer and checkout |
| Privacy | `/privacy/` | Explain data practices | Must reflect actual tracking and data handling; legal review |

## URL and indexation principles
Use lowercase, stable, readable paths; one canonical URL per product; breadcrumbs; pagination appropriate to platform; and controlled faceting. Keep cart, checkout, account, internal search results, and low-value filter URLs out of indexation where appropriate. Use redirects for retired URLs and preserve relevant equity. Final rules depend on platform and crawl testing.

## Language strategy
Support English and Urdu only if the business can provide high-quality translated content and customer support. Use distinct language URLs and correct language annotations when offering true translated equivalents. Validate English, Urdu-script, and Roman Urdu query behavior in Module 03; do not machine-translate sensitive product guidance without review.
