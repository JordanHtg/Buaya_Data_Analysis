
# TRPL AI Capstone — Week 1

## Judul Proyek
Crocodile_Analyst

## Problem Statement
- **Masalah**: Lembaga konservasi internasional kekurangan analisis data terpusat untuk memahami hubungan antara karakteristik fisik buaya (panjang, berat), lokasi geografis, dan status keterancamannya. Pemahaman ini krusial untuk mengarahkan sumber daya konservasi secara efektif.
- **Pengguna**: Peneliti biologi, manajer program konservasi, dan pembuat kebijakan lingkungan.
- **Nilai**: Proyek ini akan menyediakan dasbor analisis dan model prediktif sederhana untuk mengidentifikasi faktor-faktor kunci yang berkorelasi dengan status "Critically Endangered", membantu prioritas alokasi dana dan upaya perlindungan di lapangan.

## Scope
- In-scope: - **In-Scope**:
    - Analisis statistik deskriptif dari `crocodile_dataset.csv`.
    - Visualisasi distribusi buaya berdasarkan negara dan status konservasi.
    - Membuat model machine learning *baseline* untuk memprediksi `Conservation Status` berdasarkan fitur fisik dan geografis.
    - Menganalisis korelasi antara panjang/berat dan status konservasi.
- Out-of-scope: **Out-of-Scope**:
    - Mengumpulkan data baru dari lapangan.
    - Membangun sistem *real-time* monitoring.
    - Analisis data genetik atau citra satelit.

## Metrik & Target
- **Metrik Utama**: **F1-Score** untuk kelas 'Critically Endangered'. Karena jumlah spesies yang terancam punah jauh lebih sedikit, F1-Score memberikan gambaran yang lebih baik daripada akurasi.
- **Target**: Mencapai F1-Score di atas **0.75** untuk kelas 'Critically Endangered'.
- **Baseline**: Model klasifikasi sederhana (seperti Regresi Logistik) yang dilatih pada data, yang mungkin memiliki F1-score awal sekitar **0.50 - 0.60**.


## Data
- **Sumber**: Kaggle.com , public data -> dataset name : crocodile_dataset.csv

## Arsitektur Ringkas
![diagram](docs/matrix.png)

## Roadmap (Mingguan)
- **M1**: Analisa Masalah
- **M2**: Pencarian Dataset
- **M3**: Pembuatan
- **M4**: Dokumentasi dan laporan akhir 

## Etika & Privasi (Risiko & Mitigasi)
- **Risiko**: Data ini mengandung nama pengamat (`Observer Name`) dan lokasi geografis spesifik (`Country/Region`, `Habitat Type`). Penyalahgunaan data ini dapat membahayakan privasi individu dan memfasilitasi perburuan liar terhadap spesies yang terancam.
- **Mitigasi**: Kolom `Observer Name` akan di-hash atau dihapus dari dataset yang digunakan untuk analisis publik. Data lokasi akan diagregasi ke tingkat regional yang lebih luas saat memvisualisasikan atau membagikan hasil untuk melindungi populasi buaya dari ancaman eksternal.

### Kotak Submisi
- Tempel link GitHub dan Google Drive Anda di sini:
    - Link Repositori GitHub: https://github.com/JordanHtg/Buaya_Data_Analysis.git
    - Link Google Drive (jika ada): https://colab.research.google.com/drive/1WX-ZcpYR7qoTYUnZcSgFu-B-ej6rIJ9Y?usp=drive_link
