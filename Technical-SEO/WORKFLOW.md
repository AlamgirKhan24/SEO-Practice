# Technical SEO Workflow

A repeatable process for producing an evidence-based technical SEO review, a prioritized action plan, and a clear record of verified fixes. It supports both live website checks and analysis of supplied data.

## Step 0 — Confirm the audit approach

Agree on the review scope, available data, and whether the audit will use live checks, supplied exports, or both. Confirm the approach for each new audit rather than assuming access to private accounts or paid tools.

- **Live review:** Use available crawlers, browser checks, performance tools, and public endpoints. Check private dashboards or CMS accounts only when access is available and authorized.
- **Supplied data:** Analyze the exports and reports provided, such as crawler exports, Search Console data, PageSpeed Insights results, or robots.txt and sitemap files.
- **Combined review:** Bring supplied data together with live checks where useful.

Record the tools, data sources, date, scope, and access limitations in the findings. Distinguish verified observations from estimates, sampled checks, and items that could not be assessed. Never infer private dashboard metrics from crawl data.

## Step 1 — Scope the audit

Decide (or ask) what's being audited:
- Whole site or specific section/pages?
- Which categories matter most right now? (see `checklists/`)

## Step 2 — Run the audit

Go through the relevant checklist(s) in `checklists/` and record findings.

Choose representative URLs and page templates; state how they were selected and how many were reviewed. For larger sites, group findings by template or issue pattern and identify the sample behind each conclusion. Record the URL, status, evidence source, collection date, and affected scope. Reproduce high-impact findings where practical, and label unverified hypotheses clearly.

## Step 3 — Create the audit folder

Create `audits/{site-name}-{YYYY-MM-DD}/` containing:
- `findings.md` — raw list of everything found (use `templates/audit-report-template.md`)
- `issue-tracker.md` — prioritized list (use `templates/issue-tracker-template.md`)

## Step 3b — Build the designed HTML report (always, not optional)

Every completed audit includes a self-contained HTML report in its folder as `report.html`, alongside the findings and issue tracker. The HTML file is portable and can be reviewed locally or shared through an approved channel.

Start from `templates/report-template.html` — it has the full design system (light/dark
theming, severity color-coding, stat tiles, finding cards, per-finding step-by-step fix
blocks) already built. Read the template notes first. Replace all site-specific placeholder content and data, then verify the final report against the audit evidence before delivery.

The report must include, for every finding, a **"How to fix it, step by step"** block: numbered
steps written for that specific site (name the actual CMS, plugins, and admin screens where
known), a code snippet where one applies, and a one-line "Done when" verification. Pull the
steps from the matching guide in `fixes/` and tailor them — don't paste the generic guide.

The template's stat cards include a real score bar (width = the actual 0-100 Lighthouse score)
and, for Core Web Vitals, a qualitative label set from Google's real published thresholds only
(e.g. LCP good <2.5s/needs work <4s/poor ≥4s) — never a guess. The findings-by-category chart
stacks each category's real findings by severity, from that audit's own counts — omit categories
with zero findings rather than padding the chart. Both are genuine data visualizations, not
decoration — never fabricate a number or trend to fill them in.

Then log the report in the audit's `CHANGELOG.md`. Complete `checklists/audit-quality.md` before handoff and reconcile figures, findings, and priorities across the report and tracker.

## Step 4 — Prioritize

Rank each issue by severity, reach, business importance, effort, and dependencies. Document the reasoning so a stakeholder can distinguish confirmed risk from an estimate. Use `templates/issue-tracker-template.md` to capture evidence, action, owner, target date, and status. Separate verified defects from optional opportunities.

| Severity | Meaning |
|---|---|
| 🔴 Critical | Blocking indexing/crawling, site broken for search engines |
| 🟠 High | Meaningfully hurting rankings or traffic |
| 🟡 Medium | Best-practice gap, moderate impact |
| 🟢 Low | Minor / cosmetic, nice-to-have |

Also note **effort**, affected templates/URLs, owner, target date, and any implementation dependencies when known. The tracker includes a priority field; use it to account for urgency and business context as well as severity.

Do not treat tool scores as impact estimates or promise ranking/traffic gains. Record a baseline when measuring the outcome of a planned change.

## Step 5 — Fix, using the step-by-step guides

For each issue, find (or create) its guide. Check `fixes/{category}/` for an existing one first
— reuse it as-is **only if it's genuinely site-agnostic** (no real domain, brand, page path, or
drafted copy anywhere in it). Otherwise create/use
`fixes/{category}/{site-domain}--{issue-name}.md`, scoped by site domain: a fix guide almost
always ends up with real specifics baked in (the actual CMS, real code snippets, real drafted
copy), so reusing one written for a *different* site under the same generic issue name hands the
client wrong instructions — wrong domain, wrong brand, wrong example — without anyone noticing.
When unsure whether a guide is generic enough to share, scope it: a duplicated generic guide
costs nothing, a misattributed specific one is a real error in delivered work.

Every fix guide follows the same beginner-friendly format:

1. **What's wrong** — plain-English explanation
2. **Why it matters** — impact on SEO
3. **How to check it yourself** — how to confirm the issue exists
4. **Step-by-step fix** — numbered, exact steps (with code snippets where relevant)
5. **How to verify the fix worked** — how to confirm it's resolved
6. **Tools to double-check** — free tools to re-test

If a guide doesn't exist yet for an issue, create one using `templates/fix-guide-template.md`.

If the issue is a **content problem** (thin content, duplicate/placeholder copy, a weak or
missing meta description, a poor/duplicate title tag, generic body copy), don't stop at telling
the client to "write real copy" — draft the actual replacement text for the real page(s)
affected, grounded in what's already on the live page (real product/location/service details,
the site's existing voice/terminology), using the guide's optional **7. Suggested rewritten
content** section. For a template shared across many pages, give 2-3 worked examples plus the
pattern to repeat, not one generic sample. Carry that drafted copy into the HTML report's fix
card too (a current-vs-suggested block), not just the steps.

## Step 6 — Verify

After fixes are applied, re-check each issue using the "How to verify" section of its guide.
Mark it resolved in `issue-tracker.md`.

## Step 7 — Log it

Update the audit folder's `CHANGELOG.md` (or the root one for repo-wide changes) with:
- Date
- What was fixed
- Who/what verified it

## Suggestions vs. fixes

Not everything is a "broken" issue — some findings are **opportunities** (e.g. "add FAQ schema
to increase rich result chances"). These get logged in `findings.md` too, but tagged
**💡 Suggestion** instead of a severity level, and are optional/lower priority by default.
