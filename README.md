# PrepFuel

High-Protein Budget Meal Prep in Under 30 Minutes — a static website for the
Pinterest affiliate business (@jdnanncy). Built 2026-11-18.

## Stack

Plain static HTML/CSS/JS. No build step, no framework, no backend, no
analytics/tracking. System fonts only — zero external requests except outbound
links (Pinterest profile, Amazon search placeholders).

## Deploy

GitHub Pages, repo `github.com/Sundala1/prepfuel`. Push the contents of this
directory to the repo root and enable Pages (branch `main`, folder `/ (root)`).
Live URL: https://sundala1.github.io/prepfuel/

All internal links and asset paths are **relative**, so the site also works
from any subpath or custom domain. If the site moves to a custom domain,
update the absolute URLs in: `<link rel="canonical">` and Open Graph tags
(every page), `sitemap.xml`, `robots.txt`, and the `image` fields in the
Recipe JSON-LD blocks.

## Pages

| File | Page |
|---|---|
| `index.html` | Homepage: hero, featured plan, recipe categories, gear guides, about teaser |
| `7-day-meal-prep-plan.html` | Flagship plan: 7-day table, Sunday schedule, grocery list, 2 anchor recipes |
| `chicken-meal-prep.html` | 5 chicken recipes (38–44 g protein each) |
| `budget-meal-prep.html` | $50/week plan: grocery list with prices, 5 recipes |
| `best-meal-prep-containers.html` | Money page: 5 product cards + comparison + FAQ |
| `high-protein-breakfast-meal-prep.html` | 5 breakfast recipes (20–28 g protein each) |
| `essential-kitchen-gear.html` | 4 product cards + "worth adding next" + FAQ |
| `about.html` | About, affiliate disclosure, photo credits |

Supporting files: `styles.css`, `script.js` (mobile nav toggle + footer year),
`sitemap.xml`, `robots.txt`, `ATTRIBUTION.md`, `assets/` (18 photos + `credits.json`).

## Before launch / TODO

1. **Pinterest site verification** — every page's `<head>` has a commented
   placeholder for the `p:domain_verify` meta tag. Add the real tag from
   Pinterest's claim flow, then claim the site.
2. **Amazon Associates** — product buttons on the containers and gear pages
   link to plain Amazon search URLs (each preceded by an HTML comment saying
   so). After Associates signup, replace them with tagged affiliate links and
   add `sponsored` to the `rel` attribute. The footer + about-page disclosure
   text already anticipates this; flip it to the standard Associates wording
   ("As an Amazon Associate, PrepFuel earns from qualifying purchases") once
   accepted. Note: Amazon requires 3 qualifying sales within 180 days.
3. **Pinterest tag** — not installed (no tracking per brief). Add later if
   the business wants conversion tracking.

## Images

18 real food photos, downloaded from Openverse (CC-licensed, commercial use
allowed), resized to max 1400 px wide, JPEG q82. Total ~1.96 MB. Full
attribution: `ATTRIBUTION.md` and the About page. No AI-generated food images.
