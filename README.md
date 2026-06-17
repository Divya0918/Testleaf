# Testleaf Website Replica

A local replica of the [Testleaf homepage](https://www.testleaf.com/), built from the live site's HTML structure with assets loaded from Testleaf's CDN (`assets.testleaf.com`).

## Quick start

```bash
npm install
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## What's included

- **Homepage** (`index.html`) — full mirror of testleaf.com including:
  - Sticky header with courses dropdown
  - Hero section with lead capture form
  - Anniversary, courses, AI reports, learner journeys
  - Testimonials carousel, comparison table, stats counters
  - Footer with links and contact info

## Tech stack (matches original)

- Bootstrap + Owl Carousel (via CDN)
- Poppins & Roboto fonts
- jQuery + custom scripts from Testleaf CDN
- Zoho form integration for lead capture

## Build for production

```bash
npm run build
npm run preview
```

## Notes

- Images, CSS, and JS are loaded from `https://assets.testleaf.com` for pixel-accurate styling.
- Internal links (e.g. `about-us.html`, `all-courses.html`) point to relative paths — add those pages to extend the full site.
- Form submissions go to Testleaf's Zoho CRM (live endpoint).

## Next steps

To build the full site, mirror additional pages from testleaf.com:

- `/all-courses.html`
- `/about-us.html`
- `/webinar.html`
- `/course/*.html`
