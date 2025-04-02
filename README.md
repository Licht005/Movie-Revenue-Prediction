
---

# **📊 Movie Revenue Prediction using Random Forest**

## **🚀 Project Overview**
This project aims to **predict worldwide movie revenue** using machine learning. After experimenting with different models like **XGBoost**, **RandomForestRegressor** proved to be the best, achieving **high accuracy** in revenue forecasting.  

📌 **Key Highlights:**  
✔ Predicts **worldwide revenue** based on **opening revenue, opening theaters, release days, and MPAA rating**  
✔ Implements **feature selection, encoding, and scaling** for optimized predictions  
✔ Achieves **R-Squared of 0.9999**, meaning **exceptionally precise revenue forecasting**  
✔ Uses **visualizations** to evaluate model performance  

---

## **📂 Dataset Information**
The dataset contains **2,694 movies**, with key features including:  
- `opening_revenue`: Revenue earned during the opening weekend.  
- `opening_theaters`: Number of theaters showing the movie during its debut.  
- `release_days`: Total number of days the movie was in theaters.  
- `MPAA`: Content rating of the movie (`PG`, `R`, etc.).  
- `world_revenue`: Total worldwide revenue (target variable).  

⚠ **Categorical features like `MPAA` were encoded**, and numerical features were **scaled** for better training.

---

## **🛠 Model Training**
After comparing models, **Random Forest Regressor** was selected due to its superior accuracy. The training process involved:

1️⃣ **Feature Engineering** – Selecting relevant predictors.  
2️⃣ **Data Preprocessing** – Scaling numerical features and encoding categorical ones.  
3️⃣ **Hyperparameter Tuning** – Optimizing **max depth, n_estimators, min_samples_split**.  
4️⃣ **Model Evaluation** – Measuring **MSE, MAE, and R-Squared** for accuracy.

✅ **Final Model Results:**  
```
Mean Squared Error: 7.53 × 10⁻⁵  
Mean Absolute Error: 0.00185  
R-Squared: 0.9999  
```

---

## **📊 Visualizations**
This project includes **several plots** for deeper insights:
📌 **Feature Importance** – Shows which variables impact revenue the most.  
📌 **Predictions vs Actual Revenue** – Scatter plot comparing predictions to actual values.  
📌 **Residual Distribution** – Analyzes model errors for bias detection.  

Example Code to Run Feature Importance Plot:
```python
import matplotlib.pyplot as plt

plt.figure(figsize=(10, 6))
plt.barh(importance_df['Feature'], importance_df['Importance'], color='skyblue')
plt.xlabel("Importance Score")
plt.ylabel("Feature")
plt.title("Feature Importance in Random Forest")
plt.gca().invert_yaxis()
plt.show()
```

---

## **📜 Next Steps**
🔹 **Validate model performance** on new movie data.  
🔹 **Explore additional features like distributor and genre** to test improvements.  
🔹 **Optimize further using ensemble stacking** to combine models for even stronger predictions.  

Would you like me to refine any sections before you upload this? 🚀  
Let me know if you need any additional details! 😊
