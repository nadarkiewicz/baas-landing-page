# BAaaS v3 landing page UX checklist

This checklist supports the BAaaS v3 landing page in English and Polish.

## Main goal

The site should make a qualified visitor either:

1. Book a 30-minute call.
2. Start with a Delivery Readiness Review.
3. Leave an email for the guide.

## Current site structure

- English page: `/`
- Polish page: `/pl/`

## Positioning

The page is positioned as:

- EN: Fractional delivery leadership for regulated and fintech teams.
- PL: Doświadczone wsparcie delivery dla zespołów regulowanych i fintech.

## Product ladder

Fixed-scope products are entry points:

- Delivery Readiness Review / Przegląd Gotowości Delivery
- Regulation into Requirements / Regulacja w wymagania
- Requirements Reset / Reset wymagań
- Decision Paper / Dokument decyzyjny

The Readiness Review is the best first step and should be visually emphasised.

## Primary CTA

The primary CTA is:

- EN: `Book a 30-minute call`
- PL: `Umów 30-minutową rozmowę`

It should appear in:

- Sticky header
- Hero
- Product section
- Pricing
- Final CTA

## Secondary high-intent CTA

The secondary high-intent CTA is:

- EN: `Start with a Readiness Review`
- PL: `Zacznij od Przeglądu Gotowości`

It should appear in:

- Hero
- Fixed-scope products
- Final CTA

## Warm CTA

The warm CTA is the guide:

- EN: `The hidden cost of unclear requirements`
- PL: `Ukryty koszt niejasnych wymagań`

It should appear in:

- Lead magnet section

## Section order

Use this order unless explicitly changed:

1. Hero
2. Problem
3. Two ways to work
4. Fixed-scope products
5. Retained monthly model
6. Pricing
7. What the subscription includes
8. What it does not include
9. Proof / who is behind it
10. FAQ
11. Lead magnet
12. Final CTA
13. Footer

## Required section IDs

Do not remove or rename these IDs without also updating analytics:

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

## Analytics rules

Google Analytics must remain optional.

This must work:

    gaMeasurementId: ""

This must also work:

    gaMeasurementId: "G-XXXXXXXXXX"

Required events:

- `section_view`
- `view_products`
- `view_pricing`
- `select_product`
- `readiness_review_start`
- `select_tier`
- `cta_book_click`
- `lead_magnet_submit`
- `faq_open`
- `outbound_click`

## Design rules

- Keep one primary CTA per screen.
- Keep the booking CTA visually strongest.
- Keep Readiness Review clearly visible but secondary to the call CTA in the hero.
- Keep pricing visible on the page.
- Highlight Pro as most chosen.
- Highlight Delivery Readiness Review as the best first step.
- Use generous spacing.
- Avoid unnecessary animation.
- Mobile must work without horizontal scrolling.

## Trust rules

The page should include:

- 17+ years experience
- Banking
- Fintech
- Regulated software
- DORA / KYC-AML
- DORA proof point
- Telecom / M&A proof point
- KYC/AML proof point
- Customer-value / retail proof point
- NDA / anonymous-client note

## Polish language rules

The Polish version should use direct but professional Polish.

Avoid these Polish phrases unless explicitly requested:

- `pojemność`
- `ślizga`
- `senior-analityk`
- `jednego analityka` in hero
- `Doświadczona analiza` in hero

Preferred Polish wording:

- `abonament`
- `na poziomie seniora`
- `doświadczony`
- `stały dostęp`
- `umów 30-minutową rozmowę`
- `Przegląd Gotowości`

## Before publishing

Run:

    npm run build

Then check:

- `/`
- `/pl/`
- language switcher
- sticky CTA
- hero CTA
- Readiness Review CTA
- product cards
- pricing CTA
- final CTA
- lead magnet form
- mobile layout
- build output has no errors

## Publish command

Run:

    git status
    git add .
    git commit -m "Update landing page"
    git push

Cloudflare deploys automatically after push.
