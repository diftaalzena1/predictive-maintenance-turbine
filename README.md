# ⚡ Predictive Maintenance for Thermal Power Plant Turbines (Dummy Project)

Halo! Ini adalah proyek portofolio saya sebagai seorang data scientist, yang berfokus pada bagaimana machine learning dapat membantu sistem industri — khususnya di sektor pembangkit listrik — dalam mendeteksi potensi gangguan lebih awal dan meningkatkan efisiensi pemeliharaan.

Dalam proyek ini, saya membangun model klasifikasi prediktif berbasis data sensor (**temperatur**, **tekanan**, **getaran**) untuk mendeteksi kemungkinan gangguan pada **turbin PLTU (Pembangkit Listrik Tenaga Uap)** menggunakan data dummy.

---

## 🧠 Latar Belakang

Turbin adalah komponen vital dalam sistem pembangkit listrik tenaga uap (PLTU). Kegagalan turbin secara mendadak dapat menyebabkan downtime mahal dan risiko kerusakan serius. Oleh karena itu, diperlukan sistem **perawatan prediktif (predictive maintenance)** yang mampu mendeteksi potensi gangguan sejak dini.

Melalui proyek ini, saya mensimulasikan pendekatan machine learning yang dapat digunakan untuk mengklasifikasikan kondisi turbin menjadi:
- ✅ **Normal**
- ❗ **Waspada**
- ⚠️ **Kritis**

Model yang dibangun dapat diintegrasikan dalam sistem pemantauan real-time seperti **SCADA/IIoT** milik PLN atau industri pembangkit lainnya.

---

## 🎯 Tujuan Proyek

Proyek ini bertujuan untuk:

- Mensimulasikan sistem prediksi gangguan turbin berbasis data sensor.
- Mengembangkan fungsi pemantauan real-time dengan tingkat akurasi tinggi.
- Memberikan insight tentang fitur sensor paling krusial dalam mendeteksi gangguan.
- Menunjukkan implementasi end-to-end machine learning project di sektor kelistrikan.

---

## 🛠️ Pendekatan & Tools

### Data & Preprocessing
- Data sensor sintetis: temperatur, tekanan, getaran selama 1000 hari
- Penentuan label gangguan: terjadi bila dua dari tiga parameter melewati ambang batas
- Penyeimbangan kelas dengan **SMOTE**
- Penskalaan fitur menggunakan **StandardScaler**

### Modeling & Evaluasi
- Model: **Random Forest**, **SVM**, dan **Logistic Regression**
- Evaluasi: **Accuracy**, **ROC AUC**, **Confusion Matrix**
- Analisis **feature importance** untuk interpretasi

### Deployment-ready
- Pipeline produksi dengan `scikit-learn Pipeline`
- Fungsi `monitor_turbine()` untuk prediksi real-time

---

## 📊 Komponen Utama

- **EDA Visual**: Pairplot, tren gangguan mingguan
- **Model Evaluation**:
  - Confusion Matrix 📌 *(Baris = label aktual, Kolom = prediksi)*
  - ROC Curve dengan highlight **AUC > 0.95**
- **Feature Importance**: Temperatur adalah indikator paling krusial
- **Monitoring Function**:

---

## 🔎 Insight & Hasil

- **Random Forest** menghasilkan akurasi 99% dan AUC 1.00 → paling ideal untuk integrasi sistem PLN.
- Model mampu meminimalkan *false alarm* dan *kesalahan deteksi*.
- **Temperatur** adalah fitur paling menentukan dalam mendeteksi gangguan.
- Fungsi `monitor_turbine()` siap digunakan di dashboard **SCADA/IIoT** atau sistem alert real-time.

---

## 📌 Catatan Tambahan

Proyek ini merupakan dummy project yang saya buat untuk menunjukkan pemahaman saya dalam membangun dashboard bisnis dan menyajikan insight berbasis data yang actionable.  
Semua nama, produk, dan data bersifat fiktif dan hanya digunakan untuk kepentingan pembelajaran.

---

## 🙏 Terima Kasih

Terima kasih telah mengunjungi proyek ini! Jika kamu punya saran, pertanyaan, atau ingin berkolaborasi, silakan hubungi saya melalui GitHub😄
