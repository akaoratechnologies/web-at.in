# Akaora Technologies V16 — SVG Edition

Website improvements in this release:
- Removed Unsplash stock-photo dependencies; homepage, carousel and product sections now use **authored local SVG artwork**.
- Dedicated SVG illustrations for Inventory Standard, Pro, POS, thermal printer and receipt workflow.
- All six other software initiatives retain their local, product-specific SVG concept illustrations.
- Interface actions and service feature icons use lightweight inline SVG. Mobile hamburger icon uses SVG too.
- Original official brand wordmarks and founder photography are preserved; these are real brand assets, not random stock images.
- All original SEO-friendly pre-rendered HTML routes are updated, not just JavaScript-rendered SPA navigation.
- Local images work without Unsplash access. Styles and scripts include V16 version identifiers to aid cache refresh.

**Visual note:** Product illustrations are graphical concepts, not actual application screenshots or guaranteed hardware models. Confirm the exact specifications before purchase.

## Deployment
Extract this ZIP and upload everything inside the `akaora-technologies-site` folder to your hosting public web root (such as `public_html`). Keep hidden `.htaccess` and the `assets/` directory. After deploying, do a hard refresh or clear the hosting cache.

## Files and credits
No npm or server framework required. The site is a static SPA with pre-rendered public routes, local images, CSS, JS, and a native browser-based WhatsApp enquiry flow.

---

# Akaora Technologies Corporate SPA — V15 Product Catalogue & Optimization

## What's new in V15

- **Stable product images across SPA navigation.** Dynamic image URLs now resolve from the site root on HTTP/HTTPS. This prevents the broken `/products/assets/img/...` references that could occur when navigating from the homepage to product detail pages.
- **Eight individually presented products.** Akaora Inventory Standard (₹4,999) and Pro (₹6,999) are shown first with package details; the six Akaora software initiatives each have their own lightweight, locally hosted concept illustration.
- **Clearer product catalogue.** Inventory packages and software initiatives are separated into named sections with accessible jump navigation, refreshed spacing, consistent cards, better responsive grid layouts, and improved image sizing.
- **Updated colors.** Midnight navy, cobalt blue and subtle teal accents complement the existing Akaora orange brand marks. Both light and dark themes remain available.
- **Performance improvements.** Local, lightweight SVG product illustrations replace remote stock images in the product catalogue; below-the-fold product images load lazily, image assets can be cached using Apache rules, and CSS/JS use V15 cache-busting URLs.
- **Navigation and metadata fixes.** Normal `#section` links no longer conflict with SPA hash routes, social metadata updates during SPA navigation, and specific product details have their own Open Graph images.
- **SEO preserved.** 20 direct URL pages contain freshly prerendered content for search crawlers, plus existing canonical links, metadata, structured data, sitemap, robots.txt and llms.txt.

### Accurate visual representations

The six software-initiative visuals are illustrative concepts **not actual application screenshots**. Contact Akaora Technologies for current software release status and availability. Inventory bundles retain the supplied promotional product images; confirm hardware models, device support, taxes and delivery before purchase.

## Deployment

1. Extract this ZIP and open `akaora-technologies-site/`.
2. Upload **all files and folders inside that folder**, including the hidden `.htaccess`, to the Hostinger domain's `public_html` root. Do **not** upload just the outer folder.
3. Make sure the server is serving the website at the domain root (`/`). On Apache or Hostinger, existing directories work as direct SEO URLs such as `/products/pro/`.
4. Hard-refresh after deployment if an older site version is cached. Query strings `?v=15` on CSS/JS help ensure the new files are loaded.
5. Visit `/products/`, `/products/standard/`, `/products/pro/`, and each `/products/apps/<slug>/` URL. Confirm image display, WhatsApp enquiries, light/dark themes, mobile layout and the header carousel.

## Notes

- This is a **static HTML, CSS and JavaScript** website with client-side SPA navigation and pre-rendered pages. No build dependencies, backend, Firebase, server-side runtime or Node.js hosting are required.
- `index.html` supports hash navigation when previewed using `file://`, but direct clean URLs are intended for web hosting. For a closer local preview use a simple HTTP server started from the site directory.
- The portfolio route and publicly named client projects remain removed from V14. The `.htaccess` rule returns HTTP 410 (Gone) at `/portfolio/` under Apache hosting.
- Home and service imagery may use remote Unsplash photographs with built-in local fallbacks. The **six software catalogue illustrations themselves are stored locally** and do not depend on external image hosts.
- Static validation checked all 20 pre-rendered pages, local image references and direct route links, as well as JavaScript syntax. Automated browser navigation was unavailable in the test environment; conduct a final live-device check after upload.
