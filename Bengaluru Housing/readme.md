# 🏠 Bengaluru House Price Prediction

This project uses **Linear Regression** to predict housing prices in Bengaluru based on features like square footage, number of bathrooms, BHK, area type, and location. It demonstrates a full machine learning pipeline with data cleaning, preprocessing, visualization, model training, and evaluation.

---

## 📌 Project Objectives

- Predict house prices in Bengaluru using structured housing data.
- Build a machine learning pipeline using `scikit-learn`.
- Explore the effect of various features on pricing.
- Evaluate model performance using RMSE and R² metrics.
- Save the trained model for deployment (e.g., with Streamlit).

---

## 📂 Dataset

- Dataset Name: `Bengaluru House Data`
- Source: [Kaggle](https://www.kaggle.com/datasets)
- Features include:
  - `total_sqft`: Total area of the property
  - `bath`: Number of bathrooms
  - `bhk`: Bedrooms (derived from size)
  - `balcony`: Number of balconies
  - `area_type`, `location`: Categorical features
  - `price`: Target variable

---

## 🔧 Technologies Used

- Python 🐍
- pandas, NumPy
- Matplotlib, Seaborn 📊
- Scikit-learn 🔬
- Jupyter Notebook 📓

---

## 📊 Model Overview

- Model Used: **Linear Regression**
- Pipeline:
  - Numerical features scaled using `StandardScaler`
  - Categorical features encoded using `OneHotEncoder`
- Data Split: Train, Validate, Test

| Metric      | Validation Set | Test Set |
|-------------|----------------|----------|
| RMSE        | ~₹10.28 Lakhs  | ~₹8.6 Lakhs |
| R² Score    | 0.53           | 0.58     |

---

## 📈 Key Visualizations

- Heatmap of correlations
- Price distribution
- Predicted vs Actual Prices (with lakhs formatting)
- Residual distribution

---

## 💾 Model Saving

The trained model is saved as:

```python
import joblib
joblib.dump(pipeline, "bengaluru_price_model.pkl")
```
---

## 🚀 Future Improvements

- Try advanced models like **Ridge/Lasso**, **Decision Trees**
- Add feature engineering for `availability` and `society`
- Perform **hyperparameter tuning** using `GridSearchCV`
- Deploy using **Streamlit** for real-time user interaction

---

## 📁 Files

- `bengaluru.ipynb`: Main notebook with model and plots
- `house_price_model.pkl`: Saved model (optional)
- `README.md`: Project documentation

---

## 🧠 Author

- 💼 B.Tech CSE Student
- 📚 Learning Machine Learning with *ISLP* and *Hands-on ML by Geron*
- 🔗 [LinkedIn – Ritabrata Dutta](https://www.linkedin.com/in/ritabrata-dutta-0a0077320/)

---

