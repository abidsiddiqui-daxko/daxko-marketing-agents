> **SOURCE FILE:** `drop-your-updated-files-here/daxko-ai/shared-knowledge-base/performance-data-schema.md`  ·  **LAST UPDATED:** 2026-08-11 (file date — no "last updated" line stated inside the document)  ·  **ORIGIN:** FRESH — from your drop folder  ·  **Placed in Agent HQ:** 2026-08-11

# Performance Data Schema

> KPI definitions, attribution model, and reporting standards.
> Used by Strategy & OKR Copilot, Performance & Insights, and Experimentation & CRO agents.

---

## Pipeline Attribution Model

Standard funnel stages for all markets:

```
MQL → SQL → Opportunity → Closed Won
```

| Stage | Definition |
|-------|-----------|
| **MQL** (Marketing Qualified Lead) | Lead has demonstrated intent — content download, demo request, multi-page visit, or fits ICP firmographic criteria |
| **SQL** (Sales Qualified Lead) | Lead has been qualified by sales — confirmed budget, authority, need, and timeline (BANT) |
| **Opportunity** | Active sales motion with documented next steps in Salesforce |
| **Closed Won** | Signed contract, revenue recognized per accounting standards |

---

## Pipeline Coverage Targets

| Market | New Logo coverage | Expansion coverage |
|--------|-------------------|---------------------|
| Nonprofit | 3x | 2x |
| Club | 3x | 2x |
| Boutique | N/A | N/A |

Pipeline coverage is calculated on a rolling 90-day forward basis.

---

## Core KPI Definitions

### Bookings
**Definition:** Total annual contract value (ACV) of contracts signed in the period.
**Source:** Salesforce closed-won opportunities
**Cadence:** Tracked monthly, reported quarterly against $41.8M target

### GRR (Gross Revenue Retention)
**Definition:** Percentage of recurring revenue retained from existing customers, excluding upsell/expansion. Calculated as (Starting ARR − Churn ARR − Downgrade ARR) / Starting ARR.
**Source:** Finance / NetSuite
**Cadence:** Monthly

### Recurring Revenue
**Definition:** Annualized run-rate revenue from subscription contracts.
**Source:** Finance
**2026 target:** $217.0M (10.5% YoY)

### AI-Enabled Bookings
**Definition:** Bookings where the closed-won opportunity has an AI product or AI-enabled SKU on the contract (Engage AI Agents, Member Intelligence 360, Smart Sending Engine, ZP Engage AI).
**2026 target:** $2.4M

### Deal Velocity
**Definition:** Average days from Opportunity Created to Closed Won.
**2026 target:** 10% improvement across all markets

### Decision-Maker NPS
**Definition:** Net Promoter Score from designated decision-maker contacts at customer accounts (e.g. Customer Advisory Board accounts for Nonprofit).
**Calculation:** % Promoters (9–10) − % Detractors (0–6)

### Product NPS
**Definition:** Per-product NPS from active users.
**2026 targets:** DO: 13 · CA: 2 · ZP: 6 · Exercise: 6

### eNPS (Employee NPS)
**Definition:** Internal employee engagement NPS.
**2026 target:** Increase from 15 to 20

### Daxko Reputation Index
**Definition:** Composite score across review platforms (G2, Capterra, Trustpilot, App Store) and earned media sentiment.
**2026 target:** Improve by 10%

### Mobile App Rating
**Definition:** Average star rating on Apple App Store and Google Play for next-gen NP, CA, and ZP apps.
**2026 target:** ≥4.5 by Q4 2026

### System Uptime SLA
**Definition:** Percentage of time platform is operational, measured monthly against contractual SLA.
**2026 target:** 99.99% (CA delivered uptime: 99.9998%)

### ART (Average Resolution Time)
**Definition:** Average time from case open to case closed for customer support tickets.
**2026 target:** <8 days while maintaining >9 customer satisfaction

### Post-Release Stability
**Definition:** Percentage of releases that ship without critical (S1/S2) bugs within 28 days.
**2026 target:** 85%

### Critical Defect Resolution
**Definition:** Time from S1/S2 bug report to production fix.
**2026 target:** Within 30 days (2 sprints)

### Cases per Customer
**Definition:** Average support cases opened per customer per month.
**2026 target:** Reduce by 15%

---

## Market-Specific KPIs

### Nonprofit

| KPI | Target | Notes |
|-----|--------|-------|
| Total pipeline | $25.9M | New Logo $9.7M + Expansion $16.2M |
| BGC market share | 27% (229 customers) | Buying universe: 850 orgs |
| YMCA market share (>$20M orgs) | 65% — 55 of 85 | Tier 1+2 accounts |
| Cash Discounting bookings | $800k ARR | New product line |
| Community Rec new logo pipeline | ~$1.03M | Scaled target |
| ART reduction | 20% | Service quality |
| Mobile app rating | 4.5+ with 80+ reviews | Next-gen NP app |

### Club

| KPI | Target | Notes |
|-----|--------|-------|
| SSS net revenue positive YoY | 70% of customers | Core objective 1 |
| Card approval rate | +5% by Dec 31, 2026 | Payment optimization |
| Implementation configuration time | -10% to -25% | Velocity |
| V1 → V2 upgrades | 50+ customers | Platform modernization |
| Online joins self-service (V2) | 40% | Member experience |
| NPS — CA | ≥2 | |
| NPS — Engage Pro | ≥13 | |
| Mobile app rating — CA | ≥4.5, 100+ reviews | |
| Platform uptime SLA | 99.99% | Across all Club platforms |

### Boutique

