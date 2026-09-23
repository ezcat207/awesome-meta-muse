# Prompts: Shopify + PayPal checkout

Context: as of late September 2026, Muse can check out via Stripe Link, Shopify's Shop Pay (auto-enabled for any Shopify merchant shipping to the US), and PayPal (1M+ merchant network) — while Amazon has blocked Muse from completing purchases on its site. Full writeup: [Meta Muse Can Now Buy Through Shopify and PayPal](https://aiextracash.com/tools/muse/muse-shopify-paypal-checkout/).

## 1. Basic shopping test

```
Find [product name] from Shopify stores that ship to [your state], under $[price].
Show me the top 3 options with price and shipping time, but don't buy anything yet —
just show me what you find.
```

## 2. Merchant self-test (see what Muse sees about your own store)

```
I'm trying to buy [your product name] — search for it the way a shopper would and
tell me exactly what stores and listings come up, what images and prices you see,
and whether you could complete checkout. Don't complete the purchase, just report
what you found.
```

Useful as the core of a paid "Muse-readiness audit" for small Shopify merchants — see the [service-idea section](https://aiextracash.com/tools/muse/muse-shopify-paypal-checkout/#an-income-angle-muse-readiness-audits-for-small-merchants) of the source article.

## 3. Competitive scan

```
Search for [product category] under $[price] that ships to [state]. List every
store you find, with price, shipping time, and how complete each listing looks
(images, description, reviews if visible).
```

## What doesn't work

Don't try to adapt these for Amazon — Muse cannot complete checkouts on Amazon.com as of the last-verified date on the source article. Any prompt telling Muse to buy on Amazon will hit that block.
