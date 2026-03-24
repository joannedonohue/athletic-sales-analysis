# Athletic Sales Analysis

US athletic retail sales analysis (2020–2021) by region, retailer, and product category — built with pandas to surface top-performing markets and women's footwear trends.

---

## Overview

This project analyzes two years of US athletic retail sales data to answer commercial questions about regional performance, retailer revenue rankings, and women's athletic footwear demand patterns. The analysis uses multi-level groupby aggregations, pivot tables, and time series resampling to identify actionable insights for pricing and promotional planning.

---

## Business Questions Addressed

1. Which US regions sold the most athletic products by units and revenue?
2. Which retailers generated the highest total sales across 2020–2021?
3. Which retailers sold the most women's athletic footwear — by day and by week?

---

## Key Findings

| Insight | Finding |
|---|---|
| Top region by units | **Northeast** |
| Top retailer by revenue | **West Gear** |
| Women's footwear demand | Strong **Q3 concentration** (varies by region) |

---

## Methodology

1. Load and combine two yearly CSV files with schema validation
2. Convert `invoice_date` to datetime format for resampling
3. Apply multi-level `groupby` on region, state, and city dimensions
4. Build pivot tables for retailer × region aggregations
5. Filter to women's athletic footwear; resample to daily and weekly totals
6. Rank retailers by women's footwear volume across both time windows

---

## Tech Stack

| Component | Tool |
|---|---|
| Data analysis | pandas |
| Time series handling | pandas datetime / resample |
| Aggregation | groupby, pivot_table |
| Notebook environment | Jupyter |
| Language | Python |

---

## Repository Structure

```
athletic-sales-analysis/
├── athletic_sales_analysis.ipynb    # Full analysis notebook
├── athletic_sales_2020.csv          # 2020 sales data
├── athletic_sales_2021.csv          # 2021 sales data
└── README.md
```

---

## Outcomes

- Identified the **Northeast** as the highest-volume region by units sold and **West Gear** as the top revenue retailer across the two-year period
- Surfaced **Q3 as the peak demand window** for women's athletic footwear with regional variation
- Built a flexible pandas pipeline combining multi-year datasets, pivot tables, and time-based resampling
- Produced retailer-level rankings that can directly inform promotional budget allocation and inventory planning

---

## Getting Started

```bash
pip install pandas jupyter
jupyter notebook athletic_sales_analysis.ipynb
```
