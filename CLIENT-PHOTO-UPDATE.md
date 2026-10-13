# Komape Attorneys — Client photo addition (13 October 2026)

At the client's request the original demo and website UI remain unchanged.

- Added a 4-photo preview gallery on the **Home** page after the introductory attorney section.
- Added all **10 supplied photos** to **About Us**, anchored at `/about/#photo-gallery`.
- Added a 4-photo preview to **Our Attorney**.
- Preserved existing hero, service photographs, attorney profile portrait, logo, contact details, SEO, footer, responsive navigation and circular WhatsApp control.
- The image gallery uses original photographs for full-size viewing and WebP versions for fast mobile browsing. No stretching; gallery thumbnails use object-fit: cover.
- Group-photo captions do not identify unidentified colleagues.
- Uploaded photo originals are between 1365–2048 pixels long/wide; filenames supplied by the user mention 4K, but the image pixels do not constitute native 4K.

To update existing GitHub/Vercel deployment, extract into `~/Downloads/komape-attorneys`, commit and push to `main`, then run `npx vercel --prod --yes`.
