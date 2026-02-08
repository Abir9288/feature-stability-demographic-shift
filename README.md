# Feature Stability under Demographic Distribution Shift

This repository contains the experimental code accompanying a research study on feature-level stability
and model robustness under natural demographic distribution shift in real-world tabular data.

The primary objective of this work is to understand how predictive relationships of individual features
change across demographic environments and how enforcing feature stability affects generalization under
distribution shift.

---

## Research Focus

The study investigates the following questions:

- Which features exhibit stable predictive behavior across demographic environments?
- How does feature instability contribute to robustness failures under distribution shift?
- Under what conditions does enforcing feature stability improve out-of-distribution generalization?
- Can feature-level stability analysis provide actionable insights beyond standard accuracy metrics?

The emphasis is on explanation and robustness analysis rather than benchmark optimization.

---

## Experimental Design

- **Data type:** Real-world tabular dataset
- **Environments:** Age-based demographic splits (Young, Middle, Old)
- **Models:** Logistic Regression and Gradient Boosting
- **Evaluation:** ROC-AUC and robustness degradation (Δ AUC across environments)

Key experimental components include:

- Construction of natural demographic environments
- Quantification of covariate shift using Population Stability Index (PSI)
- Feature-level stability analysis based on effect variability
- Incremental feature ablation for causal robustness assessment
- Multi-seed evaluation and statistical significance testing

## Repository Structure

feature-stability-demographic-shift/
│
├── data/
│   ├── raw/
│   │   └── application_train.csv
│   └── processed/
│
├── notebooks/
│   └── feature_stability.ipynb
 
│
├── README.md
└── .gitignore

