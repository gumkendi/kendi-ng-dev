# Kendi Ng — Portfolio Website Project Plan
> For implementation in Claude Code

---

## Project Overview

Build a personal portfolio website for a Marketing Analytics & Digital Marketing professional targeting Data Analyst, CRM Analytics, and Digital Marketing roles in Hong Kong. The site should be clean, professional, and technically credible — demonstrating both marketing domain expertise and data engineering capability.

**Target audience:** HK recruiters and hiring managers at banks, insurers, tech companies, and retail brands

**Live URL:** Custom domain (to be purchased — e.g. kendings.com or similar)
**Hosting:** GitHub Pages (free, signals technical credibility)
**Stack:** HTML / CSS / vanilla JS — clean and fast, no over-engineering

---

## Site Structure

```
index.html          ← Single page portfolio (all sections)
/assets
  /css
    style.css
  /js
    main.js
  /images
    profile.jpg
    project screenshots (anonymised)
  /videos
    (Loom embed links — no local video files)
README.md
```

---

## Section 1 — Hero / About

**Content:**
- Name: Kendi Ng
- Title line: `Marketing Analytics & Digital Strategist | Python & AI Integration | China Media | Hong Kong`
- 3-sentence positioning paragraph:

> I build data systems that turn raw marketing signals into business decisions — and I have spent 15 years understanding the platforms those signals come from. My background spans China media platforms (Baidu, Tencent, Douyin, RED) and international channels (Google, Meta, LinkedIn), and I have built my own analytics stack on top: Python ETL pipelines, PostgreSQL, self-built Streamlit dashboards, and production Claude AI API integration. I am looking for in-house roles in Hong Kong where data, marketing, and technology intersect.

**CTAs:**
- [View Projects] — anchor link to projects section
- [LinkedIn] — opens linkedin.com/in/[profile]
- [GitHub] — opens github.com/[username]
- [Download CV] — links to hosted PDF of Data Analyst CV

---

## Section 2 — Skills Matrix

Display as a clean grid grouped by category. Do NOT use a wall of text — use tag/badge style chips.

**Categories and skills:**

| Category | Skills |
|---|---|
| Data Engineering | Python, ETL Pipelines, PostgreSQL, SQL, VBA Excel, GitHub |
| Analytics & Visualisation | Streamlit, Looker Studio, GA4, Google Search Console, Power BI (learning) |
| Marketing Technology | Google Ads, LinkedIn Ads, GA4, GTM, Claude AI API, Azure Graph API, Google Apps Script |
| China & APAC Platforms | Baidu Search & Display, WeChat Moments Ads, Tencent Video, Douyin (platform trained), RED/Xiaohongshu (platform trained) |
| CRM & BA | Odoo CRM, Zoho CRM, Jira, UAT, Requirements Gathering, Data Mapping |
| Automation | Windows Task Scheduler, Microsoft Graph API, Outlook 365 automation, BeautifulSoup |

---

## Section 3 — Featured Projects

Each project card should include:
- Project title
- Problem statement (1 sentence)
- What was built (2-3 sentences)
- Tech stack badges
- Links: [GitHub] [Demo / Video] where available

---

### Project 1 — Marketing Analytics Dashboard (MAIN SHOWCASE)

**Title:** Self-Built Marketing Analytics App

**Problem:** Marketing and sales data sat in disconnected systems — LinkedIn Ads, Search Console, and website leads had no unified view, and Odoo CRM was missing historical data.

**What was built:** Built a complete data pipeline from scratch — LinkedIn Ads API and Google Search Console API pulling into a local PostgreSQL database on Windows Server, with a self-built Streamlit analytics application as the front end. The app provides cross-source campaign attribution, lead conversion analysis, and SEO keyword performance tracking in one place.

**Tech stack:** Python · PostgreSQL · Streamlit · LinkedIn Ads API · Search Console API · Windows Task Scheduler · Pandas

**Demo:** Loom screen recording (see recording instructions below)

**GitHub:** Link to anonymised ETL pipeline code

