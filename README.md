# Komape Attorneys — Website concept

Static HTML, CSS, JavaScript; no build step or paid dependencies.

## Local preview

`python3 -m http.server 8000` then http://localhost:8000

## Deployment

Vercel: Other framework; root directory `.`; output directory `.`; `npx vercel --prod` from the repository root.

## Firm details for confirmation

- Firm: Komape Attorneys, founded in 2022.
- Founder and director: Godfrey Komape.
- Tembisa office: 99 Julius Nyerere Street, Ibazelo Section, Tembisa, Gauteng 1632, South Africa
- Landline: +27 10 825 3971; mobile: +27 72 416 7243.
- The WhatsApp icon points to +27 72 416 7243 (number is listed as WhatsApp in directory screenshots; functionality untested).
- Email: info@komapeattorneys.com.
- Main resources: user-supplied attorneys.co.za screenshots; professional directory search results.
- Logo is a 4K-width enlargement of the supplied artwork, not a new vector master. Header and footer variants use transparent backgrounds.
- Supplied portrait appears on homepage and on Our Attorney page only. Original portrait contains available photographic detail; it is not native 4K.
- Stock imagery is externally hosted by Pexels and must be visually checked after deployment.
- Contact form opens a user-controlled email draft; no server-side submission, inbox, or storage.
- SEO fields include page titles, canonical tags, JSON-LD, OG metadata, sitemap; indexing is disabled pending attorney approval.
- Remove demo noindex and confirm legal notices and business data only with firm authorisation.
- If Vercel allocates a different domain from https://komape-attorneys.vercel.app, update canonical meta tags, structured data and sitemap.xml.

## Sources

- https://www.attorneys.co.za/ResultsPage.asp?AreaID=440&LanguageID=-1&Name=&RegionID=14&SpecialtyID=-1&sMode=C
- https://za.linkedin.com/in/godfrey-komape-7148a97b

## Pre-launch review

Confirm professional descriptions, telephone, WhatsApp, listed opening hours, maps marker, photo permissions, POPIA compliance and services with the firm before an official website launch.

Header: logo-header-4k.png is a transparent horizontal layout of the uploaded logo artwork. The original vertical branding is used in the footer.
