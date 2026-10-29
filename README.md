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

## Sharing links

Crawlers ignore the part after `#`, so share these addresses to get the right title with the logo preview: `/products.html`, `/services.html`, and `/svc-<service>.html` for each service. They open the matching page of the site. `/` and `/index.html` use the home preview.

## Reviews, FAQ, client logos, project pages

- Reviews: slideshow in the contact area, managed in Admin > Reviews. The three "Sample Reviewer" reviews are placeholders.
- FAQ, Client logos and the Blog link are editable in Admin (FAQ, Client logos, Site & footer).
- Each portfolio card opens `#work-<project-name>`. Fill in the description, highlights and live link in Admin > Portfolio.
- Footer shows GitHub and Linktree icons once you paste their links in Admin > Site & footer.
