# Landing page UX checklist

Internal codename: BAaaS.

Public brand: Piotr Nadarkiewicz.

Public offer: fractional delivery & requirements lead.

Do not display "Business Analyst as a Service" or "BAaaS" in the public site.

## Main goal

The site should make a qualified visitor either:

1. Book a 30-minute call.
2. Start with a fixed-scope Readiness Review.
3. Leave an email for the guide.

## Current site structure

- English page: `/`
- Polish page: `/pl/`

## Primary CTA

The primary CTA is:

- EN: `Book a 30-minute call`
- PL: `Umów 30-minutową rozmowę`

It should appear in:

- Hero
- Sticky header
- Product section
- Pricing
- Final CTA

## Secondary CTA

The highest-intent secondary CTA is:

- EN: `Start with a Readiness Review`
- PL: `Zacznij od Przeglądu Gotowości`

The lower-friction warm CTA is the guide:

- EN: `The hidden cost of unclear requirements`
- PL: `Ukryty koszt niejasnych wymagań`

## Section order

Use this order unless explicitly changed:

1. Hero
2. Problem
3. Two ways to work
4. Fixed-scope products
5. Retained monthly capacity
6. Pricing
7. What the subscription includes
8. What it does not include
9. Who is behind it
10. FAQ
11. Lead magnet
12. Final CTA

## Required section IDs

Do not remove or rename these IDs without updating analytics:

- `hero`
- `problem`
- `ways-to-work`
- `fixed-scope-products`
- `retained`
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
- `view_hero`
- `view_pricing`
- `view_faq`
- `cta_book_click`
- `select_product`
- `readiness_review_start`
- `select_tier`
- `lead_magnet_submit`
- `faq_open`
- `outbound_click`

## Product tracking

Fixed-scope product CTAs must send `select_product`.

Product keys:

- `readiness_review`
- `regulation_requirements`
- `requirements_reset`
- `decision_paper`

Readiness Review CTAs must also send `readiness_review_start`.

## Hero rules

The hero must answer:

- Who is this?
- What is the offer?
- Who is it for?
- Why should I care?
- What do I do next?

Hero must include:

- Piotr Nadarkiewicz
- Fractional delivery & requirements lead
- Regulated / fintech context
- Primary booking CTA
- Readiness Review CTA
- Credibility strip

## Pricing rules

Pricing must remain visible on the page.

Pricing must show:

- Core
- Pro
- Prime

Pro should be visually marked as the common / most chosen option.

Do not hide pricing behind a call.

## Trust rules

The page should include:

- 17+ years experience
- Banking
- Fintech / regulated software
- DORA / KYC-AML
- DORA proof point
- Telecom / M&A proof point
- KYC/AML proof point
- Customer-value / retail proof point
- NDA / clients anonymous note

## Design rules

- Use generous spacing.
- Keep one visual accent colour.
- Do not add unnecessary animation.
- Do not add competing CTA types.
- Primary CTA must be visually stronger than secondary CTA.
- Mobile must work without horizontal scrolling.
- The page must remain readable on a phone.

## Language rules

EN and PL pages should stay structurally similar.

Polish should be direct and professional.

Preferred Polish wording:

- `lider delivery i wymagań`
- `w abonamencie`
- `projekt o ustalonym zakresie`
- `Przegląd Gotowości Delivery`
- `Umów 30-minutową rozmowę`

## Before publishing

Run:

    npm run build

Then check:

- `/`
- `/pl/`
- sticky header
- language switcher
- hero CTA
- Readiness Review CTA
- product cards
- pricing CTA
- final CTA
- lead magnet form
- mobile layout

## Publish command

Run:

    git status
    git add .
    git commit -m "Update landing page"
    git push

Cloudflare deploys automatically after push.
