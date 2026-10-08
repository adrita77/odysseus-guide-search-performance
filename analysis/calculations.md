# Reproducing the Odysseus guide's search-performance results

## Source and filters

- Source: author's original Google Search Console CSV export.
- Search type: **Web** (`../data/Filters.csv`).
- Reporting period: **June 2–8, 2026** (`../data/Filters.csv`).
- Target: exact guide URL in `../data/Pages.csv`: [PewDiePie AI Tool: How to Install PewDiePie Odysseus?](https://miraiyo.com/pewdiepie-ai-tool-how-to-install-pewdiepie-odysseus/).

## Article-specific CTR: step by step

From the exact matching row in [`../data/Pages.csv`](../data/Pages.csv):

| Input | Value |
|---|---:|
| Clicks | **3,324** |
| Impressions | **190,767** |

**Step 1:** Write the standard click-through-rate formula.

`CTR (%) = (Clicks / Impressions) × 100`

**Step 2:** Substitute the observed article-level values.

`CTR (%) = (3,324 / 190,767) × 100`

**Step 3:** Round the result to two decimal places.

**CTR = 1.74%**

This agrees with the **1.74%** shown in the article row of `Pages.csv`.

## Daily data in Chart.csv — broader site view, not this article

[`../data/Chart.csv`](../data/Chart.csv) contains daily rows for the Search Console view whose recorded filters are **Web** and **June 2–8, 2026**. The filter export does **not** include an article URL filter. The daily rows therefore must **not** be labeled as the article's individual daily performance.

| Date | Clicks | Impressions |
|---|---:|---:|
| June 2, 2026 | 82 | 6,418 |
| June 3, 2026 | 765 | 39,085 |
| June 4, 2026 | **1,243** | **62,702** |
| June 5, 2026 | 815 | 41,706 |
| June 6, 2026 | 225 | 18,838 |
| June 7, 2026 | 114 | 13,273 |
| June 8, 2026 | 111 | 11,787 |
| **Daily-series total** | **3,355** | **193,809** |

The sum of daily clicks is:

`82 + 765 + 1,243 + 815 + 225 + 114 + 111 = 3,355`

The sum of daily impressions is:

`6,418 + 39,085 + 62,702 + 41,706 + 18,838 + 13,273 + 11,787 = 193,809`

**Highest day in the overall daily export:** June 4, 2026, with **1,243 clicks** and **62,702 impressions**. Both metrics peak on this date in the exported daily rows.

**Scope warning:** These daily totals are different from the article-specific **3,324 clicks** and **190,767 impressions** in `Pages.csv`. We cannot identify the article's highest individual day from these exports alone. Article-filtered daily export: **[FILL IN]**.

## Limitations

The export supports the article's measured visibility and calculated CTR. It does **not** establish that publication speed, writing structure, an FAQ, or any other single change caused those results. No installation completions, conversion rate, or comparable before-and-after test data were provided: **[FILL IN]** if available.

**Data exported from Google Search Console by the author. Shared with permission of Miraiyo.**