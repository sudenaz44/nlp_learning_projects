Word Embeddings Mini Projesi (IMDB Dataset)
📌 Proje Amacı

Bu proje, doğal dil işleme (NLP) alanında kelime vektör temsillerini öğrenmek ve görselleştirmek için hazırlandı. Amaç:

Kelimelerin anlam benzerliklerini yakalamak
Word2Vec kullanarak kelime vektörleri oluşturmak
Kelime ilişkilerini analiz etmek ve görselleştirmek
NLP projelerinde anlam temelli özellikler kullanmayı öğrenmek

Bu proje, özellikle metin temsili ve derin öğrenme tabanlı NLP görevlerinde temel bir yapı taşıdır.

📚 Kullanılan Teknikler
Veri Ön İşleme
HTML tag temizleme
Küçük harfe çevirme
Noktalama ve özel karakterleri kaldırma
Stopwords çıkarma
Tokenizasyon (kelime listesi oluşturma)
Word Embeddings
Word2Vec (Gensim) kullanılarak kelimeler vektörlere dönüştürüldü
Parametreler:
vector_size=100 → kelime vektör boyutu
window=5 → kelimenin çevresindeki kelime sayısı
min_count=2 → en az geçen kelimeler
sg=1 → Skip-gram modeli
Kelime Benzerlikleri
Model ile belirli bir kelimenin en yakın anlamlı kelimeleri bulundu
Örnek: 'good' kelimesine en benzer kelimeler
Görselleştirme
WordCloud ile sık geçen kelimeler görselleştirildi
Kelimelerin boyutu, metin içerisindeki sıklığına göre ayarlandı
🛠️ Kullanılan Kütüphaneler
pandas → veri manipülasyonu
nltk → stopwords ve tokenization
gensim → Word2Vec modeli
wordcloud → kelime bulutu görselleştirme
matplotlib → görselleştirme
📊 Örnek Çıktılar
Word2Vec modelinden 'good' kelimesine en benzer 10 kelime:
[('decent', 0.746), ('welldone', 0.739), ('admirable', 0.732), ...]
WordCloud görselleştirmesi:

(Burada görseli notebook içinde gösteriyoruz)

⚡ Özet
Bu proje, kelimelerin anlamlarını sayısal vektörler ile temsil etme yeteneğini gösterir.
Word2Vec sayesinde kelimeler arası semantik ilişkiler yakalanır.
Kelime bulutu ve benzerlikler ile veriye dair anlamlı görselleştirmeler yapılabilir.
Proje, NLP portföyü ve CV için güçlü bir örnektir.