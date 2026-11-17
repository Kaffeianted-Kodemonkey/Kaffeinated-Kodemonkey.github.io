# Website baseline — November 17, 2026

Status: initial source review and supplied Search Console analysis. This is not a completed accessibility evaluation or conformance statement.

## Evidence

Repository: Kaffeianted-Kodemonkey/Kaffeinated-Kodemonkey.github.io, reviewed commit `50b17deb4adbb0ea3a2885314584e7cfcc3f937a`.

Search Console sources supplied by Heather: Performance-on-Search-2026-11-17.xlsx (Chart, Queries, Pages, Countries, Devices, Filters) and Coverage-2026-11-17.xlsx (Chart, Critical issues, Metadata). Raw exports remain outside the public repository.

Performance filter: Web (text-based), Last 3 months. Daily rows cover August 16–November 15, 2026. Summing daily clicks/impressions gives 4 clicks / 2,460 impressions; CTR = 4 / 2,460 = 0.163%. This is Google organic search for the supplied URL-prefix property, not all traffic or all hostname variants. The export does not establish inquiries, sales, conversion rate, or causes of lost business. Query rows omit some search activity and must not substitute for chart totals.

| Evidence | Implication and task |
| --- | --- |
| `wcag audit`: 422 impressions, 0 clicks, average position 52.09 | Relevant commercial demand reaches the site, but ranking is weak. Strengthen service clarity, relevant internal links and evidence; do not expect a title change alone to resolve this. |
| Audit-versus-scan guide: 909 impressions, 0 clicks, position 46.59 | First existing guide to improve and connect to a clearly scoped manual audit offer. Preserve its published URL until a URL inventory establishes destinations. |
| Audit service `/services/web_accessibility_audits/`: 54 impressions, 0 clicks, position 65.63 | Improve the buying page alongside the guide; confirm packages and pricing with Heather. |
| `/MonkeyHub/`: 372 impressions, 1 click, position 8.37; `monkeyhub` query: 181 impressions, 0 clicks | Relatively strong position for a hub term does not establish qualified buyer demand. Inspect historical uppercase/lowercase paths. |
| Homepage: 109 impressions, 0 clicks, position 5.8 | Low volume and unknown query mix prevent a reliable conversion or broad ranking conclusion. Inspect page-filtered queries before prescribing a snippet fix. |
| United States: 1 click, 1,160 impressions | Target-market discovery is very limited; do not infer a conversion problem from four global clicks. |

Latest coverage snapshot, November 12: 38 indexed and 33 not indexed. An early populated snapshot, August 20, showed 15 indexed and 22 not indexed. Indexing increased; the export does not identify which individual URLs changed status.

| Coverage reason | Count | Treatment |
| --- | ---: | --- |
| Not found (404), validation Failed | 12 | Export the reason-specific affected URL list, map each to current content, fix internal references and redirect only when a relevant replacement exists. Intentional removals may remain 404. |
| Page with redirect | 2 | Verify expected destination and internal/sitemap links; not automatically a defect. |
| Alternate page with proper canonical | 2 | Verify canonical intent; not automatically a defect. |
| Crawled — currently not indexed | 9 | Inspect affected URLs, canonical selection, duplication, relevance and internal links. No root cause established yet. |
| Discovered — currently not indexed | 8 | Inspect affected URLs and crawl/indexing evidence before remediation. |

The supplied coverage workbook contains reason counts, not affected URL lists. Those lists are needed to resolve individual indexing issues.

## Accessibility source observations

| ID | Evidence | Status / next verification |
| --- | --- | --- |
| A01 | `_includes/header.html` links to `#main-content`; `_layouts/homepage-template.html` places hero/H1 and expertise content before that main landmark. | Confirmed structural concern: the skip target bypasses primary introductory content. Review reading order and landmark placement in the rendered homepage; assess WCAG 1.3.1 and 2.4.1 before assigning a failure. |
| A02 | `_includes/contact-form.html` has no autocomplete tokens for first name, last name, email or phone. | Source finding associated with 1.3.5: add purpose tokens and verify the rendered form. |
| A03 | Phone is required and accepts only `123-456-7890` through a pattern. | Confirmed usability/conversion friction; do not equate a required phone field alone with a WCAG failure. Make optional per approved inquiry design; verify instructions, validation and error recovery (3.3.1/3.3.2). |
| A04 | Navigation toggle is a native button with an accessible name, controls and expanded state; styles include focus-visible rules. | Existing positives. Keyboard, expanded-state synchronization, hidden-link focus, close behavior and narrow viewport behavior remain untested. |
| A05 | Shared layouts declare English, use main landmarks, and the form has explicit labels. | Existing positives from source only. Contrast, accessible names in rendered context and screen-reader navigation remain unverified. |
| A06 | Hero infographic alternative describes its topic and selected claims; an equivalent for all meaningful graphic information was not established in this inspection. | Review actual graphic and adjacent equivalent text before assessing 1.1.1. Do not invent a failure from alt length. |

## Audit completion scope

Sample homepage, About, each service page, MonkeyHub, Learning Center landing page, one standalone guide, one series post, contact flow, accessibility statement and 404. Exercise shared header, mobile menu, sidebar, footer, accordions and third-party booking/form handoffs. Verify content variants discovered during inventory.

For each test record URL, commit/build, date, browser/OS/assistive-technology versions, viewport, steps, expected/actual behavior, WCAG criterion where applicable, severity, evidence and retest. Test keyboard-only access, focus visibility/obscuration/order, names/roles/states, headings/landmarks, images, contrast, 200% text resize, 320 CSS-pixel reflow, text spacing, target size, forms/errors and applicable WCAG 2.2 AA requirements. Heather completes NVDA/VoiceOver checks unavailable in the execution environment.

Not performed in this baseline: rendered automated scan, browser interaction audit, color measurements, NVDA/VoiceOver evaluation, form delivery or booking verification. Ruby and Bundler are absent in the current execution environment, so a fresh Jekyll build could not run. Tracked `_site/` output is not treated as a fresh build or proof of live behavior.

## Initial priorities

1. Establish GitHub tracking and the deployment/build baseline.
2. Obtain reason-specific indexing URL exports; map legacy URLs before redirects.
3. Complete representative accessibility testing and fix confirmed shared barriers.
4. Confirm offers, audience and current prices; improve homepage, service copy and inquiry flow in small batches.
5. Improve the existing audit-versus-scan guide and add verified client evidence with permission.
6. Measure search visibility monthly alongside qualified inquiries and outcomes in vtiger. Compare matched periods, label small samples and avoid ranking/client guarantees.
