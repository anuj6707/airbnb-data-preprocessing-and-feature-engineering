# Airbnb Data Preprocessing & Analysis Pipeline 

##  Overview

This project focuses on building a structured data preprocessing and analysis pipeline for an Airbnb listings dataset. The goal is to transform raw, inconsistent data into a clean and meaningful format suitable for analysis.

---

##  Objectives

* Handle missing values using appropriate strategies
* Clean and standardize raw dataset columns
* Encode categorical variables
* Detect and remove outliers
* Perform feature engineering
* Extract insights using exploratory data analysis (EDA)

---


## ⚙️ Pipeline Steps

### 🧹 1. Missing Value Handling

* Filled text columns with `"unknown"`
* Used median for numerical columns
* Logical handling for review-related fields
* Dropped rows with critical missing values (price, location)

---

### 🧽 2. Data Cleaning

* Converted price and service fee to numeric format
* Removed unnecessary columns (`country_code`, `license`)
* Standardized column names

---

### 📉 3. Outlier Removal

* Applied IQR (Interquartile Range) method
* Removed extreme values from the `price` column

---

### 🔢 4. Feature Encoding

* One-hot encoding for `host_identity_verified`
* Ordinal mapping for `cancellation_policy`

---

### 🧠 5. Feature Engineering

* `price_per_night` → normalized pricing
* `availability_level` → categorized availability
* `is_active` → listing activity indicator
* `is_highly_rated` → rating-based feature
* `host_experience` → categorized host listings

---

### 📊 6. Exploratory Data Analysis (EDA)

* Price distribution visualization
* Relationship analysis (price vs availability, ratings)
* Correlation heatmap
* Category distribution plots

---

## 📈 Key Insights

* Most listings fall within lower to mid price ranges
* Price distribution is right-skewed
* Higher-rated listings tend to have higher prices
* Availability shows moderate relationship with pricing

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn

---


---

## 🚀 Future Improvements

* Add machine learning model for price prediction
* Perform advanced feature engineering
* Build interactive dashboards

---


