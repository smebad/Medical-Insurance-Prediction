# 📊 Medical Insurance Prediction

**Author:** [Syed Muhammad Ebad](https://www.kaggle.com/syedmuhammadebad)  
**Date:** 28-Oct-2024  
📧 [Send me an email](mailto:mohammadebad1@hotmail.com)  
💻 [Visit my GitHub profile](https://github.com/smebad)

**Dataset:** [Medical Cost Personal Datasets](https://www.kaggle.com/datasets/mirichoi0218/insurance)

---

## 📝 Project Overview
In this project, we aim to predict **medical insurance costs** based on variables such as age, BMI, smoking habits, and region. The models explored include **Linear Regression** and **XGBoost Regression**. Linear Regression serves as a baseline, while XGBoost, a powerful gradient-boosting model, provides enhanced predictive accuracy with its ability to model complex data patterns.

---

## 🔍 Exploratory Data Analysis (EDA)
1. **Importing Libraries**:
Essential libraries such as pandas, numpy, matplotlib, seaborn, scikit-learn, and xgboost are imported.

2. **Loading the Dataset**:
Load the data and review initial details, including data types and potential missing values.

3. **Statistical Summary**:
Provides a statistical overview, including min, max, mean, and standard deviation, of numerical features.

4. **Data Visualization**:
Visualizations of distributions for features like age, bmi, children, and charges aid in identifying patterns and outliers.

5. **Encoding Categorical Variables**:
Transform categorical data into numerical form (e.g., sex, smoker, region), enabling compatibility with regression models.

6. **Correlation Analysis**:
A heatmap reveals relationships between variables, notably a strong positive correlation between smoker status and charges.

## 🧠 Model Building and Evaluation
1️⃣ Baseline Model - Linear Regression
Linear Regression provides a straightforward model for examining relationships between input features and charges.

* R² Score and Mean Absolute Error (MAE) are evaluated.
* Observation: Linear Regression may not fully capture complex, non-linear relationships.

2️⃣ Enhanced Model - XGBoost
XGBoost Regression captures non-linear patterns and offers higher accuracy.

* R² Score and MAE are re-evaluated.
* Observation: XGBoost demonstrates improved predictive accuracy and is better suited to model the dataset.

## 📊 Example Prediction
``` # Linear Regression Prediction
input_data = (28, 0, 33, 3, 0, 1)
input_data_reshaped = np.array(input_data).reshape(1, -1)
prediction_lr = model.predict(input_data_reshaped)
print('Linear Regression Prediction:', prediction_lr[0])

# XGBoost Prediction
prediction_xgb = xgb.predict(input_data_reshaped)
print('XGBoost Prediction:', prediction_xgb[0])
```
## 📝 Summary
This project explores predicting medical insurance costs using Linear Regression and XGBoost models. The analysis suggests that XGBoost is preferable due to its advanced prediction capabilities. Key factors like age, BMI, and smoking habits significantly impact insurance charges, and this project demonstrates how machine learning can help in deriving these insights.

### Happy Coding! 😊

  
