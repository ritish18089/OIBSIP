<div align="center">
  <h1>🍷 Wine Quality Prediction</h1>
  <p><i>A comprehensive Machine Learning Classification project that predicts wine quality based on its physicochemical properties.</i></p>
  
  ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
  ![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
  ![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
  ![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
  ![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
</div>

<br/>

## 🚀 Overview
This project performs exploratory data analysis, handles class imbalance, engineers quality classes, trains multiple classification models, evaluates their performance, and identifies the most important chemical features influencing wine quality using **Python, Pandas, NumPy, Matplotlib, Seaborn, and Scikit-learn**.

---

## ✨ Features
- **Dataset loading and inspection**: Data type and missing value analysis.
- **Descriptive statistics**: Understand the distribution of data.
- **Quality score distribution analysis**: Distribution plots for all chemical features.
- **Correlation heatmap**: Understand relationships between features.
- **Class imbalance analysis**: Handling skewed datasets.
- **Binary quality classification**: Stratified train/test split.
- **Machine Learning Models**: 
  - Random Forest Classification
  - Stochastic Gradient Descent (SGD) Classification
  - Support Vector Classifier (SVC)
- **Evaluation**: Accuracy evaluation, Classification reports, Confusion matrices.
- **Feature Importance**: Random Forest feature importance extraction.
- **Model performance comparison**: Final model selection and deployment recommendation.

---

## 🛠️ Tech Stack
- **Language**: Python
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
- **Environment**: Jupyter Notebook

---

## 📂 Project Structure
```text
Wine-Quality-Prediction/
│
├── winequality-red.csv
├── Wine Quality Prediction.ipynb
├── README.md
└── images/
    ├── quality_distribution.png
    ├── feature_distributions.png
    ├── correlation_heatmap.png
    ├── rf_confusion_matrix.png
    ├── sgd_confusion_matrix.png
    ├── svc_confusion_matrix.png
    └── feature_importance.png
```

---

## 📦 Installation & Usage

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/Wine-Quality-Prediction.git
   ```

2. **Move into the project directory**
   ```bash
   cd Wine-Quality-Prediction
   ```

3. **Install the required libraries**
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```

4. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook
   ```
   *Open `Wine Quality Prediction.ipynb` and run all the cells sequentially.*

---

## 📊 Dataset
The dataset contains **1,143 wine samples** and **13 columns**.

### Dataset Features (Physicochemical Properties):
- `Fixed Acidity`
- `Volatile Acidity`
- `Citric Acid`
- `Residual Sugar`
- `Chlorides`
- `Free Sulfur Dioxide`
- `Total Sulfur Dioxide`
- `Density`
- `pH`
- `Sulphates`
- `Alcohol`

### Target Variable:
- `Quality` — Original wine quality score ranging from 3 to 8.

### Additional Column:
- `Id` — Unique identifier for each wine sample; excluded from model training.

---

## 📈 Analysis Performed

### 1️⃣ Data Inspection
- Dataset shape, Column names, Data types, Missing value analysis.

### 2️⃣ Descriptive Statistics
- Mean, Median, Standard deviation, Min/Max values, Quartiles.

### 3️⃣ Quality Score Distribution
- Original scores: `3, 4, 5, 6, 7, 8`.
- Analysis shows that scores 5 and 6 are most common, while 3 and 8 are highly underrepresented.

### 4️⃣ Exploratory Data Analysis (EDA)
- Distribution plots for all 11 chemical features to identify data distribution, skewness, spread, and outliers.

### 5️⃣ Correlation Analysis
- Correlation matrix and heatmap used to investigate relationships between properties and quality.

### 6️⃣ Class Imbalance Analysis
- The dataset is imbalanced (e.g., Quality 5 → 483 samples, Quality 3 → 6 samples). 
- To address this, class weighting and stratified splitting are used.

---

## ⚙️ Feature Engineering
The original quality scores are converted into a binary classification problem.

- **Classification Rule**: 
  - `Quality < 7`  → **Bad**
  - `Quality ≥ 7` → **Good**

**Why Binary Classification?** 
The original scores are highly imbalanced, making individual multi-class prediction difficult. Binary classification provides a more practical approach.

---

## 🔀 Train/Test Split
The dataset is divided into **80% Training Data** and **20% Testing Data** using a **stratified split** to preserve the Good/Bad class ratio.

```python
train_test_split(X, y, test_size=0.20, random_state=42, stratify=y)
```

---

## 🤖 Machine Learning Models

### 1️⃣ Random Forest Classifier
Uses multiple decision trees. Configuration: `n_estimators = 100`, `criterion = gini`, `max_depth = 10`, `class_weight = balanced`.

### 2️⃣ Stochastic Gradient Descent (SGD)
Linear classification approach. Feature standardization applied using `StandardScaler` and balanced class weights.

### 3️⃣ Support Vector Classifier (SVC)
Trained using `RBF kernel`, `StandardScaler`, and balanced class weights to capture nonlinear relationships.

---

## 📊 Model Evaluation
Each model is evaluated using:
- **Accuracy**: Overall percentage of correctly classified wines.
- **Precision, Recall, F1-Score**: Detailed class-level performance metrics.
- **Classification Report & Confusion Matrix**: To track True Positives, True Negatives, False Positives, and False Negatives.

### 📈 Model Comparison
*(Values are generated directly from the trained models in the notebook)*

| Model | Accuracy | Precision | Recall | F1-Score |
|---|---|---|---|---|
| Random Forest | — | — | — | — |
| SGD | — | — | — | — |
| SVC | — | — | — | — |

---

## 🌟 Feature Importance
Random Forest feature importance determines which chemical properties contribute most to wine quality prediction.
**Key insights:** Alcohol, Volatile Acidity, and Sulphates play important roles.

---

## 💡 Model Selection
**Random Forest** is selected as the most suitable model for deployment based on:
- Strong classification performance.
- Handles nonlinear relationships effectively.
- Works well with mixed ranges of numerical features.
- Supports class weighting for imbalanced data.
- Provides interpretable feature importance.

---

## 📊 Visualizations
###  📊 Wine Quality Score Distribution
<img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-WineQualityPredictionTask2/Images/1.png" height="1000px">

### 📈 Chemical Feature Distribution Plots
<img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-WineQualityPredictionTask2/Images/1.png" height="1000px">

### 🔥 Correlation Heatmap
<img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-WineQualityPredictionTask2/Images/1.png" height="1000px">

### ⚖️ Class Distribution
<img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-WineQualityPredictionTask2/Images/1.png" height="1000px">

### 🌲 Random Forest Confusion Matrix
<img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-WineQualityPredictionTask2/Images/1.png" height="1000px">

### 📉 SGD Confusion Matrix
<img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-WineQualityPredictionTask2/Images/1.png" height="1000px">

### 🎯 SVC Confusion Matrix
<img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-WineQualityPredictionTask2/Images/1.png" height="1000px">

### ⭐ Random Forest Feature Importance Chart
<img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-WineQualityPredictionTask2/Images/1.png" height="1000px">

### 📊 Model Performance Comparison
<img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-WineQualityPredictionTask2/Images/1.png" height="1000px">

## 📊 Visualizations

<details>
<summary><b>Click to View Visualizations</b></summary>

|📊 Wine Quality Score Distribution| 📈 Chemical Feature Distribution Plots |
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-Predicting%20House%20Prices%20with%20Linear%20RegressionTask1/Images/1.png" height="300px"> | <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-Predicting%20House%20Prices%20with%20Linear%20RegressionTask1/Images/2.png" height="300px"> |

|🔥 Correlation Heatmap | ⚖️ Class Distribution |
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-Predicting%20House%20Prices%20with%20Linear%20RegressionTask1/Images/3.png" height="300px"> | <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-Predicting%20House%20Prices%20with%20Linear%20RegressionTask1/Images/4.png" height="300px"> |

| 🌲 Random Forest Confusion Matrix |  📉 SGD Confusion Matrix |
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-Predicting%20House%20Prices%20with%20Linear%20RegressionTask1/Images/5.png" height="300px"> | <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-Predicting%20House%20Prices%20with%20Linear%20RegressionTask1/Images/6.png" height="300px"> |

| SVC Confusion Matrix|  ⭐ Random Forest Feature Importance Chart|
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-Predicting%20House%20Prices%20with%20Linear%20RegressionTask1/Images/5.png" height="300px"> | <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-Predicting%20House%20Prices%20with%20Linear%20RegressionTask1/Images/6.png" height="300px"> |




</details>
---

## ▶️ Sample Code
```python
import pandas as pd
from sklearn.model_selection import train_test_split
from sklearn.ensemble import RandomForestClassifier

# Load dataset
df = pd.read_csv("winequality-red.csv")

# Create binary quality class
df['quality_class'] = df['quality'].apply(lambda x: 'Good' if x >= 7 else 'Bad')

# Prepare features and target
X = df.drop(columns=['quality', 'quality_class', 'Id'], errors='ignore')
y = df['quality_class']

# Train/test split
X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.20, random_state=42, stratify=y
)

# Random Forest
rf_classifier = RandomForestClassifier(
    n_estimators=100, criterion='gini', max_depth=10, 
    random_state=42, class_weight='balanced'
)

rf_classifier.fit(X_train, y_train)

# Prediction
predictions = rf_classifier.predict(X_test)
print("Random Forest model trained successfully!")
```

---

## 📌 Future Improvements
- [ ] Hyperparameter tuning using `GridSearchCV` or `RandomizedSearchCV`.
- [ ] Cross-validation for more reliable model evaluation.
- [ ] Testing additional ensemble algorithms such as XGBoost.
- [ ] Multiclass wine quality prediction / Probability-based quality prediction.
- [ ] Interactive dashboard using Power BI or Tableau.
- [ ] Deployment using Flask, FastAPI, or Streamlit (Cloud deployment).
- [ ] Automated wine quality prediction system.

---

## 👨‍💻 Author

**Ritish Kannur**  
*Python Developer | Java Full Stack Developer | Data Analytics Enthusiast | Machine Learning Enthusiast*

---

## ⭐ Support
If you found this project useful, consider giving it a ⭐ on GitHub. **Happy Coding! 🍷🚀**
