# 🎯 Kimlik Avı (Phishing) Web Sitelerinin Tespitinde URL ve İçerik Analizi

Bu proje, **sahte (phishing) web sitelerini** tespit etmek amacıyla URL yapısı ve sayfa içeriğini analiz eden bir sistem geliştirmeyi amaçlar. Makine öğrenmesi teknikleri kullanılarak, kullanıcıları kandırmaya yönelik URL ve içerik desenleri üzerinden yüksek doğrulukta tahminler yapılmaktadır.

## 📌 Problem Tanımı

Kimlik avı (phishing), kullanıcıları sahte e-postalar veya web siteleriyle kandırarak kişisel bilgilerini çalmayı hedefleyen yaygın bir siber saldırı türüdür. Mevcut antivirüs ve filtre sistemleri her zaman yeterli koruma sağlayamamaktadır. Bu nedenle bu çalışmada, URL ve içerik analizi yaparak phishing sitelerini otomatik olarak tespit eden bir sistem tasarlanmıştır.

## 📚 Kullanılan Veri Seti

- 📦 Kaynak: [Kaggle - Phishing Websites Dataset](https://www.kaggle.com/)
- 🔢 Veri Sayısı: 11.055 örnek URL
- 🧠 Özellik Sayısı: 85+ (URL yapısı + HTML içerik özellikleri)
- 🔖 Etiketler:
  - `0` → Gerçek (Legitimate)
  - `1` → Phishing (Sahte)
- 🔍 Eğitim/Test Ayrımı: %80 Eğitim / %20 Test

## 🧪 Öne Çıkan Özellikler

- URL uzunluğu
- Subdomain sayısı
- HTTPS kullanımı
- Şüpheli kelimeler (login, verify, update vb.)
- HTML form yapıları
- JavaScript içerik analizi
- Meta ve başlık tutarsızlıkları

## 🤖 Kullanılan Makine Öğrenmesi Modelleri

- Decision Tree
- Random Forest ✅ (En iyi performansı verdi)
- Naive Bayes
- Support Vector Machine (SVM)

### 🎯 Değerlendirme Metrikleri

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

> 📈 En yüksek başarı oranı Random Forest algoritması ile elde edilmiştir.

## 📊 Görselleştirmeler

- Confusion Matrix
- Özellik Önem Grafiği (Feature Importance)

## 📁 Proje Dosyaları

```plaintext
📦 phishing-tespit
├── KİMLİK AVI (PHISHING) WEB SİTELERİNİN TESPİTİNDE.pptx  # Sunum dosyası
├── kod.ipynb                                             # Makine öğrenmesi kodları
└── README.md                                             # Proje tanıtım metni (bu dosya)

👨‍💻 Geliştirici
Arif Yarencik
Bilgisayar Mühendisliği, Düzce Üniversitesi
2025