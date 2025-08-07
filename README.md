# 🔄 Customer Churn Analysis with Classification Models

## 📌 Project Overview

Proyek ini bertujuan untuk menganalisis dan memprediksi **churn pelanggan** menggunakan teknik **machine learning** berbasis **klasifikasi**. Churn terjadi ketika pelanggan berhenti menggunakan layanan perusahaan, dan memprediksi hal ini penting untuk strategi retensi pelanggan.

## 📂 Dataset

Dataset berisi informasi pelanggan, termasuk:
- Demografi (umur, jenis kelamin, dsb.)
- Informasi langganan
- Riwayat transaksi atau penggunaan layanan
- Status churn (target variabel: churned vs. retained)

## 🔧 Workflow & Metodologi

1. **Exploratory Data Analysis (EDA)**
   - Analisis distribusi fitur
   - Korelasi antar fitur
   - Perbandingan antara pelanggan churn dan tidak churn

2. **Data Preprocessing**
   - Handling missing values
   - Encoding variabel kategorikal
   - Feature scaling (jika diperlukan)
   - Train-test split
   - (Optional) SMOTE untuk penanganan class imbalance

3. **Modeling**
   Beberapa model klasifikasi digunakan:
   - **Logistic Regression**
   - **Random Forest Classifier**
   - **XGBoost Classifier**
   - **LightGBM Classifier**

4. **Hyperparameter Tuning**
   - Menggunakan **GridSearchCV** atau **RandomizedSearchCV** untuk optimasi model

5. **Evaluation Metrics**
   - Accuracy
   - Precision
   - Recall
   - F1-score
   - Confusion Matrix
   - ROC AUC Curve

## 📊 Insight

- Beberapa fitur seperti lama berlangganan, jumlah interaksi, atau jenis produk yang digunakan, sangat mempengaruhi kemungkinan pelanggan churn.
- Model terbaik memiliki **akurasi tinggi** dan **kemampuan generalisasi yang baik**, terutama setelah proses **SMOTE** dan **tuning hyperparameter** dilakukan.
- ROC AUC digunakan untuk menentukan threshold optimum dalam mengambil keputusan bisnis (misal: pelanggan mana yang perlu diberi penawaran retensi).

## 🧰 Tools & Libraries

- `pandas`, `numpy`, `matplotlib`, `seaborn`
- `scikit-learn`
- `xgboost`
- `lightgbm`
- `imblearn`
