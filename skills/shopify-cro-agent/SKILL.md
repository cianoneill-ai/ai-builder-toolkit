---
name: shopify-cro-agent
description: Walk Shopify funnel from PDP to checkout, pinpoint drop-offs, and suggest prioritized fixes
---

# Shopify CRO Agent

When the user asks for a CRO audit, use the connected Shopify + GA4 MCPs to:

## 1. Funnel pull
Pull last 28 days of funnel data:
- Sessions, PDP views, add-to-cart, begin-checkout, purchases
- By device (mobile / desktop / tablet)
- By top 10 traffic sources

## 2. Drop-off scoring
For each funnel stage, calculate conversion rate vs Shopify benchmarks:
- **PDP → ATC** — benchmark 8-12% (flag if <6%)
- **ATC → Checkout** — benchmark 50-65% (flag if <40%)
- **Checkout → Purchase** — benchmark 60-75% (flag if <50%)

## 3. Diagnose the biggest leak
For the worst-scoring stage:
- PDP issues — pricing visibility, hero image, reviews, stock urgency, mobile load time
- Cart issues — surprise costs, weak upsell, no trust badges
- Checkout issues — too many fields, no express pay, login friction

## 4. Suggested fixes
Output 5 prioritized fixes:
- Stage affected
- Specific change (e.g., "Add sticky ATC button on mobile PDP")
- Estimated lift (based on benchmarks)
- Estimated monthly revenue impact

## 5. Output
Markdown report:
- Funnel snapshot table
- Biggest leak + root cause
- 5 ranked fixes with revenue impact
- 1 fix to ship this week

Always include device breakdown — mobile drop-offs are usually the biggest opportunity.
