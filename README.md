# 🛳️ Titanic — Exploratory Data Analysis (Task 5)

## 📌 Overview
This project is part of the **Data Analyst Internship Task 5**.  
The goal is to perform **Exploratory Data Analysis (EDA)** on the Titanic dataset to uncover patterns, trends, and anomalies related to passenger survival.

## 📂 Files in this Repository
- **train.csv** — Training dataset used for EDA.
- **test.csv** — Dataset reserved for prediction/evaluation.
- **gender_submission.csv** — Sample submission file.
- Jupyter Notebook containing all EDA steps, code, and visualizations.
- Final report summarizing key findings and recommendations.
- **README.md** — Project documentation.

## 🎯 Objective
- Explore and visualize the Titanic dataset.
- Identify key factors influencing survival.
- Generate insights for feature engineering and predictive modeling.

## 🛠 Tools & Libraries Used
- **Python**
- **Pandas** — Data manipulation and cleaning.
- **Matplotlib** — Basic plotting.
- **Seaborn** — Advanced statistical visualizations.
- **Jupyter Notebook** — Interactive analysis.

## 📊 EDA Steps Performed
1. **Data Loading & Inspection**
   - `.info()`, `.describe()` for structure and summary.
   - Checked missing values and data types.
2. **Univariate Analysis**
   - Distribution plots for `Age`, `Fare`.
   - Count plots for `Survived`, `Sex`, `Pclass`, `Embarked`.
3. **Bivariate Analysis**
   - Survival rates by `Sex`, `Pclass`, `Age`, `Fare`, `Embarked`.
   - Boxplots, Violin plots, Scatterplots.
4. **Correlation Analysis**
   - Heatmap of numeric features.
   - Pairplots for relationships.
5. **Insights & Recommendations**
   - Women and first-class passengers had the highest survival rates.
   - Younger passengers and those with higher fares survived more often.
   - Missing values in `Age` and `Cabin` require imputation or feature engineering.

## 📌 Key Insights
- **Sex**: Females ~70% survival rate; males ~20%.
- **Pclass**: 1st > 2nd > 3rd survival rates.
- **Fare**: Higher fares correlate with survival.
- **Age**: Children had a survival advantage.
- **Cabin**: Sparse data, but deck extraction could help.

## 📝 Recommendations for Modeling
- Impute missing `Age` values based on group medians.
- Extract `Title` from `Name` and `Deck` from `Cabin`.
- Create `FamilySize` and `IsAlone` features.
- Use baseline models (Logistic Regression, Random Forest, Gradient Boosting).
