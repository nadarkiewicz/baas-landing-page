# BAaaS landing page project instructions

This is an Astro static landing page deployed to Cloudflare Workers static assets.

## Project structure

- English page: `src/pages/index.astro`
- Polish page: `src/pages/pl/index.astro`
- Shared layout: `src/layouts/Layout.astro`
- Shared styles: `src/styles/global.css`
- Site config: `src/config/site.ts`
- Reusable components: `src/components/`

## Current positioning

The page is now v3: fractional delivery leadership for regulated and fintech teams.
The commercial structure is:

1. Fixed-scope products as entry points.
2. Monthly retained senior capacity as the ongoing model.

Keep the split in tone:

- Fixed-scope products: plain commercial language.
- Retained model: slightly more elevated, senior, strategic language.

## Rules

- Do not remove Google Analytics safety logic.
- `gaMeasurementId` may be empty. If it is empty, the page must still build and work.
- Keep English at `/`.
- Keep Polish at `/pl/`.
- Keep EN and PL pages structurally similar.
- Do not add server-side rendering.
- This should remain a static Astro site.
- Do not add a database unless explicitly asked.
- Do not redesign the whole site unless explicitly asked.

## Required section IDs

Do not remove these IDs without updating analytics:

- `hero`
- `problem`
- `two-ways`
- `products`
- `how-it-works`
- `pricing`
- `included`
- `not-included`
- `proof`
- `faq`
- `lead-magnet`
- `contact`

## Required GA events

Keep support for:

- `page_view`
- `section_view`
- `view_hero`
- `view_products`
- `view_pricing`
- `select_product`
- `readiness_review_start`
- `select_tier`
- `cta_book_click`
- `lead_magnet_submit`
- `faq_open`
- `outbound_click`

## Before suggesting a commit

Run:

    npm run build

## Deployment

Changes are published by pushing to GitHub:

    git add .
    git commit -m "Update landing page"
    git push

Cloudflare deploys automatically after push.
