# 🎬 IMDB Sentiment Analysis (NLP Project)

## 🧠 Overview

This project focuses on performing **sentiment analysis** on the IMDB movie reviews dataset using traditional NLP techniques.

The goal is to classify reviews as **positive** or **negative** using machine learning.

---

## 📊 Dataset

* IMDB Dataset (50,000 movie reviews)
* Balanced dataset:

  * 25,000 positive
  * 25,000 negative

---

## ⚙️ Methods Used

### 🔹 Text Representation

* TF-IDF (Term Frequency - Inverse Document Frequency)
* N-gram (1,2)

### 🔹 Model

* Logistic Regression (scikit-learn)

---

## 🚀 Pipeline

1. Load dataset
2. Text preprocessing (cleaning, lowercasing)
3. TF-IDF vectorization
4. Train/Test split (80/20)
5. Model training (Logistic Regression)
6. Evaluation

---

## 📈 Results

* **Accuracy:** ~90%
* Balanced performance across both classes
* F1-score: ~0.90

---

## 📊 Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix

---

## 🧠 Key Learnings

* How to convert text into numerical features (TF-IDF)
* Importance of preprocessing in NLP
* Working with large real-world datasets
* Evaluating classification models

---

## 🛠 Technologies

* Python
* Pandas
* Scikit-learn
* Matplotlib / Seaborn

---

## 📁 Project Structure

```bash
imdb.ipynb
README.md
```

---

## 🎯 Future Improvements

* Use Word Embeddings (Word2Vec, FastText)
* Apply Deep Learning (LSTM, BERT)
* Hyperparameter tuning

---

## 🔥 Conclusion

This project demonstrates that even simple models like Logistic Regression combined with TF-IDF can achieve strong performance in NLP tasks.

---
IMDB Sentiment Analysis 

Hedef: Gerçek dataset kullanarak TF-IDF + Logistic Regression ile duygu analizi yapmak.
Adımlar:

---
Yorumları:
Precision (kesinlik): Modelin “pozitif tahminlerinin” ne kadarının gerçekten pozitif olduğunu gösterir.
Negative için 0.91 → Model negatif dediğinde %91 doğru.
Positive için 0.90 → Model pozitif dediğinde %90 doğru.
Recall (duyarlılık): Gerçek pozitiflerin kaçını doğru tahmin etti.
Negative için 0.89 → Gerçek negatiflerin %89’u doğru tahmin edilmiş.
Positive için 0.92 → Gerçek pozitiflerin %92’si doğru tahmin edilmiş.
F1-Score: Precision ve Recall’un dengeli ortalaması → her iki sınıf için ~0.90 → dengeli bir model.
Support: Test setindeki her sınıfın örnek sayısı.
4961 negative, 5039 positive → neredeyse eşit, dengeli veri.
----
