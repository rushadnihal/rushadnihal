# Hi, I'm Rushad Nihal

**Biostatistician** with an M.S. in Biostatistics (Arizona State University) and a B.Tech in Biotechnology. I work where statistics meets biology: turning messy clinical, omics and bioprocess data into analyses that are reproducible and honest about what they can and cannot show.

---

## Two results I'm proud of

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
| [multi-omics-biomarker-pipeline](https://github.com/rushadnihal/multi-omics-biomarker-pipeline) | Leakage-controlled survival biomarker for lung adenocarcinoma (TCGA-LUAD), validated on two external cohorts | Python |
| [causal-survival-analysis](https://github.com/rushadnihal/causal-survival-analysis) | Target trial emulation of ACEi/ARB use and cardiovascular death in type 2 diabetes with CKD, using NHANES | Python |
| [myco-rsm](https://github.com/rushadnihal/myco-rsm) | Response surface and multi-objective media optimizer for submerged mycelial fermentation | R, Shiny |
| [adni-subgroup-calibration-code](https://github.com/rushadnihal/adni-subgroup-calibration-code) | *Work in progress:* audit of how well MCI-to-dementia risk models are calibrated across landmark times and demographic subgroups in ADNI (code only; ADNI data cannot be redistributed) | R |

## Toolbox

**Languages:** Python, R, SQL, SAS
**Python:** pandas, scikit-learn, scikit-survival, lifelines, statsmodels
**R:** tidyverse, caret, survival, nlme, lme4, rsm, Shiny, Quarto
**Methods:** survival analysis, causal inference, mixed-effects models, design of experiments, time-series forecasting, supervised machine learning
**Lab background:** microbiology, molecular biology, PCR, bioprocess protocols, quality control

## Background

- **M.S. Biostatistics**, Arizona State University (2025, GPA 3.97/4.00)
- **B.Tech Biotechnology**, Manipal Institute of Technology (2023)
- Data Science Analyst on a collaboration between ASU and the Global Observatory for Physical Activity (GoPA!)
- iGEM with the Manipal team: Bronze (2021) and Gold (2022)

## Currently

Writing up a calibration audit of dementia risk prediction in ADNI, and learning German (A1).

## Get in touch

Email is the best way to reach me: [rushadisatwork@gmail.com](mailto:rushadisatwork@gmail.com)
