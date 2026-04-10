# 🏠 House Price Prediction

## 📌 Objective
Build a regression model to predict house prices using housing dataset.

---

## 📊 Dataset Features
- Bedrooms, Bathrooms
- Square Foot Living & Lot
- Floors, Waterfront, View
- Year Built & Renovation
- City (encoded)

---

## ⚙️ Techniques Used
- Data Cleaning & Preprocessing
- One-Hot Encoding (City)
- Log Transformation on Price
- Feature Scaling (StandardScaler)

---

## 🤖 Models Used
- Linear Regression
- Random Forest Regressor
- Gradient Boosting Regressor

---

## 📈 Evaluation Metrics
- MAE (Mean Absolute Error)
- RMSE (Root Mean Squared Error)

---

## 📊 Result
Gradient Boosting performed best with lowest RMSE.

---

## 🔮 Inference Example

```python
import joblib
import numpy as np

model = joblib.load('house_model.pkl')

# example input (already scaled)
prediction = model.predict(sample_scaled)

print("Predicted Price:", np.expm1(prediction[0]))
