<div align="center">
  <h1>📱 Unveiling the Android App Market</h1>
  <p><i>A comprehensive Exploratory Data Analysis (EDA) project on Google Play Store app and user review data.</i></p>
  
  ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
  ![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
  ![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
  ![Matplotlib](https://img.shields.io/badge/Matplotlib-ffffff?style=for-the-badge&logo=matplotlib&logoColor=black)
  ![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=plotly&logoColor=white)
  ![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
</div>

<br/>

## 🚀 Overview
This project explores app categories, ratings, installations, pricing, estimated revenue, and user sentiment to generate **data-driven insights for developers** planning to launch a new Android application. Built using **Python, Pandas, Matplotlib, Seaborn, Plotly, and TextBlob**.

---

## ✨ Features
- **Comprehensive Data Inspection**: Loading, data type, and null value analysis for both apps and reviews datasets.
- **Robust Data Cleaning**: Preprocessing, duplicate detection, and removal.
- **In-depth Category Analysis**: App distribution and identification of highly saturated categories.
- **Ratings & Popularity Analysis**: Rating distribution, average rating by category, and app size vs. installation analysis.
- **Monetization & Pricing Analysis**: 
  - Free vs. paid app analysis
  - Price distribution of paid applications
  - Estimated revenue analysis by category
- **User Sentiment Analysis**: 
  - Positive, negative, and neutral classification using **TextBlob**
  - Sentiment analysis by app category
- **Interactive Visualizations**: Dynamic charts built with **Plotly**.
- **Actionable Business Recommendations**: Data-driven insights for app developers.

---

## 🛠️ Tech Stack
- **Language**: Python
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Plotly, TextBlob
- **Environment**: Jupyter Notebook

---

## 📂 Project Structure
```text
Unveiling-the-Android-App-Market/
│
├── googleplaystore.csv
├── googleplaystorereviews_sentiment.csv
├── Unveiling Android App Market.ipynb
├── README.md
└── images/
```

---

## 📦 Installation & Usage

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/Unveiling-the-Android-App-Market.git
   ```

2. **Move into the project directory**
   ```bash
   cd Unveiling-the-Android-App-Market
   ```

3. **Install the required libraries**
   ```bash
   pip install pandas numpy matplotlib seaborn plotly textblob
   ```

4. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook
   ```
   *Open `Unveiling Android App Market.ipynb` and run all the cells sequentially.*

---

## 📊 Datasets

### 1️⃣ Play Store Apps Dataset
Contains fields including: `App`, `Category`, `Rating`, `Reviews`, `Size`, `Installs`, `Type`, `Price`, `Content Rating`, `Genres`, `Last Updated`, `Current Version`, `Android Version`.

### 2️⃣ User Reviews Dataset
Contains sentiment-analysis information: `App`, `Category`, `Translated Review`, `Sentiment`.
*(Note: The `Translated_Review` values used in this project were generated for demonstrating the sentiment-analysis workflow. Results should not be interpreted as genuine Google Play user feedback.)*

---

## 📈 Analysis Performed

### 1️⃣ Data Inspection & Cleaning
- Converted `Reviews`, `Installs` (e.g., `10,000+`), `Price`, and `Rating` into numeric formats.
- Converted app sizes into MB.
- Handled missing values and removed duplicate records.

### 2️⃣ Category Analysis
- Distribution across categories to identify the most saturated and competitive markets.

### 3️⃣ Ratings Analysis
- Distribution of app ratings and average ratings by category to identify highly-rated domains.

### 4️⃣ Size and Installs Analysis
- Scatter plot and correlation analysis between app size and popularity (installs).

### 5️⃣ Pricing Analysis
- Free vs. Paid app distribution and price distribution of paid apps.
- **Estimated Revenue** = `Price × Installs` (calculated by category).

### 6️⃣ Sentiment Analysis
- User review text analyzed using **TextBlob**.
- Classified into 🟢 **Positive**, ⚪ **Neutral**, 🔴 **Negative**.
- Sentiment by category to identify areas with higher positive/negative feedback.

---

## 🔍 Key Insights
- **Family, Game, and Tools** are among the highly populated categories, indicating strong competition.
- Most app ratings are concentrated around the **4.0–4.5** range, showing generally positive feedback.
- **App size does not strongly correlate** with the number of installs (size alone isn't a major predictor of popularity).
- **Free applications dominate** the Play Store compared to paid applications.
- **Estimated revenue varies significantly** between categories depending on price and installation volume.

---

## 💡 Business Recommendations
1. **Choose the category strategically**: Evaluate saturation; target less crowded segments or introduce unique features in highly competitive ones.
2. **Focus on quality**: Maintain high ratings through good performance, usability, and regular updates.
3. **Consider a freemium model**: Offer a free basic version with premium features, as free apps dominate the market.
4. **Optimize application size**: Keep the application reasonably lightweight without compromising functionality.
5. **Leverage user feedback**: Use sentiment analysis to guide future improvements and feature requests.

---

## 📊 Visualizations

<details>
<summary><b>Click to View Visualizations</b></summary>

| Fraud vs. Non-Fraud Class Distribution| 💰 Transaction Amount Distribution |
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-FraudDetectionTask3/Images/1.png" height="300px"> | <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-FraudDetectionTask3/Images/2.png" height="300px"> |

| 🕐 Transaction Distribution by Time of Day| 📈 Fraud Percentage by Hour |
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-FraudDetectionTask3/Images/3.png" height="300px"> | <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-FraudDetectionTask3/Images/4.png" height="300px"> |

| ⚖️ Class Distribution After SMOTE | 📉 AUC-ROC Curve |
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-FraudDetectionTask3/Images/5.png" height="300px"> | <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-FraudDetectionTask3/Images/6.png" height="300px"> |

|🌲 Random Forest Feature Importance |  |
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-FraudDetectionTask3/Images/7.png" height="300px"> | |

</details>

---

## ▶️ Sample Code

### Interactive Plotly Visualization
```python
import plotly.express as px

# Create an interactive bar chart
fig = px.bar(
    category_counts.reset_index(),
    x="Category",
    y="count",
    title="Interactive App Distribution Across Categories"
)

fig.show()
```

### Sentiment Analysis
```python
from textblob import TextBlob

# Example of obtaining sentiment polarity
def get_sentiment(text):
    return TextBlob(str(text)).sentiment.polarity
```

---

## 📌 Future Improvements
- [ ] Use a genuine Google Play user-review dataset for sentiment analysis.
- [ ] Build an interactive dashboard using Power BI or Tableau.
- [ ] Develop an app-installation prediction model.
- [ ] Perform app success prediction using Machine Learning.
- [ ] Build a recommendation system for Android applications.
- [ ] Analyze app update frequency and its relationship with ratings.

---

## 👨‍💻 Author

**Ritish Kannur**  
*Python Developer | Java Full Stack Developer | Data Analytics Enthusiast | Machine Learning Enthusiast*

---

## ⭐ Support
If you found this project useful, consider giving it a ⭐ on GitHub. **Happy Coding! 🚀**
