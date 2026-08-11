<div align="center">
  <h1>😊 Amazon Sentiment Analysis</h1>
  <p><i>A comprehensive NLP project to classify Amazon customer reviews into Positive, Negative, and Neutral sentiments.</i></p>
  
  ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
  ![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
  ![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
  ![NLTK](https://img.shields.io/badge/NLTK-2C5E19?style=for-the-badge&logo=python&logoColor=white)
  ![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
  ![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
</div>

<br/>

## 📌 Project Overview
Customer reviews play a crucial role in understanding customer satisfaction and product quality. This project analyzes **Amazon product reviews** using Natural Language Processing (NLP) techniques and machine learning algorithms to automatically predict customer sentiment. 

The workflow includes data preprocessing, feature extraction using **TF-IDF**, model training using **Naive Bayes** and **Logistic Regression**, performance evaluation, and visualization of customer sentiments.

---

## 🚀 Features
- **Data Pipeline**: Dataset loading, inspection, and sentiment distribution analysis.
- **Robust NLP Text Preprocessing**: Tokenization, Lowercase conversion, Stopword removal, and Lemmatization.
- **Feature Extraction**: TF-IDF (Term Frequency-Inverse Document Frequency) Vectorization.
- **Machine Learning Models**: 
  - Naive Bayes Classifier
  - Logistic Regression Classifier
- **Comprehensive Evaluation**: Accuracy, Precision, Recall, F1-Score, Confusion Matrix, and Classification Report.
- **Data Visualization**: Sentiment Distribution, WordClouds (Positive, Negative, Neutral).
- **Error Analysis**: Misclassified reviews and model limitations.

---

## 🛠️ Tech Stack
- **Language**: Python
- **Libraries**: Pandas, NumPy, NLTK, Scikit-learn, Matplotlib
- **Environment**: Jupyter Notebook

---

## 📂 Project Structure
```text
Amazon-Sentiment-Analysis/
│
├── amazon_with_sentiment.csv
├── Sentiment_Analysis.ipynb
├── README.md
└── images/
```

---

## 📦 Installation & Usage

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/Amazon-Sentiment-Analysis.git
   ```

2. **Move into the project directory**
   ```bash
   cd Amazon-Sentiment-Analysis
   ```

3. **Install the required libraries**
   ```bash
   pip install pandas numpy nltk scikit-learn matplotlib
   ```

4. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook
   ```
   *Open `Sentiment_Analysis.ipynb` and run all the cells sequentially.*

---

## 📊 Dataset
The dataset contains Amazon customer review information, including:
- Product Name, Category, Rating
- Review Title, Review Content
- Sentiment Label
- Price, Discount, Product Information

---

## 📈 Project Workflow

### 1️⃣ Dataset Inspection
Dataset shape, viewing first/last records, examining columns, and data type analysis.

### 2️⃣ Sentiment Distribution
Analyzing the count of Positive, Negative, and Neutral reviews using visualizations.

### 3️⃣ Text Preprocessing
- Lowercase conversion
- Removal of punctuation and numbers
- Tokenization
- Stopword removal
- Lemmatization

### 4️⃣ Feature Extraction
**TF-IDF Vectorization** to convert textual text into numerical features for machine learning.

### 5️⃣ Train-Test Split
- 80% Training Data
- 20% Testing Data

### 6️⃣ Machine Learning Models
- **Naive Bayes**: Model Training & Prediction
- **Logistic Regression**: Model Training & Prediction

### 7️⃣ Model Evaluation
Evaluation metrics include: Accuracy, Precision, Recall, F1-Score, Confusion Matrix, and Classification Report.

### 8️⃣ Visualization
- Sentiment Distribution Bar Chart
- Positive, Negative, and Neutral WordClouds

### 9️⃣ Error Analysis
- Displaying misclassified reviews, analyzing incorrect predictions, and discussing model limitations.

---

## 📷 Visualizations

<details>
<summary><b>Click to View Visualizations</b></summary>

| 📊 Sentiment Distribution | 📈 TF-IDF Features |
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level1-SentimentAnalysisTask4/Images/1.png" height="300px"> | <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level1-SentimentAnalysisTask4/Images/2.png" height="300px"> |

| 📉 Confusion Matrix & Report | ☁️ WordClouds |
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level1-SentimentAnalysisTask4/Images/3.png" height="300px"> | <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level1-SentimentAnalysisTask4/Images/4.png" height="300px"> |

| 🔍 Error Analysis | |
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level1-SentimentAnalysisTask4/Images/5.png" height="300px"> | |

</details>

---

## 🔍 Key Insights
- **Logistic Regression** achieved higher accuracy than Naive Bayes.
- **TF-IDF** effectively converted text into numerical features.
- **Text preprocessing** significantly improved model performance.
- Most customer reviews were classified as **Positive**.
- Reviews containing **sarcasm or mixed opinions** were difficult to classify correctly.

---

## 💡 Real-World Applications
- Product Review Analysis & Brand Reputation Monitoring
- Opinion Mining & Social Media Sentiment Analysis
- E-commerce Recommendation Systems
- Customer Satisfaction Measurement

---

## ▶️ Libraries
```python
import pandas as pd
import numpy as np
import nltk
import matplotlib.pyplot as plt

from sklearn.feature_extraction.text import TfidfVectorizer
from sklearn.naive_bayes import MultinomialNB
from sklearn.linear_model import LogisticRegression
```

---

## 📌 Future Improvements
- [ ] Implement Deep Learning using LSTM.
- [ ] Utilize BERT-based Sentiment Analysis.
- [ ] Perform Hyperparameter Optimization.
- [ ] Build a Real-Time Review Prediction pipeline.
- [ ] Create an Interactive Dashboard.
- [ ] Enable Multi-language Sentiment Analysis.

---

## 👨‍💻 Author

**Ritish Kannur**  
*Python Developer | Java Full Stack Developer | Data Analytics Enthusiast | Machine Learning Enthusiast*

---

## ⭐ Support
If you found this project useful, consider giving it a ⭐ on GitHub. **Happy Coding! 🚀**
