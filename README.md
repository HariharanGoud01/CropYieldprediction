# CropYieldprediction
# 🌾 Crop Prediction Using Machine Learning

## 📖 Overview
This project is designed to help farmers and agricultural experts **predict the most suitable crop** to grow based on soil and weather conditions using **Machine Learning**.

It analyzes parameters such as **Nitrogen (N)**, **Phosphorus (P)**, **Potassium (K)**, **pH**, **temperature**, **humidity**, and **rainfall**, and predicts the **best crop** that can yield maximum production.

A simple **Tkinter-based GUI** is also developed for users to easily upload datasets, train models, view accuracy graphs, and make predictions without using code.

---

## 🎯 Objectives
- Predict the best crop for a given soil and weather condition.
- Help farmers make data-driven agricultural decisions.
- Improve yield and resource utilization.
- Provide fertilizer and yield recommendations.

---

## ⚙️ Technologies Used
- **Programming Language:** Python  
- **Libraries:** 
  - `pandas`, `numpy` – for data handling  
  - `scikit-learn` – for machine learning models  
  - `matplotlib`, `seaborn` – for visualization  
  - `tkinter` – for GUI design
- **Algorithms Used:**
  - Decision Tree Classifier  
  - Random Forest Classifier  
  - Support Vector Machine (SVM)  
  - Passive Aggressive Classifier

---

## 🧩 Dataset Description
The dataset includes agricultural features such as:
| Feature | Description |
|----------|-------------|
| N | Nitrogen content in soil |
| P | Phosphorus content in soil |
| K | Potassium content in soil |
| Temperature | Average temperature in °C |
| Humidity | Relative humidity in % |
| pH | Acidity level of the soil |
| Rainfall | Annual rainfall in mm |
| Crop | Crop name (Target variable) |

The dataset can be sourced from open agricultural datasets or local farm data.

---

## 🚀 Project Workflow

### 1️⃣ Data Collection
- Gather data from agricultural sources (farm records, government datasets).
- Include soil nutrients, pH, weather data, and crop yield information.

### 2️⃣ Data Preprocessing
- Remove null or duplicate entries.  
- Encode categorical data (crop names).  
- Split dataset into **Training (70%)** and **Testing (30%)** sets.

### 3️⃣ Model Training
Train multiple machine learning models:
```python
from sklearn.tree import DecisionTreeClassifier
from sklearn.ensemble import RandomForestClassifier
from sklearn.svm import SVC
from sklearn.linear_model import PassiveAggressiveClassifier
