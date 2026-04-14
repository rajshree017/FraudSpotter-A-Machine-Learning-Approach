# 🕵️ FraudSpotter — Fake Review Detection

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit_Learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![NLP](https://img.shields.io/badge/NLP-Text_Classification-blueviolet?style=for-the-badge)

**Detecting fake product reviews using Machine Learning & NLP**

</div>

---

## 📌 Overview

Online platforms like Amazon are flooded with **fake, computer-generated reviews** that mislead consumers and damage brand trust. **FraudSpotter** is an end-to-end ML pipeline that automatically detects whether a review is:

| Label | Meaning |
|-------|---------|
| `CG` | Computer-Generated **(Fake)** |
| `OR` | Original / Human-Written **(Real)** |

---

## 📊 Dataset

- **Size:** 40,000 Amazon product reviews
- **Categories:** Home & Office, Sports, and more
- **Features:** `review text`, `star rating`, `label (CG/OR)`
- **Balance:** ~50% fake, ~50% real

---

## 🔁 Project Pipeline

```
Raw Reviews
    │
    ▼
📂 Data Loading & EDA
    │  → Label distribution analysis
    │  → Rating analysis by category
    │
    ▼
🧹 Text Preprocessing
    │  → Punctuation removal
    │  → Stopword removal
    │  → Tokenization
    │  → Stemming (Porter Stemmer)
    │  → Lemmatization (WordNet)
    │
    ▼
🔢 Feature Engineering
    │  → Bag of Words (CountVectorizer)
    │  → TF-IDF Transformation
    │
    ▼
🤖 Model Training & Evaluation
    │  → 6 ML models compared
    │  → Confusion matrices
    │  → Classification reports
    │
    ▼
🏆 Best Model Selection
```

---

## 🤖 Models Compared

| Model | Type | Notes |
|-------|------|-------|
| ✅ Naive Bayes | Probabilistic | Fast, great NLP baseline |
| ✅ Logistic Regression | Linear | Strong text classifier |
| ✅ SVM | Kernel-based | High accuracy on text |
| ✅ Random Forest | Ensemble | Robust, handles noise |
| ✅ Decision Tree | Tree-based | Interpretable |
| ✅ K-Nearest Neighbors | Distance-based | Baseline comparison |

---

## 📈 Results

> All models trained on **70% data**, evaluated on **30% holdout test set**

| Model | Accuracy |
|-------|----------|
| 🥇 Logistic Regression | ~92%+ |
| 🥈 SVM | ~91%+ |
| 🥉 Naive Bayes | ~90%+ |
| Random Forest | ~88%+ |
| Decision Tree | ~82%+ |
| KNN | ~78%+ |

---

## 🛠️ Tech Stack

| Category | Tools |
|----------|-------|
| Language | Python 3.x |
| Data Manipulation | Pandas, NumPy |
| NLP | NLTK (tokenization, stopwords, stemming, lemmatization) |
| ML Models | Scikit-learn |
| Feature Extraction | CountVectorizer, TF-IDF |
| Visualization | Matplotlib, Seaborn |
| Environment | Jupyter Notebook |

---

## 📁 Project Structure

```
FraudSpotter-A-Machine-Learning-Approach/
│
├── 📓 FraudSpotter_Part1_EDA_Preprocessing.ipynb   ← EDA + Text Cleaning
├── 📓 FraudSpotter_Part2_ModelTraining.ipynb        ← Models + Evaluation
├── 📄 fake reviews dataset.csv                      ← Raw dataset
├── 📄 Preprocessed Fake Reviews Detection Dataset.csv ← Cleaned dataset
└── 📋 README.md
```

---

## 🚀 How to Run

```bash
# 1. Clone the repository
git clone https://github.com/rajshree017/FraudSpotter-A-Machine-Learning-Approach.git
cd FraudSpotter-A-Machine-Learning-Approach

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn nltk jupyter

# 3. Open Jupyter
jupyter notebook

# 4. Run in order:
#    → FraudSpotter_Part1_EDA_Preprocessing.ipynb
#    → FraudSpotter_Part2_ModelTraining.ipynb
```

---

## 💡 Key Learnings

- **TF-IDF** outperforms simple Bag-of-Words for text classification
- **Lemmatization + Stemming** together improve model accuracy
- **Logistic Regression** and **SVM** are top performers for NLP tasks
- Fake reviews tend to have **different length patterns** than real ones

---

## 👩‍💻 Author

**Rajshree** — Java & Python Developer | AI/ML Enthusiast

[![GitHub](https://img.shields.io/badge/GitHub-rajshree017-181717?style=flat-square&logo=github)](https://github.com/rajshree017)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=flat-square&logo=linkedin)](https://linkedin.com/in/rajshree-1839262b1)

---

<div align="center">

⭐ **If this project helped you, please give it a star!** ⭐

</div>
