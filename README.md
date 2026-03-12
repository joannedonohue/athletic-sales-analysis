# Athletic Sales Analysis

Retail sales analysis across US athletic stores for 2020-2021 — identifying top-performing regions, retailers, and product categories using pandas groupby operations, pivot tables, and time series resampling.

## Overview

This analysis answers key commercial questions for an athletic goods business: which retailers drive the most volume, where is women's footwear growing fastest, and how does weekly sales performance vary by region? The findings support regional pricing, assortment, and promotional planning.

## Key Questions Answered

- Which US regions sold the most athletic products by unit volume and revenue?
- Which retailers generated the highest total sales across the two-year period?
- Which retailers sold the most women's athletic footwear — by day and by week?

## Methodology

1. **Data loading & inspection**: Combined two yearly CSVs; validated schema consistency
2. **Date conversion**: Parsed invoice_date to datetime and set as index for resampling
3. **Regional analysis**: Multi-level groupby on region/state/city, sorted by units and revenue
4. **Retailer analysis**: Pivot table aggregations for sales by retailer x region
5. **Footwear deep dive**: Filtered to women's athletic footwear; resampled to daily and weekly totals

## Sample Findings

- Top region by units sold: **Northeast**
- Top retailer by total revenue: **West Gear**
- Women's footwear peak week: varied by region, with strong Q3 concentration

## Stack

Python | pandas | Jupyter Notebook

## Usage

Run: pip install pandas jupyter
Then: jupyter notebook athletic_sales_analysis.ipynb
