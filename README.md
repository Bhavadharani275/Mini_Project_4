# Mini-Project-4
**Project Title**: *🏝️ Tourism Experience Analytics Dashboard*

---

**Domain:** Tourism  
**Tools Used:** Streamlit, Pandas, Plotly, SQL, Google Colab, Machine Learning (Regression, Classification & Recommendation)

---

## 📘 Project Overview
This project aims to develop an **end-to-end Tourism Analytics System** that predicts tourist visit modes, analyzes travel trends, and recommends personalized attractions using machine learning models.  
It integrates **Regression**, **Classification**, and **Recommendation** modules inside an interactive **Streamlit dashboard**.

---

## 🚀 Objectives
- Predict **visit mode** (Solo, Family, Friends, Couples, Business) using classification models.
- Forecast **tourism ratings** using regression models.
- Recommend **top attractions** to travelers using clustering-based recommendation systems.
- Provide **visual insights** on visitor patterns, regional popularity, and user behavior.

---
## 🧹 Data Cleaning
The data was preprocessed from multiple sources — including transactions, users, cities, and attractions.

**Steps performed:**
1. **Handle missing values** in transaction, user, and city datasets.  
2. **Resolve discrepancies** in city names, visit modes, and attraction type IDs.  
3. **Standardize date/time formats** across all records.  
4. **Handle outliers** in numeric fields such as ratings and visitor counts.  
5. **Remove duplicate or irrelevant records** where necessary.

---

## ⚙️ Data Preprocessing & Feature Engineering
- **Encoding:** Convert categorical variables (`VisitMode`, `Continent`, `Country`, `AttractionTypeId`, etc.) using Label Encoding or OneHot Encoding.  
- **Feature Aggregation:** Aggregate user-level features such as average rating per user or visit mode.  
- **Data Integration:** Merge transaction, user, city, and attraction tables into a single unified dataset.  
- **Normalization:** Scale numerical features (`Rating`, `Year`, etc.) using `StandardScaler` for model stability.  

---

## 📊 Exploratory Data Analysis (EDA)
EDA was performed to extract meaningful insights:
- 🗺️ Distribution of users across continents, countries, and regions.  
- 🎡 Popular attraction types based on user ratings.  
- 👨‍👩‍👧 Relationship between **VisitMode** and user demographics.  
- ⭐ Rating distribution across different regions and attractions.

---

## 🤖 Model Training

### 🔹 **Regression**
- Predicts attraction ratings using `Linear Regression` and `Random Forest Regressor`.
- Evaluated using **R² Score**, **MSE**, **MAE**, and **RMSE**.

### 🔹 **Classification**
- Predicts visit mode (Solo, Family, Friends, Couples, Business) using:
  - `Random Forest`
  - `XGBoost`
  - `LightGBM`
- Evaluated using **Accuracy**, **Precision**, **Recall**, and **F1-score**.

### 🔹 **Recommendation System**
- Implemented **K-Means Clustering** to segment users by travel preferences.  
- Provides personalized attraction recommendations based on cluster similarity and attraction ratings.  
- Evaluated using **RMSE** and **MAP**.


---

## 💻 Deployment - Streamlit Dashboard
A user-friendly **Streamlit web app** was built to make predictions and display insights interactively.

### 🔧 Features:
- **Select model type:** Regression, Classification, or Recommendation.
- **Dynamic input forms** for Continent, Country, Region, City, Visit Year, Month, and Attraction.
- **Automatic encoding and scaling** before model prediction.
- **Interactive visualizations** using Plotly:
  - Top-rated attractions  
  - Top regions by visitor count  
  - Cluster-based user segments (3D visualization)  
- **Personalized recommendations** based on user cluster.

---

## 📈 End Output
A fully interactive Streamlit app where users can:
- 🧭 Get predicted visit mode (e.g., Family Traveler, Business Traveler).
- 🎯 Receive attraction recommendations.
- 🌍 Explore data-driven visual insights on tourism trends.

---

## 📂 Project Structure

- `Tourism.ipynb` — Main Colab notebook
- `data/` - All Excel data files
  
---

## 🔹 How to Run in Google Colab

1. **Open the Notebook**  
   Upload or open `Tourism.ipynb` in [Google Colab](https://colab.research.google.com/).

2. **Upload the Data**  
   - Place all `.xlsx` files in the `data/` folder.

3. **Run All Cells**  
   The notebook performs:  
   - Data Cleaning & EDA  
   - Model Training  
   - Evaluation & Visualization  

4. **View Results**  
   - Interactive Plotly charts  
   - Model metrics table  
   - Actual vs Predicted plots  

---

## 👩‍💻 Author

**Bhavadharani**  
Mini-Project 4 — *Tourism Experience Analytics Dashboard*  

