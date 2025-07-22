# Mağaza Yorumları Üzerinden Türkçe Duygu Analizi

Bu projede, Türkçe mağaza yorumlarını kullanarak duygu analizi gerçekleştirdim. Yorumları **olumlu**, **olumsuz** ve **tarafsız** olmak üzere üç sınıfa ayıran bir makine öğrenmesi modeli geliştirdim.

## 📁 Veri Seti

Veri setini Kaggle üzerinde [Duygu Analizi İçin Ürün Yorumları](https://www.kaggle.com/datasets/burhanbilenn/duygu-analizi-icin-urun-yorumlari) başlıklı çalışmadan aldım.  
Bu veri seti Türkçe yorumları ve bunlara ait duygu etiketlerini içeriyor.

## ⚙️ Kullandığım Teknolojiler

- Python 3
- pandas, numpy
- scikit-learn
- matplotlib, seaborn

## 🧪 Yaptığım Çalışmalar

1. **Veri Temizleme ve Ön İşleme**  
   - Yorumları küçük harfe çevirdim.  
   - Noktalama işaretlerini ve gereksiz boşlukları kaldırdım.  

2. **Görselleştirme ve Keşifsel Veri Analizi (EDA)**  
   - Sınıf dağılımını inceledim.  
   - Örnek yorumları sınıflarına göre görüntüledim.  

3. **Metin Vektörleştirme**  
   - Yorumları sayısal verilere dönüştürmek için **TF-IDF (Term Frequency - Inverse Document Frequency)** yöntemini kullandım.

4. **Model Eğitimi ve Tahmin**  
   - Makine öğrenmesi modeli olarak **Multinomial Naive Bayes (MultinomialNB)** algoritmasını kullandım.  
   - Eğitim ve test verisini `train_test_split` ile ayırdım.

5. **Model Değerlendirme**  
   - Başarıyı ölçmek için **doğruluk (accuracy)** ve diğer metrikleri kullandım.

## 🚀 Nasıl Çalıştırılır?

1. Kaggle’daki veri setini indir:  
   [https://www.kaggle.com/datasets/burhanbilenn/duygu-analizi-icin-urun-yorumlari](https://www.kaggle.com/datasets/burhanbilenn/duygu-analizi-icin-urun-yorumlari)

2. `dataset.csv` dosyasını proje klasörüne koy.

3. Gerekli kütüphaneleri yükle:

```bash
pip install -r requirements.txt
