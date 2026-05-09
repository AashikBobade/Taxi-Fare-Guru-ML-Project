# 🚕 Taxi Fare Guru: Total Amount Prediction

## 📌 Overview

**Taxi Fare Guru** is a machine learning project developed to predict the **total fare amount** paid by passengers for taxi rides. The model leverages trip-related features such as distance, time, passenger count, and location data to make accurate predictions.

This project was completed as part of a college Machine Learning coursework and also submitted on Kaggle.

---

## 🎯 Objective

To build a robust regression model that accurately predicts the **`total_amount`** of taxi rides using historical trip data.

---

## 📊 Dataset Description

The dataset consists of three main files:

* **train.csv** – Contains features along with the target variable `total_amount`
* **test.csv** – Contains features only (target variable to be predicted)
* **sample_submission.csv** – Format for submission

### 🔑 Key Features

| Feature                 | Description                       |
| ----------------------- | --------------------------------- |
| `total_amount`          | Total fare paid (target variable) |
| `VendorID`              | Taxi vendor identifier            |
| `tpep_pickup_datetime`  | Pickup timestamp                  |
| `tpep_dropoff_datetime` | Drop-off timestamp                |
| `passenger_count`       | Number of passengers              |
| `trip_distance`         | Distance traveled                 |
| `RatecodeID`            | Rate code                         |
| `store_and_fwd_flag`    | Data storage flag                 |
| `PULocationID`          | Pickup location ID                |
| `DOLocationID`          | Drop-off location ID              |
| `payment_type`          | Payment method                    |

---

## 🛠️ Tech Stack

* **Python**
* **Scikit-learn**
* **XGBoost**
* **Pandas, NumPy**
* **Matplotlib, Seaborn**
* **Kaggle**

---

## 📦 Data Access

The dataset is already included in this repository for convenience.

Alternatively, you can download it directly from Kaggle using `kagglehub`:

```python
import kagglehub

# Download latest version
path = kagglehub.competition_download('taxi-fare-guru-total-amount-prediction-challenge')

print("Path to competition files:", path)
```


---

## 🔍 Workflow

### 1. Exploratory Data Analysis (EDA)

* Analyzed distributions and correlations
* Identified outliers and missing values
* Visualized trip patterns and fare relationships

### 2. Data Preprocessing

* Handled missing values
* Converted datetime features into useful components
* Encoded categorical variables

### 3. Feature Engineering

* Extracted time-based features (hour, day, etc.)
* Derived useful relationships between variables

### 4. Model Training

Tested multiple regression algorithms:

* Linear Regression
* Decision Tree Regressor
* Random Forest Regressor
* Gradient Boosting Regressor
* Extra Trees Regressor
* XGBoost Regressor

### 5. Model Evaluation

* Metric used: **R² Score**
* Compared performance across models

---

## 📈 Results

* ✅ **Best R² Score:** `0.94871`
* 🏆 **Kaggle Rank:** 30 / 714 participants

The model demonstrated strong predictive performance and generalization capability.

---

## 📓 How to Run

Open the notebook:

1. Final Notebook.ipynb
2. Run all cells sequentially to reproduce results
3. Ensure dataset files are in the same directory as the notebook

---

## 📌 Key Learnings

* Importance of feature engineering in regression tasks
* Comparing multiple models improves final performance
* Handling real-world noisy data effectively
* Practical experience with Kaggle competitions

---

## 🔮 Future Improvements

* Deployment as a web application
* Incorporating geospatial features
* Using deep learning models for further improvement

---

## 🙌 Acknowledgements

* Kaggle for providing the dataset and competition platform
* Open-source ML libraries for tools and frameworks

---


