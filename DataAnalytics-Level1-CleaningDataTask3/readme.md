<div align="center">
  <h1>🧹 NFL Data Cleaning & Preprocessing</h1>
  <p><i>A comprehensive Data Cleaning project focused on the NFL Play-by-Play Dataset (2009–2016).</i></p>
  
  ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
  ![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
  ![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
  ![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
</div>

<br/>

## 🚀 Overview
This project focuses on improving data quality for the **NFL Play-by-Play Dataset (2009–2016)**. It utilizes **Python, Pandas, and NumPy** to handle missing values, remove duplicate records, correct data types, standardize data formats, detect outliers, and prepare the dataset for exploratory data analysis (EDA) and machine learning.

---

## ✨ Features
- **Data Quality Assessment**: Comprehensive review of dataset integrity.
- **Missing Value Handling**: Identification and resolution of null values using multiple imputation techniques.
- **Duplicate Removal**: Detection and removal of redundant records.
- **Data Standardization & Type Correction**: Normalizing text, formats, and casting columns to proper data types (e.g., datetimes).
- **Outlier Detection**: Statistical outlier identification using the **IQR method**.
- **Impact Tracking**: Before vs. After data quality comparison to quantify improvements.
- **Clean Export**: Generation of a pristine dataset ready for ML/EDA.

---

## 🛠️ Tech Stack
- **Language**: Python
- **Libraries**: Pandas, NumPy
- **Environment**: Jupyter Notebook

---

## 📂 Project Structure
```text
NFL-Data-Cleaning/
│
├── NFL Play by Play 2009-2016 (v3).csv
├── NFL_Data_Cleaning.ipynb
├── NFL_PlayByPlay_Cleaned.csv
├── README.md
└── images/
```

---

## 📦 Installation & Usage

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/NFL-Data-Cleaning.git
   ```

2. **Move into the project directory**
   ```bash
   cd NFL-Data-Cleaning
   ```

3. **Install the required libraries**
   ```bash
   pip install pandas numpy
   ```

4. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook
   ```
   *Open `NFL_Data_Cleaning.ipynb` and run all notebook cells sequentially.*

---

## 📊 Dataset
The dataset contains detailed **NFL Play-by-Play records (2009–2016)** including:
- **Game Info**: Game ID, Date, Quarter, Time Remaining
- **Team Info**: Offensive Team, Defensive Team
- **Play Info**: Down, Distance, Yard Line, Play Type
- **Game Stats**: Passing, Rushing, Touchdowns, Penalties, Scores
- **Advanced Metrics**: Win Probability, Expected Points

---

## 📈 Data Cleaning Process

### 1️⃣ Dataset Inspection
Loaded the dataset, reviewed the shape, examined column names, and analyzed raw data types.

### 2️⃣ Data Quality Report
Counted missing values, detected duplicate rows, checked data types, and identified range anomalies.

### 3️⃣ Missing Value Handling
Applied techniques like Mean, Median, Mode imputation, Forward Fill, and row deletion (where appropriate) with strong justifications for each strategy.

### 4️⃣ Duplicate Removal
Detected and removed duplicate records, documenting the number of rows purged.

### 5️⃣ Data Standardization
Removed unnecessary spaces, standardized text formatting, and normalized inconsistent values.

### 6️⃣ Data Type Correction
Converted `Date` columns to `datetime`, `ID` columns to strings, and ensured appropriate precision for numerical data.

### 7️⃣ Outlier Detection
Identified outliers using the **IQR (Interquartile Range) Method**, analyzed extreme values, and documented whether they were retained, capped, or removed.

### 8️⃣ Before vs. After Comparison
Verified row counts, missing value tallies, duplicate counts, and data types before and after processing.

### 9️⃣ Export Clean Dataset
Saved the cleaned dataset as a new CSV file (`NFL_PlayByPlay_Cleaned.csv`), preserving the original raw data.

---

## 📷 Visualizations

<details>
<summary><b>Click to View Visualizations</b></summary>

| 📋 Data Quality Report | 📊 Missing Value Summary |
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level1-CleaningDataTask3/Images/1.png" height="300px"> | <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level1-CleaningDataTask3/Images/2.png" height="300px"> |

| 📋 Duplicate Record Summary | 📈 Outlier Detection Report |
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level1-CleaningDataTask3/Images/3.png" height="300px"> | <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level1-CleaningDataTask3/Images/4.png" height="300px"> |

| 📋 Before vs. After Comparison | 📁 Cleaned Dataset (CSV) |
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level1-CleaningDataTask3/Images/5.png" height="300px"> | <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level1-CleaningDataTask3/Images/6.png" height="300px"> |

</details>

---

## 🔍 Key Outcomes
- Improved overall data quality and reduced errors.
- Missing values and duplicate records were handled using context-appropriate techniques.
- Outliers were successfully identified using the IQR method.
- The **cleaned dataset is now primed and ready** for Exploratory Data Analysis (EDA) and Machine Learning.

---

## 💡 Business & Analytical Benefits
- **Reliability**: Vastly improves dataset reliability for modeling.
- **Compatibility**: Ensures format compatibility with various ML algorithms.
- **Reusability**: Provides a robust, cleaned baseline dataset for future sports analytics projects.

---

## ▶️ Libraries
```python
import pandas as pd
import numpy as np

# Load raw dataset
df = pd.read_csv("NFL Play by Play 2009-2016 (v3).csv")
```

---

## 📌 Future Improvements
- [ ] Develop an automated data validation pipeline.
- [ ] Create an interactive data quality dashboard.
- [ ] Implement advanced anomaly detection techniques.
- [ ] Integrate feature engineering for predictive modeling.

---

## 👨‍💻 Author

**Ritish Kannur**  
*Python Developer | Java Full Stack Developer | Data Analytics Enthusiast | Machine Learning Enthusiast*

---

## ⭐ Support
If you found this project useful, consider giving it a ⭐ on GitHub. **Happy Coding! 🚀**
