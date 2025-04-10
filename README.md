# 🧪 A/B Testing Analysis - FaceZonGoogAppFlix Webpage Experiment

## 📋 Project Overview

This project involves conducting an A/B testing analysis to evaluate the impact of a new landing page designed by the e-commerce company **FaceZonGoogAppFlix**. The company aims to increase its current conversion rate of **12.0%** by **at least 0.35%**. The dataset was collected over 23 days using an external software tool named 'A/B Tester'.

Our goal is to determine whether the new page performs better than the current one using statistical techniques and to provide clear, actionable insights based on the results.

---

## 📂 Dataset Information

**Columns:**
- `user_id`: Unique identifier for each user
- `timestamp`: Timestamp of when the user visited the page
- `group`: Whether the user was in the 'control' or 'treatment' group
- `landing_page`: The page shown ('old_page' or 'new_page')
- `converted`: Whether the user converted (1) or not (0)

---

## 🧮 Statistical Techniques Used

- ✅ Conversion rate calculation
- ✅ Z-test for proportions
- ✅ Sample size power analysis
- ✅ Segmented analysis (day of week)
- ✅ Logistic regression (optional deeper analysis)
- ✅ Visualizations using Seaborn/Matplotlib

---

## 📊 Key Results

| Metric                        | Value          |
|------------------------------|----------------|
| Control Conversion Rate      | 12.11%         |
| Treatment Conversion Rate    | 12.38%         |
| Z-statistic                  | -0.5718        |
| p-value                      | 0.7163         |
| Required Sample Size (per group) | 14,535     |

### ✅ Interpretation:

- The **treatment group showed a slight improvement**, but it is **not statistically significant**.
- The **p-value (0.7163)** is much higher than the 0.05 threshold → we **fail to reject the null hypothesis**.
- The **test was underpowered**: actual sample size was **less than 14,535** per group → results may not be reliable.

---

## 📌 Recommendation

At this stage, we **do not recommend implementing the new page**. While it performed slightly better, the improvement is not statistically significant, and the test was underpowered. We suggest:

- Collecting more data (reach ~14,535 users per group)
- Testing a larger or more impactful change
- Analyzing user segments for more targeted insights

---

## 📁 Files in Repository

- `ab_testing_analysis.ipynb` – Full Jupyter Notebook analysis
- `README.md` – This file
- `ecommerce_ab_data.csv` – Dataset used (if permitted to share)

---

## 📈 Tools & Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- StatsModels

---

## 🙌 Credits

This project was inspired by real-world A/B testing methodologies and aims to help data teams make informed decisions based on statistical evidence.

