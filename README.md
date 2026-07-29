# 📄 Resume Classification Project

Automatically classify resumes into categories like **React Developer**, **Workday**, **Peoplesoft**, or **SQL Developer** using Natural Language Processing and Machine Learning.

App Link - https://resume-classification-project-esdoqdtnuvhnyahjrjtjxe.streamlit.app/
---

## 🚀 Features

- ✅ Upload resumes in **PDF, DOC, or DOCX**
- ✅ Automatically extract and clean text
- ✅ Predict resume category with **Multinomial Naive Bayes** model
- ✅ Show confidence score with threshold
- ✅ Supports **single or multiple** resume uploads
- ✅ Download results as CSV
- ✅ Beautiful UI with **Streamlit**

---

## 🧠 Machine Learning Pipeline

- **Text Preprocessing**:
  - HTML & URL removal
  - Lowercasing
  - Tokenization (with `nltk`)
  - Stopword removal
- **Feature Extraction**:
  - `TfidfVectorizer` (max 3000 features)
- **Model**:
  - `MultinomialNB` (best parameters via GridSearchCV)
- **Pipeline**:
  - Custom `TextCleaner` class → TF-IDF → Naive Bayes
- **Label Encoding**:
  - Encodes and decodes resume categories

---
