---
name: shopify-product-description-rewriter
description: Rewrite Shopify product descriptions in brand voice, 60-90 words each, with consistent structure
---

# Product Description Rewriter

When the user asks to rewrite descriptions, use the connected Shopify MCP to:

## 1. Pull products
- Filter by collection, tag, or vendor (ask the user)
- Pull title, current description, product type, top tags, top 3 review snippets if available

## 2. Brand voice profile
Confirm with the user:
- Tone (premium / playful / clinical / streetwear)
- Forbidden words
- Required phrases (warranty, certifications)
- Voice example from an existing best-performing PDP

## 3. Rewrite structure (60-90 words)
For each product, write 4 short blocks:
- **Hook** — primary benefit in one sentence
- **Why it works** — 2-3 features tied to benefits
- **Proof** — review snippet, certification, or claim
- **CTA line** — short, action oriented

## 4. SEO awareness
- Front-load the primary keyword (product type + key attribute)
- Include 1 long-tail variant
- Keep meta description under 155 chars (separate output)

## 5. Output
Markdown table:
| SKU | Old description (first line) | New description | Word count |

Then a staging plan: which products to push first (highest traffic), and the exact Shopify metafield / body_html to update.

Never auto-write to Shopify — always preview first.