---

### Project 2 — AI-Powered SEO Reporting Pipeline

**Title:** Claude AI Executive Reporting System

**Problem:** Monthly SEO performance reporting required hours of manual analysis and formatting before it could be sent to senior management.

**What was built:** Integrated Claude AI API with Google Apps Script and Search Console API to automatically generate HTML executive summaries with MoM and YoY keyword analysis across Brand and Focus keyword segments. Reports are distributed automatically to 9 stakeholders via Microsoft Azure Graph API on a scheduled basis — zero manual intervention.

**Tech stack:** Claude AI API · Google Apps Script · Search Console API · Azure Graph API · HTML · JavaScript

**GitHub:** Link to Apps Script code (anonymised)

**Note:** Show a sample anonymised output report as a screenshot or PDF

---

### Project 3 — Job Application Tracker Automation

**Title:** Automated Job Application Tracker

**Problem:** Manually tracking dozens of concurrent job applications across JobsDB was time-consuming and error-prone.

**What was built:** Python automation that reads Outlook 365 emails from JobsDB via Microsoft Graph API, parses application status updates (confirmations, rejections, employer views), and updates an Excel tracking file on OneDrive automatically. Runs hourly via Windows Task Scheduler.

**Tech stack:** Python · Microsoft Graph API · Azure AD · openpyxl · BeautifulSoup · Windows Task Scheduler · OneDrive

**GitHub:** Link to full code

**Note:** This is a good one to show — it is original, useful, and demonstrates Azure AD + Graph API competency. Fully public since it contains no client data.

---

### Project 4 — CRM Lead Assignment App

**Title:** Streamlit Lead Assignment App

**Problem:** Sales team was manually assigning inbound leads with no consistent logic, causing uneven workload distribution and delayed follow-up.

**What was built:** Self-built Streamlit web application with weighted lead distribution logic deployed to the sales team. Built independently when the CRM system could not support the required assignment rules and dev team capacity was unavailable.

**Tech stack:** Python · Streamlit · Weighted Distribution Algorithm

**Demo:** Loom screen recording (see recording instructions below)

---

### Project 5 — Zoho CRM Migration Consulting (Freelance)

**Title:** CRM Migration Planning — Social Enterprise Research Academy

**Problem:** Client needed to migrate from legacy system to Zoho CRM with no internal technical resource to manage the process.

**What was built:** Led the full migration planning engagement as sole consultant — conducted stakeholder requirements interviews, evaluated Zoho CRM modules against business needs, and produced complete data mapping documentation for the migration.

**Deliverables shown:** Anonymised data mapping template / requirements framework (PDF or screenshot)

**Note:** No code to show — this is a BA/consulting project. Show the documentation artefact.

---

## Section 4 — Career Timeline

Simple visual horizontal timeline:

```
2007 ──── 2010 ──── 2015 ──── 2024 ──── Now
 AXA    Publicitas   iClick          Gain Miles
Finance  APAC Pubs  China Media    MPF/Insurance
                   Senior Dir.    CRM & Analytics
```

Keep it minimal — years, company, one-line role description. Not a full CV repeat.

---

## Section 5 — Contact

- Email: kendi@leary.hk
- LinkedIn: [link]
- GitHub: [link]
- Location: Hong Kong

Simple clean footer. No contact form needed.

---

## Loom Screen Recording Instructions

> Complete these BEFORE building the site — you need the embed links

### For Streamlit Analytics App (Project 1):

**Before recording:**
1. Replace all real company/client names in the displayed data with generic labels:
   - Company names → "Client A", "Client B" etc.
   - Personal names → "User 1", "User 2" etc.
   - Use Python to create a demo dataset with fake but realistic-looking data
   - OR blur sensitive fields using screen recording software (Loom supports blur regions on paid plan — free plan: use fake data instead)

