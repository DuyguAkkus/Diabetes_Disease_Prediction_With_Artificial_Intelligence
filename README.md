# Diyabet Hastalığı Tahmini

Bu proje, kadın hastalara ait sağlık ölçümleri verilerini analiz ederek diyabet hastalığını tahmin eden makine öğrenimi modelleri geliştirmeyi amaçlamaktadır.

## 📋 Proje İçeriği

- **Veri Analizi:**
  - Veri setinin incelenmesi ve ön işlenmesi.
  - Eksik verilerin kontrolü ve temizlenmesi.
  - Veri görselleştirme teknikleri (Histogram, Scatter Plot, Pair Plot vb.).

- **Makine Öğrenimi Modelleri:**
  - **Lojistik Regresyon**:
    - **Doğruluk Oranı**: %78.57
    - **Ölçeklendirme** (StandardScaler) ile aynı doğruluk oranı elde edilmiştir.
  - **GridSearchCV ile Optimizasyon**:
    - **En iyi model**: Lojistik Regresyon, farklı hiperparametrelerle optimize edildi.
    - **Doğruluk Oranı (Optimizasyon Sonrası)**: %75.97
  - **ADASY Resampling**:
    - Dengesiz veri setini dengelemek için kullanıldı.
    - **Doğruluk Oranı (ADASY Kullanımı ile)**: %78.57

## 📊 Kullanılan Veri Seti

- **Kaggle’dan alınan diyabet veri seti.**
- **Değişkenler:**
  - `Pregnancies`: Hamilelik sayısı.
  - `Glucose`: Kandaki glikoz seviyesi.
  - `BloodPressure`: Kan basıncı.
  - `SkinThickness`: Deri kalınlığı.
  - `Insulin`: Kandaki insülin seviyesi.
  - `BMI`: Vücut kitle indeksi.
  - `DiabetesPedigreeFunction`: Genetik diyabet yatkınlığı.
  - `Age`: Kişinin yaşı.
  - `Outcome`: Diyabet durumu (1: Hasta, 0: Sağlıklı).

## 🛠️ Kullanılan Teknikler

1. **Veri Ölçeklendirme (StandardScaler):**
   - Lojistik regresyon modeli için veri ölçeklendirme yapılarak model performansı gözlemlendi.

2. **Hiperparametre Optimizasyonu (GridSearchCV):**
   - Çeşitli `C` ve `solver` parametreleri test edilerek en iyi model seçildi.

3. **Dengesiz Veri İçin Resampling (ADASY):**
   - Azınlık sınıflarının daha iyi temsil edilmesi için veri çoğaltma teknikleri kullanıldı.

## 🚀 Proje Kurulumu

1. Bu projeyi klonlayın:
   ```bash
   git clone <proje-repo-url>
   cd <proje-dizin-adi>
