# N-Gram Mini Projesi: Unigram vs Bigram TF-IDF + Logistic Regression

## 🔹 Proje Hakkında
Bu proje, küçük bir IMDB film yorumları datasetinde **Unigram** ve **Bigram** TF-IDF vektörleri kullanılarak **Logistic Regression** ile duygu analizi yapılmasını göstermektedir.  
Amaç, farklı N-Gram yapılandırmalarının model performansına etkisini karşılaştırmak ve temel NLP metin temsili yöntemlerini öğrenmektir.

---

## 🗂 Dataset
- Kaynak: [IMDB Dataset](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews)  
- Toplam örnek: 50.000 yorum  
- Bu mini proje için: 10.000 yorum kullanıldı (hızlı prototip için)

Datasetin iki sütunu vardır:
1. `review` – Film yorumu metni
2. `sentiment` – Duygu etiketi (`positive` / `negative`)

---

## 🛠 Yapılan İşlemler
1. Dataset yüklendi ve etiketler numerik hale getirildi (`positive → 1`, `negative → 0`).  
2. Küçük örneklem alındı (10.000 yorum)  
3. Train/Test ayrımı yapıldı (%80 / %20)  
4. TF-IDF vektörleştirme uygulandı:  
   - **Unigram:** 1-gram, max_features=5000  
   - **Bigram:** 1-2 gram, max_features=5000  
5. Logistic Regression ile sınıflandırma yapıldı  
6. Accuracy hesaplandı ve modeller karşılaştırıldı  

---

## 📊 Sonuçlar

| Model   | Accuracy |
|---------|----------|
| Unigram | 0.876    |
| Bigram  | 0.872    |

> Küçük dataset ve n-gram seçimi nedeniyle Unigram modeli biraz daha iyi performans gösterdi.

---

## 🔍 Kullanım
1. Colab veya Jupyter Notebook üzerinde çalıştırın.  
2. `IMDB Dataset.csv` dosyasını yükleyin.  
3. Kod hücrelerini sırayla çalıştırın ve sonuçları gözlemleyin.  

```python
# Örnek
df_small = df.sample(10000, random_state=42)
vec_uni = TfidfVectorizer(max_features=5000, ngram_range=(1,1))
vec_bi = TfidfVectorizer(max_features=5000, ngram_range=(1,2))