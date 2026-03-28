NLP Metin Temsili Karşılaştırma Projesi
📌 Proje Amacı

Bu projede, iki farklı sentiment veri seti üzerinde farklı metin temsili yöntemlerini karşılaştırdık:

TF-IDF (Unigram)
TF-IDF (Unigram + Bigram)
Word Embeddings (Word2Vec)

Amaç, aynı dataset üzerinde farklı yöntemlerin performansını ölçmek ve hangisinin daha iyi sonuç verdiğini görmektir. Bu, NLP portföyünde güçlü bir CV öğesi oluşturur, çünkü farklı metin temsili tekniklerini tek bir çatı altında karşılaştırıyoruz.

📂 Kullanılan Datasetler
IMDB Dataset (Film Yorumları)
50.000 yorum
İkili duygu sınıflandırması (0 → negatif, 1 → pozitif)
Kaynak: Kaggle IMDB Dataset


Sentiment Data Dataset (Yeni Dataset)
241.145 yorum
Üçlü duygu sınıflandırması (0 → negatif, 1 → nötr, 2 → pozitif)
Kaynak: Kullanıcı tarafından sağlanmış (/content/sentiment_data.csv)

📊 Accuracy Karşılaştırması
Dataset	TF-IDF Unigram	TF-IDF Bigram	Word2Vec
IMDB (50k yorum)	0.876	0.872	0.8545
Sentiment Data (241k yorum)	0.6750	0.6735	0.5120


📈 Yorumlar
IMDB Dataset
TF-IDF yöntemleri yüksek performans gösterdi (~0.87-0.88)
Word2Vec de iyi sonuç verdi (~0.85)
Yani bu dataset küçük ve temiz olduğu için hem TF-IDF hem Word2Vec etkili.
Sentiment Data Dataset
Daha büyük ve üç sınıflı olduğu için accuracy düştü (~0.51-0.67)
TF-IDF yine Word2Vec’den daha iyi performans gösteriyor
Büyük ve dengesiz veri setlerinde Word2Vec’in tek yorum ortalamaları ile performans kaybı yaşanıyor.


🔧 Kullanılan Teknolojiler ve Kütüphaneler
Python 3.x
Pandas
Scikit-learn
Gensim (Word2Vec)
NLTK (stopwords)
WordCloud
Matplotlib / Seaborn


📝 Sonuç
TF-IDF, küçük ve orta boy datasetlerde hâlâ güçlü bir yöntemdir.
Word2Vec, büyük datasetlerde daha fazla veri ile güçlü olabilir, ancak küçük sample veya ortalama vektör kullanımı performansı düşürebilir.
Bu proje sayesinde, farklı metin temsili yöntemlerinin karşılaştırmalı etkilerini tek bir çatı altında görmek mümkün oldu.
