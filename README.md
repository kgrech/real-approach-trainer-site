# Real Approach Trainer website

Permanent product website, privacy policy and support information for Real Approach Trainer. Plain HTML and CSS, with no framework, dependencies, build step, JavaScript, analytics, forms or cookies.

## Public pages

- Product landing page: https://kgrech.github.io/real-approach-trainer-site/
- Privacy policy: https://kgrech.github.io/real-approach-trainer-site/privacy/
- Support and bug reports: https://kgrech.github.io/real-approach-trainer-site/support/

GitHub Pages publishes the repository root from `main`. Edit the HTML and shared `styles.css`, commit and push to update the site. Keep application source, internal documentation and credentials out of this repository.

For local preview, run `python3 -m http.server 8000` in this directory.

## Design and assets

All three pages share the app's charcoal surfaces, amber accents, HSI icon, typography, navigation and footer. The landing page uses genuine app artwork and screenshots, responsive WebP images, and only FAA approach plates. See [asset credits](ASSETS.md) and [source mappings](assets/sources.json). Below-the-fold screenshots are lazy-loaded; all image dimensions are specified. Full-size screenshots are normalized for EXIF orientation before resizing.

Visible text is platform agnostic. Availability is “Coming soon”; no production or public beta link is claimed. Add a verified public store or beta URL only when available, distinguishing a free beta from the planned paid app. The buy-once wording promises no recurring fee to keep using the purchased app, not perpetual updates or support.

## Verification

Check all three pages at phone, tablet and desktop widths, keyboard navigation, links, image loading and absence of horizontal overflow. Ensure privacy wording still matches the app before changing data-handling claims. Verify the deployed pages over HTTPS after publication.
