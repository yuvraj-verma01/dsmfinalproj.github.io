# Scheduled Tribe Education, Poverty, and Livelihood Outcomes in India

This repository contains a static GitHub Pages project for a data analysis of how educational outcomes among Scheduled Tribe (ST) populations relate to poverty, employment, gender gaps, and livelihood distress across Indian states with significant ST populations.

The project is organized as an explanatory dashboard/blog. It combines a written policy argument, a data aggregation and schema discussion, key findings, question-by-question analysis dropdowns, visual evidence, and policy recommendations.

## Project Overview

Scheduled Tribes constitute approximately 8.6 percent of India's population and are among the most constitutionally protected groups in the country. Indian education and welfare policy has long recognized that ST communities face structural disadvantages that cannot be addressed through general welfare schemes alone. This project studies whether education indicators such as literacy, enrolment, gross enrolment ratio (GER), dropout, and gender parity are actually associated with better livelihood outcomes for ST communities.

The central analytical problem is that education access indicators can look encouraging even when poverty, weak work opportunities, public-employment dependence, and dropout remain high. The project therefore does not assume that schooling access automatically produces economic security. Instead, it tests relationships between education indicators and livelihood outcomes directly.

## Research Question

The project asks:

> How do differences in educational outcomes among Scheduled Tribe populations relate to employment and poverty across states with high populations of Scheduled Tribes in India?

## What the Site Contains

The site is structured around five main sections:

- **Introduction**: explains the constitutional, policy, and development context for ST education and livelihood disadvantage.
- **Problem Statement**: frames the analytical problem as a mismatch between access-focused schooling metrics and actual livelihood outcomes.
- **Data Aggregation and Schema**: documents the state-level analytical database, main variables, table-level schema, and the full schema CSV.
- **Key Findings and Analysis Results**: summarizes findings by theme and provides Q1-Q13 dropdowns with detailed visual and statistical interpretation.
- **Recommendations and Suggestions**: translates the findings into policy priorities around retention, livelihood support, MGNREG, literacy gaps, gender outcomes, and education-to-work pathways.

## Data and Schema

The analysis uses a state-level database that aggregates education, demographic, employment, poverty, MGNREG, scholarship, household, village, and tribe-level indicators.

The full schema report records:

- **20 tables** across raw, derived, and analysis-ready data.
- **618 columns** across the full database schema.
- **200 columns** in the final state-level analysis dataset.

The schema is documented in:

- `database_schema_report.csv`

The final analysis focuses on variables related to:

- ST literacy and literacy gaps.
- Gross enrolment ratio across class groups.
- Primary, upper-primary, and secondary dropout.
- Gender parity index and girls' GER.
- ST poverty by residence category.
- Labour-force participation, work participation, and unemployment.
- MGNREG demand, unmet demand, days worked, and 100-plus-day work indicators.
- Scholarship release, utilization, and per-capita support.
- ST population concentration and tribal village concentration.

## Analysis Questions

The dashboard includes detailed dropdown sections for 13 analysis questions:

1. How do ST literacy and literacy gaps describe long-term educational exclusion?
2. Do states with stronger ST schooling participation, measured by GER, also have lower dropout and lower ST poverty?
3. Are enrolment and GER enough to indicate educational progress, or do dropout rates tell a different story?
4. Does the ST literacy gap matter more than the ST literacy level?
5. Are there states where educational indicators look reasonable, but employment or poverty outcomes remain weak?
6. Does MGNREG unmet demand reflect deeper livelihood distress among ST households?
7. Are scholarship-supported states seeing lower secondary dropout among ST students?
8. Do states with high ST schooling participation still depend heavily on MGNREG?
9. Does gender parity in enrolment translate into better female literacy and work outcomes?
10. Does secondary dropout appear to be a stronger warning signal of poverty and weak labour outcomes than literacy alone?
11. Do high-ST-share states systematically perform worse, or do outcomes vary substantially?
12. Do states with high concentrations of ST villages show different education and livelihood outcomes?
13. Are there gender-specific disadvantages hidden behind state averages?

## Main Findings

The main findings are:

- **Literacy rate alone is incomplete.** The ST literacy gap is more useful than ST literacy alone because it shows whether ST communities are falling behind the broader state population.
- **GER should not be treated as a welfare indicator by itself.** High GER can coexist with poverty, delayed progression, repeat enrolment, and weak labour-market outcomes.
- **Dropout is more informative than enrolment.** Secondary dropout better captures whether students are leaving the school system before completing important stages of education.
- **Work participation is ambiguous.** Higher work participation can reflect stronger opportunity, but it can also reflect distress-driven labour entry when students leave school early.
- **MGNREG unmet demand is a major livelihood distress signal.** States with higher unmet MGNREG demand also tend to show higher secondary dropout, suggesting that household livelihood stress and school retention problems cluster together.
- **Scholarship support does not show a clear relationship with dropout in this analysis.** Scholarship variables are statistically insignificant as standalone predictors of lower dropout.
- **Gender parity in enrolment is not the same as gender equality in livelihoods.** Girls' schooling participation can improve while women still face barriers to work, income, mobility, and equal opportunity.

## Policy Implications

The project argues that ST education policy should move beyond enrolment expansion alone. A more useful monitoring framework would track education and livelihood indicators together.

The recommendations emphasize:

- Moving from increasing GER to reducing dropout.
- Using the ST literacy gap as a targeting tool.
- Treating secondary dropout as a poverty and livelihood warning signal.
- Coordinating dropout reduction with MGNREG and rural livelihood support.
- Interpreting work participation alongside dropout and poverty.
- Connecting secondary education to local employment pathways.
- Moving beyond gender parity in enrolment toward girls' completion, skills, and work outcomes.

## Repository Structure

```text
.
├── index.html
├── styles.css
├── README.md
├── database_schema_report.csv
└── assets/
    ├── figures/
    ├── q2/
    ├── q4/
    ├── q6/
    ├── q8/
    ├── q10/
    └── q12/
```

## How to View the Project Locally

This is a static site. No build step is required.

Open `index.html` directly in a browser, or run a simple local server from the repository root:

```bash
python -m http.server 8000
```

Then visit:

```text
http://localhost:8000
```

## Deployment

The project is designed for GitHub Pages. Since the site is static, deployment only requires pushing `index.html`, `styles.css`, `assets/`, `database_schema_report.csv`, and `README.md` to the GitHub repository branch configured for Pages.

## Notes on Interpretation

This is an exploratory data analysis. The relationships shown in the dashboard should be interpreted as descriptive associations, not causal estimates. State-level aggregation can hide district-level and tribe-level variation, and source indicators may differ by year, category, or measurement definition. The analysis is most useful for identifying patterns, mismatches, and policy priorities that need deeper investigation.
