# The Clap Academy: Pre-Pitch SEO Check

- **Site:** https://theclapacademy.com
- **Business:** Career training for people from diverse and underrepresented backgrounds: practical skills, real-world experience and structured support for high-growth careers in the digital economy
- **Status:** In progress
- **Started:** 2026-10-31

## Checks completed

### 1. Indexed pages (`site:theclapacademy.com`)
- `site:theclapacademy.com` (Tools → result count): **about 7,340 results**
- `site:theclapacademy.com casino`: **about 2,970 results** (about 40% of everything indexed mentions casino)
- A training organization like this would normally have roughly 20–100 real pages, so the vast majority of the 7,340 is likely spam.
- Results include pages that have nothing to do with the business:
  - `/profile/cryptoonlinecasi...`: "See What Rainbet Crypto Casino Online Tricks The Celebs..."
  - `/cryptocurrencycasino4803`: "The 3 Greatest Moments In Rainbet Crypto Casino History..."
  - A guide about power tools in the United Kingdom

### 2. Where the spam sits
- Only 25 of the indexed pages are under `/profile/`. Most spam is elsewhere, e.g. root-level addresses like `/cryptocurrencycasino4803`.
- Note: Google's result counts are estimates and are unreliable at large numbers. Use them for scale, not as exact figures.

## Findings

| # | Finding | Type | Priority |
|---|---|---|---|
| 1 | About 7,340 pages indexed, about 2,970 mention casino. Spam (crypto casino, power tools) indexed under the site's domain, apparently through user profile pages or injected pages | Security / spam / indexing | Critical |

## Still to check

- [x] **A1.** `site:theclapacademy.com casino`: about 2,970
- [x] **A2.** `site:theclapacademy.com inurl:profile`: only **25**, so most spam is NOT profile pages (possible hack or another open area)
- [ ] **A3.** `site:theclapacademy.com casino -inurl:profile`: screenshot first 2 pages, note the URL patterns (folders) the spam sits in
- [ ] **A4.** Try `inurl:forum`, `inurl:blog`, `inurl:post`, `inurl:group` with `site:theclapacademy.com`
- [ ] **Platform:** what the site is built with (view source, or https://builtwith.com)
- [ ] **B. Real pages:** what the legitimate pages are, and how many
- [ ] **C. Sitemap:** `theclapacademy.com/sitemap.xml`
- [ ] **D. robots.txt:** `theclapacademy.com/robots.txt`
- [ ] **E. Branded search:** search "Clap Academy" and see what shows up
- [ ] **F. PageSpeed Insights (mobile):** https://pagespeed.web.dev/
- [ ] **G. Rich Results Test (structured data):** https://search.google.com/test/rich-results
