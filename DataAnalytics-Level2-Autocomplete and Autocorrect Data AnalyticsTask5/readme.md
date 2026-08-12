<div align="center">
  <h1>📊 Autocomplete & Autocorrect Data Analytics</h1>
  <p><i>A comprehensive NLP-based data analytics project focused on implementing and evaluating autocomplete and autocorrect algorithms using a real-world hotel review dataset.</i></p>
  
  ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
  ![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
  ![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
  ![NLTK](https://img.shields.io/badge/NLTK-2C5E19?style=for-the-badge&logo=python&logoColor=white)
  ![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
  ![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
</div>

<br/>

## 🚀 Overview
This project uses text preprocessing, frequency-based **Bigram and Trigram language models**, and **Levenshtein edit distance** to predict the next word and correct spelling errors. The project compares algorithm performance using Precision, Recall, and Accuracy, along with visualizations such as word-frequency charts and an autocorrect confusion matrix.

---

## ✨ Features
- **NLP Text Preprocessing**: Tokenization, Lowercasing, Punctuation removal, and Stopword analysis.
- **Language Models**: 
  - Bigram autocomplete implementation
  - Trigram autocomplete implementation
  - Top-3 predictions for 10+ input prefixes
- **Spell Correction**: 
  - Levenshtein-distance-based autocorrect
  - Testing on 20 deliberately misspelled words
- **Evaluation & Metrics**: 
  - Precision and Recall calculation
  - Bigram vs. Trigram algorithm comparison
  - Autocorrect correction accuracy evaluation
- **Visualizations**: Top 20 frequent words, Autocorrect confusion matrix.

---

## 🛠️ Tech Stack
- **Language**: Python
- **Libraries**: Pandas, NumPy, NLTK, Scikit-learn, Collections, Matplotlib
- **Environment**: Jupyter Notebook

---

## 📂 Project Structure
```text
Autocomplete-and-Autocorrect/
│
├── deceptive-opinion.csv
├── Autocomplete and Autocorrect.ipynb
├── README.md
└── images/
    ├── top_20_words.png
    ├── autocomplete_comparison.png
    ├── autocorrect_confusion_matrix.png
    └── algorithm_comparison.png
```

---

## 📦 Installation & Usage

1. **Clone the repository**
   ```bash
   git clone https://github.com/ritish18089/Autocomplete-and-Autocorrect.git
   ```

2. **Move into the project directory**
   ```bash
   cd Autocomplete-and-Autocorrect
   ```

3. **Install the required libraries**
   ```bash
   pip install pandas numpy nltk scikit-learn matplotlib
   ```

4. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook
   ```
   *Open `Autocomplete and Autocorrect.ipynb` and run all the cells sequentially.*

---

## 📊 Dataset
This project uses the **Deceptive Opinion Spam / Hotel Review** dataset, which contains:
- Review text
- Deceptive/Truthful classification
- Hotel name, Review polarity, Review source

The **text column** is used as the primary text corpus for the NLP analysis.

---

## 📝 NLP Preprocessing
The text corpus is processed using several essential NLP techniques:
1. **Tokenization**: Reviews are divided into individual words/tokens.
2. **Lowercasing**: All words are converted to lowercase to maintain a consistent vocabulary.
3. **Punctuation Removal**: Unnecessary punctuation marks are removed.
4. **Stopword Handling**: Common English stopwords are analyzed (but retained where necessary, such as `the`, `to`, `is`, for accurate next-word prediction).

---

## 📈 Analysis Performed

### 1️⃣ Bigram Autocomplete
Predicts the next word using the previous word based on training corpus frequency.
- *Example*: `hotel` → `was` | `room` → `was`

### 2️⃣ Trigram Autocomplete
Predicts the next word using the previous two words, providing more contextual information.
- *Example*: `the hotel` → `was` | `the room` → `was`

### 3️⃣ Autocorrect Implementation
Uses a custom **Levenshtein edit-distance** algorithm to identify and correct spelling mistakes via *Insertions, Deletions, and Substitutions*.

### 4️⃣ Autocorrect Testing
Tested on deliberately misspelled words:
- `recieve` → `receive`
- `teh` → `the`
- `adress` → `address`
- `definately` → `definitely`

### 5️⃣ Algorithm Comparison

| Algorithm | Context | Pros/Cons |
|---|---|---|
| **Bigram** | Previous 1 word | Simple, computationally efficient, less data sparsity |
| **Trigram** | Previous 2 words | Better context awareness, higher data sparsity |

---

## 🔍 Key Insights
- **Frequent words** provide useful information for frequency-based autocomplete.
- **Bigram models** are simple and computationally efficient, while **Trigram models** provide better context but suffer from data sparsity.
- **Levenshtein Distance** successfully handles common spelling mistakes, but performance depends heavily on the vocabulary.
- Basic edit-distance correction does **not** understand sentence context or meaning.

---

## ⚠️ Limitations vs. Production Systems (e.g., Google Keyboard)
- Uses a relatively small hotel-review corpus instead of a massive, diverse dataset.
- Bigram/Trigram models have limited contextual understanding compared to **neural language models** (e.g., Transformers, LLMs).
- Does not personalize predictions for individual users.
- May struggle with names, slang, abbreviations, and new words.

---

## 📊 Visualizations

<details>
<summary><b>Click to View Visualizations</b></summary>

| 📊 Top 20 Most Frequent Words| 📈 Bigram vs. Trigram Performance |
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-Autocomplete%20and%20Autocorrect%20Data%20AnalyticsTask5/Images/1.png" height="300px"> | <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-Autocomplete%20and%20Autocorrect%20Data%20AnalyticsTask5/Images/2.png" height="300px"> |

| ⭐ Autocomplete Precision and Recall| 🔤 Autocorrect Performance on 20 Misspelled Words |
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-Autocomplete%20and%20Autocorrect%20Data%20AnalyticsTask5/Images/3.png" height="300px"> | <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-Autocomplete%20and%20Autocorrect%20Data%20AnalyticsTask5/Images/4.png" height="300px"> |

| 🔥 Autocorrect Confusion Matrix | |
| :---: | :---: |
| <img src="https://github.com/ritish18089/OIBSIP/blob/main/DataAnalytics-Level2-Autocomplete%20and%20Autocorrect%20Data%20AnalyticsTask5/Images/5.png" height="300px"> | |

</details>

---

## ▶️ Sample Code
```python
import pandas as pd
import re
from collections import Counter, defaultdict

# Load dataset
df = pd.read_csv("deceptive-opinion.csv")

# Create text corpus
corpus = " ".join(df["text"].dropna().astype(str))

# Lowercase and tokenize
tokens = re.findall(r'\b[a-z]+\b', corpus.lower())

# Create Bigram model
bigram_counts = defaultdict(Counter)
for i in range(len(tokens) - 1):
    bigram_counts[tokens[i]][tokens[i + 1]] += 1

# Display top predictions
print(bigram_counts["hotel"].most_common(3))
```

---

## 📌 Future Improvements
- [ ] Implement **neural language models** & Transformer-based autocomplete.
- [ ] Add contextual embeddings (e.g., Word2Vec, BERT).
- [ ] Implement personalized autocomplete & multilingual support.
- [ ] Implement a **Trie** or **BK-tree** for faster word search in autocorrect.
- [ ] Deploy the model as an interactive Web API (Flask/FastAPI).

---

## 👨‍💻 Author

**Ritish Kannur**  
*Python Developer | Java Full Stack Developer | Data Analytics Enthusiast | Machine Learning Enthusiast*

---

## ⭐ Support
If you found this project useful, consider giving it a ⭐ on GitHub. **Happy Coding! 🚀**
