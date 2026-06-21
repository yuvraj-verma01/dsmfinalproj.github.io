# Scheduled Tribe Education, Poverty, and Livelihood Outcomes in India

This repository contains the published static site for a data analysis project on how educational outcomes among Scheduled Tribe (ST) populations relate to poverty, employment, gender gaps, public-work demand, and livelihood distress across Indian states.

The project is presented as an explanatory dashboard/blog. It combines policy context, a state-level data schema, key findings, question-by-question analysis, generated visualizations, and recommendations for monitoring ST education and livelihood outcomes together.

## Project Links

- Project site: `index.html` in this repository, designed for GitHub Pages.
- Expected GitHub Pages URL: <https://yuvraj-verma01.github.io/dsmfinalproj.github.io/>
- Interactive dashboard: <https://st-education-poverty-outcomes.streamlit.app/>
- Full report: <https://drive.google.com/file/d/1rQ2fdQ8y2z0uQJD95zxeZAiTNuFYw4CW/view>
- Schema report: [`database_schema_report.csv`](database_schema_report.csv)

## Executive Overview

Scheduled Tribes constitute about 8.6 percent of India's population and are among the country's most constitutionally protected groups. Education and welfare policy has long recognized that ST communities face structural barriers related to geography, poverty, school access, language, social exclusion, labour markets, and public-service delivery.

This project studies a specific policy problem: education access indicators can improve while livelihood outcomes remain weak. ST literacy, enrolment, and gross enrolment ratio (GER) may rise, but those improvements do not automatically mean that ST students complete secondary education, avoid poverty, enter secure employment, or experience gender-equitable outcomes.

The analysis therefore treats education and livelihoods as linked systems. It compares schooling indicators with poverty, work participation, unemployment, MGNREG demand, scholarship support, gender indicators, and ST settlement concentration to identify where educational progress is matched by livelihood improvement and where it is not.

## Central Research Question

> How do differences in educational outcomes among Scheduled Tribe populations relate to employment and poverty across states with high populations of Scheduled Tribes in India?

## Analytical Approach

The project uses state-level exploratory data analysis. It does not claim causal effects. Instead, it looks for descriptive relationships, mismatches, and warning signals across education and livelihood indicators.

The analysis is organized around four connected ideas:

- School access is not the same as school completion.
- Literacy level is less informative without the ST-general literacy gap.
- Work participation can indicate opportunity, but it can also indicate distress-driven labour.
- Livelihood stress, especially unmet MGNREG demand, can overlap with school dropout and poverty.

## What The Site Contains

The static site is structured as a long-form policy analysis with the following sections:

- Introduction: explains the constitutional, social, and policy context for ST educational and livelihood disadvantage.
- Problem Statement: frames the mismatch between access-focused education metrics and real livelihood outcomes.
- Data Aggregation and Schema: documents the state-level database and the core variables used in the analysis.
- Key Findings: summarizes the major patterns found across education, poverty, employment, gender, and MGNREG indicators.
- Analysis and Results: provides expandable question-by-question interpretations with visual evidence.
- Recommendations and Suggestions: translates findings into policy priorities around dropout, literacy gaps, livelihood support, gender outcomes, and education-to-work pathways.
- References: lists the major public data and policy sources used for the project.

## Data And Schema

The analysis is built from a state-level database that aggregates education, demographic, employment, poverty, public-work, scholarship, household, village, and tribe-level indicators.

The schema report documents:

- 20 tables.
- 618 total columns.
- 200 columns in `state_analysis_dataset_all_states`.
- 200 columns in `state_analysis_dataset_high_st_states`.

Major table groups include:

- Demographics: ST population, state population share, ST share of state population, and decadal growth.
- Education: ST literacy, literacy gaps, enrolment, GER, gender parity, and dropout.
- Employment: labour-force participation, work participation, unemployment, and gendered work indicators.
- Poverty: ST below-poverty-line indicators by residence category.
- MGNREG: job cards, work received, days worked, 100-plus-day work, and unmet demand.
- Scholarships: annual and cumulative scholarship release, utilization, and per-capita support indicators.
- Settlement geography: tribal village concentration at different ST population thresholds.
- Tribe-level indicators: tribe-weighted literacy, sex ratio, work participation, and related socioeconomic variables.

The full schema dictionary is stored in [`database_schema_report.csv`](database_schema_report.csv).

## Analysis Questions Covered

