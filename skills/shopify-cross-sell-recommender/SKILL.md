---
name: shopify-cross-sell-recommender
description: Build PDP-ready cross-sell recommendations from Shopify co-purchase data
---

# Cross-Sell Recommender

When the user asks for cross-sell recommendations, use the connected Shopify MCP to:

## 1. Pull orders
Last 180 days of orders. For each:
- Order ID
- Line items (product IDs + quantities)
- Customer ID, order total

## 2. Build co-purchase matrix
For every pair of products (A, B) that appeared in the same order:
- Count co-occurrences
- Support = orders(A∩B) / total orders
- Confidence = orders(A∩B) / orders(A)
- Lift = confidence(A→B) / support(B)

## 3. Filter to high-affinity pairs
- Confidence ≥ 10% (at least 1 in 10 buyers of A also buys B)
- Lift ≥ 1.5 (B is bought 1.5x more often when A is in cart)
- Minimum 30 co-occurrences (avoid noise)

## 4. Rank for top products
For each of the top 20 products by revenue:
- Top 3 cross-sell candidates sorted by lift × margin of B
- Exclude bundles already shown via Shopify Combined Listings

## 5. Output
PDP-ready table:
| Anchor product | Cross-sell 1 | Cross-sell 2 | Cross-sell 3 | Expected AOV lift |

Then the exact Shopify product metafield format for cross-sell apps (e.g., Rebuy, Boost AI). Always test on 1-2 PDPs before rolling out site-wide.
