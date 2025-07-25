# 🌤️ Weather Classification using Machine Learning

This project is a **multiclass classification** system that predicts weather conditions — **Sunny**, **Cloudy**, **Partly Cloudy**, or **Rainy** — based on features like **humidity**, **altitude**, **region type**, and **cloud coverage**. Multiple machine learning models were implemented and compared, with **Random Forest** achieving the highest accuracy of **91.74%** after tuning.

---

## 📌 Problem Statement

Predict the type of weather condition using structured data containing environmental features. The project aims to classify each sample into one of the following weather types:

- ☀️ Sunny  
- ☁️ Cloudy  
- 🌤️ Partly Cloudy  
- 🌧️ Rainy

---

## 📊 Dataset

- **Source**: Kaggle  
- **Filename**: `weather_classification_data.csv`  
- **Features**: Humidity, Altitude, Region Type, Cloud Coverage, and more  
- **Target**: Weather condition (encoded as 0.0, 1.0, 2.0, 3.0)

> 📎 *Note: Please download the dataset manually from Kaggle and place it in the working directory.*

---

## ⚙️ Data Preprocessing

- ✅ Handled **missing values**
- ✅ Applied appropriate **encoding** strategies:
  - Label Encoding
  - One-Hot Encoding
  - Categorical Encoding (based on column types)
- ✅ **Standardized** numerical features
- ✅ **Train-test split** for evaluation

---

## 🤖 Models Trained

| Model               | Accuracy | Notes                            |
|--------------------|----------|----------------------------------|
| Random Forest       | 91.74%   | Best performance, tuned with `RandomizedSearchCV` |
| K-Nearest Neighbors | 89.92%   | Good performance with tuning     |
| Logistic Regression | 86.06%   | Baseline linear model            |

---

## 🧪 Random Forest: Classification Report

          precision    recall  f1-score   support

     0.0       0.94      0.93      0.93       315
     1.0       0.88      0.89      0.89       341
     2.0       0.95      0.92      0.94       337
     3.0       0.91      0.93      0.92       327

accuracy                           0.92      1320

---

## 🛠️ Tech Stack / Libraries

- `pandas` – data manipulation  
- `numpy` – numerical operations  
- `scikit-learn` – machine learning and preprocessing  
- `matplotlib`, `seaborn` – visualization  
- `RandomizedSearchCV` – hyperparameter tuning  
- `LabelEncoder`, `StandardScaler`, etc.

---

## ▶️ How to Run the Project

1. **Clone the repository**:
   ```bash
   git clone https://github.com/<your-username>/weather-classification.git
   cd weather-classification
pip install -r requirements.txt
jupyter notebook Weather_Classification.ipynb

📈 Key Results
Best model: Random Forest

Highest accuracy: 91.74%

Robust performance across all four weather classes

