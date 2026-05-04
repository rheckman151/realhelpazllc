# Real Help LLC Website

Static website for Real Help LLC, a family-owned Tucson handyman service focused on practical home repairs, cleanup, installs, demo prep, yard labor, landscaping help, and honest pricing.

## Live Site

- Main website: https://realhelpazllc.com
- Golf pamphlet landing page: https://realhelpazllc.com/golf/

## What This Site Includes

- Main homepage with services, trust details, reviews, FAQ, contact paths, and quote request form.
- QR/ad landing page in `/golf/` for golf course pamphlet traffic.
- Formspree-powered estimate request forms.
- SEO metadata, structured business data, `robots.txt`, and `sitemap.xml`.
- Local optimized hero images and favicon assets.
- Apache/cPanel `.htaccess` cache and compression rules.

## Important Files

- `index.html` - main website.
- `golf/index.html` - QR/pamphlet landing page.
- `images/` - logos, favicon files, and optimized hero images.
- `robots.txt` - crawler access and sitemap reference.
- `sitemap.xml` - sitemap submitted to Google Search Console.
- `.htaccess` - caching/compression rules for cPanel hosting.

## Form Service

The quote forms submit through Formspree using the endpoint configured in the HTML:

```txt
https://formspree.io/f/xaqljrdo
```

Formspree forwards estimate requests to the configured work email.

## Updating The Site

1. Edit `index.html` for the main site.
2. Edit `golf/index.html` for the QR/pamphlet landing page.
3. Upload changed files to the site root in cPanel.
4. If assets change, upload the matching files from `images/`.
5. Retest the live site on desktop and mobile.

## Git Workflow

```bash
git status
git add .
git commit -m "Describe the update"
git push
```

## Notes

- Keep the main site mostly static HTML for speed and SEO.
- Keep visible images optimized, especially above-the-fold assets.
- If the favicon appears stale, clear browser cache or bump the favicon query string in the HTML.
- If PageSpeed reports `robots.txt` issues, check whether Cloudflare is injecting managed robots/content-signal rules.
