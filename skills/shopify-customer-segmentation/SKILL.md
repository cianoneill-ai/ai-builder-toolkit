---
name: shopify-customer-segmentation
description: Build behavioral customer segments from Shopify data for retention and re-engagement
---

# Customer Segmentation

When the user asks for a customer segment, use the connected Shopify MCP to:

## 1. Parse the segment definition
Confirm with the user:
- Time window (last 30 / 60 / 90 / 365 days)
- Order behavior (1 order, 2+ orders, lapsed, never bought)
- Product / collection filter
- Channel filter (acquired via Meta, Google, organic, etc.)
- Email engagement filter (opened welcome flow Y/N, if Klaviyo connected)

## 2. Query Shopify
- Pull customers matching filters
- For each: email, first/last order date, order count, total spent, top product, tags

## 3. Score recency + value
For each customer:
- Recency score (days since last order)
- Frequency score (order count percentile)
- Monetary score (LTV percentile)
- RFM segment (Champion, Loyal, At Risk, Hibernating, Lost)

## 4. Suggested campaign
Based on the segment:
- Lapsed VIPs → re-engagement with comeback discount
- Repeat buyers who skipped welcome → backfill the welcome series
- One-time buyers in 30-60 day window → second-purchase nudge with cross-sell

## 5. Output
- Segment size + estimated revenue opportunity
- CSV with: email, first_name, tag, RFM segment, suggested offer
- 3 subject-line variants for the campaign
- Klaviyo / Shopify Email import steps

Always exclude unsubscribed customers.
