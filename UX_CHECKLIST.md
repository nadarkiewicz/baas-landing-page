# Piotr Nadarkiewicz landing page UX checklist

Internal codename: BAaaS. Public brand: Piotr Nadarkiewicz.

## Main goal

The page should help win a small number of well-aligned B2B clients by making a qualified visitor either:

1. Book a 25-minute call.
2. Start with a fixed-scope Delivery Readiness Review.
3. Request the guide/checklist as a lower-friction fallback.

## Required conversion paths

- Booking: Cal.eu call link.
- Readiness Review: Cal.eu Readiness Review link.
- Guide request: Tally EN/PL links.
- Email: footer/contact fallback only.

## Trust requirements

The page should include:

- Portrait.
- LinkedIn link.
- Domain email.
- Testimonials / client feedback.
- Specific anonymised proof points.
- Privacy page.
- Clear footer with business context.

## Design direction

- Regulated/fintech credible.
- Cooler palette, strong text contrast, restrained accent.
- Clear visual hierarchy.
- Mobile sticky CTA.
- Readiness Review and Pro should be visually emphasised.

## Public copy rule

Do not use public-facing `BAaaS` or `Business Analyst as a Service`.

## Before publishing

Run:

```powershell
npm run build
```

Then check:

- `/`
- `/pl/`
- `/privacy/`
- `/pl/privacy/`
- Cal.eu links
- Tally links
- LinkedIn link
- mobile sticky CTA
- language switcher
- GA4 page load
