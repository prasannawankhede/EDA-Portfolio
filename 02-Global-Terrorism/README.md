
# 🌍 Global Terrorism EDA — The Human & Economic Cost of War

It is with a heavy heart that I present this analysis. This project is not just 
about numbers and graphs — it is about real people, real families, and real pain 
that has shaped our world over the last 50 years.

---

## 📌 About This Project

This project performs **Exploratory Data Analysis (EDA)** on the **Global Terrorism 
Database (GTD)** — one of the most comprehensive open-source datasets on terrorist 
attacks worldwide, covering **1970 to 2017**.

The dataset contains **1,81,691 attacks** across **205 countries** with **135 features** 
per incident — maintained by researchers at the University of Maryland.

---

## 🎯 Objective

> *"To understand the devastating human and economic impact of terrorism on ordinary 
> people — and why the world desperately needs peace."*

Through data, this project uncovers:
- 📈 How terrorism grew over 50 years
- 🌍 Which regions and countries suffered the most
- 💀 The true human cost — lives lost and wounded
- 💰 The economic destruction left behind
- 🕊️ What this data tells us about the urgent need for world peace

---

## 📂 Dataset Information

| Property | Details |
|---|---|
| Source | Global Terrorism Database (GTD) |
| Maintained By | START, University of Maryland |
| Time Period | 1970 — 2017 |
| Total Records | 1,81,691 attacks |
| Total Columns | 135 |
| Columns Used | 15 |
| Target Column | `success` (1 = Attack succeeded, 0 = Failed) |

---

## 📊 EDA Structure

| Step | Description |
|---|---|
| Step 1 | Import Libraries |
| Step 2 | Load Dataset |
| Step 3 | First Look at Data |
| Step 4 | Drop Unnecessary Columns |
| Step 5 | Handle Missing Values |
| Step 6 | Encode Categorical Columns |
| Step 7 | Univariate Analysis |
| Step 8 | Bivariate Analysis |
| Step 9 | Multivariate Analysis |
| Step 10 | Conclusions & World Peace Message |

---

## 🔑 Key Findings

| Finding | Insight |
|---|---|
| 1,81,691 attacks in 47 years | Terrorism never stopped — it only grew |
| Middle East & South Asia suffered most | Poorest regions pay the heaviest price |
| Civilians are the #1 target | War was never about armies |
| Bombing is most common attack | Cheap, accessible and maximally destructive |
| Attacks exploded after 2010 | The world became MORE dangerous, not less |
| 4,11,868 people killed | Nearly half a million lives lost forever |
| 5,23,869 people wounded | Survivors carry scars for life |

---

## 💰 The Real Economic Cost

The true cost of terrorism goes far beyond what this dataset captures.

The **War on Terror alone cost $8 trillion** between 2001-2021.

**With $8 trillion we could have:**
- 🏫 Built **80 lakh schools** across the developing world
- 🏥 Built **40 lakh hospitals** in regions with no healthcare
- 💧 Provided **clean drinking water** to every person on earth
- ⚡ Powered **entire continents** with renewable energy
- 🌾 Ended **world hunger** for the next 50 years

---

## 📁 Repository Structure

- `global_terrorism_eda.ipynb` — Main EDA notebook
- `globalterrorismdb_0718dist.csv` — Dataset
- `README.md` — This file
- `gtd_images/` — All generated graphs




---

## 🛠️ Libraries Used

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
from scipy.stats import chi2_contingency, f_oneway
```

---

## 🕊️ Final Message

This analysis is a reminder that behind every row in this dataset is a human 
story — a family destroyed, a village burned, a child who never got to grow up.

Data science gives us the power to see patterns — and the pattern here is clear.

**War has never built anything. Peace does.**

> *"Every bomb that was built — was a school that was never constructed"*

> *"The regions that can least afford war — suffer from it the most"*

> *"4,11,868 people didn't die in this dataset — they were fathers, mothers, 
> children and dreamers"*

---

*Made with data, empathy and a deep desire for world peace* 🕊️

*— Prasanna Wankhede | FSDS Student | Pune, India 🇮🇳*
