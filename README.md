# Real Approach Trainer website

Permanent product website, privacy policy and support information for Real Approach Trainer. Plain HTML and CSS, with no framework, dependencies, build step, JavaScript, analytics, forms or cookies.

## Public pages

- Product landing page: https://approachtrainer.com/
- Privacy policy: https://approachtrainer.com/privacy/
- Support and bug reports: https://approachtrainer.com/support/

GitHub Pages publishes the repository root from `main`. Edit the HTML and shared `styles.css`, commit and push to update the site. Keep application source, internal documentation and credentials out of this repository.

For local preview, run `python3 -m http.server 8000` in this directory.

## Domain and publishing

`approachtrainer.com` is the dedicated Real Approach Trainer product domain; the application name and Grekon Studio publisher identity are unchanged. Porkbun handles registration, renewal and authoritative DNS. GitHub Pages serves the site with the apex hostname as its custom domain. Enable Enforce HTTPS after GitHub issues the certificate for the apex and `www` hostnames; verify secure access and redirects before considering a domain setup complete. The root `CNAME` file preserves that hostname when publishing from `main`.

DNS configuration, with a 600-second TTL:

| Name | Type | Value |
| --- | --- | --- |
| `@` | A | `185.199.108.153` |
| `@` | A | `185.199.109.153` |
| `@` | A | `185.199.110.153` |
| `@` | A | `185.199.111.153` |
| `@` | AAAA | `2606:50c0:8000::153` |
| `@` | AAAA | `2606:50c0:8001::153` |
| `@` | AAAA | `2606:50c0:8002::153` |
| `@` | AAAA | `2606:50c0:8003::153` |
| `www` | CNAME | `kgrech.github.io` |

Keep Porkbun's authoritative nameservers. Replace conflicting parking records, preserve unrelated email/verification records, and do not add wildcard DNS records. GitHub Pages redirects `www.approachtrainer.com` and the former `https://kgrech.github.io/real-approach-trainer-site/` URLs to the canonical domain. Each HTML page declares its own canonical URL; `robots.txt` advertises the three-page sitemap.

Use the authenticated Porkbun MCP connection for domain administration and authenticated GitHub Pages tooling for repository settings. Domain-specific API Access must be enabled in Porkbun. Credentials belong in the agent host's protected configuration, never this repository. The domain was registered on 5 November 2026 with an initial expiry of 5 November 2027. Porkbun quoted $11.81/year for registration and renewal on that date ($59.05 for five years at unchanged rates, excluding applicable taxes); this is a planning figure, not a purchase receipt or guaranteed future price. Auto-renew was enabled when inspected; any paid renewal or billing change requires owner authorization.

Future applications can have independent domains and repositories without changing this site's hostname. Adding an approved publisher subdomain instead requires a CNAME to the owning GitHub account's Pages hostname and a matching custom domain on that application's repository. One Pages site has one configured custom hostname.

For a future domain migration, arrange permanent HTTP redirects from the old hostname to the new one, preserving page paths; DNS alone cannot redirect. Update canonical metadata, sitemap, robots.txt, public documentation and app-store website/privacy/support links, verify the new property in Search Console and submit its sitemap, and use Change of Address where supported. Retain the old domain and redirects during migration. Search Console and store-console changes require their respective access and authorized scope. Account-level GitHub Pages domain verification can additionally protect the hostname; keep its generated TXT challenge record if configured.

## Design and assets

All three pages share the app's charcoal surfaces, amber accents, HSI icon, typography, navigation and footer. The landing page uses genuine app artwork and screenshots, responsive WebP images, and only FAA approach plates. See [asset credits](ASSETS.md) and [source mappings](assets/sources.json). Below-the-fold screenshots are lazy-loaded; all image dimensions are specified. Full-size screenshots are normalized for EXIF orientation before resizing.

Visible text is platform agnostic. Availability is “Coming soon”; no production or public beta link is claimed. Add a verified public store or beta URL only when available, distinguishing a free beta from the planned paid app. The buy-once wording promises no recurring fee to keep using the purchased app, not perpetual updates or support.

## Verification

Check all three pages at phone, tablet and desktop widths, keyboard navigation, links, image loading and absence of horizontal overflow. Ensure privacy wording still matches the app before changing data-handling claims. Verify the deployed pages over HTTPS after publication.
