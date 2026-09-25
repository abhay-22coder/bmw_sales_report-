# 🚗 BMW Global Sales Dashboard (2018–2025)
![preview image](/<img <img width="1075" height="601" alt="Screenshot 2026-09-25 at 11 32 50 AM" src="https://github.com/user-attachments/assets/b49c5bb4-fca1-4648-8d67-43a69dc2626f" />
/>
)

## Overview

This dashboard tracks BMW's global sales across 8 models and 4 regions over an 8-year period, giving a full picture of revenue trends, seasonal patterns, and market mix.

## Data Source

- **File:** `bmw_global_sales_2018_2025.csv`
- **Records:** 3,072 rows
- **Period:** 2018–2025 (monthly granularity)
- **Regions:** Europe, China, USA, RestOfWorld
- **Models:** 3 Series, 5 Series, X3, X5, X7, i4, iX, MINI

### Columns

| Column | Description |
|---|---|
| `Year`, `Month` | Time period of the record |
| `Region` | Sales region |
| `Model` | BMW model line |
| `Units_Sold` | Vehicles sold |
| `Avg_Price_EUR` | Average selling price |
| `Revenue_EUR` | Total revenue for that row |
| `BEV_Share` | Share of battery-electric vehicles |
| `Premium_Share` | Share of premium trim/configuration |
| `GDP_Growth` | Macroeconomic GDP growth (%) for the period |
| `Fuel_Price_Index` | Fuel price index for the period |

## Dashboard Sections

1. **KPI Cards** — Total Revenue (€2T), Total Units Sold (25M), Average Order Value (€64.08K), Avg. Premium Share, Avg. GDP Growth, Avg. Fuel Price Index
2. **Month Wise Revenue And Units Sold** — Combo chart (bars + line) showing revenue and units sold by month, sorted chronologically (Jan–Dec). Reveals a clear quarter-end sales spike pattern (Mar, Jun, Sep, Dec).
3. **Units Sold by Model** — Horizontal bar chart ranking all 8 models by total units sold.
4. **Units Sold by Region** — Pie chart showing the near-even 25/25/25/26% split across Europe, China, USA, and RestOfWorld.
5. **Year over Year Sales Analysis** — YoY % revenue growth by year (2019–2025).
6. **Sum of Revenue_EUR by Year** — Annual revenue trend, 2018–2025.

## Filters

- **Years**, **Month**, **Quarter**, **Model Name** — all cross-filter the entire dashboard.
- **Clean** button resets all filters to default (All).

## Design System

| Element | Color | Hex |
|---|---|---|
| Background | Dark navy | `#0F1420` |
| Card background | Lighter navy | `#1A2030` |
| Primary data (bars, revenue) | BMW blue | `#1C69D4` |
| Secondary data (units sold line) | Silver-grey | `#C4C9D4` |
| Alerts / negative trend | Coral red | `#E8544D` |
| Primary text | White | `#FFFFFF` |
| Secondary/axis labels | Muted grey-blue | `#8A93A6` |

**Region donut/pie gradient** (darkest = highest share):

| Region | Hex | Share |
|---|---|---|
| China | `#1C69D4` | 26% |
| Europe | `#4B8FE8` | 25% |
| RestOfWorld | `#7FADEE` | 25% |
| USA | `#B3CEF5` | 25% |

## Key Insights

- **Revenue grew steadily** from €177bn (2018) to €216bn (2025), with a notable +10.8% YoY jump in 2020.
- **Seasonal pattern:** revenue and units sold both spike at quarter-end months (March, June, September, December) — a recurring dealer/sales-push cycle.
- **Model mix drives revenue, not volume:** units sold per model are nearly flat (~3.0–3.1M each), but revenue varies widely — the X7 generates ~2.3x the revenue of the MINI on similar volume, reflecting price positioning (X7 avg. price ~€92K vs. MINI ~€42K).
- **Regional split is balanced:** no single region dominates; China leads narrowly at 26%.

## Changelog

- Fixed month-wise chart sort order (was sorted by value, now chronological Jan–Dec)
- Replaced dual-axis line/bar model chart with a cleaner horizontal bar ranking
- Applied consistent BMW-blue color system across all visuals
- Recolored region pie/donut chart to a blue gradient for brand consistency
- Renamed KPI card labels and chart series to remove raw field names (e.g., "Sum of Revenue_EUR" → "Total Revenue")
- Added/verified legend on the month-wise combo chart
- Restored full year labels (2019–2025) on the YoY chart

## Tools

- **Power BI** — dashboard build and visuals
## 👨‍💻 Author
**Abhay Maurya**

- Power BI Enthusiast
- Learning Data Analytics, SQL, Excel, and DAX
