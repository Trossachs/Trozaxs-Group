# Trozaxs Group site

Static site, no build step. Every file is in one flat folder with lowercase names.

## Deploy on Vercel
1. Push this folder's contents to the root of a GitHub repo.
2. Vercel > Add New Project > import the repo. Framework Preset: Other. Leave Build Command, Install Command and Output Directory empty. Deploy.

The admin is at /admin. To publish edits: Admin > Backup & publish > Download content.js, replace content.js in the repo, commit and push.

## Products page and social preview

- `#products` lists ready-made websites. Edit them in Admin > Products (name, price, features, image, demo link, payment link).
- A product with a payment link (Paystack, Flutterwave, Stripe) shows **Buy now**. Without one, the button opens the contact form with the product and price filled in. The site cannot take payments itself.
- Prices are placeholders. Change them before launch.
- Social preview: in `index.html`, replace `https://trossachs-group.atwebpages.com` (og:url, og:image, twitter:image) with your real domain. Re-scrape the link in Facebook's Sharing Debugger, X and WhatsApp after deploying.
