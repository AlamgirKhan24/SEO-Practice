# Module 5: Technical SEO

## Project context

- **Practice business:** GlowCare Salon (fictional)
- **Target area:** University Town, Peshawar, Pakistan
- **Site status:** No live website yet. No crawl, speed scores, indexing status, or technical errors have been measured.
- **How to use this module:** Once the demo website is live, run the checks below and enter real findings in the tracker. Do not record a fix unless you have applied and rechecked it.

## What to do

Technical SEO checks whether search engines can access the site and whether the site works well for visitors. Start with the baseline findings from Module 2. Fix issues that affect important pages first, then crawl and measure again.

## Checklist

- [ ] Crawl the live site with Screaming Frog SEO Spider (free crawl limit is currently up to 500 URLs) and save the crawl/export.
- [ ] Review broken internal links and 404 responses. Update links to the right live URL; add a 301 redirect when a removed URL has a clear replacement.
- [ ] Identify redirect chains and loops. Update internal links to the final URL and redirect old URLs directly to the destination.
- [ ] Confirm HTTPS works across the site and HTTP redirects to the preferred HTTPS version.
- [ ] Check key templates on mobile: readable text, usable buttons, no horizontal overflow, and working navigation/forms.
- [ ] Run PageSpeed Insights on the home page and key service pages. Record mobile and desktop performance scores and the Core Web Vitals field data/lab data separately where shown.
- [ ] Address the measured causes of poor LCP, INP, or CLS. Possible actions include resizing/compressing images, reducing unnecessary JavaScript, reserving space for images/embeds, and improving server response. Re-measure after each meaningful change.
- [ ] Generate an XML sitemap, check that it contains canonical URLs intended for indexing, and submit it in Search Console.
- [ ] Review `/robots.txt` to ensure important pages and resources are not blocked. Include the sitemap URL if appropriate.
- [ ] Check that each indexable page has a valid canonical URL and that HTTP/HTTPS and www/non-www versions resolve consistently.
- [ ] Review duplicate titles/content and pages with little useful content. Improve, consolidate, or noindex pages where appropriate.
- [ ] Add accurate structured data only for information shown on the page. A suitable LocalBusiness subtype may be used when the business is real and its details are confirmed. Use Article markup for a qualifying article. FAQ markup does not guarantee a search result feature.
- [ ] Validate structured data with Google's Rich Results Test where the type is eligible, and use Schema.org Validator for general syntax checks.
- [ ] Review Search Console's indexing report and URL Inspection after launch. Request indexing for important updated pages when appropriate; requests do not guarantee indexing.
- [ ] Re-crawl and re-test the pages after fixes. Save dated before-and-after evidence.

## Suggested technical fix tracker

| Issue found | Page URL | Tool used | Fix applied | Date fixed | Recheck result | Status |
| --- | --- | --- | --- | --- | --- | --- |
| N/A — no live site to crawl | — | — | Pending launch | — | — | Not measured |

Add one row per issue. Use clear statuses such as **Open**, **Fixed**, **Monitoring**, or **Not applicable**. Keep the original crawl export to compare against the re-crawl.

## Baseline and after-fix measurements

| Check | Before | After | Date / evidence |
| --- | --- | --- | --- |
| Crawl: broken internal URLs / 4xx pages | N/A — no live site | Pending | Save crawl exports |
| Redirect chains / loops | N/A — no live site | Pending | Save crawl exports |
| HTTPS and preferred hostname | N/A — no live site | Pending | Record final URL behavior |
| Mobile usability observations | N/A — no live site | Pending | Save screenshots/notes |
| PageSpeed mobile score | N/A — no live site | Pending | Test same URLs and conditions |
| PageSpeed desktop score | N/A — no live site | Pending | Test same URLs and conditions |
| Core Web Vitals (LCP / INP / CLS) | N/A — no live site | Pending | Note whether field or lab data |
| Sitemap status | N/A — no live site | Pending | Save Search Console evidence |
| Robots.txt status | N/A — no live site | Pending | Save robots.txt copy or screenshot |
| Canonical checks | N/A — no live site | Pending | Record URLs checked |
| Structured data validation | N/A — no live site | Pending | Save validation result |
| Indexed pages / issues | N/A — no live site | Pending | Save Search Console report |

## Free tools

- Screaming Frog SEO Spider (free crawl limit)
- Google Search Console
- PageSpeed Insights
- Chrome Lighthouse for mobile and desktop checks
- Google Rich Results Test
- Schema.org Validator
- A CMS SEO plugin or a reputable schema generator, if appropriate
- Google Sheets for the tracker

## Final report evidence

- Dated crawl exports and screenshots before and after fixes.
- PageSpeed Insights results for the same URLs, device types, and test dates; note lab versus field data.
- Core Web Vitals before and after, if field data is available. New or low-traffic sites may not have enough field data.
- Search Console sitemap submission/status evidence.
- Structured data validation results and URLs tested.
- Completed issue tracker with fixes, dates, recheck results, and any outstanding issues.
- Notes explaining issues that could not be checked because the site was unavailable or lacked sufficient data.

## Important notes for this case study

GlowCare is a fictional practice business. Do not publish fabricated address, phone number, opening hours, reviews, business credentials, or schema properties. Create technical evidence only after a demo site is live. If real business information is later used, confirm it with the owner first.
