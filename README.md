# Estimating-vehicle-loading-times
# Sevkiyat Yükleme Süresi Tahmin Projesi 🚢⏱️

Bu proje, sevkiyat operasyonlarındaki yükleme sürelerini tahmin etmek ve operasyonel verimliliği artırmak amacıyla geliştirilmiş bir makine öğrenmesi modelidir.

## 📈 Projenin Yolculuğu ve Elde Edilen Başarı

Projenin başlangıcında, ham veriyle eğitilen model tamamen başarısız sonuçlar vermiştir (Negatif R2 Skoru). Yapılan derinlemesine veri analizi, sorunun kaynağının veri setindeki **aşırı uç (aykırı) değerler** olduğunu ortaya çıkarmıştır.

Bu aykırı değerler istatistiksel yöntemlerle temizlendikten sonra model yeniden eğitilmiş ve şu çarpıcı sonuçlara ulaşılmıştır:

* **Ortalama Hata Payı (MAE):** 3 saati aşan bir süreden **~12.6 dakikaya** düşürüldü.
* **Model Başarısı (R2 Skoru):** Negatif değerden **0.17**'ye yükseltilerek modelin istatistiksel olarak anlamlı tahminler yapabildiği kanıtlandı.

## 📊 Analiz Grafikleri

Proje kapsamında yapılan bazı analizler:

#### Kaynak Adreslerine Göre Yükleme Süreleri
*(Buraya `grafik_kaynak_adresler.png` grafiğini sürükleyip bırakabilirsiniz)*

#### Sevkiyat Türüne Göre Yükleme Süreleri
*(Buraya `grafik_sevkiyat_turu.png` grafiğini sürükleyip bırakabilirsiniz)*


## 🛠️ Kullanılan Teknolojiler
- Python
- Pandas & NumPy
- Scikit-learn
- Matplotlib & Seaborn

## 📂 Proje Yapısı
- `ana_kod.py`: Veri işleme, analiz, model eğitimi ve kaydetme adımlarını içeren ana Python betiği.
- `grafik_*.png`: Veri analiz sürecinde oluşturulan görselleştirmeler.

**Not:** Bu projede kullanılan veri seti, örneklem verilerden oluşmaktadır ve boyutu nedeniyle depoya dahil edilmemiştir.
