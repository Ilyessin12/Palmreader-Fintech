# Overview
Tugas 1 Mata Kuliah Financial Technology Kelompok 5 Prototype Palm-reader untuk Biometrik Payment Technology

## Anggota Kelompok 
- Lyan Nazhabil Dzuquwwa (2308428)
- Mochamad Zidan Rusdhiana (2305464)

## Dataset
Karena dataset yang cukup besar maka untuk dataset bisa didownload terlebih dahulu di https://www.kaggle.com/datasets/mahdieizadpanah/sapienza-university-mobile-palmprint-databasesmpd. File nanti bisa disimpan di /datasets.

## Cara Penggunaan

Seluruh alur kerja terdapat di dalam `palmreader.ipynb`.

1.  **Menambahkan Pengguna Baru (Enrollment)**
    -   Buat folder baru di dalam direktori `datasets/` dengan ID unik (misalnya `096`).
    -   Masukkan minimal 40 gambar telapak tangan pengguna tersebut ke dalam folder yang baru dibuat.

2.  **Melatih Model**
    -   Buka file `palmreader.ipynb`.
    -   Jalankan semua sel dari atas ke bawah (**Kernel > Restart & Run All**). Notebook akan secara otomatis memuat data baru, melatih model, dan menyimpan versi terbaiknya sebagai `best_palm_model.keras`.

3.  **Menguji Prototipe**
    -   Siapkan gambar uji yang tidak ada dalam dataset pelatihan.
    -   Buat subfolder di dalam `test_images/` dengan nama pengguna yang sesuai (misalnya `test_images/pengguna_baru/`).
    -   Masukkan gambar uji ke dalam subfolder tersebut.
    -   Jalankan sel terakhir di notebook (`Phase 3: Prototype Demonstration & Testing`). Sel ini akan secara otomatis menemukan gambar uji, memvisualisasikannya, dan menjalankan inferensi menggunakan model yang telah dilatih.