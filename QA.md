# First-draft verification

## Checks completed

- Dependency-free static build using Node.js.
- Local asset references, all fragment links and unique element IDs validated.
- One primary heading; language and viewport metadata; descriptive image alternatives; intrinsic image dimensions.
- Canonical URL, Open Graph and Twitter card metadata; Organization JSON-LD; robots.txt and sitemap.xml.
- Social image exported as a 1200 × 630 JPEG; favicons and application icons exported at declared sizes.
- Responsive desktop review in Chromium, plus same-origin preview frames at 320, 390 and 768 CSS pixels. At 320 and 768, the body scroll width matched its client width with no horizontal overflow.
- Mobile navigation opens, closes with Escape, restores focus, and uses expanded-state semantics.
- Native focus-section disclosure interaction verified, including Compute.
- Image and stylesheet budgets validated using `npm run check`.
- Contact links use connect@silvertine.si.

## Limits

The managed Chrome environment blocks DevTools, so a formal Lighthouse audit and numerical scores could not be obtained. No Lighthouse score is claimed. Frame-based responsive review does not replace physical iOS/Android testing. Live HTTPS, deployed security headers, search indexing, and WhatsApp/social fetch behavior require the domain to be connected to Vercel. The mail link opens the visitor's email client; mailbox provisioning is external.

After domain deployment, run Google PageSpeed Insights against https://silvertine.si/ for both mobile and desktop. Review performance, accessibility, best practices and SEO, then verify social card fetching against the public domain.
