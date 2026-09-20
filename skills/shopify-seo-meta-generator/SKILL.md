---
name: shopify-seo-meta-generator
description: Generate intent-matched meta titles and descriptions for Shopify PDPs using Search Console queries
---

# SEO Meta Generator

When the user asks for product meta titles, use Shopify + Google Search Console MCPs to:

## 1. Identify top product URLs
- Pull last 90 days of GSC data for /products/* URLs
- Sort by impressions
- Take top 50 by impressions (or filter by collection)

## 2. Mine intent per URL
For each URL:
- Top 5 queries by impressions (head + long tail)
- Avg CTR vs site avg (flag CTR <2% — biggest improvement opportunity)
- Current meta title + description

## 3. Write the new meta
For each PDP:
- **Meta title (≤60 chars)** — primary keyword + product name + benefit + brand
- **Meta description (≤155 chars)** — match top query intent, include 1 specific number/proof, end with CTA verb

Voice rules:
- No "Buy [product] online" filler
- Front-load the value
- Include a number where credible (warranty length, ingredient count, return window)

## 4. Predict CTR lift
For each new meta:
- Estimated CTR improvement based on current avg CTR and SERP position
- Estimated monthly extra clicks at current impressions

## 5. Output
| URL | Current title | New title | Current desc | New desc | Predicted CTR lift | Extra monthly clicks |

Then a Shopify-ready bulk update format (CSV with handle, page_title, meta_description columns) and the exact bulk editor path.

Always preserve brand name suffix on title for category consistency.
