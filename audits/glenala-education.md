# Glenala Education: Pre-Pitch SEO Check

- **Site:** https://www.glenala.co.uk
- **Business:** Training / education provider (Hamilton and Lanark, near Glasgow), full-time, part-time and evening courses, international students
- **Status:** In progress
- **Started:** 2026-10-30

## Checks completed

### 1. Indexed pages (`site:glenala.co.uk`)
- Google shows **10 results**. Same 10 after "repeat the search with the omitted results included".

### 2. Sitemap (`glenala.co.uk/sitemap.xml`)
- **12 pages** listed.

| # | Sitemap page | Indexed? |
|---|---|---|
| 1 | / (homepage) | Yes |
| 2 | /courses | Yes |
| 3 | /business-solutions | Yes |
| 4 | /employability-skills | Yes |
| 5 | /contact-us | Yes |
| 6 | /testimonials | Yes |
| 7 | /business-blogs | **No** |
| 8 | /international | Yes |
| 9 | /international-student-agency | **No** |
| 10 | /understanding-scqf | Yes |
| 11 | /funding | Yes |
| 12 | /legal-notice | Yes |

**Result:** 10 of 12 indexed (83%).

### 3. Course pages
- All courses are listed on `/courses` only. No course has its own page.

## Findings

| # | Finding | Type | Priority |
|---|---|---|---|
| 1 | No individual course pages, so nothing can rank for specific course searches | Architecture / content | High |
| 2 | 2 of 12 sitemap pages not indexed (business-blogs, international-student-agency) | Indexing | Medium (cause not known yet) |
| 3 | No blog posts in the sitemap | Indexing / content | Medium |
| 4 | Sitemap uses non-www addresses (`glenala.co.uk`), Google shows www | Technical | To confirm |
| 5 | All sitemap dates identical (2023-10-23) and every page set to "daily" | Technical | Low |

## Still to check

- [ ] **A. Redirect:** open `https://glenala.co.uk/funding` and see whether it changes to `www.glenala.co.uk/funding`
- [ ] **B. Non-indexed pages:** open `/business-blogs` and `/international-student-agency`. Do they load properly? View source (Ctrl + U), search for `noindex`
- [ ] **C. Blog:** does `/business-blogs` link to individual posts with their own addresses?
- [ ] **D. robots.txt:** open `glenala.co.uk/robots.txt`
- [ ] **E. Page source:** check 2–3 pages for unique titles, meta descriptions and visible text in the source
- [ ] **F. PageSpeed Insights (mobile):** https://pagespeed.web.dev/
- [ ] **G. Rich Results Test (structured data):** https://search.google.com/test/rich-results
- [ ] **H. Screaming Frog crawl:** broken links, missing or duplicate titles

## Pitch line (draft)

> "When a student searches for a specific course, like 'SVQ Health and Social Care Hamilton', Google looks for a page about that course. Right now, all your courses share one page, so Google has nothing specific to show. Giving each course its own page is the single biggest opportunity on your site."
