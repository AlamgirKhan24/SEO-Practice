# SEO KPI Dashboard Instructions

The companion CSV is a dashboard layout/data dictionary, not a populated report. No sample numbers are included. After launch, load dated GSC and GA4 exports into separate tabs and calculate from each source independently.

## Suggested Excel formulas

Assuming a `GSC Data` tab with Clicks in column G, Impressions H, CTR I and Average Position J, and rows 2–200:

- Clicks: `=IF(COUNT('GSC Data'!G2:G200)=0,"Not available",SUM('GSC Data'!G2:G200))`
- Impressions: `=IF(COUNT('GSC Data'!H2:H200)=0,"Not available",SUM('GSC Data'!H2:H200))`
- CTR: `=IFERROR(SUM('GSC Data'!G2:G200)/SUM('GSC Data'!H2:H200),"Not available")`
- Weighted average position (approximate using impressions): `=IFERROR(SUMPRODUCT('GSC Data'!J2:J200,'GSC Data'!H2:H200)/SUM('GSC Data'!H2:H200),"Not available")`

For GA4, calculate sessions, users and engaged sessions from their own export. Do not add GSC clicks to GA4 sessions. Build a time-series chart only after dated actual data exists; do not chart invented/sample data. Excel tables with filters are appropriate for query, landing page and action logs. Conditional formatting can flag verified critical statuses after fields are populated.

Current values are unavailable and the XLSX export tool failed in this environment. The CSV does not contain functional formulas, charts, filters, or conditional formatting; use these instructions when converting it to an Excel workbook.
