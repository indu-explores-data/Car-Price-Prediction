# 🚗 Car Price Prediction using Machine Learning

## 📘 Project Overview
This project focuses on predicting car prices using ensemble machine learning models — **Random Forest** and **Gradient Boosting**.  
It demonstrates how these models perform on regression tasks and compares their predictive accuracy using key metrics.  
The project also includes an analysis of feature importance and how **feature reduction** impacts model performance.

---

## 🎯 Objectives
- Build predictive models to estimate car prices based on multiple attributes.  
- Compare **Random Forest** and **Gradient Boosting** regressors.  
- Evaluate model performance using **MAE**, **RMSE**, and **R² Score**.  
- Analyze the effect of **feature reduction** on model accuracy.  
- Identify the most influential features that drive car prices.  

---

## 🧠 Key Methods
- **Data Preprocessing:** Cleaned dataset by removing irrelevant columns, handling missing values, and encoding categorical variables.  
- **Feature Importance:** Extracted and ranked features contributing most to price prediction.  
- **Model Training:** Applied **Random Forest Regressor** and **Gradient Boosting Regressor**.  
- **Model Evaluation:** Compared models using regression metrics (MAE, RMSE, R²).  
- **Feature Reduction:** Evaluated model performance with top 5 most important features.

---

## 📊 Visualizations & Insights

### 1️⃣ Distribution of Car Prices  
Understanding how car prices are distributed helps identify skewness and potential outliers.  
![Distribution of Car Prices](./images/Distribution%20of%20Car%20Prices.png)

---

### 2️⃣ Log-Transformed Distribution of Car Prices  
A log transformation was applied to normalize the price distribution and reduce skewness.  
![Log-Transformed Distribution of Car Prices](./images/Log-Transformed%20Distribution%20of%20Car%20Prices.png)

---

### 3️⃣ Boxplot of Car Prices  
Visualizes spread, median, and outliers in car prices.  
![Boxplot of Car Prices](./images/Boxplot%20of%20Car%20Prices.png)

---

### 4️⃣ Correlation of Features with Car Price  
Highlights which features are most correlated with price — engine size, horsepower, and curb weight stand out.  
![Correlation of Features with Car Price](./images/Correlation%20of%20Features%20with%20Car%20Price.png)

---

### 5️⃣ Model Performance Comparison  
Compares **Random Forest** and **Gradient Boosting** models using R², MAE, and RMSE metrics.  
![Model Performance Comparison](./images/Model%20Performance%20Comparison.png)

---

### 💡 Insight: Impact of Feature Reduction on Model Performance

This comparison illustrates how reducing the feature set to the **top 5 most important features** affects the performance of the **Random Forest** regression model in predicting car prices.

---

#### 📊 Metrics Compared
- **R² Score** – Measures the proportion of variance explained by the model.  
- **MAE (Mean Absolute Error)** – Average absolute error in predicted vs actual price (**in USD**).  
- **RMSE (Root Mean Squared Error)** – Penalizes larger errors more than MAE (**in USD**).

---

#### 📈 Observations
- **R² Score**
  - Random Forest (Full): ~0.958  
  - Random Forest (Top 5): ~0.951  
  - 🔹 Slight decrease in explanatory power (−0.7%).

- **MAE (USD)**
  - Random Forest (Full): ~1,710 USD  
  - Random Forest (Top 5): ~1,755 USD  
  - 🔹 Slightly higher average error (+45 USD).

- **RMSE (USD)**
  - Random Forest (Full): ~2,590 USD  
  - Random Forest (Top 5): ~2,690 USD  
  - 🔹 Larger errors increased marginally (+100 USD).

---

#### 🧩 Conclusion
- The **Random Forest (Full)** model performs slightly better across all metrics.  
- However, the **difference is minimal**, showing that:
  - The **top 5 features capture most predictive power**.  
  - **Feature reduction** yields a simpler, faster model with nearly identical accuracy.  
- Ideal for **real-time systems** where efficiency and interpretability are key.

![Model Comparison Full vs Top 5 Features](./images/Model%20Comparison%20Full%20vs%20Top%205%20Features.png)  
![R² Score Comparison Full vs Top 5 Features](./images/R²%20Score%20Comparison%20Full%20vs%20Top%205%20Features.png)

---

## 💡 Key Insights & Outcomes
- Both ensemble models deliver **high predictive accuracy**.  
- **Engine size**, **horsepower**, and **curb weight** are the strongest predictors of price.  
- **Gradient Boosting** performs competitively but requires more tuning.  
- **Random Forest** provides strong accuracy with less tuning effort.  
- Reducing features leads to **simpler and faster** models with only minor accuracy loss.  

---

## 🧰 Technologies Used
- **Language:** Python  
- **Libraries:** pandas, numpy, matplotlib, seaborn, scikit-learn  
- **Environment:** Jupyter Notebook  

---

## ⚙️ Setup & Installation
**1. Clone the repository:**
   ```bash
   git clone https://github.com/indu-explores-data/Car-Price-Prediction.git
   cd Car-Price-Prediction
   ```
**2. Install dependencies:**
   ```
   pip install -r requirements.txt
   ```
**3. Run the notebook:**
  ```
  jupyter notebook "Car Price Prediction.ipynb"
  ```
---

## ▶️ Usage Instructions

- Open the notebook **Car Price Prediction.ipynb**.
- Run all cells to:
- Load and preprocess data
- Train Random Forest and Gradient Boosting models
- Compare their results and visualize performance

---

## 🔗 Connect with Me

Let’s connect on LinkedIn for project discussions or data-driven collaborations:

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Profile-blue?logo=linkedin)](https://www.linkedin.com/in/indu-r-3a3767170/)

---

## 🙌 Feedback & Support

If you found this project helpful, please ⭐ star the repository and share your thoughts. Suggestions and contributions are always welcome!
