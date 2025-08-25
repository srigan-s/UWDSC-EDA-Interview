# 🏅 Predicting Olympic Success: 120 Years of Athlete Data Analysis

![Python](https://img.shields.io/badge/Python-3.11-blue) ![Pandas](https://img.shields.io/badge/Pandas-Data%20Wrangling-green) ![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-yellow) ![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-orange)

**University of Waterloo Data Science Club – Exploratory Data Analysis**

---

## 🚀 Project Overview
This project explores **120 years of Olympic athlete data** to uncover trends in participation, demographics, and performance, and predicts medal success using machine learning.

**Objectives:**
1. Explore historical patterns in athlete participation, age, gender, and body metrics.  
2. Engineer meaningful features for modeling athlete success.  
3. Build predictive models to forecast medal outcomes.  
4. Provide actionable insights for coaches, analysts, and national teams.

---

## 📊 Dataset
**Contents:**
- Demographics: `Name`, `Sex`, `Age`, `Height`, `Weight`, `Team`, `NOC`  
- Event info: `Games`, `Year`, `City`, `Sport`, `Event`  
- Outcome: `Medal`  

**Scope:** ~100,000+ athlete records spanning 120 years.

---

## 🧹 Data Cleaning
- Filled missing values for `Age`, `Height`, `Weight` using mean values.  
- Replaced missing `Medal` entries with `"No Medal"`.  
- Removed duplicates to ensure clean, accurate records.  

---

## ⚙️ Feature Engineering
- **BMI:** `Weight / (Height^2)` to capture athlete body composition.  
- **Height-to-Weight Ratio:** To assess relative physique advantages.  
- **Age²:** Captures non-linear effects of age on performance.  
- **Categorical Encodings:** Sex, Sport, and Age Group for modeling.  
- **Target Variable:** `Medal_Won` = 1 if Gold/Silver/Bronze, 0 otherwise.  

**Optional Advanced Features:**
- BMI × Sport interaction  
- Physical percentiles per sport  
- Cumulative Olympic experience for repeat athletes  

---

## 📈 Exploratory Data Analysis (EDA)
**Key Insights:**
- **Participation Trends:** Steady increase in athletes; female participation rises dramatically post-1950.  
- **Age & Body Metrics:** Peak performance occurs in 20s; athletes have become taller and heavier, but BMI remains stable.  
- **Sport & Country:** Athletics dominates participation; U.S. consistently wins the most medals.  
- **Medal Patterns:** Staggered Winter/Summer Olympics post-1994 explain medal count fluctuations.

**Visualizations:**
- Gender distribution, age/height/weight histograms  
- Medal counts by sport and country  
- Athlete trends over time (height, weight, BMI)  
- Multivariate correlations: Age, BMI, height, weight vs. medals  

*Sample Visualization:*  
![Athlete BMI Distribution](https://raw.githubusercontent.com/yourusername/repo/main/images/bmi_distribution.png)  

*(Replace URL with your actual GitHub image path)*

---

## 🤖 Predictive Modeling
- **Target:** `Medal_Won` (binary classification)  
- **Features:** Age, Height, Weight, BMI, Sex, Sport, Age Group  
- **Models Implemented:** Logistic Regression, Random Forest, Gradient Boosting  
- **Key Findings:**  
  - BMI, Age, and Sport Type are most predictive of medal success  
  - Height and Weight contribute moderately once BMI is included  
  - Broad demographic attributes (Sex, Age Group) less predictive  

*Feature Importance (Random Forest):*  
![Feature Importance](https://raw.githubusercontent.com/yourusername/repo/main/images/feature_importance.png)  

---

## 💡 Key Findings
1. Athlete participation has steadily increased, with female representation approaching parity.  
2. Physical attributes (BMI, height, weight) correlate strongly with sport-specific success.  
3. U.S. athletes dominate medals; Athletics is the most popular sport.  
4. Predictive models show physical and sport-specific features are more important than broad demographics.

---

## 🏆 Resume-Worthy Highlights
- Analyzed 120 years of Olympic history with **100,000+ records**.  
- Engineered features like **BMI, Age², and sport-specific interactions**.  
- Built **machine learning models** achieving strong predictive accuracy.  
- Derived **actionable insights** for athlete performance optimization.

---

## ⚡ Optional Next Steps
- Multi-class medal prediction (Gold, Silver, Bronze, No Medal)  
- Interactive dashboards using **Plotly** or **Streamlit**  
- Country-level efficiency analysis (medals per athlete)  
- Time-series modeling for repeat Olympians  
