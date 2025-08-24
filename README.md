# 🏡 Regression Analysis with Feature Selection

This project explores the application of **Linear Regression**, **Ridge Regression**, and **Lasso Regression** models on the **California Housing dataset**.  
The goal is to predict housing values based on various features and investigate the impact of **feature selection** using Lasso regression.

---

## 📊 Analysis Steps Performed

1. **Data Loading and Preparation**  
   - Loaded the California Housing dataset.  
   - Split data into training and testing sets.  

2. **Initial Model Training and Evaluation**  
   - Trained Linear, Ridge, and Lasso regression models on the full dataset.  
   - Calculated R² scores for model performance.  

3. **Feature Selection using Lasso**  
   - Analyzed Lasso model coefficients.  
   - Identified features with **non-zero coefficients**.  

4. **Retraining with Selected Features**  
   - Retrained Linear, Ridge, and Lasso models using only features selected by the Lasso model.  

5. **Comparison of Results**  
   - Compared R² scores of models trained with **all features** vs. **selected features**.  

---

## 🔑 Key Findings

- **Non-zero features identified by Lasso:**  
  - `MedInc`  
  - `HouseAge`  
  - `Population`  
  - `AveOccup`  
  - `Latitude`  
  - `Longitude`

- **Model Performance with Selected Features:**  
  - Linear Regression: **R² ≈ 0.5820**  
  - Ridge Regression: **R² ≈ 0.5820**  
  - Lasso Regression: **R² ≈ 0.5318**

- **Comparison (All Features vs. Selected Features):**

  | Model              | All Features R² | Selected Features R² |
  |--------------------|-----------------|-----------------------|
  | Linear Regression  | 0.5758          | 0.5820               |
  | Ridge Regression   | 0.5759          | 0.5820               |
  | Lasso Regression   | 0.5318          | 0.5318               |

---

## 💡 Insights

- Using only **Lasso-selected features** slightly improved or maintained performance for **Linear** and **Ridge Regression**.  
- Lasso regression performance remained the same, indicating it effectively discarded less useful features.  
- The discarded features contributed little to predictive power.  

---

## 🚀 Next Steps

- Experiment with different **regularization strengths (alpha values)** for Ridge and Lasso.  
- Explore **alternative feature selection methods** (e.g., Recursive Feature Elimination, PCA).  
- Apply **other regression algorithms** (e.g., ElasticNet, Decision Tree Regressor, Random Forest Regressor).  

---

## 📂 Project Structure

