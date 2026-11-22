# SEO Alert and Issue Detection Framework

No TechFind alerts are configured and no actual incidents are reported. Thresholds below are proposed starting points; calibrate after a reliable baseline and route alerts to named owners.

| Alert | Detection | Severity | Investigation and response |
|---|---|---|---|
| Organic clicks/sessions suddenly fall | GSC and GA4 weekly/daily anomaly review; compare same weekdays and complete date windows | High; Critical if major landing/checkout pages are affected | Check GSC clicks vs GA4 sessions to distinguish demand from tracking; segment query/page/device/country; inspect indexing, status, inventory, deployment, seasonality and SERP changes. Escalate confirmed site outage/indexability regression. |
| Important URLs become excluded/noindexed | GSC Pages trend, URL Inspection, crawl on release | Critical for key category/product templates | Inspect robots, meta/X-Robots, canonical, server response, render and template release. Correct only after confirming intended indexing; verify with live test and GSC. |
| Sitemap fetch/error spike | GSC sitemap report or scheduled fetch | High | Validate syntax, host, response, canonical/indexable URL set and server; restore valid sitemap and monitor processing. |
| Website downtime / TLS error | Uptime/SSL monitoring | Critical | Verify externally, notify engineering/hosting, check DNS/CDN/certificate and checkout. Record start/end and affected templates. |
| Broken important URL / 5xx surge | Scheduled crawler and server logs | High/Critical depending on commerce impact | Verify response, source links, deployment and backend dependency; restore page or redirect to closest equivalent if permanently moved. Test links and status after fix. |
| CWV field status deteriorates | PSI/CrUX monthly or post-release; Lighthouse lab for diagnosis | Medium/High when broad templates affected | Separate field and lab data; identify affected template/device; profile main image, scripts, layout shifts and server response; verify with same measurement conditions. |
| Structured data errors increase | Rich Results/Search Console enhancements where available; validation on release | Medium | Compare markup to visible page facts; correct eligible fields; do not add ratings/prices/availability that are false. |
| Ranking/query decline | GSC query/page trend and rank tracker with fixed settings | Medium/High if important commercial cluster | Verify same query/location/device and matching period; inspect cannibalization, content, stock, intent, internal links and SERP changes. Do not react to one fluctuating rank. |
| Tracking events stop or duplicate | GA4 DebugView/Realtime, Tag Assistant, backend reconciliation | Critical for purchase event integrity | Test event path and consent conditions; check tag release, transaction ID, currency, duplicate firing and backend orders. Annotate data gap. |
| Unexpected backlink spike/loss | GSC Links/provider snapshots plus manual source-page review | Low until substantiated; elevate for clear manipulation/security issue | Verify links manually and distinguish index coverage changes from live links. Do not disavow from automated toxicity scores alone; investigate actual evidence and current Search Console guidance. |
| Content or product pages disappear | GSC landing page and URL inventory/crawl comparison | High | Check inventory/stock, CMS state, internal links, canonical/indexation, redirects and whether removal is appropriate. Preserve useful pages and alternatives where justified. |

## Alert hygiene

- Use one owner, evidence URL/export, detected time, affected scope, severity, response and verification fields.
- Set anomaly thresholds from a 28-day/seasonal baseline; suppress alerts for incomplete recent data and known maintenance windows.
- Keep GA4 and GSC monitoring independent; divergent changes can reveal tracking issues.
- Close an issue only after a reproducible verification check and a recorded post-fix observation.
