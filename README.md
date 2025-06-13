# 🎮 Predicting Video Game Revenue with Machine Learning

This project explores global video game sales trends and builds predictive models to forecast future game sales using machine learning.  
It was developed as part of a data science course project in ASU.

---

## 🛠️ Tools & Technologies

- **Python** (pandas, scikit-learn, matplotlib, seaborn)
- **Jupyter Notebook**
- **Excel** (for initial data review)
- **ML Techniques**: Linear Regression, Decision Trees, and more

---

## 📊 Project Overview

- Cleaned and explored historical video game sales data by platform, genre, and region
- Built regression models to predict global sales (`Global_Sales`) using features like:
  - Genre
  - Platform
  - Publisher
  - Critic and user scores
  - Year of release

---

## 🔍 Key Insights

- **Action** and **Shooter** games dominate sales, especially on PlayStation platforms
- Critic Score and Platform had strong correlations with sales
- The Neural Network model demonstrated **strong predictive ability** based on the R² Score, but showed **larger-than-ideal** prediction errors on some examples:
    **R² Score: 0.988**
    Indicates the model explains 98.8% of the variance in global sales — a very strong fit. This means the model effectively captured the relationship between features like genre, platform, and scores.
    **Mean Squared Error (MSE): 20,873,287**
    The average squared **difference** between predicted and actual sales was **high**. This suggests the model may be **less accurate** for extremely high-selling or low-selling games, which skew error due to the squared term.
    **Mean Absolute Error (MAE): 3,749.04**
    On average, **predictions were off** by approximately 3,749 units. While still reasonable, this reflects **room for improvement** in precision, especially for outlier titles.
- Missing data (e.g., scores for niche games) required imputation or row exclusion

---

## 📁 Files

| File | Description |
|------|-------------|
| [`Gaming-Trends-2024.xlsx`](data/Gaming-Trends-2024.xlsx) | Video game sales dataset |
| [`PredictingGameRevenueUsingMachineLearning.ipynb`](notebooks/PredictingGameRevenueUsingMachineLearning.ipynb) | Notebook with EDA, feature engineering, modeling |
| [`PredictingGameRevenueUsingMachineLearning.pdf`](reports/PredictingGameRevenueUsingMachineLearning.pdf) | Final formatted report |

---

## 🛠️ Future Improvements

- Use NLP on game titles or descriptions (if available) to improve features
- Incorporate more modern data from APIs (e.g., Steam, Metacritic)
- Apply ensemble models like Random Forest or XGBoost

---

## 📎 License

Distributed under the MIT License or Creative Commons BY 4.0.

