<div align="center">
  <h1>🛒 Customer Segmentation (K-Means Clustering)</h1>
  <p><i>A comprehensive Customer Segmentation project applying RFM Analysis and K-Means Clustering to e-commerce data.</i></p>
  
  ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
  ![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
  ![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
  ![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
  ![Seaborn](https://img.shields.io/badge/Seaborn-4E8B99?style=for-the-badge&logo=python&logoColor=white)
  ![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
</div>

<br/>

## 🚀 Overview
This project applies **RFM (Recency, Frequency, Monetary) Analysis** and **K-Means Clustering** to an e-commerce dataset to group customers based on their purchasing behavior. It provides actionable business insights for targeted marketing strategies.

---

## ✨ Features
- **Data Preprocessing**: Handling missing values, duplicates, and cleaning invalid records.
- **Feature Engineering**: Comprehensive **RFM** analysis.
- **Data Standardization**: Scaling features using `StandardScaler`.
- **Machine Learning**: 
  - Optimal cluster selection using the **Elbow Method**.
  - Customer segmentation using **K-Means Clustering**.
- **Exploratory Analysis**: Cluster profiling, customer type identification, and distribution analysis.
- **Data Visualization**: Scatter plots of customer clusters, Elbow Method graphs.
- **Business Insights**: Targeted marketing recommendations based on customer segments.

---

## 🛠️ Tech Stack
- **Language**: Python
- **Libraries**: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
- **Environment**: Jupyter Notebook

---

## 📂 Project Structure
```text
Customer-Segmentation-using-KMeans/
│
├── ecommerce_data.csv
├── Customer_Segmentation.ipynb
├── README.md
└── images/
```

---

## 📦 Installation & Usage

1. **Clone the repository**
   ```bash
   git clone https://github.com/ritish18089/Customer-Segmentation-using-KMeans.git
   ```

2. **Move into the project directory**
   ```bash
   cd Customer-Segmentation-using-KMeans
   ```

3. **Install the required libraries**
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```

4. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook
   ```
   *Open `Customer_Segmentation.ipynb` and run all the cells sequentially.*

---

## 📊 Dataset
The dataset contains e-commerce transaction records, including:
- **Invoice Number** & **Invoice Date**
- **Stock Code** & **Product Description**
- **Quantity** & **Unit Price**
- **Customer ID** & **Country**

---

## 📈 Analysis Performed

### 1️⃣ Data Inspection & Cleaning
- **Inspection**: Analyzed shape, data types, missing values, and duplicates.
- **Cleaning**: Removed duplicates and missing values, converted `Invoice Date` to datetime format, and removed invalid `Quantity` / `Unit Price` values.

### 2️⃣ Feature Engineering (RFM Analysis)
Calculated three critical customer metrics:
- **Recency**: Days since the last purchase.
- **Frequency**: Total number of purchases.
- **Monetary**: Total amount spent.

### 3️⃣ Descriptive Statistics & Standardization
- Evaluated Average Purchase Value, Purchase Frequency, and Customer Lifetime Value (CLV).
- Standardized data using **StandardScaler** to ensure all features contribute equally to the clustering process.

### 4️⃣ K-Means Clustering
- **Elbow Method**: Used to determine the optimal number of clusters.
- **Segmentation**: Applied K-Means to divide the customer base into distinct, actionable segments.

### 5️⃣ Cluster Visualization & Profiling
- Visualized clusters using Scatter Plots (Recency vs. Monetary, Frequency vs. Monetary).
- Evaluated Mean RFM values for each cluster to identify customer types and distribution.

### 6️⃣ Business Insights
Generated targeted marketing recommendations, customer retention strategies, and business growth opportunities for each segment.

---

## 📷 Visualizations

<details>
<summary><b>Click to View Visualizations</b></summary>

| 📉 Elbow Method Plot | 📊 Recency vs Monetary |
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level1-Customer%20SegmentationTask2/Images/2.png" height="300px"> | <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level1-Customer%20SegmentationTask2/Images/3.png" height="300px"> |

| 📊 Frequency vs Monetary | 📈 Customers per Cluster |
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level1-Customer%20SegmentationTask2/Images/4.png" height="300px"> | <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level1-Customer%20SegmentationTask2/Images/5.png" height="300px"> |

| 📋 Cluster Profile Table | |
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level1-Customer%20SegmentationTask2/Images/1.png" height="300px"> | |

</details>

---

## 🔍 Key Insights
- Customers were successfully segmented based on their purchasing behavior using RFM analysis.
- **High-value customers** exhibit high purchase frequency and significant spending.
- Different segments require completely different marketing approaches (e.g., retention strategies vs. re-engagement campaigns).
- Customer segmentation empowers businesses to personalize their marketing efforts to increase customer satisfaction.

---

## 💡 Marketing Recommendations
1. **Loyal Customers**: Reward them with exclusive offers and loyalty programs.
2. **Potential Loyalists**: Encourage recurring purchases through personalized product recommendations.
3. **Occasional Customers**: Engage them using promotional discounts and seasonal campaigns.
4. **At-Risk Customers**: Re-activate them through win-back offers and reminder emails.

---

## ▶️ Libraries
```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

from sklearn.preprocessing import StandardScaler
from sklearn.cluster import KMeans
```

---

## 📌 Future Improvements
- [ ] Develop an Interactive Dashboard using **Power BI** or **Tableau**.
- [ ] Implement **Customer Churn Prediction**.
- [ ] Experiment with Advanced Clustering Algorithms (e.g., DBSCAN, Hierarchical Clustering).
- [ ] Build a Customer Recommendation System.
- [ ] Develop a Real-Time Customer Segmentation pipeline.

---

## 👨‍💻 Author

**Ritish Kannur**  
*Python Developer | Java Full Stack Developer | Data Analytics Enthusiast | Machine Learning Enthusiast*

---

## ⭐ Support
If you found this project useful, consider giving it a ⭐ on GitHub. **Happy Coding! 🚀**
