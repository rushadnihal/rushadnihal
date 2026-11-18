# Hi, I'm Rushad Nihal

Biostatistics M.S. graduate (Arizona State University, 2025) with a B.Tech in Biotechnology. I work where statistics meets biology: turning messy clinical, omics and bioprocess data into analyses that are reproducible and honest about what they can and cannot show.

**Looking for:** biostatistician or statistical programmer roles in clinical development, in the US or EU.

---

## Three results I'm proud of

**A trial-style analysis with a frozen plan.** A natural-history MMRM of brain-volume decline in OASIS-2 under a statistical analysis plan tagged in git before any outcome analysis, with an ICH E9(R1) estimand, missing-data sensitivity analyses, SAS and R agreeing to 1e-6, and a simulation of 888,000 virtual trials giving type I error, power and sample size for a two-arm trial on this endpoint.
→ [oasis2-mmrm-trial-simulation](https://github.com/rushadnihal/oasis2-mmrm-trial-simulation)

**A biomarker that held up on data it never saw.** A frozen clinical + 5-gene signature for lung adenocarcinoma, built with every data-dependent step refit inside each training fold, then tested without refitting on two independent cohorts: Harrell C **0.715** (n=226) and **0.697** (n=442). Inside TCGA, multi-omics did *not* detectably beat a clinical-only model, and the repo reports that as the pre-specified result rather than hiding it.
→ [multi-omics-biomarker-pipeline](https://github.com/rushadnihal/multi-omics-biomarker-pipeline)

**A target trial emulation that ends in an honest null.** ACEi/ARB use and cardiovascular death in type 2 diabetes with CKD (NHANES 2005-2018, n=2,540). After weighting, covariate balance is good (largest SMD 0.051), but the estimates are inconclusive. The project diagnoses why (residual healthy-user bias, limited sample size) and checks its machinery against simulations with a known truth.
→ [causal-survival-analysis](https://github.com/rushadnihal/causal-survival-analysis)

---

## What I work on

- **Survival analysis and biomarkers:** leakage-controlled modeling of high-dimensional omics data, with frozen signatures and external validation.
- **Causal inference:** target trial emulation, inverse-probability weighting, g-formula and competing-risks methods on observational health data.
- **Multilevel and clinical-trial data:** mixed-effects models for clustered and longitudinal data, including cluster randomized trials.
- **Bioprocess optimization:** response surface methodology and design of experiments for fermentation media, so fewer wet-lab runs answer more questions.
- **Reproducible research:** pipelines that rebuild every table and figure from raw data, with tests and recorded checksums.

## Selected projects

| Project | What it is | Stack |
|---|---|---|
| [oasis2-mmrm-trial-simulation](https://github.com/rushadnihal/oasis2-mmrm-trial-simulation) | Natural-history MMRM of brain-volume decline in OASIS-2 under a frozen SAP and estimand, missing-data sensitivity analyses, SAS/R cross-check, and a simulation study of a two-arm trial (type I error, power, sample size) | R, SAS |
| [cdisc-pilot-sas-adam-tlf](https://github.com/rushadnihal/cdisc-pilot-sas-adam-tlf) | SDTM to ADaM to tables, Kaplan-Meier/Cox and a repeated measures model on the public CDISC pilot study, with the derived datasets checked against the published PHUSE ADaM files (PROC COMPARE) | SAS |
| [multi-omics-biomarker-pipeline](https://github.com/rushadnihal/multi-omics-biomarker-pipeline) | Leakage-controlled survival biomarker for lung adenocarcinoma (TCGA-LUAD), validated on two external cohorts | Python |
| [causal-survival-analysis](https://github.com/rushadnihal/causal-survival-analysis) | Target trial emulation of ACEi/ARB use and cardiovascular death in type 2 diabetes with CKD, using NHANES | Python |
| [aact-trial-outcomes-sql-sas](https://github.com/rushadnihal/aact-trial-outcomes-sql-sas) | What predicts early termination and late or missing results reporting in 44k Phase 2/3 drug trials on ClinicalTrials.gov (AACT): PostgreSQL cohort build, then SAS logistic and Cox models with sponsor-clustered errors | SQL, SAS |
| [adni-subgroup-calibration-code](https://github.com/rushadnihal/adni-subgroup-calibration-code) | *Work in progress:* audit of how well MCI-to-dementia risk models are calibrated across landmark times and demographic subgroups in ADNI (code only; ADNI data cannot be redistributed) | R |
| [myco-rsm](https://github.com/rushadnihal/myco-rsm) | *Side project from my biotechnology background:* response surface and multi-objective media optimizer for submerged mycelial fermentation | R, Shiny |

## Toolbox

**Languages:** Python, R, SQL, SAS
**Python:** pandas, scikit-learn, scikit-survival, lifelines, statsmodels
**R:** tidyverse, caret, survival, nlme, lme4, rsm, Shiny, Quarto
**Methods:** survival analysis, causal inference, mixed-effects models, design of experiments, time-series forecasting, supervised machine learning
**Lab background:** microbiology, molecular biology, PCR, bioprocess protocols, quality control

## Background

- **M.S. Biostatistics**, Arizona State University (2025, GPA 3.97/4.00)
- **B.Tech Biotechnology**, Manipal Institute of Technology (2023)
- Data Science Analyst on a collaboration between ASU and the Global Observatory for Physical Activity (GoPA!): built a country-year panel from physical-activity publication records and socioeconomic indicators for six African countries, compared naive-drift, ETS and ARIMA forecasts to 2030, and screened predictors with correlation, PCA and lagged cross-correlation (GoPA! data are confidential and not shared)
- iGEM with the Manipal team: Bronze (2021) and Gold (2022)

## Currently

Writing up a calibration audit of dementia risk prediction in ADNI, and learning German (A1).

## Get in touch

Email is the best way to reach me: [rushadisatwork@gmail.com](mailto:rushadisatwork@gmail.com)
