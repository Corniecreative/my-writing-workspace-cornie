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

### 4. Platform and likely gap
- **WordPress 6.7 + Tutor LMS.** Tutor LMS gives each registered student/instructor a public profile page at `/profile/username`, which matches the spam addresses (`/profile/livecasino4367`).
- Likely gap: open registration (student and/or "become an instructor") + public profiles indexable by Google + no CAPTCHA / approval.
- Top-level spam addresses (`/igaming-platform5541`) still need explaining: posts by registered users with publishing rights, or a hack. Confirm with dashboard access and a security scan.
- WordPress 6.7 is not the latest version: outdated core/plugins are a security risk.

### 5. Brand search (`Clap Academy`)
- **No casino pages on page 1.** Homepage ranks first with sitelinks. Brand reputation is not visibly damaged yet.
- Sitelinks shown: Course, **Login**, **Registration**, AI & Automation, **Student Registration** (form: First Name, Last Name, User Name, E-Mail, Password), Project Management with AI. Confirms a public, indexed student sign-up form (the likely door for bots). Three of six sitelinks are login/registration pages instead of programmes. The "Registration" sitelink description reads "Welcome Back · Enter your details to log into the platform" (login text on a registration page).
- **Second domain:** `clapacademy.co.uk` also ranks (About page), and Trustpilot reviews are filed under `clapacademy.co.uk`. Two websites for one brand.
- **Google Business Profile:** "Clap Academy", 4.8 stars, 54 Google reviews, Training centre, phone 07722 936139, hours listed, but shows **"Add website"**: no website linked.
- Other profiles: LinkedIn (210+), Instagram (40+), YouTube, X, Facebook, Skool community.
- Homepage: hero "Break Into High-Demand Tech Roles...", buttons "Book a Free 1-to-1 Career Call" and "Join our community"; AI chat assistant "Chima" built on Zapier.
- "People also search for" shows unrelated children's schools and daycares: Google's understanding of what the brand is looks weak.

## Findings

| # | Finding | Type | Priority |
|---|---|---|---|
| 1 | About 7,340 pages indexed, about 2,970 mention casino. Spam (crypto casino, power tools) indexed under the site's domain, most likely through fake user accounts (bot usernames like keyword + 4 digits) | Security / spam / indexing | Critical |
| 2 | Only about 27 clean pages found against about 7,340 indexed, so the genuine site is buried under spam | Indexing / reputation | Critical |
| 3 | WordPress + Tutor LMS public profiles and open registration with no bot protection (likely gap) | Security / configuration | Critical |
| 4 | WordPress 6.7, not the latest version | Security | High |
| 5 | Two domains for one brand (theclapacademy.com and clapacademy.co.uk), Trustpilot tied to the .co.uk | Technical / authority | Low–Medium: .co.uk 301-redirects to .com (2-hop chain); Trustpilot, old Google results and profile links still point to .co.uk |
| 6 | Google Business Profile has no website linked (54 reviews, 4.8 stars) | Local SEO | High, quick win |
| 7 | Sitelinks dominated by Login / Registration pages; registration page shows login text | On-page / architecture | Medium |
| 8 | Weak brand entity signals (unrelated "People also search for") | Structured data / entity | Medium |

## Still to check

