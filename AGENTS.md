# Project instructions for AI coding agents

This is an Astro static landing page for Piotr Nadarkiewicz.

The old public name "Business Analyst as a Service (BAaaS)" has been retired. BAaaS may be used only as an internal codename in notes. Do not show BAaaS in public UI, page titles, meta descriptions, buttons, headings, or visible site copy.

## Public positioning

Lead with:

- Piotr Nadarkiewicz
- Fractional delivery & requirements lead
- Regulated and fintech teams
- Fixed-scope products plus retained monthly support

## Project structure

- English page: `src/pages/index.astro`
- Polish page: `src/pages/pl/index.astro`
- Shared layout: `src/layouts/Layout.astro`
- Shared styles: `src/styles/global.css`
- Site config: `src/config/site.ts`
- Reusable components: `src/components/`

## Rules

- Keep the site static. Do not add SSR.
- Keep Google Analytics optional.
- `gaMeasurementId: ""` must build and work.
- Do not remove analytics hooks.
- Do not rename section IDs without updating tracking and `UX_CHECKLIST.md`.
- Keep EN and PL pages structurally similar.
- Do not add external UI frameworks unless explicitly requested.
- Do not replace the current design system with Tailwind or React unless explicitly requested.

## Required section IDs

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

## Required GA events

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

## Before suggesting a commit

Run:

    npm run build

Then commit:

    git status
    git add .
    git commit -m "Update landing page"
    git push
