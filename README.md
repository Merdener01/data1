# Türkiye Hava Durumu Veri Analizi & Sıcaklık Tahmin Modeli

Bu proje, Türkiye'deki günlük hava durumu verileri kullanılarak sıcaklık trendlerini analiz etmeyi ve geleceğe yönelik tahminlerde bulunmayı amaçlamaktadır. Projede Python ile veri temizleme, analiz, görselleştirme ve regresyon tabanlı tahminleme yöntemleri uygulanmıştır.

---

## 📌 Projenin Amacı

- Ham meteorolojik verileri işlemek ve analiz etmek
- Veri içindeki trendleri, değişimleri ve istatistiksel ilişkileri incelemek
- Basit regresyon modeli kullanarak kısa vadeli sıcaklık tahminleri üretmek
- Ortaya çıkan bulguları grafiklerle açıklayıcı bir şekilde sunmak

Bu proje, veri hazırlama → analiz → modelleme → görselleştirme sürecini *uçtan uca* göstermektedir.

---

## 🧰 Kullanılan Teknolojiler ve Kütüphaneler

| Alan | Kullanım |
|------|---------|
| Python | Genel analiz süreci |
| Pandas | Veri seti işleme ve temizleme |
| NumPy | Sayısal hesaplama işlemleri |
| Matplotlib | Görselleştirme ve grafik üretimi |
| Scikit-learn (opsiyonel) | Regresyon modeli geliştirme |
| Jupyter Notebook (opsiyonel) | Analiz adımlarını interaktif yürütme |

---

## 📂 Proje Yapısı


> *Bu klasör yapısı öneri niteliğindedir. Kendi projenle uyumlu şekilde düzenleyebilirsin.*

---

## 🔄 Veri İşleme Adımları

1. Veri setinin içe aktarılması
2. Eksik gözlemlerin belirlenmesi ve temizlenmesi
3. İlgili kolonların seçilmesi ve dönüştürülmesi
4. Sıcaklık değerlerinin hareketli ortalama üzerinden yumuşatılması
5. Regresyon modeli ile tahmin yapılması
6. Tahmin sonuçlarının grafiksel olarak gösterilmesi

---

## 🤖 Model

Proje kapsamında **basit doğrusal regresyon modeli** uygulanmıştır.  
Model, son X günün sıcaklık verilerinden yola çıkarak bir sonraki günün sıcaklığını tahmin eder.

```python
from sklearn.linear_model import LinearRegression

model = LinearRegression()
model.fit(X_train, y_train)
predictions = model.predict(X_test)

---

## 📊 Örnek Görselleştirme

> Bu görüntüleri daha sonra ekleyeceğiz — sen kodu çalıştırınca grafikler oluşturulacak.