The site's analysis section currently covers 12 detailed question blocks:

1. How do ST literacy and literacy gaps describe long-term educational exclusion?
2. Do states with stronger ST schooling participation, measured by GER, also have lower dropout and lower ST poverty?
3. Are enrolment and GER enough to indicate educational progress, or do dropout rates tell a different story?
4. Does the ST literacy gap matter more than the ST literacy level?
5. Does MGNREG unmet demand reflect deeper livelihood distress among ST households?
6. Are scholarship-supported states seeing lower secondary dropout among ST students?
7. Do states with high ST schooling participation still depend heavily on MGNREG?
8. Does gender parity in enrolment translate into better female literacy and work outcomes?
9. Does secondary dropout appear to be a stronger warning signal of poverty and weak labour outcomes than literacy alone?
10. Do high-ST-share states systematically perform worse, or do outcomes vary substantially?
11. Do states with high concentrations of ST villages show different education and livelihood outcomes?
12. Are there gender-specific disadvantages hidden behind state averages?

## Main Findings

The project's main findings are:

- ST literacy alone is incomplete. The ST-general literacy gap is more useful because it shows whether ST communities are improving at the same pace as the broader state population.
- GER should not be treated as a welfare indicator by itself. High GER can coexist with poverty, delayed progression, repeat enrolment, and weak labour-market outcomes.
- Dropout is more informative than enrolment for identifying educational risk. Secondary dropout is especially important because it captures whether students leave before completing a critical stage of education.
- Work participation is ambiguous. Higher work participation can reflect stronger opportunity, but it can also reflect distress-driven labour entry when students leave school early or households face income pressure.
- MGNREG unmet demand is a major livelihood distress signal. States with higher unmet demand tend to show overlapping concerns around poverty, dropout, and weak livelihood security.
- Scholarship indicators do not show a clear standalone relationship with lower secondary dropout in this analysis.
- Gender parity in enrolment is not the same as gender equality in livelihoods. Girls may be enrolled while women still face barriers to completion, work, mobility, and income.
- ST village concentration appears more closely tied to livelihood-access challenges than to education outcomes alone.

## Policy Implications

The project argues that ST education policy should move beyond enrolment expansion alone. A stronger monitoring framework would track education and livelihood indicators together.

Recommended policy directions include:

- Shift from maximizing GER to reducing dropout and improving completion.
- Use the ST literacy gap as a targeting indicator, not only the absolute ST literacy rate.
- Treat secondary dropout as a poverty and livelihood warning signal.
- Coordinate dropout prevention with MGNREG work provision and rural livelihood support.
- Interpret work participation alongside dropout, poverty, and job quality.
- Link secondary education to local employment, vocational training, and transition pathways.
- Move beyond gender parity in enrolment toward girls' completion, skills, and work outcomes.

## Repository Structure

```text
.
|-- index.html
|-- styles.css
|-- README.md
|-- database_schema_report.csv
`-- assets/
    |-- figures/
    |-- q2/
    |-- q4/
    |-- q6/
    |-- q8/
    |-- q10/
    `-- q12/
```

Key files:

- [`index.html`](index.html): the full static article and analysis page.
- [`styles.css`](styles.css): presentation styles for the article, schema tables, navigation, and analysis dropdowns.
- [`database_schema_report.csv`](database_schema_report.csv): schema summary and column dictionary for the analytical database.
- [`assets/`](assets/): generated PNG figures used throughout the analysis.

## How To View Locally

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

The project is designed for GitHub Pages. Since it is static, deployment only requires pushing the site files to the branch configured for Pages.

Files required for deployment:

- `index.html`
- `styles.css`
- `database_schema_report.csv`
- `assets/`
- `README.md`

## Reproducibility Note

This repository stores the published site, generated figures, and schema documentation. It does not currently include the original data-ingestion scripts, notebooks, or database files used to generate the figures. To make the analysis fully reproducible, future work should add the data pipeline, source-download steps, transformation scripts, and figure-generation scripts.

## Interpretation Caveats

This is exploratory state-level analysis. The relationships shown in the dashboard should be interpreted as descriptive associations, not causal estimates. State-level aggregation can hide district-level, village-level, household-level, and tribe-level variation. Source indicators may also differ by year, measurement definition, gender category, residence category, or education stage.

The project is most useful for identifying patterns, mismatches, and policy priorities that need deeper investigation.
