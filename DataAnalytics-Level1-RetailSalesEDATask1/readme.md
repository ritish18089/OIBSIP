<div align="center">
  <h1>📊 EDA on Retail Sales Data</h1>
  <p><i>A comprehensive Exploratory Data Analysis (EDA) project on a Retail Sales dataset to uncover actionable business insights.</i></p>
  
  ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
  ![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
  ![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
  ![Matplotlib](https://img.shields.io/badge/Matplotlib-ffffff?style=for-the-badge&logo=matplotlib&logoColor=black)
  ![Seaborn](https://img.shields.io/badge/Seaborn-4E8B99?style=for-the-badge&logo=python&logoColor=white)
  ![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
</div>

<br/>

## 🚀 Overview
This project explores sales patterns, customer behavior, product performance, and provides actionable business insights through statistical analysis and visualizations. It is built using **Python, Pandas, Matplotlib, Seaborn, and Jupyter Notebook**.

---

## ✨ Features
- **Data Inspection & Cleaning**: Dataset loading, data type analysis, and null value analysis.
- **Statistical Analysis**: Comprehensive descriptive statistics.
- **Time Series Analysis**: Monthly and quarterly sales trend analysis.
- **Demographics & Segmentation**: Customer demographics analysis (age & gender).
- **Product Insights**: Product category analysis and revenue generation.
- **Correlation**: Heatmap analysis for numerical variables.
- **Actionable Insights**: Data-driven business recommendations based on findings.

---

## 🛠️ Tech Stack
- **Language**: Python
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn
- **Environment**: Jupyter Notebook

---

## 📂 Project Structure
```text
EDA-on-Retail-Sales/
│
├── retail_sales_dataset.csv
├── EDA on Retail.ipynb
├── README.md
└── images/
```

---

## 📦 Installation & Usage

1. **Clone the repository**
   ```bash
   git clone https://github.com/ritish18089/EDA-on-Retail-Sales.git
   ```

2. **Move into the project directory**
   ```bash
   cd EDA-on-Retail-Sales
   ```

3. **Install the required libraries**
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```

4. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook
   ```
   *Open `EDA on Retail.ipynb` and run all the cells sequentially.*

---

## 📊 Dataset
The dataset contains retail transaction details, including:
- **Transaction ID & Date**
- **Customer Details**: Customer ID, Gender, Age
- **Product Details**: Product Category, Quantity, Price per Unit
- **Revenue**: Total Amount

---

## 📈 Analysis Performed

### 1️⃣ Data Inspection
- Dataset loading, analyzing the shape, data types, and identifying missing values.

### 2️⃣ Descriptive Statistics
- Calculated Mean, Median, Mode, Standard Deviation, and full summary statistics to understand data distribution.

### 3️⃣ Time Series Analysis
- **Monthly Sales Trend**: Evaluated how sales perform on a month-to-month basis.
- **Quarterly Sales Trend**: Grouped data to observe broader seasonal patterns.

### 4️⃣ Customer Demographics
- **Distribution of Customer Age Groups**: Segmented customers to find the most active buyers.
- **Gender Breakdown**: Analyzed purchase parity among different genders.

### 5️⃣ Product Analysis
- **Top Best-Selling Product Categories**: Identified volume leaders.
- **Revenue by Product Category**: Identified which categories generate the most income.

### 6️⃣ Correlation Analysis
- Built a **Correlation Matrix** and visualized it with a **Heatmap** to understand the relationships between numerical variables (like Quantity and Total Amount).

### 7️⃣ Additional Visualization
- **Average Spending by Age Group**: Explored which age demographics possess the highest purchasing power.

---

## 📷 Visualizations

<details>
<summary><b>Click to View Visualizations</b></summary>

| 📈 Monthly Sales Trend | 📉 Quarterly Sales Trend |
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level1-RetailSalesEDATask1/Images/1.png" height="300px"> | <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level1-RetailSalesEDATask1/Images/2.png" height="300px"> |

| 👥 Customer Age Group Distribution | 🚻 Gender Breakdown |
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level1-RetailSalesEDATask1/Images/3.png" height="300px"> | <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level1-RetailSalesEDATask1/Images/4.png" height="300px"> |

| 🛍️ Top Best-Selling Categories | 💰 Revenue by Product Category |
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level1-RetailSalesEDATask1/Images/5.png" height="300px"> | <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level1-RetailSalesEDATask1/Images/6.png" height="300px"> |

| 🔥 Correlation Heatmap | 📊 Average Spending by Age Group |
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level1-RetailSalesEDATask1/Images/7.png" height="300px"> | <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level1-RetailSalesEDATask1/Images/8.png" height="300px"> |

</details>

---

## 🔍 Key Insights
- Sales vary significantly across different months and quarters.
- Customer purchases are well-distributed across multiple age groups.
- Different product categories contribute uniquely to total revenue.
- `Quantity` and `Total Amount` show a strong positive relationship.
- Customer spending patterns differ notably across age groups.

---

## 💡 Business Recommendations
1. **Inventory Management**: Maintain sufficient inventory for high-demand product categories to prevent stockouts.
2. **Targeted Marketing**: Implement marketing campaigns tailored specifically based on customer demographics (Age/Gender).
3. **Sales Promotions**: Launch promotional offers during historically lower-sales periods to stabilize and increase revenue.

---

## ▶️ Libraries
```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

# Example visualization setup
plt.figure(figsize=(10, 6))
sns.set_theme(style="whitegrid")
```

---

## 📌 Future Improvements
- [ ] Create an Interactive Dashboard using **Power BI** or **Tableau**.
- [ ] Implement Sales Forecasting using Machine Learning (e.g., ARIMA, Prophet).
- [ ] Perform Customer Segmentation using Clustering (e.g., K-Means).
- [ ] Develop Automated Business Reports.

---

## 👨‍💻 Author

**Ritish Kannur**  
*Python Developer | Java Full Stack Developer | Data Analytics Enthusiast | Machine Learning Enthusiast*

---

## ⭐ Support
If you found this project useful, consider giving it a ⭐ on GitHub. **Happy Coding! 🚀**
