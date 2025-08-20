# Market Segmentation using Autoencoders

## Deskripsi Proyek
Proyek ini bertujuan untuk melakukan segmentasi pelanggan menggunakan algoritma clustering K-Means yang diterapkan pada data pelanggan yang telah direduksi dimensinya menggunakan Autoencoder. Data yang digunakan adalah `Marketing_data.csv`, yang berisi berbagai fitur terkait perilaku pembelian dan penggunaan layanan kredit pelanggan.

## Dataset
Dataset `Marketing_data.csv` berisi 18 fitur yang mencakup informasi seperti saldo, frekuensi saldo, jenis pembelian (satu kali dan cicilan), uang muka tunai, frekuensi pembelian, frekuensi uang muka tunai, jumlah transaksi pembelian dan uang muka tunai, limit kredit, pembayaran, pembayaran minimum, persentase pembayaran penuh, dan tenor.

## Metode
Proyek ini menggunakan langkah-langkah berikut:
1.  **Memuat dan Memahami Data:** Memuat dataset dan melakukan eksplorasi awal untuk memahami struktur data, missing values, dan distribusi fitur.
2.  **Pra-pemrosesan Data:** Menangani missing values dengan mengisi dengan nilai mean, dan menghapus kolom identitas pelanggan (`CUST_ID`). Data kemudian diskalakan menggunakan `StandardScaler`.
3.  **Penentuan Jumlah Cluster Optimal (Metode Elbow):** Menerapkan metode elbow pada data yang diskalakan untuk menentukan jumlah cluster yang optimal.
4.  **Penerapan K-Means:** Menerapkan algoritma K-Means dengan jumlah cluster yang ditentukan.
5.  **Visualisasi Cluster (PCA):** Mengurangi dimensi data menggunakan PCA untuk memvisualisasikan cluster dalam ruang 2D.
6.  **Penerapan Autoencoder:** Membangun dan melatih model Autoencoder untuk reduksi dimensi.
7.  **Penentuan Jumlah Cluster Optimal (Metode Elbow dengan Autoencoder):** Menerapkan metode elbow pada data yang telah direduksi dimensinya oleh Autoencoder untuk menentukan jumlah cluster yang optimal.
8.  **Penerapan K-Means dengan Autoencoder:** Menerapkan algoritma K-Means pada data yang direduksi dimensinya oleh Autoencoder.
9.  **Visualisasi Cluster (PCA dengan Autoencoder):** Mengurangi dimensi data yang direduksi oleh Autoencoder menggunakan PCA untuk memvisualisasikan cluster.
10. **Analisis Hasil:** Menganalisis karakteristik masing-masing cluster yang dihasilkan dari K-Means pada data yang direduksi dimensinya oleh Autoencoder.

## Hasil
Proyek ini menghasilkan 4 cluster pelanggan yang karakteristiknya dijelaskan dalam analisis hasil. Visualisasi cluster menggunakan PCA menunjukkan pemisahan cluster yang lebih jelas setelah reduksi dimensi menggunakan Autoencoder dibandingkan dengan hanya menggunakan PCA pada data yang diskalakan.
