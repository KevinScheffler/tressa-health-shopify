# Tressa Health

A custom Shopify theme built from scratch on Shopify's [Skeleton](https://github.com/Shopify/skeleton-theme) starter.

Tressa Health is a fictional telehealth and supplement brand. I created it as a working environment for building the storefront patterns this category actually needs, without the constraints that come with client work. Everything here is written by me from Shopify's documentation.

## Why this exists

Most of my paid Shopify work is under NDA and cannot be shown. This repository is where I build the same categories of feature independently, so the code is available to read.

It is also a deliberate exercise in working without AI assistance. Every section, snippet, and schema here was written against the Shopify docs, and `docs/friction-log.md` records where I got stuck and how I worked through it. The log distinguishes between gaps in syntax, architecture, platform knowledge, and tooling, so I can tell which ones need practice rather than lookup.

## The problems I am building for

Telehealth and supplement storefronts share a set of front end problems that generic themes handle badly:

- Subscription pricing that renders correctly on first paint instead of after a third party widget loads
- Eligibility and intake steps that gate purchase without breaking the cart
- Compliance and trust content that merchants can edit without touching code
- Product data that varies by dose, plan, and format rather than by size and color

## Build status

This theme is in active development. Features land incrementally and each one is documented below as it ships.

| Feature | Status |
| --- | --- |
| Skeleton scaffold and theme setup | Complete |
| Friction log | Ongoing |
| Server rendered subscription pricing | In progress |
| Eligibility gated add to cart | Planned |
| Merchant editable compliance blocks | Planned |
| Metafield driven product content | Planned |

## Stack

Liquid, JavaScript, CSS, Shopify CLI, Theme Check

## Running locally

Requires the [Shopify CLI](https://shopify.dev/docs/api/shopify-cli) and a development store.

```bash
git clone https://github.com/KevinScheffler/tressa-health-shopify.git
cd tressa-health-shopify
shopify theme dev --store your-store.myshopify.com
```

Theme Check runs against the config in `.theme-check.yml`:

```bash
shopify theme check
```

## Notes

Tressa Health is not a real company. The brand, product catalog, and copy are invented for the purposes of this build.