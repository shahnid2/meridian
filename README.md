# Meridian — Private Concierge

A private, by-referral concierge marketing site. Single self-contained page:
luxury travel, worldwide private aviation, yacht charters, VIP access, and
bespoke lifestyle requests — arranged from **New York**, **California**, and worldwide.

## Structure

- `index.html` — the entire site (HTML + CSS + JS + embedded photography, no external dependencies).
- `robots.txt` — search-crawler directives (update the sitemap URL once deployed).

The page is fully self-contained — the destination photography is embedded as
base64 data URIs, and the rotating "meridian globe" hero is drawn on `<canvas>`.
No build step, no framework, no network calls.

## Run locally

Just open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8080
# then open http://localhost:8080
```

## Deploy

Drop the folder on any static host (Netlify, Vercel, Cloudflare Pages, GitHub Pages, S3).

## Before going live (SEO)

`index.html` ships with a keyword-rich `<title>`, meta description, Open Graph /
Twitter cards, and JSON-LD `ProfessionalService` structured data. Replace every
`your-domain.com` placeholder with the real domain, then:

1. Add a Google Business Profile (biggest lever for local "concierge" searches).
2. Register the domain in Google Search Console and submit a sitemap.
3. Earn press / backlinks.

## Notes

- "Meridian" is a working name — rename freely.
- The press strip ("Noted in") uses placeholder outlet names; replace with real
  mentions once earned. Do not list real publications that haven't featured you.
- Destination photography is royalty-free (Unsplash license, free for commercial use).
