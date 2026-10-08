# Google Search Console data dictionary

This folder contains the **original CSV exports supplied by the author** for the Google Search Console performance view. The files have been copied without editing their values.

## Export filters and interpretation

[`Filters.csv`](Filters.csv) records:

| Filter | Exported value |
|---|---|
| Search type | Web |
| Date | Jun 2, 2026–Jun 8, 2026 |

**Use `Pages.csv` for the article's results.** Its row matching the [Odysseus guide URL](https://miraiyo.com/pewdiepie-ai-tool-how-to-install-pewdiepie-odysseus/) records **3,324 clicks**, **190,767 impressions**, and **1.74% CTR**. The daily rows in `Chart.csv` belong to the broader Search Console view and must not be presented as an article-level daily series.

## Column definitions

The following meanings apply to the column names present in these exports:

| Column | Meaning |
|---|---|
| **Date** | Calendar date associated with a daily performance row. |
| **Top pages** | URL for a page in the exported page report. |
| **Top queries** | Search query as represented in the query export. |
| **Country** | Country listed for that report row. |
| **Device** | Device category listed for that report row. |
| **Search Appearance** | Search-appearance category listed for that report row. |
| **Filter** | Name of an applied export setting. |
| **Value** | Value of that setting. |
| **Clicks** | Clicks attributed to the row in the exported Search Console report. |
| **Impressions** | Impressions attributed to the row in the exported report. |
| **CTR** | Exported click-through rate, shown as a percentage; calculated as clicks divided by impressions × 100. |
| **Position** | Average position metric reported by Search Console for the row; not a guaranteed fixed ranking. |

## Files and their exact column order

| File | Column order | Scope and intended use |
|---|---|---|
| [`Pages.csv`](Pages.csv) | `Top pages`, `Clicks`, `Impressions`, `CTR`, `Position` | **Primary evidence for the guide:** choose the row with the exact article URL. |
| [`Filters.csv`](Filters.csv) | `Filter`, `Value` | Confirm search type and reporting window. |
| [`Chart.csv`](Chart.csv) | `Date`, `Clicks`, `Impressions`, `CTR`, `Position` | Daily totals for the broader exported view, **not the article's daily totals**. |
| [`Queries.csv`](Queries.csv) | `Top queries`, `Clicks`, `Impressions`, `CTR`, `Position` | Query breakdown as exported; do not assume the rows add up to the complete article's totals. |
| [`Countries.csv`](Countries.csv) | `Country`, `Clicks`, `Impressions`, `CTR`, `Position` | Country breakdown for the exported view. |
| [`Devices.csv`](Devices.csv) | `Device`, `Clicks`, `Impressions`, `CTR`, `Position` | Device breakdown for the exported view. |
| [`Search appearance.csv`](Search%20appearance.csv) | `Search Appearance`, `Clicks`, `Impressions`, `CTR`, `Position` | Search-appearance breakdown as exported. |

## Important reading notes

- The screenshot displays rounded **overall performance** cards and a **specific page row**. Those are different scopes. The primary article figures come from the exact URL in `Pages.csv`.
- `Chart.csv` gives **3,355 clicks** and **193,809 impressions** when its daily rows are summed. Those are **not** the article's **3,324 clicks** and **190,767 impressions**.
- The query, page, and other breakdown exports should not be treated as interchangeable sums or as evidence of article-specific daily performance.
- If an exact writing time, publication workflow, detailed test results, or per-day page metric is needed, it must be supplied separately: **[FILL IN]**.

**Data exported from Google Search Console by the author. Shared with permission of Miraiyo.**