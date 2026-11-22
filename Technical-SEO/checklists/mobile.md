# Checklist: Mobile Experience

Review important page types on a narrow viewport and confirm that mobile users and search crawlers can access the same essential content and resources.

- [ ] Viewport metadata is configured so pages render at the device width
- [ ] Primary content, metadata, and structured data are available in the mobile-rendered page
- [ ] Important images, CSS, and JavaScript resources are not blocked from crawling
- [ ] Text is readable without horizontal scrolling or forced zoom
- [ ] Navigation, forms, and primary actions are usable with touch and keyboard input
- [ ] Tap targets are adequately sized and spaced for the interaction
- [ ] No page content or key action is obscured by intrusive overlays
- [ ] No unintended horizontal overflow appears at common narrow widths
- [ ] Mobile performance is reviewed with both field data (when available) and repeatable lab tests
- [ ] Responsive templates are checked across representative browsers and page types

Google retired the [Mobile-Friendly Test and Search Console Mobile Usability report](https://developers.google.com/search/blog/2023/04/page-experience-in-search) in December 2023. Use current browser inspection, URL Inspection rendering where available, and performance or accessibility tools instead of relying on the retired test.

**Related fix guides:** `fixes/mobile/`
