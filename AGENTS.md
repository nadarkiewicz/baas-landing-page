# Piotr Nadarkiewicz landing page project instructions

Internal codename: BAaaS. Public brand: Piotr Nadarkiewicz.

This is an Astro static landing page deployed to Cloudflare Workers static assets.

## Public positioning

- Lead with: `Piotr Nadarkiewicz`
- Offer: `Fractional delivery & requirements lead`
- Do not use `Business Analyst as a Service` or `BAaaS` in public-facing copy.
- Keep English at `/` and Polish at `/pl/`.

## Project structure

- English page: `src/pages/index.astro`
- Polish page: `src/pages/pl/index.astro`
- Privacy page: `src/pages/privacy/index.astro`
- Polish privacy page: `src/pages/pl/privacy/index.astro`
- Shared layout: `src/layouts/Layout.astro`
- Shared styles: `src/styles/global.css`
- Site config: `src/config/site.ts`
- Portrait: `public/piotr-nadarkiewicz.jpg`

## Rules

- Keep Google Analytics safety logic intact.
- Keep section IDs stable unless analytics is updated.
- Keep EN and PL pages structurally similar.
- Do not add server-side rendering.
- This should remain a static Astro site.
- Tally is used for guide requests.
- Cal.eu is used for booking and Readiness Review.
- Email is a fallback/contact path only, not the main conversion path.

## Build check

Before suggesting a commit, run:

```powershell
npm run build
```

## Deployment

```powershell
git add .
git commit -m "Refine trust and conversion path"
git push
```
