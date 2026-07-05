# SME Capstone Project — AI-Powered Business Intelligence Dashboard

**Group 18 · Tek4dev 5.1**
Smart analytics for SMEs in Nigeria, built on Power BI · Data Analysis & Technical Project Management tracks

---

## Overview

This project delivers a full business intelligence solution for **Inner Space Interior Design Company**, a Nigerian SME offering design, renovation, and fit-out services. Starting from a raw, messy project-level dataset (300 records), the team cleaned and structured the data, then built an interactive Power BI dashboard to turn it into decisions a manager can actually act on — revenue performance, service profitability, pipeline health, and customer/regional insights.

The goal wasn't just to visualize numbers, but to answer the questions an SME owner genuinely needs answered:

- Are we making enough profit per project?
- Are we finishing projects on time and on budget?
- Which clients, states, or services bring in the most value?
- Where is the business losing money or leads?

## Business Context

Inner Space Interior Design Company runs project-based work rather than selling a single product — each project has its own client, budget, team, and timeline, spanning both residential and commercial work across multiple Nigerian states.

## Data Pipeline

1. **Raw data audit** — 300 project records with missing values, inconsistent text formatting, duplicate entries, and logical inconsistencies (e.g. completion dates on projects that were still ongoing).
2. **Cleaning** — handled column-by-column based on what each gap actually meant:
   - Derived values from related fields where possible (e.g. Completion Date from Start Date + Days to Complete)
   - Matched repeat clients via Client ID to recover missing names
   - Flagged rather than fabricated values that couldn't be recovered (e.g. "Unknown", "Not Yet Estimated")
   - Removed logically invalid completion dates from Ongoing/Cancelled projects
   - Identified and documented duplicate records and statistical outliers for review
3. **Analysis layer** — built Key Indicators, Business Correlations, Business Metrics, and Performance Indices directly off the cleaned dataset in Excel.
4. **Dashboarding** — modeled and visualized in Power BI Desktop, including a decomposition tree, geographic mapping, and an interactive NLP Q&A feature.

## Dashboard Structure

| Page | What it covers |
|---|---|
| **Executive Performance Overview** | Headline KPIs (Revenue, Profit, Margin, Project Volume), monthly revenue/profit trend, property type distribution, decomposition tree |
| **Product & Services Analysis** | Revenue by service category, residential vs. commercial split, cost-vs-revenue matrix, profit margin scatter profile |
| **Customer & Regional Insights** | Geographic footprint by state, referral source performance, payment status matrix (Outstanding/Paid/Part Payment), pipeline health (Completed/Ongoing/Delayed/Cancelled) |

## Key Figures

- **Total Revenue:** ₦2.48bn
- **Total Profit:** ₦716.85M
- **Overall Profit Margin:** 28.95%
- **Projects Managed:** 299
- **Pipeline:** 137 Completed · 6 Ongoing · 75 Delayed · 81 Cancelled

## Key Insights

- Revenue and profit are healthy overall, with a stable ~29% margin across the full project portfolio.
- Residential projects out-earn Commercial ones by volume, though Office and Retail properties anchor a disproportionate share of contract value.
- Painting is the top-earning service category, followed by Decoration and Renovation; core Interior Design services generate the least revenue by comparison.
- Over 27% of signed projects end up cancelled — a significant pipeline leak worth investigating operationally.
- ₦842.86M of the total pipeline value remains outstanding, with Corporate clients carrying the largest share of unpaid balances.

## Recommendations

1. **Automated milestone alerts** — flag projects stalled in "Ongoing" past a set threshold, so PMs can intervene before deadlines slip.
2. **Revised corporate onboarding & payment terms** — tie project milestones to cash collection and raise upfront deposit requirements for corporate clients.
3. **Audit low-performing referral sources** — cross-reference cancellation rates against referral channel to redirect marketing spend toward higher-intent leads.
4. **Vendor SLAs for top service categories** — secure supply agreements for Painting, Decoration, and Renovation materials to reduce delivery-driven delays.

## Tech Stack

- **Microsoft Excel** — data cleaning, validation, and formula-driven metric calculations
- **Power BI Desktop** — data modeling, DAX measures, and interactive dashboarding

## Team

Group 18, Tek4dev 5.1 Capstone Program — Data Analysis & Technical Project Management tracks.

---

*This dashboard was built as a final capstone project and is intended as a demonstration of end-to-end BI workflow: from messy raw data to a decision-ready analytics tool for a real-world SME use case.*
