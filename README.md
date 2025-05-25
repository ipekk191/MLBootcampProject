# MLBootcampProject

Veri Tabanlı Siber Saldırı Tespiti: Makine Öğrenmesi ile Saldırı Sınıflandırma Modeli

📝 Proje Hakkında

Bu proje, NF-UNSW-NB15 veri seti kullanılarak ağ trafiğindeki saldırıların tespiti amacıyla denetimli makine öğrenmesi algoritmalarıyla geliştirilmiştir. Çok sınıflı sınıflandırma yöntemleriyle 9 farklı saldırı türü ve normal trafik ayrıştırılmaktadır.

# 🔗 Kaggle Notebook Linki
Bu projeyi Kaggle üzerinde incelemek için aşağıdaki bağlantıya tıklayabilirsiniz:  
👉 [Kaggle Notebook - ML Bootcamp Project](https://www.kaggle.com/code/sevvalpektopcu/mlbootcampproject)

📊 Veri Seti Bilgileri
- Veri Seti: NF-UNSW-NB15

- Özellik Sayısı: 9

- Kayıt Sayısı: ~2.5M (örneklenmiş)

- Hedef Değişken: 10 sınıf (9 saldırı türü + normal trafik)

Ana Özellikler:

L4_SRC_PORT

PROTOCOL

IN_BYTES

OUT_PKTS

TCP_FLAGS

FLOW_DURATION_MILLISECONDS

python
# Veri dağılımı
print(df['Label'].value_counts())
# Benign: 1550712, Exploits: 24736, Fuzzers: 19463, ...
🛠️ Kullanılan Teknolojiler
Makine Öğrenmesi Algoritmaları
Random Forest (Ana model)

Decision Tree

XGBoost

Lojistik Regresyon

KNN

Ön İşleme Teknikleri
- Label Encoding

- StandardScaler/MinMaxScaler

- SMOTE (Dengesiz veri için)

Değerlendirme Metrikleri
- Accuracy

- Precision/Recall

- F1 Score (Weighted/Macro)

- Confusion Matrix

📈 Sonuçlar
Model	Accuracy	Weighted F1	Macro F1
Random Forest	0.9823	0.9819	0.8924
XGBoost	0.9785	0.9781	0.8742
Decision Tree	0.9712	0.9708	0.8516
Confusion Matrix
Feature Importance

🚀 Kurulum ve Çalıştırma
Gereksinimleri yükleyin:

bash
pip install -r requirements.txt
Jupyter Notebook'u çalıştırın:

bash
jupyter notebook notebooks/attack_detection.ipynb
Alternatif olarak Kaggle'da çalıştırın:
Open in Kaggle

🌍 Gerçek Hayat Uygulamaları
Siber Güvenlik Sistemleri: IDS/IPS entegrasyonu

SOC Analizleri: Anomali tespiti

Ağ Yönetimi: Otomatik tehdit algılama

Hazırlayan: Şevval İpek Topçu
Eğitim: Akbank Machine Learning Bootcamp
Tarih: 25 Temmuz 2025

