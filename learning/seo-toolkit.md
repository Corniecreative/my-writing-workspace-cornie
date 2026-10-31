# My SEO Toolkit

Tools, searches and links I've actually used in real checks, what each one is for, and how to use it next time.
First used on: Glenala Education and The Clap Academy (October 2026).

---

## 1. Google search operators

Type these straight into the Google search box. No tools or access needed.

| Search | What it does | Why I use it | Example |
|---|---|---|---|
| `site:domain.com` | Shows every page Google has indexed for that site (subdomains included) | See how many pages Google holds, and spot junk | `site:glenala.co.uk` |
| `site:domain.com word` | Only indexed pages that mention that word | Measure a problem, e.g. spam | `site:theclapacademy.com casino` |
| `-word` | Excludes results containing that word | Strip out the junk to see the real pages | `site:theclapacademy.com -casino -crypto -profile` |
| `inurl:word` | Only pages whose web address contains that word | Find a section of the site, e.g. profiles | `site:theclapacademy.com inurl:profile` |
| `-inurl:word` | Excludes pages whose address contains that word | Find pages outside a section | `site:theclapacademy.com casino -inurl:profile` |
| `"exact phrase"` | Only results with that exact phrase | Brand checks | `"The Clap Academy"` |
| Brand name, no operators | What a normal person sees | Check the brand isn't damaged, find the Business Profile, other domains and reviews | `Clap Academy` |

**How to get the result count**
1. Run the search.
2. Click **Tools** (right, under the search box) → the count appears ("About 7,340 results").
3. For a more accurate number, click through to the **last page of results**, then check Tools again.
4. If Google says it "omitted some entries very similar", click **"repeat the search with the omitted results included"** and count again.

**Lessons learned**
- Counts are **estimates**: in a pitch say "thousands", not "7,340".
- `inurl:` is **not reliable**: it still showed profile pages when I excluded them. Treat it as a clue.
- `site:domain.com` works without `https://` or a trailing slash. That's the standard form.
- **Never click spam results**: read the address and title from the results page only.

---

## 2. Checks in the browser address bar

| Type this | What it shows | What to look for |
|---|---|---|
| `domain.com/sitemap.xml` | The list of pages the site wants Google to index | How many pages; do they match what Google has indexed? |
| `domain.com/sitemap_index.xml` or `domain.com/wp-sitemap.xml` | Same, for other setups (WordPress) | Use if the first one errors |
| `domain.com/robots.txt` | The instructions to search engine bots | A `Sitemap:` line at the bottom; nothing important under `Disallow:`; `Disallow: /` alone = whole site blocked |
| The non-www or old domain, e.g. `glenala.co.uk/funding` | Whether the site redirects | Does the address change? (www vs non-www, old domain → new) |

**Counting pages in a sitemap:** on the sitemap page press **Ctrl + F**, type `https://domain` → the box shows "1/12". The number after the slash = total pages.

**Comparing the two numbers**
| Result | Meaning |
|---|---|
| Google count much **lower** than the sitemap | Pages aren't being indexed |
| Google count much **higher** | Junk or duplicate pages are indexed (this is how I found the Clap Academy spam) |
| Roughly equal | Indexing looks fine |

**Sitemap red flags I've seen:** every page with the same `lastmod` date and set to "daily" (auto-generated, not maintained); sitemap uses a different version of the domain from Google's (non-www vs www).

---

## 3. View page source

**How:** open the page → **Ctrl + U** (Mac: Cmd + Option + U) → **Ctrl + F** to search inside it.

| Search for | Why |
|---|---|
| A sentence you can see on the page | If it's missing, the content loads by JavaScript and bots may not see it (common on AI-built sites) |
| `<title>` | Is there a page title, and is it different on each page? |
| `name="description"` | Is there a meta description? |
| `noindex` | If on an important page, it's telling Google not to index it |
| `wp-content` / `wix` / `squarespace` / `webflow` | Which platform built the site |

---

## 4. Free websites

| Tool | Link | What I used it for | How |
|---|---|---|---|
| **BuiltWith** | [builtwith.com](https://builtwith.com) | Find what a site is built on (found WordPress 6.7 + Tutor LMS on Clap Academy) | Type the domain → scroll to **Content Management System**. Ignore Analytics/Tracking for this question |
| **httpstatus.io** | [httpstatus.io](https://httpstatus.io) | Check redirect type (found `301 → 301 → 200` on clapacademy.co.uk) | Paste the address → **Check status** → read the codes left to right |

**Status codes to remember**
| Code | Means |
|---|---|
| 200 | Page loaded fine |
| 301 | Permanent redirect ✅ right for a domain move |
| 302 | Temporary redirect ❌ wrong for a domain move |
| 404 | Page not found |
| Two redirects in a row | A redirect chain (works, but one hop is cleaner) |

*Optional alternative to BuiltWith:* the Wappalyzer browser extension shows the same thing while you're on the site.

---

## 5. Things to look at in Google's results page

| What | Where | What it told me |
|---|---|---|
| **Google Business Profile** | Box on the right of a brand search | Clap Academy: 4.8★, 54 reviews, but "Add website" = no website linked |
| **Sitelinks** | Links under the homepage result | Clap Academy: 3 of 6 were Login/Registration pages |
| **People also search for** | Right panel or bottom of results | Unrelated businesses = Google is unsure what the brand is |
| **Other domains and review sites** | Normal results for the brand | Found the old clapacademy.co.uk and Trustpilot under it |

---

## 6. My pre-pitch check, in order

1. `site:domain.com` → indexed count (Tools)
2. `domain.com/sitemap.xml` → page count (Ctrl + F)
3. Compare the two
4. If the count is much higher → `site:domain.com` + spam words (`casino`, `crypto`) and `-word` searches to size it
5. `domain.com/robots.txt`
6. View source on 2–3 pages
7. BuiltWith → platform
8. Brand search → Business Profile, sitelinks, other domains
9. httpstatus.io → any redirects
10. PageSpeed Insights (mobile score)

---

## 7. Next tools to learn (not used yet)

| Tool | Link | For |
|---|---|---|
| PageSpeed Insights | [pagespeed.web.dev](https://pagespeed.web.dev/) | Mobile speed and Core Web Vitals (aim for 70+ on mobile) |
| Rich Results Test | [search.google.com/test/rich-results](https://search.google.com/test/rich-results) | Structured data (schema) |
| Screaming Frog | [screamingfrog.co.uk/seo-spider](https://www.screamingfrog.co.uk/seo-spider/) | Full site crawl: broken links, titles, descriptions, images (free up to 500 URLs) |
| Google Search Console | [search.google.com/search-console](https://search.google.com/search-console) | Real indexing data, crawl stats, manual actions. Needs the owner's access, so it's for paid audits |
| SEO Pro Chrome extension | Chrome Web Store | Quick checks of status codes, canonicals and robots.txt on the page you're on |

---

## 8. Client communication rules

- Call the first look a **"first SEO health check"**, not an audit. The full technical audit is the paid next step.
- **Show what you found, never how you found it.** Crop search bars from screenshots; no tool names; no DIY fix steps.
- Use rounded numbers and "most likely" for causes you haven't confirmed.
- Lead with the biggest risk, add one quick win, keep the rest for the call.
