# HTTPS and Redirect Management

## HTTPS/security-related checks
Use a valid TLS certificate and one-hop HTTP-to-HTTPS redirect; normalize host consistently. Inspect rendered pages for mixed-content requests and use HTTPS third-party assets. Consider basic security headers with developer/security review (e.g., HSTS after confirming HTTPS readiness, Content-Security-Policy, X-Content-Type-Options, Referrer-Policy); test for compatibility. This is not penetration testing or a security audit.

## Status code guidance
- 200: successful canonical content.
- 301: permanent move/normalization; direct to closest relevant destination.
- 302: temporary move; retain original URL as intended canonical when appropriate.
- 404: missing page without a useful replacement.
- 410: intentionally and permanently removed page where appropriate.
- 500: server failure; investigate promptly.
- 503: temporary maintenance/outage; include Retry-After when appropriate and restore quickly.

For removed products, redirect only to a genuinely close replacement/category when helpful; otherwise return 404/410. Do not redirect all deleted products to the homepage. Keep redirects single-hop and update internal links/sitemaps to final URLs. Maintain a redirect map and verify status/location after release.

## Regional/language SEO
Target Pakistan through country-relevant content, PKR where actual, and clear delivery policies. Start in English as the documented project language. Add Urdu pages only if a real reviewed translation and support experience exists. Use hreflang only for genuine equivalent language/region variants with reciprocal valid URLs and self-reference; do not use hreflang as a country-targeting shortcut. No separate country code domain or city pages are justified by current inputs.
