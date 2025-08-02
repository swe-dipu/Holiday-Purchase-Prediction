# Holiday Purchase Prediction 🚀

**Objective**  
This project builds a machine learning model to predict whether a customer will purchase a holiday/travel package based on demographic, behavioral, and engagement features.

---

## 🎯 Project Overview

Customers are presented with various holiday package options (e.g., Basic, Standard, Deluxe, Super Deluxe, King), but historically only ~18% make a purchase. With marketing randomly targeting customers, this leads to high costs. This project aims to:

- Use customer data to identify likely purchasers
- Improve marketing ROI by focusing outreach on high‑propensity customers ([GitHub](https://github.com/rezakalmas/Holiday-Package-Prediction?utm_source=chatgpt.com), [GitHub](https://github.com/frzkstudio/holiday_package_prediction?utm_source=chatgpt.com))

---

## 🧩 Dataset & Features

Typical dataset structure includes around 4,800 rows and ~20 columns, which may include:

- **CustomerID** — unique identifier  
- **ProdTaken** — target (0 = no purchase, 1 = purchase)  
- Demographic & behavioral features such as:  
  - Age, Gender, CityTier  
  - TypeOfContact (invited vs inquiry)  
  - DurationOfPitch, NumberOfFollowups  
  - ProductPitched category  
  - PreferredPropertyStar, MaritalStatus, Occupation  
  - NumberOfTrips, Passport status, MonthlyIncome, etc.
---

## 🧪 Workflow & Methodology

1. **Data Exploration & Cleaning**  
   - Univariate & multivariate analysis  
   - Handle missing values, inconsistent labels, duplicates, and outliers
2. **Feature Engineering**  
   - Combine or transform features (e.g. total visitors)  
   - Encode categorical variables with label encoding or one-hot encoding  
   - Normalize or standardize continuous variables

3. **Feature Selection**  
   - Perform feature importance analysis using methods like variance threshold, chi-square, Pearson correlation, and tree-based importances

4. **Model Training & Evaluation**  
   - Algorithms: Logistic Regression, Decision Tree, Random Forest, AdaBoost, XGBoost  
   - Evaluation metrics focus on classification: accuracy, F1-score, AUC — especially given class imbalance
5. **Insights & Business Impact**  
   - Key influential features: ProductPitched, Passport ownership, MaritalStatus, CityTier  
   - Typical outcomes: predictive lift of ~4× using top percentile of customers; significantly reduce marketing costs by targeting likely buyers (baseline 18% purchase rate) ([GitHub](https://github.com/rezakalmas/Holiday-Package-Prediction?utm_source=chatgpt.com))


### Prerequisites
- Python 3.x  
- Libraries: pandas, numpy, scikit-learn, XGBoost, matplotlib, seaborn


Best performing model: Typically XGBoost demonstrates highest F1-score and AUC
False positive reduction: Focusing on top decile of predicted probabilities often captures > 80% of buyers
Marketing optimization: Target high‑propensity customers to significantly cut outreach cost and increase conversion
📝 LicenseMIT License — educational and research use encouraged.
👤 AuthorDipu Ghosh– [@swe‑dipu]
