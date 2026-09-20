---
name: shopify-pricing-margin-audit
description: Audit Shopify pricing and discounts to find SKUs sold below margin floor
---

# Pricing + Margin Audit

When the user asks for a margin audit, use the connected Shopify MCP to:

## 1. Pull pricing data
For every product variant:
- Compare-at price (regular)
- Sale price
- Cost per item (Shopify cost field or metafield)
- Discount % = (compare_at - sale) / compare_at

## 2. Compute true margin
For each SKU sold in the last 30 days:
- Gross margin = (sale price - cost) / sale price
- Allocated ad cost per unit = (ad spend on SKU) / (units sold)
- Net margin = gross margin - allocated ad cost - shipping cost

## 3. Flag the problem SKUs
**Critical** — Discount ≥20% AND net margin <15%
**Warning** — Discount 10-20% AND net margin <25%
**Healthy** — Discount <10% OR net margin ≥30%

## 4. Quantify impact
For each Critical SKU:
- Monthly units sold × negative margin = monthly profit loss
- Sum across all Critical SKUs = total monthly leak

## 5. Output
Ranked list:
| SKU | Sale price | Cost | Discount | Net margin | Monthly leak | Suggested action |

Suggested actions:
- Raise price by X%
- Remove from automatic discount
- Exclude from ad spend
- Bundle with higher-margin product

Always include the Shopify discount or automatic discount ID so the user can act in one click.
