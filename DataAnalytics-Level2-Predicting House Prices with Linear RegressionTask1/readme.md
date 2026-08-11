<div align="center">
  <h1>🏠 House Price Prediction using Linear Regression</h1>
  <p><i>A comprehensive Exploratory Data Analysis (EDA) project on Google Play Store app and user review data.</i></p>
  
  ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
  ![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
  ![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
  ![Matplotlib](https://img.shields.io/badge/Matplotlib-ffffff?style=for-the-badge&logo=matplotlib&logoColor=black)
  ![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=plotly&logoColor=white)
  ![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
</div>

<br/>


## 🚀 Features

- Dataset loading and inspection
- Null value analysis
- Descriptive statistics
- Target variable distribution analysis
- Feature selection
- Missing value handling
- One-Hot Encoding of categorical features
- Correlation heatmap
- 80/20 train-test split
- Linear Regression model training
- Model evaluation using MSE, RMSE, and R² Score
- Actual vs. predicted price visualization
- Residual analysis
- Regression coefficient analysis
- Ridge Regression comparison
- Model performance comparison
- Business-oriented interpretation of results



## 🛠️ Tech Stack

- **Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
- **Environment:** Jupyter Notebook



## 📂 Project Structure

```text
House-Price-Prediction/
│
├── csvdata.csv
├── House Price Prediction.ipynb
├── README.md
└── images/
```



## 📦 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/House-Price-Prediction.git
   ```
2. **Move into the project directory**
   ```bash
   cd House-Price-Prediction
   ```
3. **Install the required libraries**
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```
4. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook
   ```
5. **Open & Run**
   Open `House Price Prediction.ipynb` and run all the cells sequentially.



## 📊 Dataset

The dataset contains house/property information used to predict house prices.

**Dataset Features:**
- `Area` – Size of the property
- `No. of Bedrooms` – Number of bedrooms in the property
- `City` – City where the property is located
- `Location` – Specific location of the property
- `Price` – Target variable representing the house price



## 🎯 Objective

The main objective of this project is to develop a machine learning model that can predict house prices based on property characteristics such as area, number of bedrooms, city, and location.



## 📈 Analysis and Machine Learning Process

### 1️⃣ Data Loading and Inspection
- Dataset loading using Pandas
- Display first few records, dataset shape, column information, and data types
- Null value analysis
  
### 2️⃣ Exploratory Data Analysis
- Descriptive statistics (Mean, median, minimum, maximum values, standard deviation)
- Distribution of the target variable
- Analysis of numerical features

### 3️⃣ Target Variable Analysis
- The `Price` column is selected as the target variable.
- A histogram with KDE is used to understand the distribution of house prices and identify skewness and variation in property prices.

### 4️⃣ Feature Selection
- Features selected as predictors: `Area`, `No. of Bedrooms`, `City`, `Location`
- Selected because property size, number of bedrooms, and location-related factors are important determinants of house prices.

### 5️⃣ Data Preprocessing
- Missing value handling: Median imputation for numerical features, most-frequent imputation for categorical features
- One-Hot Encoding: The categorical features `City` and `Location` are converted into numerical representations.

### 6️⃣ Correlation Analysis
- A correlation heatmap is created for numerical variables to understand relationships between `Price`, `Area`, and `No. of Bedrooms`.

### 7️⃣ Train-Test Split
- 80% Training Data / 20% Testing Data
- A random state of 42 is used to ensure reproducible results.

### 8️⃣ Linear Regression Model
- A Linear Regression model is trained using Scikit-learn to learn the relationship between features and the target variable `Price`.

### 9️⃣ Model Evaluation
- Evaluated using Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R² Score.

### 🔟 Actual vs. Predicted Prices
- A scatter plot compares actual and predicted house prices. Points closer to the diagonal indicate more accurate predictions.

### 1️⃣1️⃣ Residual Analysis
- A residual plot examines prediction errors to check if they are randomly distributed around zero.

### 1️⃣2️⃣ Coefficient Analysis
- Analyzes regression coefficients to identify features with the highest positive and negative impact on predicted house prices.

### 1️⃣3️⃣ Ridge Regression Comparison
- Compares Ridge Regression with Linear Regression using MSE, RMSE, and R² Score to evaluate regularized performance.


## 📊 Visualizations

<details>
<summary><b>Click to View Visualizations</b></summary>

| 📊 Distribution of House Prices | 🔥 Correlation Heatmap |
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-Predicting%20House%20Prices%20with%20Linear%20RegressionTask1/Images/1.png" height="300px"> | <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-Predicting%20House%20Prices%20with%20Linear%20RegressionTask1/Images/2.png" height="300px"> |

| 🏠 Actual vs. Predicted House Prices | 📉 Residual Plot |
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-Predicting%20House%20Prices%20with%20Linear%20RegressionTask1/Images/3.png" height="300px"> | <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-Predicting%20House%20Prices%20with%20Linear%20RegressionTask1/Images/4.png" height="300px"> |

| 📈 Regression Coefficient Analysis | ⚖️ Linear Regression vs. Ridge Regression Comparison |
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-Predicting%20House%20Prices%20with%20Linear%20RegressionTask1/Images/5.png" height="300px"> | <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-Predicting%20House%20Prices%20with%20Linear%20RegressionTask1/Images/6.png" height="300px"> |

</details>

---

## 🔍 Key Insights

- House prices show considerable variation across different properties.
- Property **Area** is an important numerical factor influencing house prices.
- The **Number of Bedrooms** provides additional information about property size and value.
- **City and Location** can capture differences in property prices between different areas.
- **One-Hot Encoding** allows categorical location features to be incorporated into the regression model.
- The **actual-versus-predicted plot** helps visualize the accuracy of the model.
- **Residual analysis** helps identify systematic prediction errors.
- **Ridge Regression** provides a regularized alternative to ordinary Linear Regression.

---

## 💡 Business Recommendations

- **Property developers** can consider area, location, and bedroom count when estimating property prices.
- **Real-estate businesses** can use price prediction models to support preliminary property valuation.
- **Marketing strategies** can be adjusted according to differences in property values across locations.
- **Additional features** such as property age, amenities, parking, and neighborhood characteristics could improve future predictions.

---

## 📚 Libraries Used

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

from sklearn.model_selection import train_test_split
from sklearn.compose import ColumnTransformer
from sklearn.preprocessing import OneHotEncoder
from sklearn.impute import SimpleImputer
from sklearn.pipeline import Pipeline
from sklearn.linear_model import LinearRegression, Ridge
from sklearn.metrics import mean_squared_error, r2_score
```

---

## 🎓 Learning Outcomes

Through this project, the following skills were developed:
- Data Loading and Inspection
- Exploratory Data Analysis
- Data Cleaning & Missing Value Handling
- Feature Selection & Categorical Feature Encoding
- Correlation Analysis
- Linear Regression & Ridge Regression
- Model Evaluation & Residual Analysis
- Regression Coefficient Interpretation
- Data Visualization
- Machine Learning Workflow

---

## 📌 Future Improvements

The model can be improved in future by:
- Adding more property-related features (e.g., property age/year built, amenities, parking, bathrooms)
- Applying feature scaling where appropriate
- Testing Lasso and Elastic Net Regression
- Performing hyperparameter tuning
- Trying advanced models such as Random Forest and Gradient Boosting
- Deploying the trained model as a web application
- Creating an interactive house-price prediction dashboard

---

## 👨‍💻 Author

**Ritish Kannur**
- Python Developer
- Java Full Stack Developer
- Data Analytics Enthusiast
- Machine Learning Enthusiast

---

## ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.
Happy Coding! 🚀
