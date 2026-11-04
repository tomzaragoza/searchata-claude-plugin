---
name: performance
description: Analyze or compare a site's Google or Bing search performance using Searchata, including traffic changes and query or page trends.
---

# Analyze search performance

Use the relevant Searchata tools available in this session. Reuse a known canonical property ID; otherwise list Google properties or Bing sites. Match the requested site and source before fetching reports.

For Google comparisons, prefer `google_search_console_compare_performance`. Use equal completed periods and consistent search type, device, and country filters. If dates are unspecified, use 28 reporting days ending three days before today and the preceding 28 days. State the exact dates and reporting timezone. Respect any source freshness warning.

Read aggregate totals separately from query and page detail. Search Console can omit query rows. Row sums can differ from totals. Missing rows do not establish zero traffic. If a baseline is zero, report the absolute change without a percentage increase. Keep Bing and Google totals separate.

Inspect the largest relevant page and query changes. Distinguish measured change from a proposed explanation. Include clicks, impressions, click-through rate, and average position where available. Explain position as an average, not a fixed rank. End with supported findings, data limits, and useful next checks. Analysis alone does not authorize a crawl, website edit, or scheduled task.
