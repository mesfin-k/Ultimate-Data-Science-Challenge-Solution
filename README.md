# 🚀 Ultimate Data Science Challenge – Springboard

### Author: [Mesfin Kebede](https://github.com/mesfin-k)
### Repository: [Ultimate-Data-Science-Challenge-Solution](https://github.com/mesfin-k/Ultimate-Data-Science-Challenge-Solution)

---

## 📘 Project Overview
This repository contains my complete solution for the **Ultimate Data Science Challenge** — a real-world data science case study provided by Springboard.  
The goal is to analyze user behavior, design an experiment, and build a predictive model for rider retention.

The challenge is divided into **three main parts**:
1. **Exploratory Data Analysis (EDA)** on login activity (`logins.json`)
2. **Experiment & Metrics Design** for toll-reimbursement policy between Gotham and Metropolis
3. **Predictive Modeling** of user retention (`ultimate_data_challenge.json`)

---

## 📂 Repository Contents
| File | Description |
|------|--------------|
| `logins.json` | Simulated user login timestamps for Part 1 |
| `logins.ipynb` | Jupyter notebook for login EDA and visualization |
| `ultimate_data_challenge.json` | User data for retention modeling |
| `ultimate_data_challenge.ipynb` | Main analysis notebook for cleaning, EDA, and modeling |
| `final.ipynb` | Consolidated notebook containing final write-up and conclusions |
| `ultimate_data_science_challenge.pdf` | Report version of the final submission |
| `README.md` | Project documentation (this file) |

---

## 🧮 Part 1 – Exploratory Data Analysis (Logins)

**Goal:**  
Aggregate login counts into **15-minute intervals** and visualize temporal patterns.

**Key Insights:**
- Strong **daily and weekly cycles** in demand.  
- Higher login frequency during **evenings and weekends**.  
- Detected minor data inconsistencies (timestamp irregularities).  

---

## 🧪 Part 2 – Experiment & Metrics Design

**Scenario:**  
Two neighboring cities (Gotham and Metropolis) have different active hours.  
A toll bridge discourages drivers from serving both cities. Management proposes reimbursing tolls.

**Proposed Design:**
- **Metric:** Proportion of drivers serving both cities.
- **Approach:** Randomized A/B test (treatment = toll reimbursement).
- **Statistical Test:** Two-sample t-test or Chi-Square on driver cross-city trips.
- **Interpretation:** If treatment group shows significant lift → rollout city-wide.

---

## 🤖 Part 3 – Predictive Modeling (Retention)

**Goal:** Predict if a user will be active in their 6th month.  

**Data Cleaning & EDA**
- Handled missing values (median/mode).  
- Removed duplicates → retained ~37.6% of valid entries.  
- Key predictors: early trips, weekday use, premium status, and city.

**Model Comparison**
| Model | AUC | Notes |
|--------|------|-------|
| **XGBoost** | **0.86** | Best balance of accuracy & speed |
| Random Forest | 0.85 | Robust & interpretable |
| Logistic Regression | 0.76 | Baseline model |

**Validation:**
- 5-fold cross-validation  
- Accuracy: 0.76–0.78  
- F1: 0.71–0.72  
- Tight confidence interval (F1 CI [0.70, 0.74])  

**Business Impact:**
- Target low-activity users via early-trip incentives or premium trials.  
- Expected **15–20% retention lift** using personalized offers.

---

## 🛠️ Tools & Libraries
- **Python:** Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn  
- **Jupyter Notebook:** Analysis, visualization, and documentation  
- **Validation:** GridSearchCV, Cross-Validation, Bootstrap CI  

---

## 📈 Results Summary
- Identified patterns in rider activity and retention behavior.  
- Built a robust model (AUC 0.86) to predict customer churn.  
- Designed a statistically sound experiment to improve cross-city driver engagement.  

---

## 🧠 Key Learning Outcomes
- Time-series aggregation and visualization  
- Statistical experiment design and evaluation  
- Machine learning model tuning and performance validation  
- Translating data insights into actionable business strategies  

---

## 📬 Contact
**Mesfin Kebede**  
📧 [mesfin.k.kebede@gmail.com](mailto:mesfin.k.kebede@gmail.com)  
🌐 [LinkedIn Profile](https://www.linkedin.com/in/mesfin-kebede/)  
💻 [GitHub Portfolio](https://github.com/mesfin-k)

---

