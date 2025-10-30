# WAVESTONE_TEST  
**Empowering Reliable Insights for Smarter Customer Retention**

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![Google Colab](https://img.shields.io/badge/Platform-Google%20Colab-orange.svg)](https://colab.research.google.com)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

### Built with the tools and technologies
`Python` • `Pandas` • `NumPy` • `Scikit-learn` • `XGBoost` • `SHAP` • `Matplotlib` • `Seaborn`

---

## Table of Contents
- [Overview](#overview)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Results & Insights](#results--insights)
- [Next Steps](#next-steps)
- [Testing](#testing)
- [Author](#author)

---

## Overview

**WAVESTONE_TEST** is a consulting-oriented machine learning case study focused on **customer churn** in the telecommunications sector.  
The goals are to:
- **Explain** the key drivers of churn (why customers leave),
- **Predict** churn with reliable, interpretable models,
- **Translate** findings into **actionable business recommendations**.

**Key deliverables**
- A clean, modular **Google Colab** notebook ready for client demo,
- A **consultant-friendly storyline**: *understand → model → interpret → recommend*,
- Visual outputs (feature importances, **SHAP** summaries) for business decision-making.

---

## Getting Started

### Prerequisites
- **Python ≥ 3.10** (Google Colab or local Jupyter)
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `xgboost`, `shap`

### Installation
```bash
# 1) Clone the repository
git clone https://github.com/YanisBoNueve/wavestone_test.git

# 2) Go to the project directory
cd wavestone_test

# 3) (Optional) Install dependencies if running locally
pip install -r requirements.txt
Project Structure
bash


wavestone_test/
├── data/
│   └── sujet_B_data_client_churn.csv      # Dataset
├── notebooks/
│   └── churn_analysis.ipynb               # Main Colab/Jupyter notebook
├── README.md
└── requirements.txt                       # Optional dependency list

### Usage
Open the notebook in Google Colab (recommended):

Colab link:
https://colab.research.google.com/github/YanisBoNueve/wavestone_test/blob/main/notebooks/churn_analysis.ipynb

### What the notebook does

Loads and profiles the dataset,

Engineers features (incl. NumServices),

Trains & compares models (Logistic Regression, Random Forest, XGBoost),

Evaluates with Accuracy, F1 and a confusion matrix,

Explains results with feature importances and SHAP,

Delivers business-ready recommendations and a predict() function for integration.

### Results & Insights
Top churn drivers typically observed:

Contract type (Month-to-month more at risk),

Tenure (lower seniority → higher churn),

MonthlyCharges,

NumServices (service bundle complexity).

Best model (example): XGBoost with strong F1 while remaining explainable via SHAP.

Business impact: Insights support retention strategies (targeted offers, contract upgrades, service bundling simplification).

### Next Steps
Hyperparameter tuning with cross-validation,

MLOps pipeline: model registry, performance & drift monitoring,

Integration into CRM workflows (priority lists, alerts),

Explainability dashboard (Streamlit / Power BI) for operations teams.

### Testing
If you maintain tests, run them with your preferred framework (e.g., pytest):

bash
Copier le code
pytest -q

### Author
Yanis Boutouba — Machine Learning & Data Lab (Wavestone Candidate Assessment)
© 2025 — All rights reserved.