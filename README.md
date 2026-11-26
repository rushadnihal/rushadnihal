# Hi, I'm Rushad Nihal

**Biostatistician** with an M.S. in Biostatistics (Arizona State University, GPA 3.97) and a B.Tech in Biotechnology. I work on clinical-trial statistics: designing trials, writing and following statistical analysis plans, fitting the models regulators expect (MMRM, Cox, logistic), and checking results in both **SAS and R**.


---

## Across the clinical trial lifecycle

| Stage | What I've built | Project |
|---|---|---|
| **Design** | Sample size, group-sequential boundaries, promising-zone re-estimation, Bayesian go/no-go and patient-level survival simulation; every number validated against `rpact`, `gsDesign` and base R | [trialdesign](https://github.com/rushadnihal/trialdesign) |
| **SAP and estimands** | SAP frozen under a git tag before any outcome was seen; ICH E9(R1) estimand; MMRM with missing-data sensitivity analyses | [oasis2-mmrm-trial-simulation](https://github.com/rushadnihal/oasis2-mmrm-trial-simulation) |
| **CDISC deliverables** | SDTM → ADaM → TLFs in SAS, with derived datasets checked against the published PHUSE ADaM files (`PROC COMPARE`) | [cdisc-pilot-sas-adam-tlf](https://github.com/rushadnihal/cdisc-pilot-sas-adam-tlf) |
| **Independent validation** | Primary MMRM fitted in R (`mmrm`) and SAS (`PROC MIXED`, DDFM=KR); estimates and SEs agree within 1e-6 | [oasis2-mmrm-trial-simulation](https://github.com/rushadnihal/oasis2-mmrm-trial-simulation) |
| **Evidence synthesis / HTA** | Random-effects meta-analysis and meta-regression with heterogeneity, publication-bias and leave-one-out checks | [bcg-vaccine-trials](https://github.com/rushadnihal/bcg-vaccine-trials) |
| **Real-world evidence** | Target trial emulation with inverse-probability weighting and survival outcomes | [causal-survival-analysis](https://github.com/rushadnihal/causal-survival-analysis) |

---

## Featured projects

### [trialdesign](https://github.com/rushadnihal/trialdesign): clinical trial design package · Python
[![PyPI](https://img.shields.io/pypi/v/gsdtrial)](https://pypi.org/project/gsdtrial/)

CLI and Python API for designing two-arm trials before the data exist (`pip install gsdtrial`).
- Sample size for continuous, binary and time-to-event endpoints: superiority, non-inferiority and equivalence
- Group-sequential designs with alpha spending and binding or non-binding futility, solved by recursive numerical integration
- Promising-zone (Cui-Hung-Wang) and blinded sample size re-estimation, and a Bayesian go/no-go interim with predictive probability of success
- Patient-level survival simulation under non-proportional hazards (delayed, waning or crossing effects) with the Fleming-Harrington weighted log-rank test
- Graphical multiple testing, end-of-trial inference (repeated CIs, median-unbiased estimates), Markdown reports and stable `--json` output
- **Validated against `rpact`, `gsDesign`, `mvtnorm` and base R** in CI; exact operating characteristics checked against 200,000-trial simulations
- Includes a [design memo](https://github.com/rushadnihal/trialdesign/blob/main/docs/design_memo.md) written the way I'd present a design to a clinical team

### [oasis2-mmrm-trial-simulation](https://github.com/rushadnihal/oasis2-mmrm-trial-simulation): MMRM, estimands and trial simulation · R, SAS
Trial-style longitudinal analysis of brain-volume decline in OASIS-2.
- **SAP v1.0 frozen before outcomes**, with every later change logged as a deviation
- MMRM primary analysis, robustness checks (covariance, time model, visit windows) and **MNAR delta-adjustment** and **reference-based imputation** (`rbmi`)
- **SAS/R double programming** that agrees to 1e-6
- ADEMP simulation study (888,000 simulated trials) of type I error, power and sample size: **64 per arm** for 80% power, 86 allowing for 30% dropout
- Quarto report, `renv`-pinned, CI runs the full pipeline on synthetic data

### [cdisc-pilot-sas-adam-tlf](https://github.com/rushadnihal/cdisc-pilot-sas-adam-tlf): CDISC SDTM → ADaM → TLF · SAS
Submission-style programming on the public CDISC pilot study (xanomeline vs placebo, 254 randomized): ADSL, ADAE and ADTTE derived from SDTM with dataset specs; disposition, baseline, exposure and adverse-event tables; Kaplan-Meier/Cox with a proportional-hazards check; ANCOVA and a repeated-measures model for ADAS-Cog. Derived datasets are reconciled against the published PHUSE ADaM files with `PROC COMPARE`, and outputs go to RTF/PDF with saved logs and a validation checklist.

### [bcg-vaccine-trials](https://github.com/rushadnihal/bcg-vaccine-trials): meta-analysis for evidence synthesis · R
Random-effects meta-analysis of 13 BCG vaccine trials (`metafor`): pooled RR 0.49 (95% CI 0.34–0.70), I² = 92%, and a latitude meta-regression that explains 76% of the heterogeneity. Includes Knapp-Hartung and permutation tests, six τ² estimators, Egger/Begg tests, trim-and-fill and leave-one-out analyses. These are the methods used in HTA submissions (e.g. IQWiG/AMNOG, NCPE).

### [aact-trial-outcomes-sql-sas](https://github.com/rushadnihal/aact-trial-outcomes-sql-sas): clinical trial registry analysis · SQL, SAS
What predicts early termination and late or missing results reporting in 44k Phase 2/3 drug trials on ClinicalTrials.gov: PostgreSQL cohort build, then SAS logistic and Cox models with sponsor-clustered standard errors.

### [causal-survival-analysis](https://github.com/rushadnihal/causal-survival-analysis): target trial emulation · Python
ACEi/ARB use and cardiovascular death in type 2 diabetes with CKD (NHANES 2005–2018, n = 2,540). Covariate balance after weighting is good (largest SMD 0.051) but the estimate is inconclusive. The repo explains why (residual healthy-user bias, sample size) and validates the methods on simulations with a known truth.

---

## More work

| Project | What it is | Stack |
|---|---|---|
| [multi-omics-biomarker-pipeline](https://github.com/rushadnihal/multi-omics-biomarker-pipeline) | Leakage-controlled clinical + 5-gene survival signature for lung adenocarcinoma (TCGA-LUAD), frozen and validated on two external cohorts (Harrell C 0.715 and 0.697) | Python |
| [myco-rsm](https://github.com/rushadnihal/myco-rsm) | Response surface / design-of-experiments media optimizer for fermentation | R, Shiny |
| [adni-subgroup-calibration-code](https://github.com/rushadnihal/adni-subgroup-calibration-code) | *In progress:* calibration audit of MCI-to-dementia risk models across landmark times and demographic subgroups in ADNI (code only; data cannot be redistributed) | R |

## Toolbox

**Languages:** SAS, R, Python, SQL
**SAS:** PROC MIXED, PHREG, LIFETEST, LOGISTIC, SURVEYLOGISTIC, FREQ, MEANS, REPORT, COMPARE, SQL, macros, ODS RTF output
**R:** `mmrm`, `emmeans`, `nlme`, `lme4`, `survival`, `rbmi`, `mice`, `metafor`, `rpact`, `gsDesign`, tidyverse, Shiny, Quarto
**Python:** numpy, scipy, pandas, statsmodels, lifelines, scikit-survival, scikit-learn
**Clinical standards:** CDISC SDTM and ADaM, ICH E9 and E9(R1) estimands, SAP writing, double programming / QC
**Methods:** group-sequential, adaptive (sample size re-estimation) and Bayesian trial design, non-proportional hazards, mixed models for repeated measures, survival analysis, missing data (MAR/MNAR, reference-based imputation), causal inference, meta-analysis, simulation studies (ADEMP)
**Reproducibility:** Git, GitHub Actions CI, `renv`, pytest, synthetic-data pipelines for confidential data

## Background

- **M.S. Biostatistics**, Arizona State University (2025, GPA 3.97/4.00)
- **B.Tech Biotechnology**, Manipal Institute of Technology (2023)
- **Data Science Analyst**, ASU × Global Observatory for Physical Activity (GoPA!): built a country-year panel for six African countries, compared naive-drift, ETS and ARIMA forecasts to 2030, and screened predictors with PCA and lagged cross-correlation (confidential data, not shared)
- **iGEM**, Manipal team: Bronze (2021) and Gold (2022)
- Lab background in microbiology, molecular biology, PCR and bioprocess QC, so I can talk to the scientists whose data I analyse

## Currently

Writing up the ADNI calibration audit and learning German (A1).

## Get in touch

Email is the best way to reach me: [rushadisatwork@gmail.com](mailto:rushadisatwork@gmail.com)
