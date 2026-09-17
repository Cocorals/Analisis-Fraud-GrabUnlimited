# Analisis-Fraud-GrabUnlimited
Analisis data berbasis Python untuk mendeteksi Fraud penggunaan diskon GrabUnlimited pada paltform GrabFood, serta pengembangan dalam menurunkan Cancelation Rate.

## Deskripsi Proyek
Proyek ini menganalisis pola penyalahgunaan (*fraud*) pada program diskon **GrabUnlimited** di layanan **GrabFood**, dan berfokus untuk mendeteksi bagaimana oknum memanfaatkan celah promosi secara ilegal, yang berdampak pada kerugian finansial perusahaan, hingga *driver* organik yang terdampak pada *cancelation rate*.

Tujuan utama dari proyek ini adalah memberikan rekomendasi berbasis data untuk memperketat keamanan sistem promosi, tanpa mengganggu kenyamanan pengguna organik. Serta, melindungi *driver* organik dari cancelation yang sering merugikan.

---

## Kebutuhan Data & Perangkat

### 1. Data yang digunakan
* **grab_food_orders.csv** : Sebagai dataset utama dalam analisis data
* **grab_users.csv** & **grab_merchants.csv** : Sebagai dataset pendukung

### 2. Perangkat
* Jupyter notebook
* Language: python
* Library: numpy, pandas, matplotlib.pyplot, seaborn, scipy.stats


## Ringkasan Analisis & Dampak Bisnis

### 1. Ringkasan Analisis Data
Pengolahan data transaksi GrabFood menunjukkan temuan utama meliputi:
* **Indikasi Fraud:** Ditemukan sebanyak 9603 baris dengan data `completed_time` yang mendahului `driver_arrived_time`.
* **Dugaan Fraudster memiliki banyak akun:** Tidak ditemukan tendensi/pola transaksi signifikan dari `user_id` maupun `merchant_id`, tetapi fraud tetap terjadi.
* **Cancelation Rate:** Banyak terjadi pembatalan transaksi yang dikarenakan Resto Tutup & Resto Tidak Ditemukan.

### 2. Dampak bagi Bisnis
Analisis ini menghasilkan rekomendasi konkret yang membantu perusahaan secara efektif:
* **Mencegah Kebocoran Dana:** Membantu perusahaan memetakan dan menghentikan terjadinya lagi subsidi diskon yang salah sasaran, sehingga anggaran promosi bisa lebih tepat.
* **Penyempurnaan Sistem Keamanan:** Memberikan masukan data kepada tim teknis & *stakeholder* untuk memperbarui aturan pembatasan / pemblokiran otomatis, verifikasi fisik pada merchant secara berkala, memperketat persyaratan menjadi mitra & member GrabUnlimited.
* **Menjaga Integritas Mitra Driver:** Membantu mendeteksi & memetakan restoran fiktif/lalai, sehingga menurunkan *Cancelation Rate* akibat Resto Tutup & Resto Tidak Ditemukan.

---
