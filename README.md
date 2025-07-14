# 📡 Fuzzy Localization in Wireless Sensor Networks (WSNs)

Bu proje, **kablosuz sensör ağlarındaki (WSN)** düğüm lokalizasyon problemini çözmek için **Mamdani tipi bulanık mantık çıkarım sistemi (FIS)** kullanan bir Python uygulamasıdır. Bursa Teknik Üniversitesi'nde BLM0468 "Esnek Hesaplamaya Giriş" dersi kapsamında geliştirilmiştir.

---

## 🎯 Amaç

Konumu bilinmeyen düğümlerin, konumu bilinen çapalı düğümler (anchor nodes) yardımıyla **ortalama lokalizasyon hatası (ALE)** değerini tahmin etmek.

---

## 📊 Kullanılan Veri Kümesi

📂 [UCI Repository - ALE Dataset](https://archive.ics.uci.edu/dataset/844/average+localization+error+(ale)+in+sensor+node+localization+process+in+wsns)

| Özellik             | Açıklama                     |
|---------------------|------------------------------|
| Anchor Ratio        | Çapa düğüm oranı             |
| Transmission Range  | İletim aralığı               |
| Node Density        | Düğüm yoğunluğu              |
| Iterations          | Yineleme sayısı              |
| ALE                 | Ortalama lokalizasyon hatası |

> Standart sapma (`sd_ale`) kullanılmamıştır.

---

## 🧠 Kullanılan Yöntemler

- **Bulanık Mantık Tipi:** Mamdani
- **Üyelik Fonksiyonu Türleri:**
  - Triangular (Üçgensel)
  - Gaussian (Gauss)
- **Defuzzification Yöntemleri:**
  - Centroid (Ağırlıklı Ortalama)
  - MOM (Maksimumların Ortalaması)
  - SOM (Maksimumların Toplamı)
  - Bisector (Alan Ortası)

Toplamda **8 farklı model kombinasyonu** denenmiştir (2 MF × 4 Defuzz).

---

## 🧰 Kullanılan Teknolojiler

- Python 3.x
- scikit-fuzzy
- NumPy, Pandas, Matplotlib, Seaborn
- scikit-learn

---
