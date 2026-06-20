BAaaS v3 site files

Copy these files into your Astro project root:
D:\Projects\BAaaS\landing-page

This package updates the site to v3:
- EN page at /
- PL page at /pl/
- v3 positioning: fractional delivery leadership for regulated and fintech teams
- fixed-scope product ladder
- retained monthly subscription model
- optional Google Analytics
- GA events for product selection, readiness review, pricing, booking CTA, FAQ and lead magnet
- reusable Astro components

Files included:
- AGENTS.md
- UX_CHECKLIST.md
- src/config/site.ts
- src/layouts/Layout.astro
- src/styles/global.css
- src/components/Button.astro
- src/components/LanguageSwitch.astro
- src/components/LeadMagnet.astro
- src/components/PricingCard.astro
- src/components/ProductCard.astro
- src/components/ProofCard.astro
- src/components/FaqItem.astro
- src/pages/index.astro
- src/pages/pl/index.astro

After copying:

npm run build

git status
git add .
git commit -m "Update landing page to v3"
git push

Cloudflare deploys automatically after push.

Edit src/config/site.ts when ready:
- gaMeasurementId
- bookingLink
- readinessReviewLink
- leadMagnetAction
- contactEmail
