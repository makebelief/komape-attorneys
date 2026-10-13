# Komape Attorneys — Production SEO and Social Preview Upgrade

This package is based on the **latest client-photo gallery update** and retains the
existing homepage, page layouts, colours, navigation, and all 10 client photographs.

## Social previews
- `/assets/komape-social-preview-2026.jpg` (1200×630, self-hosted) puts the **existing
  original firm logo alongside the supplied attorney portrait showing the robe and
  brick-wall logo**. The photograph and logo were composited without AI alterations.
- Every page includes Open Graph and Twitter/X metadata with the absolute image URL,
  width/height, alt text, locale, canonical URL, and unique page title/description.
- The actual site favicon has been upgraded from a plain `K` to the firm emblem.
- Social networks cache link preview cards. On the first share, wait for scrapers to
  fetch the URL. Use Facebook Sharing Debugger and LinkedIn Post Inspector to
  re-scrape if a previous card is cached. WhatsApp previews cannot be guaranteed.

## Search discovery and launch
- `robots.txt` allows crawling; an XML sitemap lists six public marketing pages.
- Those six pages use `index,follow` tags; 404, Privacy and Terms remain `noindex`.
- Added `LegalService`, `WebSite`, `WebPage`, `BreadcrumbList`, and founder `Person`
  JSON-LD using contact details already on the site (no fabricated ratings).
- **Before deployment for search indexing, ensure the firm has approved publicly
  representing the website as its official site.** This was previously an unindexed
  demonstration. Once authorised, register the verified site with Google Search
  Console and submit `https://komape-attorneys.vercel.app/sitemap.xml`.
- Google chooses actual search-result thumbnails and favicons; Open Graph tags
  primarily control messaging/social link previews. Neither is guaranteed.

## Security
- CSP restricts JavaScript to local files and hashes of the exact JSON-LD metadata, allows approved font/image hosts and
  Google Maps iframe, and blocks object/embed, unapproved iframes and mixed content.
- HTTPS/HSTS, anti-sniffing, referrer and limited permissions headers are configured.
- Form remains an email draft (`mailto:`), *not* a hosted form or backend.
- Website does not require accounts, payments or a database, reducing attack surface.
- Only the bundled static files are published; do not add keys/passwords to source.
- Photos are kept from the previous approved demo with no newly added EXIF data.

## Update existing GitHub/Vercel (Ubuntu)
Download the ZIP into Downloads and paste one command:

```bash
cd ~/Downloads && unzip -oq komape-attorneys-seo-production.zip && cd komape-attorneys && git add -A && (git diff --cached --quiet || git commit -m "Improve Komape SEO, social image and site security") && git push origin main && npx vercel --prod --yes
```

Because the GitHub repo is connected to Vercel, the push can already trigger
production deployment automatically. Verify it before retrying if the CLI
returns an authorization error.
