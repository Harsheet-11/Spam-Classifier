# 📧 Spam Email Classifier 

<img width="1536" height="1024" alt="Spam (1)" src="https://github.com/user-attachments/assets/e7b3cd66-c9cc-4653-8b0f-ee716abd720e" />


---

## 📌 Project Overview
This project aims to classify emails as either **"Spam"** (junk) or **"Ham"**. 

I had performed the following processes:
1.  **Data Preprocessing:** Cleaning and normalizing text.
2.  **Feature Engineering:** Converting text to numerical vectors using TF-IDF.
3.  **Model Building:** Training a classifier using Scikit-Learn Pipelines.
4.  **Evaluation:** Validating performance with Precision, Recall, and F1-Score.

---

## 🛠️ Technical Architecture

### 1. The Dataset
* **Source:** SMS Spam Collection Dataset.
* **Size:** ~5,572 messages.

### 2. The Tech Stack
* **Language:** Python 
* **Libraries:** Pandas, NumPy, Scikit-Learn.
* **Key Tools:**
    *  `TfidfVectorizer` (for text-to-number conversion).
    * `Pipeline` (for streamlining the workflow).
    * `RandomForestClassifier` (The final model).

---

## 🤖 Algorithm Selection

After testing multiple algorithms (KNN, Naive Bayes, and Random Forest), I chose **Random Forest** for the final model.

**Why Random Forest?**
* **Accuracy:** It outperformed KNN and Naive Bayes in my tests, achieving the highest F1-Score.
* **Robustness:** It handles high-dimensional data (like text vectors) well and is less prone to overfitting than a single Decision Tree.
* **Ensemble Power:** By averaging multiple decision trees, it reduced variance and provided stable predictions for unseen emails.

---

## 📊 Performance Metrics

My final model achieved the following results on the Test Set (20% split):

| Metric | Score |
| :--- | :--- |
| **Accuracy** | **~98%** |
| **Precision** | **1.00** |
| **Recall** | **0.85** |
| **F1-Score** | **0.92** |


---

## 📚 Learning Sources & References
* **Pandas:** To understand how to use pandas from youtube channel [Tech with Tim]
* **Data Processing:** : NLTK and Python documentation (re, string)
* **Scikit-Learn Documentation:** For understanding Pipelines and TfidfVectorizer.
* **Codebasics (YouTube):** "TF-IDF & Text Classification" tutorial for conceptual understanding of NLP vectorization.


---
