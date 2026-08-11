<div align="center">
  <h1>💳 Fraud Detection</h1>
  <p><i>A comprehensive Machine Learning Fraud Detection project performed on a highly imbalanced credit card transaction dataset.</i></p>
  
  ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
  ![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
  ![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
  ![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
  ![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
</div>

<br/>

## 🚀 Overview
This project analyzes fraudulent transaction patterns, handles severe class imbalance using SMOTE, trains multiple classification models, and evaluates their performance using fraud-focused metrics. Built using **Python, Pandas, NumPy, Scikit-learn, Imbalanced-learn, Matplotlib, and Seaborn**.

---

## ✨ Features
- **Exploratory Data Analysis**: Dataset loading, inspection, data type, and missing value analysis.
- **In-depth Fraud Analysis**: 
  - Class imbalance analysis
  - Fraudulent transaction percentage analysis
  - Transaction amount distribution analysis
  - Time-of-day fraud analysis
- **Data Preprocessing**: Stratified train/test splitting & Class imbalance handling using **SMOTE**.
- **Machine Learning Models**:
  - Logistic Regression
  - Random Forest
- **Advanced Evaluation**:
  - Precision, Recall, and F1-Score evaluation
  - AUC-ROC curve analysis
  - Feature importance analysis
  - Precision vs. Recall trade-off discussion
- **System Design**: Model scalability discussion and Data-driven conclusions.

---

## 🛠️ Tech Stack
- **Language**: Python
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Imbalanced-learn
- **Environment**: Jupyter Notebook

---

## 📂 Project Structure
```text
Credit-Card-Fraud-Detection/
│
├── credit_card_fraud_10k.csv
├── Fraud Detection.ipynb
├── README.md
└── images/
```

---

## 📦 Installation & Usage

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/Credit-Card-Fraud-Detection.git
   ```

2. **Move into the project directory**
   ```bash
   cd Credit-Card-Fraud-Detection
   ```

3. **Install the required libraries**
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn
   ```

4. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook
   ```
   *Open `Fraud Detection.ipynb` and run all the cells sequentially.*

---

## 📊 Dataset
The project uses a **10,000-transaction** credit card fraud dataset containing information such as Transaction ID, Transaction Amount, Transaction Hour, Merchant Category, and Fraud Indicator.

### Target Variable: `is_fraud`
| Value | Meaning |
|---|---|
| `0` | Non-Fraudulent Transaction |
| `1` | Fraudulent Transaction |

---

## 📈 Analysis Performed

### 1️⃣ Data Inspection
- Dataset shape, Column information, Data types, Missing values, and Duplicates.

### 2️⃣ Class Imbalance Analysis
- **9,849** non-fraudulent transactions (98.49%)
- **151** fraudulent transactions (1.51%)
- *Conclusion: Severe class imbalance.*

### 3️⃣ Transaction Amount Analysis
- Explored differences in transaction amounts using box plots to identify distribution patterns and outliers.

### 4️⃣ Time-of-Day Analysis
- Analyzed transaction activity and fraud occurrence across different hours of the day to spot high-risk time periods.

### 5️⃣ Evaluation Metrics (Accuracy Limitation)
- Standard accuracy is misleading for highly imbalanced datasets.
- The primary evaluation focuses on **Precision, Recall, F1-Score, and AUC-ROC**.

### 6️⃣ Class Imbalance Handling
- Applied **SMOTE** (Synthetic Minority Over-sampling Technique) to the training dataset to generate synthetic examples of the minority fraud class, preventing data leakage.

### 7️⃣ Train/Test Split
- Divided the dataset using **stratified sampling** to preserve the original class distribution in both sets.

---

## 🤖 Machine Learning Models

### 1️⃣ Logistic Regression
Used as a baseline model.
- **Advantages**: Simple, Fast, Interpretable, Efficient for large datasets.

### 2️⃣ Random Forest
- **Advantages**: Captures non-linear relationships, Handles complex interactions, Provides feature importance, Supports parallel processing.

---

## 📊 Model Evaluation

- **Precision**: How many transactions predicted as fraud were actually fraudulent.
- **Recall**: How many actual fraudulent transactions were successfully detected. *(Crucial for fraud detection)*
- **F1-Score**: Balance between Precision and Recall.
- **AUC-ROC**: Effectiveness in distinguishing between classes across thresholds.

---

## 🔍 Key Insights
- Only **1.51%** of transactions are fraudulent, indicating severe class imbalance.
- **SMOTE** successfully helps the models learn patterns from the minority class.
- **Recall** is critical because missing actual fraud results in financial loss, but **Precision** is needed to prevent excessive false alerts.
- **Transaction amount and timing** provide highly useful information for identifying suspicious activity.
- **Random Forest** offers excellent feature importance to identify influential characteristics.

---

## ⚖️ Precision vs. Recall Trade-Off
In fraud detection, **Recall** is generally prioritized to minimize financial losses. However, maximizing Recall increases false positives, reducing Precision. 
A practical system aims for:
✅ High Recall + ✅ Reasonable Precision + ✅ Strong F1-Score + ✅ High AUC-ROC

---

## 🚀 Scalability
A production system processing 1 million transactions/hour needs to handle ~278 transactions/second.

**Strategies for high volumes:**
- Deploy via real-time API (FastAPI/Flask).
- Load balancing across multiple servers.
- Use **Kafka** or message queues for streaming.
- **Random Forest** can leverage multi-core CPUs.
- Continuous model monitoring (latency, false positives, data drift).

---

## 💡 Business Recommendations
1. Prioritize high recall to reduce missed fraudulent transactions.
2. Maintain reasonable precision to avoid unnecessarily blocking legitimate customers.
3. Continuously monitor fraud patterns and retrain models when behavior changes.
4. Use real-time scoring for high-risk transactions.
5. Combine machine learning predictions with additional banking security rules.

---

## ▶️ Sample Code
### Load & Resample
```python
import pandas as pd
from imblearn.over_sampling import SMOTE

# Load dataset
df = pd.read_csv("credit_card_fraud_10k.csv")

# SMOTE
smote = SMOTE(random_state=42)
X_train_smote, y_train_smote = smote.fit_resample(X_train_scaled, y_train)
```

### Model Training
```python
from sklearn.linear_model import LogisticRegression
from sklearn.ensemble import RandomForestClassifier

# Logistic Regression
logistic_model = LogisticRegression(max_iter=1000, random_state=42)
logistic_model.fit(X_train_smote, y_train_smote)

# Random Forest
rf_model = RandomForestClassifier(n_estimators=100, random_state=42, n_jobs=-1)
rf_model.fit(X_train_smote, y_train_smote)
```

---

## 📌 Future Improvements
- [ ] Real-time fraud detection API using `FastAPI`
- [ ] Deploy the model using Docker
- [ ] Hyperparameter tuning & Cross-validation
- [ ] XGBoost or LightGBM comparison
- [ ] Real-time transaction streaming using `Kafka`
- [ ] Interactive dashboard using Power BI or Tableau
- [ ] Automated model retraining & data drift detection

---

## 👨‍💻 Author

**Ritish Kannur**  
*Python Developer | Java Full Stack Developer | Data Analytics Enthusiast | Machine Learning Enthusiast*

---

## ⭐ Support
If you found this project useful, consider giving it a ⭐ on GitHub. **Happy Coding! 🚀**