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

### 2b. Spam address patterns (`site:theclapacademy.com casino -inurl:profile`)
- Results STILL include `/profile/` pages (`/profile/casino-jackpot-a...`, `/profile/livecasino4367`, `/profile/new-crypto-casi...`), so Google's `inurl:` filter is unreliable here and the earlier count of 25 profile pages is an undercount.
- Top-level addresses follow the same pattern: keyword + 4 digits (`/igaming-platform5541`, `/casino-aggregator9552`, `/cryptocurrencycasino4803`). That pattern is typical of **bot-generated usernames**.
- Titles carry author names ("...by Troy", "...by Ethan"), which points to content published by user accounts.
- **Revised conclusion:** most likely an open sign-up / user-content gap (fake accounts creating pages), not a hack. Confirm with the platform check and dashboard access.

### 3. Clean pages (`site:theclapacademy.com -casino -crypto -profile`)
- **About 27 results** (shown on page 3 of results, where Google's count is more accurate).
- Includes a subdomain, `portfolio.theclapacademy.com/project/...`, with student data-analysis projects (US Crime Analysis Report, Air Canada Express Customer Feedback Analysis, HR Employee Exit and Promotions Analysis). These look legitimate.
- So roughly 27 clean pages against about 7,340 indexed: well over 90% of the indexed site looks like spam (estimates only).

## Findings

| # | Finding | Type | Priority |
|---|---|---|---|
| 1 | About 7,340 pages indexed, about 2,970 mention casino. Spam (crypto casino, power tools) indexed under the site's domain, most likely through fake user accounts (bot usernames like keyword + 4 digits) | Security / spam / indexing | Critical |
| 2 | Only about 27 clean pages found against about 7,340 indexed, so the genuine site is buried under spam | Indexing / reputation | Critical |

## Still to check

- [x] **A1.** `site:theclapacademy.com casino`: about 2,970
- [x] **A2.** `site:theclapacademy.com inurl:profile`: only **25**, so most spam is NOT profile pages (possible hack or another open area)
- [x] **A3.** `site:theclapacademy.com casino -inurl:profile`: done, see 2b
- [ ] **Sign-up check:** find the Sign up / Join / Register / Log in button on the site and note what it offers (don't register)
- [ ] **A4.** Try `inurl:forum`, `inurl:blog`, `inurl:post`, `inurl:group` with `site:theclapacademy.com`
- [ ] **Platform:** what the site is built with (view source, or https://builtwith.com)
- [ ] **B. Real pages:** what the legitimate pages are, and how many
- [ ] **C. Sitemap:** `theclapacademy.com/sitemap.xml`
- [ ] **D. robots.txt:** `theclapacademy.com/robots.txt`
- [ ] **E. Branded search:** search "Clap Academy" and see what shows up
- [ ] **F. PageSpeed Insights (mobile):** https://pagespeed.web.dev/
- [ ] **G. Rich Results Test (structured data):** https://search.google.com/test/rich-results