| KPI | Target | Notes |
|-----|--------|-------|
| Total bookings | $9,884,869 | 186.4% YoY (includes Exercise.com) |
| Net revenue growth | 3.4% | While growing MMS units by 100 |
| Decision Maker NPS | ≥10 | |
| Monthly churn reduction | 10% per platform | Unit and revenue churn |
| Martial Arts market penetration | ~6% → 7% | |
| Functional Fitness market penetration | ~5.5% → 7% | |
| Marketplace revenue growth | 10% YoY | |
| Online/Hybrid NPS | ≥15 | |

---

## Reporting Cadence

| Report | Cadence | Owner |
|--------|---------|-------|
| Pipeline attainment | Weekly | Market strategists |
| Bookings vs. target | Monthly | Finance + Strategy |
| Campaign performance | Bi-weekly | Performance & Insights agent |
| KR status (on-track / at-risk / off-track) | Monthly | Strategy & OKR Copilot |
| Cross-market patterns | Quarterly | Performance & Insights agent |

---

## Performance Report Schema (Performance → Strategist)

```yaml
vertical: [nonprofit | club | boutique]
period: ""
headline_insight: ""        # Single most important takeaway
kr_status:                  # KR: on-track | at-risk | off-track
  kr_name: status
top_campaigns:              # What's working
  - name: ""
    why: ""
    next_steps: ""
underperformers:            # What's not
  - name: ""
    hypothesis: ""
    action: ""
cross_market_patterns: []
recommended_actions: []
```

---

---

## Carried Forward From the Previous Version

> **PROVENANCE.** The section(s) below were present in the pre-May 2026 `daxko-ai/shared-knowledge-base/performance-data-schema.md`
> (Nick Lindauer / Claude) and did not survive the May rewrite. They are reproduced verbatim on
> 2026-08-05 so no data is lost in consolidation. Nothing above this line was altered.
> Where the older text conflicted with a correction Abhishek made, the conflicting lines were
> removed rather than reproduced — any such removal is noted below.

## KPI Definitions

### Marketing KPIs
| KPI | Definition | Data Source | Reporting Frequency |
|-----|-----------|-------------|---------------------|
| Pipeline Generated | Total $ value of Opportunities created from marketing-sourced leads | Salesforce CRM | Weekly |
| MQL Volume | Number of leads meeting qualification threshold | MAP (HubSpot / Marketo) | Weekly |
| MQL→SQL Rate | % of MQLs accepted by sales | CRM | Bi-weekly |
| Cost per MQL | Total marketing spend divided by MQL volume | Finance + MAP | Monthly |
| Content Engagement | Average engagement rate across published content | CMS + Social tools | Weekly |
| Email Performance | Open rate, CTR, and unsubscribe rate | MAP | Per send |

### Market-Specific Targets
| KPI | Nonprofit | Club | Boutique |
|-----|-----------|------|----------|
| Pipeline target (quarter) | [AWAITING SME] | [AWAITING SME] | [AWAITING SME] |
| Avg deal size | [AWAITING SME] | [AWAITING SME] | [AWAITING SME] |
| Avg sales cycle | 6-18 months | 3-6 months (single) / 6-12 months (multi) | Days to weeks |
| Key conversion bottleneck | [AWAITING SME] | [AWAITING SME] | [AWAITING SME] |

---

## Data Sources

| System | Tool | Purpose |
|--------|------|---------|
| CRM | Salesforce | Single source of truth for pipeline and deal data |
| MAP | HubSpot / Marketo / Pardot | Lead scoring, email, and nurture campaigns (confirm which is active) |
| Web Analytics | Google Analytics 4 | Web traffic and conversion events |
| Tag Management | Google Tag Manager | Tracking and event management |
| Social & Engagement | Sprout Social or equivalent | Social engagement and content performance metrics |
| BI / Dashboards | Tableau / Looker | Cross-source reporting and executive dashboards |
| Data Enrichment | ZoomInfo | Contact enrichment, prospecting data, and firmographic signals |
| Sales Engagement | Outreach | SDR/BDR sequence and call tracking |

---

## Attribution Model

- **Model type:** Multi-touch, time-decay weighted — emphasizes recent touchpoints closer to conversion
- **First touch / Last touch / Assist credit split:** [AWAITING SME — confirm % breakdown]
- **Attribution window:** [AWAITING SME — days from first touch to Closed Won]
- **CMO dashboard:** [AWAITING SME — confirm tool and report name]

---


---

## Carried Forward From the Previous Version (second pass)

> **PROVENANCE.** Reproduced verbatim on 2026-08-05 from the pre-May 2026 `daxko-ai/shared-knowledge-base/performance-data-schema.md`
> (Nick Lindauer / Claude). This content did not survive the May rewrite. Nothing above this
> line was altered.

## Pipeline Stages

All agents must use these exact stage definitions when referencing pipeline data:

| Stage | Definition | Conversion Benchmark |
|-------|-----------|---------------------|
| Lead | Known contact who has engaged with Daxko / brand content | — |
| MQL | Lead meeting behavioral + firmographic scoring threshold — accepted into marketing qualified status | [AWAITING SME — exact scoring threshold] |
| SQL / SAL | MQL accepted by sales after qualification call (also referenced as SAL in some funnel definitions) | [AWAITING SME] |
| Opportunity | Active deal with identified budget, authority, need, and timeline | [AWAITING SME] |
| Closed Won | Signed contract, revenue recognized | [AWAITING SME] |
| Closed Lost | Deal lost — reason captured in CRM for analysis | — |

---


## Change Log
- [2026-05-25] Created from source OKR files and pipeline attribution standards. Codified market-specific KPIs from NP-01, CL-01, BO-01. — Abhishek Bhandari
