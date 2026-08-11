# 🏠 House Price Prediction using Linear Regression

A comprehensive Machine Learning project focused on predicting house prices using **Linear Regression**. The project uses **Python**, **Pandas**, **NumPy**, **Matplotlib**, **Seaborn**, and **Scikit-learn** to perform data exploration, preprocessing, model training, evaluation, visualization, and coefficient analysis.



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

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook



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
Clone the repository
```bash
git clone https://github.com/your-username/House-Price-Prediction.git
```
Move into the project directory
```bash
cd House-Price-Prediction
```
Install the required libraries
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```
Launch Jupyter Notebook
jupyter notebook
Open:
```bash
House Price Prediction.ipynb
```
Run all the cells sequentially.

## 📊 Dataset
The dataset contains house/property information used to predict house prices.
Dataset Features:
- Area – Size of the property
- No. of Bedrooms – Number of bedrooms in the property
- City – City where the property is located
- Location – Specific location of the property
- Price – Target variable representing the house price


## 🎯 Objective
The main objective of this project is to develop a machine learning model that can predict house prices based on property characteristics such as area, number of bedrooms, city, and location.

## 📈 Analysis and Machine Learning Process
### 1️⃣ Data Loading and Inspection
- Dataset loading using Pandas
- Display first few records
- Dataset shape
- Column information
- Data types
- Null value analysis
  
### 2️⃣ Exploratory Data Analysis
- Descriptive statistics
- Mean, median, minimum, and maximum values
- Standard deviation
- Distribution of the target variable
- Analysis of numerical features

### 3️⃣ Target Variable Analysis
- The Price column is selected as the target variable.
- A histogram with KDE is used to understand the distribution of house prices and identify skewness and variation in property prices.

### 4️⃣ Feature Selection
The following features are selected as predictors:
- Area
- No. of Bedrooms
- City
- Location
- These features were selected because property size, number of bedrooms, and location-related factors are important determinants of house prices.

### 5️⃣ Data Preprocessing
- The dataset is prepared for machine learning using:
- Missing value handling
- Median imputation for numerical features
- Most-frequent imputation for categorical features
- One-Hot Encoding for categorical variables
- The categorical features City and Location are converted into numerical representations so that they can be used by the Linear Regression model.

### 6️⃣ Correlation Analysis
- A correlation heatmap is created for numerical variables to understand relationships between:
- Price
- Area
- No. of Bedrooms
- The correlation with Price is analyzed to identify potentially important numerical predictors.

### 7️⃣ Train-Test Split
- The dataset is divided into:
- 80% Training Data
- 20% Testing Data
- A random state of 42 is used to ensure reproducible results.

### 8️⃣ Linear Regression Model
- A Linear Regression model is trained using Scikit-learn.
- The model learns the relationship between the selected house features and the target variable Price.

### 9️⃣ Model Evaluation
- The Linear Regression model is evaluated using:
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score
- Lower MSE and RMSE indicate lower prediction errors, while a higher R² score indicates better model performance.

### 🔟 Actual vs. Predicted Prices

- A scatter plot is created to compare:
- Actual house prices
- Predicted house prices
- Points closer to the diagonal reference line indicate more accurate predictions.

### 1️⃣1️⃣ Residual Analysis
- A residual plot is used to examine the prediction errors.
- The residuals should ideally be randomly distributed around zero without a systematic pattern.
- This helps determine whether Linear Regression is an appropriate model for the selected features.

### 1️⃣2️⃣ Coefficient Analysis
- Regression coefficients are analyzed to identify features with:
- Highest positive impact
- Highest negative impact
- Positive coefficients indicate a positive contribution to predicted house prices, while negative coefficients indicate a negative contribution.

### 1️⃣3️⃣ Ridge Regression Comparison
- As an additional experiment, Ridge Regression is compared with Linear Regression.
- Both models are evaluated using:
- MSE
- RMSE
- R² Score
- The model with lower prediction errors and a higher R² score is considered to have better performance on the test data.

## 📊 Visualizations
The project includes the following visualizations:
### 📊 Distribution of House Prices
<p align="center"><img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-Predicting%20House%20Prices%20with%20Linear%20RegressionTask1/Images/1.png" height="1000px">
  
### 🔥 Correlation Heatmap
<p align="center"><img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-Predicting%20House%20Prices%20with%20Linear%20RegressionTask1/Images/2.png" height="1000px">
  
### 🏠 Actual vs. Predicted House Prices
<p align="center"><img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-Predicting%20House%20Prices%20with%20Linear%20RegressionTask1/Images/3.png" height="1000px">
  
### 📉 Residual Plot
<p align="center"><img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-Predicting%20House%20Prices%20with%20Linear%20RegressionTask1/Images/4.png" height="1000px">
  
### 📈 Regression Coefficient Analysis
<p align="center"><img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-Predicting%20House%20Prices%20with%20Linear%20RegressionTask1/Images/5.png" height="1000px">
  
### ⚖️ Linear Regression vs. Ridge Regression Comparison
<p align="center"><img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-Predicting%20House%20Prices%20with%20Linear%20RegressionTask1/Images/6.png" height="1000px">

## 🔍 Key Insights
- House prices show considerable variation across different properties.
- Property Area is an important numerical factor influencing house prices.
- The Number of Bedrooms provides additional information about property size and value.
- City and Location can capture differences in property prices between different areas.
- One-Hot Encoding allows categorical location features to be incorporated into the regression model.
- The actual-versus-predicted plot helps visualize the accuracy of the model.
- Residual analysis helps identify systematic prediction errors.
- Ridge Regression provides a regularized alternative to ordinary Linear Regression.

## 💡 Business Recommendations
- Property developers can consider area, location, and bedroom count when estimating property prices.
- Real-estate businesses can use price prediction models to support preliminary property valuation.
- Marketing strategies can be adjusted according to differences in property values across locations.
- Additional features such as property age, amenities, parking, and neighborhood characteristics could improve future predictions.

## 📚 Libraries Used
```text
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

## 🎓 Learning Outcomes:
- Through this project, the following skills were developed:
- Data Loading and Inspection
- Exploratory Data Analysis
- Data Cleaning
- Missing Value Handling
- Feature Selection
- Categorical Feature Encoding
- Correlation Analysis
- Linear Regression
- Model Evaluation
- Residual Analysis
- Regression Coefficient Interpretation
-Regularization using Ridge Regression
- Data Visualization
- Machine Learning Workflow

## 📌 Future Improvements
The model can be improved in future by:
- Adding more property-related features
- Including property age/year built
- Including amenities such as parking and bathrooms
- Applying feature scaling where appropriate
- Testing Lasso and Elastic Net Regression
- Performing hyperparameter tuning
- Trying advanced models such as Random Forest and Gradient Boosting
- Deploying the trained model as a web application
- Creating an interactive house-price prediction dashboard

## 👨‍💻 Author
### Ritish Kannur
- Python Developer
- Java Full Stack Developer
- Data Analytics Enthusiast
- Machine Learning Enthusiast

## ⭐ Support
If you found this project useful, consider giving it a ⭐ on GitHub.
Happy Coding! 🚀
