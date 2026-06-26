# NHS England Operational Performance Dashboard
### Oct 2025 – Mar 2026 | Python · Tableau · NHS Open Data

[![Dashboard](https://img.shields.io/badge/View%20Dashboard-Tableau%20Public-blue)](https://public.tableau.com/app/profile/dorjada.halili/viz/NHSEnglandOperationalPerformanceDashboardOct25-Mar26/NHSEnglandOperationalPerformanceDashboardOct2025Mar2026)

## Overview
An end-to-end data analytics project analysing NHS England operational performance across 6 months of real government data. Built using Python for data cleaning and Tableau Public for interactive visualisation.

## Live Dashboard
[View the interactive dashboard on Tableau Public](https://public.tableau.com/app/profile/dorjada.halili/viz/NHSEnglandOperationalPerformanceDashboardOct25-Mar26/NHSEnglandOperationalPerformanceDashboardOct2025Mar2026)

## Key Findings
- **Trauma & Orthopaedic** has the largest waiting list at **5.1 million patients** — 38% larger than any other specialty
- **No specialty** came close to the NHS 92% 18-week RTT target — best performer (Ophthalmology) reached only ~74%
- **Every NHS region** is below the 95% A&E 4-hour target — regional performance ranges from ~75% to ~85%
- The total waiting list declined slowly from **7.3M to 7.1M patients** between October 2025 and March 2026

## Data Sources
| Dataset | Source | Period |
|---|---|---|
| RTT Waiting Times (Full CSV) | NHS England Statistics | Oct 2025 – Mar 2026 |
| A&E Attendances & Admissions | NHS England Statistics | Q3–Q4 2025-26 |

All data is publicly available at [england.nhs.uk/statistics](https://www.england.nhs.uk/statistics)

## Methodology
### Python (Pandas)
- Loaded and merged **6 monthly CSV files** totalling 1,093,888 rows
- Calculated **% within 18 weeks** from 17 individual wait band columns
- Cleaned A&E data from multi-sheet XLS files with non-standard headers
- Exported two clean CSVs (`rtt_clean.csv` and `ae_clean.csv`) for Tableau

### Tableau
- Built 4 interactive charts with filters and reference lines
- Added NHS target reference lines (92% RTT, 95% A&E)
- Assembled into a single dashboard with consistent colour coding

## Dashboard Charts
1. **Waiting List by Specialty** — Top 10 specialties by total patients waiting
2. **18-Week RTT Performance Trend** — Monthly % within target for top 5 specialties
3. **A&E 4-Hour Performance by Region** — All 7 NHS regions vs 95% target
4. **Waiting List Trend** — Total monthly waiting list Oct 2025 – Mar 2026

## Tools & Skills
`Python` `Pandas` `Jupyter Notebook` `Tableau Public` `NHS Open Data` `Data Cleaning` `Data Visualisation`

## Files
| File | Description |
|---|---|
| `NHS_Dashboard_Cleaning.ipynb` | Full Python cleaning notebook |
| `rtt_clean.csv` | Cleaned RTT data (310,306 rows) |
| `ae_clean.csv` | Cleaned A&E data (396 rows) |
