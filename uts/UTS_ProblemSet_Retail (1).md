# UTS AI & Big Data: Problem Set 1 - Customer Segmentation

## Deskripsi Kasus
Anda berperan sebagai Data Scientist di sebuah perusahaan e-commerce. Anda diminta untuk mengelompokkan pelanggan berdasarkan perilaku belanja mereka untuk strategi pemasaran yang lebih personal.
**Dataset**: [E-commerce Customer Behavior Dataset](https://www.kaggle.com/datasets/uom190346a/e-commerce-customer-behavior-dataset)

## Subtask 1: EDA & Data Preparation
1. **Data Cleaning**: Identifikasi *missing values* dan *outliers* pada fitur `Total Spend`. Gunakan Z-Score atau IQR untuk menentukan apakah *outlier* tersebut adalah pelanggan VIP atau data error. (10)
2. **Feature Engineering**: Buat fitur `Purchase_Intensity` yang menggambarkan seberapa impulsif, atau seberapa banyak pembelian yang dilakukan, bila relatif terhadap hari terakhir pembelian. Jika `Days Since Last Purchase` adalah 0, gunakan nilai 1 untuk menghindari pembagian dengan nol. (20)
3. **Standardization**: Terapkan `StandardScaler` pada fitur numerik (`Age`, `Total Spend`, `Items Purchased`, `Average Rating`, `Days Since Last Purchase`). Jelaskan mengapa ini krusial sebelum masuk ke clustering. (15)

## Subtask 2: Unsupervised Learning
1. **K-Means**: Tentukan jumlah klaster (K) menggunakan *Elbow Method*, lalu, visualisasikan klaster. (15)
2. **DBSCAN**: Tentukan parameter `eps` dan `min_samples`. Identifikasi berapa banyak pelanggan yang terdeteksi sebagai *noise* (outlier). (15)
3. **Analisis Kritis**: Bandingkan hasil segmentasi. Manakah yang lebih efektif untuk menentukan target promosi diskon? Mengapa? (25)
