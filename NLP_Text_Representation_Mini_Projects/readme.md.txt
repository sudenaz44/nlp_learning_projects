# NLP Text Representation Mini Projects

## Amaç
Bu notebook ile doğal dil işleme alanında metin temsili yöntemlerini öğreniyoruz:
1. N-Gram modelleri (Unigram vs Bigram)
2. Word Embeddings (Word2Vec ile kelime benzerlikleri ve kelime bulutu)
3. Mini Karşılaştırma Projesi (TF-IDF vs N-Gram vs Word Embeddings)

## Dataset
- Küçük sentiment dataset (IMDB mini / rastgele 10.000 örnek)
- Her proje için aynı veri kullanıldı
- Ön işleme: HTML temizleme, stopwords çıkarma, lowercase

## Metodoloji
1. **N-Gram:** TF-IDF ile Unigram ve Bigram modelleri kuruldu ve doğrulukları karşılaştırıldı.
2. **Word Embeddings:** Word2Vec kullanılarak kelime vektörleri çıkarıldı; kelime benzerlikleri ve kelime bulutu görselleştirildi.
3. **Mini Karşılaştırma:** Aynı dataset ile TF-IDF, N-Gram ve Word Embeddings modellerinin doğrulukları karşılaştırıldı.

## Sonuçlar
- Accuracy ve görselleştirmeler ile hangi yöntemin daha etkili olduğu gözlemlendi.
- Bu üç mini proje, metin temsili yöntemlerini kavramak ve CV için güçlü bir örnek oluşturmak amacıyla hazırlandı.

## Kullanım
- Notebook'u çalıştırın
- Adım adım projeleri takip edin
- Sonuçları görselleştirin ve yorumlayın