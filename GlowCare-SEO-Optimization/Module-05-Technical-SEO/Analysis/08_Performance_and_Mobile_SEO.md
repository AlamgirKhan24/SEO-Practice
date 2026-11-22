# Performance and Mobile SEO Plan

No live URL exists; no PageSpeed Insights, Lighthouse, Chrome UX Report, or Core Web Vitals measurements were run. Do not treat proposed thresholds as observed results.

## Measurement
For representative homepage, category, product, and guide templates: use PSI for lab diagnostics and available field data; use Lighthouse/DevTools for repeatable lab runs; use Search Console CWV and CrUX for field outcomes where data exists. Field data reflects real users and may be absent for a new/low-traffic page. Keep lab and field evidence separate.

Google’s “good” CWV targets at the 75th percentile: LCP ≤2.5s, INP <200ms, CLS <0.1. [Google CWV](https://developers.google.com/search/docs/appearance/core-web-vitals) · [PSI](https://developers.google.com/speed/docs/insights/v5/about)

## LCP
Prioritize the actual largest content element; reduce server response time; avoid lazy-loading the likely LCP hero image; compress and correctly size it; preload only when justified; remove render-blocking CSS/JS; cache and use CDN close to Pakistani users where economics permit.

## INP
Profile real interactions including menu, search, variant selection, filters, add-to-cart and checkout. Split/defer non-critical scripts, reduce long main-thread tasks, limit third-party tags, and keep event handlers responsive.

## CLS
Set width/height or aspect ratios for images/video; reserve space for banners, reviews and recommendations; avoid late-injected content above existing content; use stable font loading and fallback metrics.

## General
Serve responsive AVIF/WebP with fallback, compress assets, minify and remove unused CSS/JS safely, cache static assets, optimize fonts/subsets, and lazy-load below-the-fold media. Verify visual parity and purchase functionality after each change. No scores or current performance issues are known.

## Mobile checklist
Responsive viewport/layout; mobile content parity; touch-friendly controls; readable type and contrast; menu/search usable with keyboard/touch; image sizing; sticky elements not covering content; product variant and stock clarity; cart/checkout usability; field CWV by template; test on representative Android/iOS devices and slow network emulation.
