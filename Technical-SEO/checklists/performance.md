# Checklist: Performance / Core Web Vitals

Use field data to understand the experience of real users and lab data to diagnose repeatable issues. They measure different conditions and should be labeled separately in findings.

- [ ] Review field Core Web Vitals when available, segmented by mobile and desktop
- [ ] Evaluate LCP, INP, and CLS at the 75th percentile; use current published thresholds
- [ ] Record the source, date range, URL/origin scope, and device type for each field metric
- [ ] If field data is unavailable or insufficient, state that clearly and use lab tests as diagnostic evidence—not as a field score
- [ ] Run repeatable lab checks on representative high-value templates and record test conditions
- [ ] Identify the largest contentful element and check its response time, priority, and delivery path
- [ ] Check image dimensions, responsive sizing, compression, and modern formats where supported
- [ ] Check that below-the-fold media is deferred appropriately and above-the-fold content is not delayed by lazy loading
- [ ] Inspect render-blocking CSS/JavaScript, unused code, and third-party scripts for measurable impact
- [ ] Review font loading, caching, CDN delivery, and server response time as diagnostic factors
- [ ] Reserve space for images, embeds, ads, and other content that loads asynchronously
- [ ] Retest after changes under comparable conditions and record the before/after evidence

Core Web Vitals guidance: [web.dev — Web Vitals](https://web.dev/articles/vitals) and [Google's threshold methodology](https://web.dev/articles/defining-core-web-vitals-thresholds).

**Related fix guides:** `fixes/performance/`
