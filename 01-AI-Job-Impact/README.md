# 🤖 AI Job Market Impact — Exploratory Data Analysis

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Pandas](https://img.shields.io/badge/Pandas-EDA-green)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![Dataset](https://img.shields.io/badge/Dataset-Synthetic-orange)

---

## 📌 Project Overview

This project explores how **Artificial Intelligence is impacting the global job market** since the rise of large language models like ChatGPT.

Using a dataset of **30,000 job records** across 8 industries and 8 countries, we perform a complete Exploratory Data Analysis (EDA) to uncover patterns in automation risk, salary trends, job growth, and AI adoption.

> ⚠️ **Note:** This is a synthetic dataset from Kaggle. Findings reflect data patterns, not real-world statistics.

---

## 📂 Project Structure

```
01-AI-Job-Impact/
├── ai_job_impact_eda.ipynb     ← Main EDA Notebook
├── ai_job_trends_dataset.csv   ← Dataset
├── report.pdf                  ← Summary Report
├── images/                     ← All saved plots
│   ├── ai_impact_distribution.png
│   ├── industry_distribution.png
│   ├── job_status_distribution.png
│   ├── required_education_distribution.png
│   ├── location_distribution.png
│   ├── salary_distribution.png
│   ├── salary_boxplot.png
│   ├── automation_risk_distribution.png
│   ├── automation_risk_boxplot.png
│   ├── correlation_heatmap.png
│   ├── scatter_salary_vs_automation.png
│   └── scatter_experience_vs_remote.png
└── README.md                   ← You are here!
```

---

## 📊 Dataset Information

| Property | Details |
|---|---|
| Source | Kaggle |
| Rows | 30,000 |
| Columns | 13 |
| Missing Values | None ✅ |
| Target Column | AI Impact Level (Low / Moderate / High) |
| Type | Synthetic Dataset |

### Columns:
| Column | Type | Description |
|---|---|---|
| Job Title | Categorical | Name of the job role |
| Industry | Categorical | Industry sector |
| Job Status | Categorical | Increasing / Decreasing |
| AI Impact Level | Categorical | Low / Moderate / High (Target) |
| Median Salary (USD) | Numerical | Annual salary in USD |
| Required Education | Categorical | Education level required |
| Experience Required (Years) | Numerical | Years of experience needed |
| Job Openings (2024) | Numerical | Current job openings |
| Projected Openings (2030) | Numerical | Projected openings by 2030 |
| Remote Work Ratio (%) | Numerical | % of remote work |
| Automation Risk (%) | Numerical | Risk of being automated |
| Location | Categorical | Country |
| Gender Diversity (%) | Numerical | Gender diversity ratio |

---

## 🛠️ Tools & Libraries

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
from scipy.stats import chi2_contingency
from scipy import stats
```

---

## 🔍 EDA Steps Followed

| Step | Description |
|---|---|
| 1 | Import Libraries |
| 2 | Load Data |
| 3 | First Look (shape, info, describe) |
| 4 & 5 | Drop Columns & Handle Missing Values |
| 6 | Encoding (deferred to multivariate stage) |
| 7 | Univariate Analysis |
| 8 | Bivariate Analysis (Chi-square & ANOVA) |
| 9 | Multivariate Analysis (Heatmap & Scatter) |

---

## 📌 Key Findings

### Univariate Analysis
- ✅ **AI Impact Level** is perfectly balanced — ~33% each (Low, Moderate, High)
- ✅ **All industries** equally represented (~12.5% each)
- ✅ **Job Status** — 50.4% Increasing, 49.5% Decreasing
- ✅ **Salary** is normally distributed, median ~$90,000, no outliers
- ✅ **Automation Risk** ranges from 0% to 99.99% — uniformly distributed
- ✅ Most columns show **uniform distribution** — typical of synthetic data

### Bivariate Analysis
| Column | Test | P-value | Result |
|---|---|---|---|
| Industry | Chi-square | 0.5577 | ❌ Independent |
| Job Status | Chi-square | 0.4575 | ❌ Independent |
| Required Education | Chi-square | 0.6308 | ❌ Independent |
| Location | Chi-square | 0.2948 | ❌ Independent |
| Median Salary | ANOVA | 0.3960 | ❌ Independent |
| Experience Required | ANOVA | 0.5223 | ❌ Independent |
| Job Openings 2024 | ANOVA | 0.6411 | ❌ Independent |
| Projected Openings 2030 | ANOVA | 0.4590 | ❌ Independent |
| Remote Work Ratio | ANOVA | 0.3448 | ❌ Independent |
| Automation Risk | ANOVA | 0.0777 | ❌ Independent |
| Gender Diversity | ANOVA | 0.7171 | ❌ Independent |

> ⚠️ All columns are independent of AI Impact Level — expected for synthetic data!

### Multivariate Analysis
- ✅ Near-zero correlation between all numerical columns
- ✅ No multicollinearity present
- ✅ Scatter plots confirm no patterns across AI Impact Levels

---

## 💡 Real World Insights

1. 🌍 **AI is a global phenomenon** — affects all countries equally
2. 🎓 **Education doesn't protect you** — PhD holders equally at risk as High School graduates
3. 💰 **Salary doesn't matter** — high paying jobs equally at risk from automation
4. 🏭 **No industry is safe** — IT, Healthcare, Finance all equally impacted
5. 📈 **Both growing and declining jobs** are equally affected by AI
6. 🤖 **Automation risk ranges 0-100%** — some jobs nearly fully automated!

---

## ⚠️ Limitations

- Dataset is **synthetic** — generated artificially, not from real companies
- In real world data, columns like **Automation Risk and Salary** would likely show significant relationships
- Projected Openings (2030) should realistically be **2-3x higher** than 2024 openings due to AI growth

---

## 👨‍💻 Author

**Prasanna Wankhede**
- 🎓 FSDS Student | Aspiring Data Scientist & AI Engineer
- 💼 Backend Developer (2+ years) transitioning to Data Science
- 📍 Pune, India
- 🐙 GitHub: [prasannawankhede](https://github.com/prasannawankhede)

---

## 📁 Part of EDA Portfolio

This project is part of my **EDA Portfolio** repository where I document my Data Science learning journey.

⭐ If you found this helpful, consider starring the repo!
