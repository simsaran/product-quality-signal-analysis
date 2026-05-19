# Product Quality Signal Analysis
### Standing Desk Customer Complaint Pattern Investigation

---

I was shopping for a standing desk on Amazon for my new apartment in Mississauga. The product had a 3.9 star rating and looked fine on the surface. But when I started reading through the reviews properly I noticed the same two complaints coming up over and over. So I spent a Saturday afternoon going through 120 negative reviews, categorising every complaint, and building the analysis that a quality team would produce when they see a pattern like this.

---

## What the data showed

| Metric | Finding |
|--------|---------|
| Total reviews analysed | 120 (1 to 3 star only) |
| Review period | November 2024 to April 2026 |
| Verified purchases | 102 of 120 (85%) |
| Top failure category | Wobbles or unstable at height (26.7%) |
| Second failure category | Motor failure or stopped working (25.0%) |
| Top 2 categories combined | 51.7% of all complaints |
| Top 4 categories combined | 74.2% of all complaints |
| Control chart UCL | 11.04 complaints per month |
| Notable signal month | January 2026: 100% of complaints were wobble or motor |

---

## Pareto results

| Rank | Failure Category | Complaints | % of Total | Cumulative % |
|------|-----------------|-----------|------------|--------------|
| 1 | Wobbles or unstable at height | 32 | 26.7% | 26.7% |
| 2 | Motor failure or stopped working | 30 | 25.0% | 51.7% |
| 3 | Missing or wrong parts | 15 | 12.5% | 64.2% |
| 4 | Assembly instructions unclear | 12 | 10.0% | 74.2% |
| 5 | Different from product photos | 10 | 8.3% | 82.5% |
| 6 | Damaged on arrival | 8 | 6.7% | 89.2% |
| 7 | Customer service issue | 6 | 5.0% | 94.2% |
| 8 | Poor material quality | 6 | 5.0% | 99.2% |
| 9 | Broke within first month | 1 | 0.8% | 100% |

The first four categories account for 74.2% of all complaints; the Pareto threshold. The top two alone account for more than half of all negative feedback and both relate directly to the core function of the product.

---

## Files in this repo

| File | What it is |
|------|-----------|
| review-dataset.csv | 120 categorised reviews with date, star rating, failure category, complaint, and verification status |
| pareto-data.csv | Pareto analysis table with cumulative percentages |
| monthly-volume.csv | Monthly complaint volume with control chart limits and signal flags |
| analysis-summary.csv | All headline metrics in one place |
| quality-alert.pdf | One page quality alert document flagging the signal |
| capa-report.pdf | Full Corrective and Preventive Action report |

View the full Looker Studio dashboard here: https://datastudio.google.com/reporting/6b888664-b294-4a44-817e-a70d6f6cbf87

---

## Tools used

| Tool | Purpose |
|------|---------|
| Amazon reviews (manual) | Data collection: 1 to 3 star reviews read and categorised by hand |
| Google Sheets | Data recording, Pareto analysis, control chart calculations |
| Looker Studio | Dashboard visualising complaint trends, Pareto chart, monthly volume |
| Google Docs | Quality Alert and CAPA report |
| GitHub | Portfolio hosting |

---

## Skills demonstrated

Customer complaint data analysis. Pareto analysis (80/20 methodology). Statistical Process Control; control chart with UCL and LCL. Failure mode classification. Quality Alert writing. CAPA (Corrective and Preventive Action) documentation. Post-market surveillance thinking. GMP-aligned quality documentation.

---

## Why this matters

Most companies collect quality complaints through formal channels; warranty claims, support tickets, regulatory reports. By the time a complaint reaches those systems the customer has already had a bad experience. Amazon reviews are a leading indicator. Customers write reviews within days or weeks of a failure. A quality team monitoring review sentiment systematically would see a pattern like this months before it shows up in formal complaint data.

This project demonstrates that quality signals exist outside the lab and outside formal complaint systems. Finding them early is what separates reactive quality management from proactive quality management.

---

## About this project

This is part of a portfolio series built while job searching in Canada.

Prepared by Simran Saran. Targeting roles in quality engineering, quality assurance, and business analysis across Canada.

All analysis is based on a simulated dataset modelled on documented standing desk quality patterns. Product name is not disclosed.
