---
name: shopify-theme-tweaks
description: Write Liquid and CSS for small Shopify theme changes without a developer
---

# Theme Tweaks (No Dev)

When the user asks for a theme tweak, use the connected Shopify MCP to:

## 1. Identify theme + template
- Pull the active theme name and version
- Identify which template the change affects (product, cart, collection, header, footer)
- Confirm the exact section / snippet file to edit

## 2. Write the change
- Liquid for logic (loops, conditionals, metafield reads)
- CSS scoped with a unique class so it cannot leak
- Mobile-first — write the mobile rules first, add desktop breakpoints

## 3. Common patterns
- **Stock counter** — read variant.inventory_quantity, show when below threshold
- **Promo banner** — site-wide section above header with dismiss cookie
- **Trust badges** — snippet rendered in PDP and cart
- **Sticky ATC** — fixed-position button on mobile PDP scroll

## 4. Safety guards
- Wrap every change in a feature flag (theme setting) so it can be toggled off
- Use {% if shop.metafields.cro.enabled %} for store-level kill switch
- Test on a copy of the theme first — never edit live theme without backup

## 5. Output
- Theme file path
- Exact Liquid / CSS diff (with line numbers)
- Step-by-step install: duplicate theme → edit code → preview → publish
- Rollback steps

Always remind the user to duplicate the theme before editing.