**What to record (60-90 seconds):**
1. Show the app loading — establish it is a real working application
2. Show the main dashboard with campaign performance charts (fake data)
3. Click into one attribution view — show LinkedIn Ads → lead conversion flow
4. Show the SEO keyword performance table
5. Show one filter interaction — demonstrate it is dynamic not static
6. Narrate throughout: "This pulls from LinkedIn Ads API and Search Console API into PostgreSQL, updated daily via Windows Task Scheduler"

**Free data anonymisation approach:**
```python
# Run this before recording to replace real data with fake data in your DB
# Create a demo_mode flag in your Streamlit app that loads fake data instead
import pandas as pd
import random

fake_companies = ["Acme Corp", "Beta Finance", "Gamma Insurance", "Delta Group"]
fake_names = ["Alice Wong", "Bob Chan", "Carol Lee", "David Ng"]
# Replace real values in display with these
```

### For Lead Assignment App (Project 4):

**What to record (30-45 seconds):**
1. Show the input form — adding a new lead
2. Show the weighted assignment logic running
3. Show the output — which sales rep was assigned and why
4. No real data needed here — just use test names

---

## GitHub Repository Setup

Create these public repositories before building the site:

| Repo Name | Contents | Notes |
|---|---|---|
| `marketing-analytics-etl` | LinkedIn Ads API + Search Console API → PostgreSQL ETL scripts | Anonymise company-specific config, keep logic |
| `ai-seo-reporter` | Google Apps Script + Claude AI API reporting pipeline | Remove API keys, add .env.example |
| `job-application-tracker` | Full Python automation code | Safe to publish as-is, no client data |
| `streamlit-lead-assignment` | Lead assignment app code | Remove any real sales rep names |
| `portfolio` | The portfolio website itself | This is also the GitHub Pages source |

**Each repo needs:**
- Clear README.md explaining what it does, why it was built, and how to run it
- requirements.txt or package.json
- .env.example showing what environment variables are needed (never commit real keys)
- Screenshots in README where possible

---

## Design Direction

**Tone:** Professional but not corporate. Clean, data-forward aesthetic.

**Colour palette suggestion:**
- Primary: Deep navy `#1a2744` (financial services credibility)
- Accent: Teal `#00b4a6` (modern, tech-forward)
- Background: Off-white `#f8f9fa`
- Text: Dark grey `#2d3748`

**Typography:**
- Headings: Inter or Plus Jakarta Sans (Google Fonts, free)
- Body: Inter
- Code snippets: Fira Code or JetBrains Mono

**Project cards:** Clean card layout with subtle shadow, tech stack as coloured badges, clear CTA buttons

**Mobile responsive:** Yes — recruiters will check on phone

---

## Implementation Order for Claude Code

1. Set up GitHub repo and GitHub Pages
2. Build HTML structure (all sections, no styling)
3. Add CSS — layout, typography, colour palette
4. Build project cards with placeholder content
5. Add skills matrix
6. Add career timeline
7. Add Loom video embeds once recordings are done
8. Add GitHub repo links once repos are set up
9. Connect custom domain
10. Test on mobile
11. Add CV PDF download link
12. Final review and deploy

---

## Domain Suggestions

Short, professional, memorable:
- `kendimg.com` — initials + mg (marketing/manager)
- `kendings.com` — name based
- `kendi-ng.com` — explicit name
- `kendi.dev` — signals technical credibility, .dev domains cost ~$12/year

Avoid: anything with "portfolio" or "hire me" in the domain — looks junior.

---

## What NOT to Include

- Real client names, company names, or data from Gain Miles
- Real performance numbers from client campaigns
- Any iClick client data
- Photos of colleagues
- Salary information
- Anything behind NDA

When in doubt — anonymise or omit.

---

## Timeline Estimate

| Task | Time |
|---|---|
| Record Loom videos (with fake data prep) | 2-3 hours |
| Set up GitHub repos with READMEs | 2-3 hours |
| Build portfolio site in Claude Code | 3-4 hours |
| Connect domain + test | 1 hour |
| **Total** | **~1 day** |

---

*Generated as project brief for Claude Code implementation*
*Kendi Ng | kendi@leary.hk*
