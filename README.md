# MLBootcampProject

Veri Tabanlı Siber Saldırı Tespiti: Makine Öğrenmesi ile Saldırı Sınıflandırma Modeli

📝 Proje Hakkında

Bu proje, NF-UNSW-NB15-v2 veri seti kullanılarak ağ trafiğindeki saldırıların tespiti amacıyla denetimli makine öğrenmesi algoritmalarıyla geliştirilmiştir. Çok sınıflı sınıflandırma yöntemleriyle 9 farklı saldırı türü ve normal trafik ayrıştırılmaktadır.

## 🔗 Kaggle Notebook Linki
Bu projeyi Kaggle üzerinde incelemek için aşağıdaki bağlantıya tıklayabilirsiniz:  
👉 [Kaggle Notebook - ML Bootcamp Project](https://www.kaggle.com/code/sevvalpektopcu/mlbootcampproject)

## 📊 Veri Seti Bilgileri
- **Veri Seti**: NF-UNSW-NB15-v2 (Kaggle notebook'ta belirtilen versiyon)
- **Özellik Sayısı**: 49 (orijinal veri setinde)
- **Kayıt Sayısı**: ~560,000 (Kaggle notebook'taki örneklenmiş veri)
- **Hedef Değişken**: 10 sınıf (9 saldırı türü + normal trafik)

**Önemli Özellikler** (Kaggle notebook'ta kullanılanlar):
- L4_SRC_PORT
- PROTOCOL
- IN_BYTES
- OUT_PKTS
- TCP_FLAGS
- FLOW_DURATION_MILLISECONDS
- L7_PROTO
- IN_PKTS
- OUT_BYTES

```python
# Veri dağılımı 
print(df['attack_cat'].value_counts())
# Normal: 440000, Generic: 40000, Exploits: 20000, ...

🛠️ Kullanılan Teknolojiler
Makine Öğrenmesi Algoritmaları

Random Forest (Ana model)

Decision Tree

XGBoost

Lojistik Regresyon

KNN

Ön İşleme Teknikleri

Label Encoding

StandardScaler

SMOTE (Dengesiz veri için)

PCA (Boyut indirgeme)

Değerlendirme Metrikleri

Accuracy

Precision/Recall

F1 Score (Weighted/Macro)

Confusion Matrix

ROC-AUC (Çok sınıflı)

📈 Sonuçlar (Kaggle notebook'taki gerçek sonuçlara göre güncellendi)
Karar Ağacı Performansı:

Doğruluk: 0.998

F1 Skoru: 0.997

Random Forest Performansı:

Doğruluk: 0.999

F1 Skoru: 0.998

Lojistik Regresyon Performansı:

Doğruluk: 0.923

F1 Skoru: 0.902

XGBoost Performansı:

Doğruluk: 0.999

F1 Skoru: 0.998

🚀 Kurulum ve Çalıştırma
Gereksinimleri yükleyin:

bash
pip install pandas numpy scikit-learn xgboost imbalanced-learn matplotlib seaborn
Jupyter Notebook'u çalıştırın:

bash
jupyter notebook attack_detection.ipynb
🌍 Gerçek Hayat Uygulamaları
Siber Güvenlik Sistemleri: IDS/IPS entegrasyonu

SOC Analizleri: Anomali tespiti

Ağ Yönetimi: Otomatik tehdit algılama

Bulut Güvenliği: Şüpheli trafik analizi

Hazırlayan: Şevval İpek Topçu
Eğitim: Akbank Machine Learning Bootcamp
Tarih: 25 Temmuz 2025
Versiyon: 1.1
