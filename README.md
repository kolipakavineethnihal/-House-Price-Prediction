# 🏠 Real Estate Price Estimation System

**Author: K Vineeth Nihal**

**Tech Stack: Python | Machine Learning | XGBoost | Flask**

## 📌 Project Summary

This **Real Estate Price Estimation System** is a complete, end-to-end Machine Learning web application built to forecast residential property values using key attributes like bedroom count, bathroom count, square footage, and neighborhood location.

At its core, the system leverages an **XGBoost Regressor** trained on historical housing records to uncover pricing patterns. It is wrapped in an intuitive **Flask** web interface that allows users to input property specifications and generate instant market price estimates.

## 🎯 Key Goals

* Explore, clean, and prepare raw real estate datasets.
* Impute and manage missing values across numerical and categorical features.
* Build and train a predictive XGBoost regression model.
* Benchmark model accuracy using MAE, RMSE, and R² metrics.
* Serialize the end-to-end preprocessing and modeling pipeline for deployment.
* Design a responsive web frontend powered by Flask.
* Deliver real-time property valuations from live user inputs.

## 🛠️ Tech Stack

* **Core Language:** Python
* **ML & Modeling:** XGBoost, Scikit-learn
* **Data Manipulation:** Pandas, NumPy
* **Model Serialization:** Joblib
* **Backend Framework:** Flask
* **Frontend:** HTML, CSS
* **Development Environment:** PyCharm

## 📂 Repository Layout

```text
HOUSE_PRICE_PREDICTION/
│
├── models/
│   └── house_price_model.pkl
│
├── static/
│   ├── css/
│   │   └── style.css
│   └── images/
│
├── templates/
│   └── index.html
│
├── app.py
├── main.py
├── data.csv
├── requirements.txt
└── README.md

```

## ⚙️ End-to-End Pipeline

1. Ingest the raw housing dataset.
2. Drop non-predictive fields such as `date` and `street`.
3. Perform data cleaning and feature preprocessing.
4. Segregate numerical variables from categorical variables.
5. Partition the dataset into training and validation/test splits.
6. Fit the XGBoost regression model on the training data.
7. Assess model accuracy against unseen test data.
8. Export the unified preprocessing and prediction pipeline to disk.
9. Integrate the serialized model into a Flask backend.
10. Serve live price predictions via the web UI.

## 📊 Model Evaluation

The trained model achieved the following performance benchmarks on the test set:

| Metric | Value |
| --- | --- |
| Mean Absolute Error (MAE) | $94,751.58 |
| Root Mean Squared Error (RMSE) | $197,159.29 |
| R² Score | 0.7387 |
| Variance Explained (R² %) | 73.87% |

*Note: Metrics reflect the latest training run. R² percentage indicates explained variance, not classification accuracy.*

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/moghaltanveer90-bot/HOUSE_PRICE_PREDICTION.git

```

### 2. Navigate to the Project Directory

```bash
cd HOUSE_PRICE_PREDICTION

```

### 3. Install Required Packages

```bash
pip install -r requirements.txt

```

### 4. Train and Save the Model

```bash
python main.py

```

### 5. Launch the Flask Server

```bash
python app.py

```

### 6. Access the Web App

Open any web browser and navigate to:

```text
http://127.0.0.1:5000

```

## 💡 Core Highlights

* Clean, intuitive web interface for effortless navigation.
* Interactive form for entering custom property attributes.
* Data-driven property valuation powered by XGBoost.
* Instantaneous server-side inference via Flask.
* Reusable serialized ML pipeline for fast loading without retraining.

## 👨‍💻 Contact & Author

**K Vineeth Nihal**

* Email: kolipakavineethnihal@gmail.com
* Phone: 7799517862

---

⭐ Found this project helpful? Feel free to star the repository, explore the code, and share your thoughts!

**Built with Python and Machine Learning.**
