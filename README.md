# 🧠 Form Yanıtlarından Satın Alma Eğilimi Tahmini

Bu proje, yapay olarak oluşturulmuş bir anket formu üzerinden bireylerin bir ürünü satın alıp almayacağını tahmin etmek için makine öğrenmesi algoritmalarının kullanıldığı bir simülasyondur.

---

## 🔍 Proje Hedefi
- Yapay veri üretimi ile form yanıtlarını simüle etmek
- Sınıflandırma algoritmaları ile satın alma tahmini yapmak
- Model başarımını karşılaştırmak
- Olasılık bazlı analizlerle farklı senaryoların etkisini değerlendirmek

---

## 🧱 Kullanılan Teknolojiler
- Python 3
- Pandas, NumPy
- Scikit-learn (RandomForest, LogisticRegression, KNN)
- XGBoost
- Matplotlib, Seaborn

---

## 📁 Klasör Yapısı (Önerilen)
```
├── data/                # Yapay veri setleri (CSV)
├── models/              # Eğitilmiş model çıktıları
├── notebooks/           # Analiz ve deneyler (Jupyter dosyaları)
├── visuals/             # Grafik çıktıları (PNG, SVG)
└── README.md            # Proje açıklaması
```

---

## 📊 Üretilen Yapay Form Verisi
| Özellik               | Açıklama                                 |
|-----------------------|-------------------------------------------|
| Yaş                   | 18–65 arası rastgele dağıtılmış           |
| Cinsiyet              | Kadın / Erkek                            |
| Eğitim Seviyesi       | Lise / Üniversite / Yüksek Lisans        |
| Gelir                 | Ortalama 15.000 TL (normal dağılım)     |
| Sosyal Medya Süresi   | 0–10 saat arası                          |
| Ürün Bilgisi          | Kullanıcının ürünü önceden duyup duymadığı |
| Kampanya Bilgisi      | Kampanya teklifinin olup olmadığı        |
| Satın Alma            | Hedef değişken (0 veya 1)                |

---

## ⚙️ Uygulanan Modeller
- **Random Forest Classifier** ✅
- **Logistic Regression**
- **K-Nearest Neighbors (KNN)**
- **XGBoost Classifier**

Her model:
- `train_test_split` ile eğitildi
- `accuracy_score` ile test edildi
- `GridSearchCV` ile hiperparametre optimizasyonu yapıldı (Random Forest)

---

## 📈 Olasılık Temelli Simülasyonlar
- Modelin her bireye verdiği "satın alma olasılığı" değerlendirildi
- Olasılıkların dağılımı histogram ve KDE ile görselleştirildi
- **Kampanya var / yok senaryoları** ayrı ayrı analiz edildi

---

## 🔍 Öne Çıkan Sonuçlar
- Kampanya bilgisi, satın alma tahmini üzerinde **yüksek etkili** bir değişken
- Random Forest modeli %87 doğruluk ile en başarılı sonuçları verdi
- Tahmin olasılıkları büyük ölçüde 0 veya 1'e yakın çıktı (emin kararlar)

---

## 👨‍💻 Geliştiren: Sefa Yasin Namlı
