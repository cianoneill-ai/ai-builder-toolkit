---
name: shopify-ltv-cohort-view
description: Compute 30/60/90-day LTV by Shopify acquisition channel, ranked by margin and LTV/CAC
---

# LTV + Cohort View

When the user asks for LTV analysis, use Shopify + GA4 + ad MCPs to:

## 1. Define cohorts
Group customers by first-order month (last 6 months). For each cohort:
- Size
- Primary acquisition channel (first-touch from UTM)

## 2. Compute LTV curves
For each cohort × channel:
- LTV at 30, 60, 90 days
- Repeat purchase rate
- Avg order value
- Margin per order (use product cost metafield if present, else gross margin estimate)

## 3. Pull CAC
For each channel:
- Total ad spend last 6 months
- Customers acquired
- CAC = spend / customers

## 4. Rank channels
For each channel, compute:
- 90-day margin-adjusted LTV
- LTV / CAC ratio
- Payback period (days to recover CAC)

## 5. Output
- Cohort LTV chart (rows = cohort month, cols = days since acquisition)
- Channel ranking table sorted by margin-adjusted LTV/CAC
- 3 recommended budget shifts based on the data
- Flag channels with LTV/CAC <1.5 (unprofitable)

Always show margin LTV, not just revenue LTV — revenue lies on heavy-discount channels.
