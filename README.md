# EDA & Inferential Analysis: Global Cancer Trends (2015-2024)

### Project Vision

This project harnesses the power of advanced analytics and global health data to uncover actionable insights into cancer care, outcomes, and disparities. Using a robust dataset of 50,000 cancer patient records collected from multiple countries between 2015 and 2024, we aim to bridge the gap between raw data and life-saving decisions.

### What the Data Covers

The dataset offers a 360-degree view of cancer patient profiles, including:

* **Demographics:** Age, Gender, Country, Year of Diagnosis.
* **Genetic & Lifestyle Risks:** Genetic Predisposition, Smoking, Alcohol Use, Obesity.
* **Environmental Exposure:** Air Pollution.
* **Clinical & Economic variables:** Cancer Type, Stage, Treatment Cost.
* **Patient Outcomes:** Survival Years, Severity Scores.

### Core Objectives

1. **Exploratory Data Analysis (EDA):** Identify key trends, patterns, and relationships while visualizing disparities in diagnosis, lifestyle, and treatment across demographics.
2. **Inferential & Predictive Analytics:** Use statistical methods to determine the relationship between risk factors and cancer severity and identify key predictors of survival.
3. **Insight Extraction:** Systematically document evidence-backed inferences linked to real-world implications for clinical and operational use.

### Key Insights & Statistical Inferences

#### 1. Risk Factor Interaction (Hypothesis Testing)
We performed a **Multiple Linear Regression** with an interaction term to see if higher genetic risk amplifies the negative effects of smoking on cancer severity.
* **Null Hypothesis ($H_0$):** No interaction effect between genetic risk and smoking.
* **Finding:** The p-value was **0.628**.
* **Conclusion:** Since $p > 0.05$, we fail to reject the null hypothesis. Smoking and genetic risk act as **independent contributors**; there is no evidence that one amplifies the other.

![Regression Test](https://github.com/chinmai-budati/EDA-on-Cancer-Dataset/blob/main/multiple_line_regression_test.png)


#### 2. Demographic Profile
* **Finding:** The patient population spans from ages **20 to 89**, with a mean age of **54.4 years**.
* **Inference:** The broad distribution allows for reliable trend analysis across different life stages, ensuring findings are applicable to both young and geriatric populations.

![Age Distribution](https://github.com/chinmai-budati/EDA-on-Cancer-Dataset/blob/main/age_distribution.png)

#### 3. Economic Impact vs. Survival
* **Method:** Used the **Kruskal-Wallis test** to evaluate if higher cancer stages lead to significantly greater treatment costs.
* **Finding:** While costs scale with severity, higher treatment costs do not always show a linear correlation with longer survival, highlighting the diminishing returns of late-stage intervention.

![Economic Burden](https://github.com/chinmai-budati/EDA-on-Cancer-Dataset/blob/main/stages.png)

### Tech Stack
* **Language:** Python
* **Analysis:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
* **Statistics:** Scipy, Statsmodels (OLS Regression)
* **Machine Learning:** Scikit-learn (Random Forest)

### Repository Structure

* `Cancer Data Analysis.ipynb`: Complete source code with data cleaning, EDA, and regression analysis.
* `global_cancer_patients_2015_2024.csv`: The primary dataset used for analysis.
* `README.md`: Project overview and key findings.