- [x] **A1.** `site:theclapacademy.com casino`: about 2,970
- [x] **A2.** `site:theclapacademy.com inurl:profile`: only **25**, so most spam is NOT profile pages (possible hack or another open area)
- [x] **A3.** `site:theclapacademy.com casino -inurl:profile`: done, see 2b
- [ ] **Sign-up check:** find the Sign up / Join / Register / Log in button on the site and note what it offers (don't register)
- [ ] **A4.** Try `inurl:forum`, `inurl:blog`, `inurl:post`, `inurl:group` with `site:theclapacademy.com`
- [x] **Platform:** BuiltWith CMS = **WordPress 6.7 + Tutor LMS** (course plugin). HighLevel is used for CRM/marketing only.
- [ ] **B. Real pages:** what the legitimate pages are, and how many
- [ ] **C. Sitemap:** `theclapacademy.com/sitemap.xml`
- [ ] **D. robots.txt:** `theclapacademy.com/robots.txt`
- [x] **E. Branded search:** done, see section 5
- [x] **H. Second domain:** typing `clapacademy.co.uk` lands on `theclapacademy.com`, confirmed with https://httpstatus.io: `http://clapacademy.co.uk` → **301 → 301 → 200** (2 permanent redirects in a chain). Correct type; a single hop would be cleaner (low priority)
- [ ] **F. PageSpeed Insights (mobile):** https://pagespeed.web.dev/
- [ ] **G. Rich Results Test (structured data):** https://search.google.com/test/rich-results

## Proposed fix plan (for the paid engagement)

1. **Close the door:** Tutor LMS settings: turn off public profiles (or noindex them); review student and instructor registration; WordPress Settings → General → check "Anyone can register" and the default role; add a CAPTCHA (e.g. Cloudflare Turnstile or reCAPTCHA) and email verification / manual approval.
2. **Rule out a hack:** security scan (e.g. Wordfence), check admin users, update WordPress core, themes and plugins.
3. **Clean up:** bulk-delete spam accounts and their content; spam URLs should return 404/410.
4. **Get Google to drop them:** Search Console → Removals for urgent patterns (e.g. `/profile/` prefix), resubmit a clean sitemap, check the Manual actions and Security issues reports.
5. **Monitor:** recheck `site:` counts weekly until spam falls out of the index.

## WhatsApp message draft (friendly, person known)

Rule: show what was found, never how it was found. Crop search bars from screenshots; no tool names or DIY steps.

**Message 1**
Hey [Name]! I've done a first SEO health check on the Clap Academy website. This is just the first layer: a full technical audit and the fixes would come after. But I already found a few things you need to know about, and one of them is serious. I've put it all together below with screenshots 👇

**Message 2** *(screenshot: casino results, search bar cropped out)*
1️⃣ **The big one: casino spam on your website**

Google is showing pages on your website like:
• "Rainbet Crypto Casino Online Tricks The Celebs..."
• "The 3 Greatest Moments In Rainbet Crypto Casino History"
• Even a guide to power tools in the UK 😅

None of that is yours. Going by Google's own estimates:
• Around **7,300 pages** indexed under theclapacademy.com
• Around **3,000** of them mention "casino"
• Only about **27** look like your actual pages

A training academy would normally have around 20–100 real pages. So almost everything Google holds for your site is junk.

**Message 3** *(no screenshot)*
**How it's happening (most likely):**
Bots are signing up through your student registration and creating thousands of fake accounts with names like "livecasino4367". Each one gets a public profile page, which they fill with casino content, and Google indexes it all under your name.

**Why spammers do it:** Google trusts your site more than theirs, so they borrow your reputation to push casino pages.

**Why it matters:** it hasn't shown up when people search "Clap Academy" yet, but if Google decides your site is spammy, it can push down your real pages too, including your programmes. Some of your website software is also out of date, which is a security risk.

**Message 4** *(screenshot: Google Business Profile showing "Add website")*
2️⃣ **Quick win: your Google Business Profile**
You've got 4.8 stars from 54 Google reviews, which is brilliant! But there's no website linked, so people who find you there can't click through to your site.

3️⃣ **Smaller things I noticed:**
• Under your homepage in Google, 3 of the 6 links are Login/Registration pages instead of your programmes
• Google isn't 100% sure what Clap Academy is yet: it's associating you with children's schools and daycares
• Your old clapacademy.co.uk redirects properly to the new site 👍 but your Trustpilot is still under the old domain

**Message 5**
**What I'd do to fix it:**
1. Close the gap the bots are using so it can't happen again
2. Check the site hasn't been compromised and secure it
3. Remove all the spam accounts and pages
4. Get Google to drop the spam from its index
5. Monitor it until your site is clean

**Message 6**
To confirm exactly how they're getting in and how big it really is, I'd need access to your Google Search Console and the website dashboard, and that's when I'd do the full technical audit.

Happy to jump on a call and walk you through it. When are you free this week? 😊
