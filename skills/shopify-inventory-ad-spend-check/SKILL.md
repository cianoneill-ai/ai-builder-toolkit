---
name: shopify-inventory-ad-spend-check
description: Find Shopify products approaching OOS while still receiving heavy paid ad spend
---

# Inventory + Ad Spend Check

When the user asks to check inventory vs ad spend, use Shopify + Meta + Google Ads MCPs to:

## 1. Pull inventory
For every product variant:
- Current inventory_quantity (across all locations)
- Daily sales velocity (units sold per day, last 30 days)
- Days of stock remaining = inventory / velocity

## 2. Pull ad spend by SKU
- Meta Ads: spend last 7 days, attributed to each product (via catalog product ID or UTM)
- Google Ads: shopping spend by item ID, last 7 days

## 3. Flag scenarios
**Critical** — <14 days of stock AND >$500 weekly ad spend (pause now)
**Warning** — 14-30 days of stock AND >$500 weekly ad spend (fast-track restock)
**Stranded spend** — Out of stock AND ads still running

## 4. Actions
For each flagged SKU:
- Suggested action (pause campaign, exclude SKU from catalog, reduce daily budget)
- Estimated wasted spend if not actioned
- Restock urgency

## 5. Output
Ranked table:
| SKU | Days of stock | Weekly spend | Status | Action | Owner |

Always include the exact campaign or ad set IDs so the user can act in one click.
