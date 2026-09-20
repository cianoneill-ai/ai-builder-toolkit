---
name: shopify-refund-pattern-analysis
description: Analyze Shopify refunds by product, reason, and cohort to find SKUs unfit for paid ads
---

# Refund Pattern Analysis

When the user asks to analyze refunds, use the connected Shopify MCP to:

## 1. Pull refund data
Last 90 days:
- Refund ID, order ID, line items, refund amount, refund reason
- Customer ID, first-order date, acquisition channel (UTM source from original order)
- Time between order and refund

## 2. Segment by SKU
For each SKU with 5+ refunds:
- Total units sold
- Refund rate (refunds / units sold)
- Avg refund amount
- Top 3 refund reasons

## 3. Segment by acquisition channel
- Refund rate by source (Meta / Google / organic / email / direct)
- Flag channels with >2x baseline refund rate

## 4. Refund-adjusted ROAS
For SKUs sold via paid ads:
- Gross ROAS - refund value = net ROAS
- Flag SKUs where net ROAS <1.0 (paid ads losing money)

## 5. Output
- Top 10 SKUs by refund rate (with $ impact)
- Channel-level refund table
- "Pull from Meta" list — SKUs where paid acquisition is unprofitable
- Top 3 product issues to fix (sizing, quality, expectation gap)

Always separate refunds from returns / exchanges if Shopify data allows.
