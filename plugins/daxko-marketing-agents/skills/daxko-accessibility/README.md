# Agent 43 — Accessibility — teammate guide

**Skill:** `daxko-accessibility` · **Owner:** Abid Siddiqui · **Version:** 1.7.37

## What it does
Checks one web page, page design, form, email or document you paste for accessibility — whether people with disabilities can use it (screen-reader users, keyboard users, people with low vision, deaf or hard-of-hearing people). It works for a Digital Services client's site or a Daxko page. You get each barrier in plain words: where it is, who it blocks, how to fix it and how sure it is, plus draft fixes for the developer. It also writes alt text for images you describe and computes colour contrast from colour codes you paste. If the page is missing, it first asks up to 3 short questions: the page, whose site and which page, and which standard (for example WCAG 2.2 AA).

## Requests to try
- "Check this page for accessibility" (paste the HTML)
- "Is this form screen-reader friendly?" (paste the form)
- "Write alt text for these images" (describe each image)
- "Do these colours pass contrast? #777777 text on #FFFFFF"

## What you get
SCOPE, a summary with the 3 barriers to fix first, a findings table, a "can't check from a paste" list, fixes under **DRAFT FIXES — needs the site's developer or editor before anything changes**, then internal notes, a NOT ON FILE list and sources with dates.

## Good to know
- Daxko has no WCAG file (owner decision 2026-11-13). Any WCAG rule it names from general knowledge is marked "confirm". Paste your team's checklist if you have one.
- It never says a site is "compliant", "passes" or "ADA-safe" and never gives a score. It finds likely barriers; a full check needs a person testing with real tools.
- It checks only what you paste. It does not fetch a URL, crawl a site or run a scanner. It pulls a page from a connector only if you say yes, read-only.
- It does not accept an "accessibility overlay" widget as a fix, and gives no legal advice.
- For Daxko pages it uses only the colours in Daxko's brand file; a client's colours only as you paste them.
- Passwords or personal details in your paste are left out.

## What it will NOT do — and who does
| Ask | Owner |
|---|---|
| Broken forms, links, menus | Agent 32 — QA & Testing |
| Brand compliance of a Daxko page | `daxko-brand-qa` |
| Rewriting page copy | Agent 35 — Web Content |
| Conversion · SEO | `daxko-page-cro` / `daxko-form-cro` · `daxko-seo-audit` |
| Site structure | Agent 28 — Information Architecture |
| Legal questions (lawsuits, demand letters) | Daxko's legal team |
| Changing the live site | the site's developer or owner |
| Gong or multi-touch sequence | `gong-sequence-builder` (your own skill) |
