Analisis Kepadatan Penduduk Indonesia per Provinsi Tahun 2021

Project Overview

Proyek ini adalah bagian dari Student Development Initiative HACKTIV8 yang bertujuan untuk menganalisis data publik mengenai Kepadatan Penduduk di 34 provinsi Indonesia pada tahun 2021. Tujuannya adalah untuk memahami tingkat kepadatan dan ketimpangan persebaran penduduk, serta menggali wawasan bermakna dari data tersebut dengan bantuan AI (IBM Granite).

Proses Analisis

Proses analisis dilakukan menggunakan Google Colab, dengan memanfaatkan library Python seperti:
- Pandas untuk manipulasi dan pembersihan data.
- Matplotlib dan Seaborn untuk membuat visualisasi data.
- Model AI IBM Granite (melalui watsonx.ai) untuk memperkaya analisis.

Raw Dataset

- Sumber Data: Badan Pusat Statistik (BPS)
- Nama Dataset: Kepadatan Penduduk menurut Provinsi, 2021
- Link Dataset: https://github.com/aprillia27/Capstone-Project-Aprillia-Adinda12/blob/da9d2d3a8fe4f05ab87e283f40fdcad35ba26629/Kepadatan%20Penduduk%20menurut%20Provinsi%2C%202021.xlsx 

Insights & Findings

Berdasarkan analisis data yang dilakukan, diperoleh beberapa temuan berikut:

1. Pembersihan & Persiapan Data
- Melewatkan satu baris header tambahan pada file Excel asli agar data dapat dibaca dengan benar.
- Mengganti nama kolom menjadi `Provinsi` dan `Kepadatan` untuk mempermudah analisis.
- Mengubah tipe data kolom `Kepadatan` dari object menjadi numerik (integer).
- Menghapus baris agregat "INDONESIA" agar tidak mengganggu skala visualisasi dan perbandingan antar provinsi.

2. Temuan Utama (Peringkat Kepadatan Penduduk)
- 5 Provinsi dengan Kepadatan Tertinggi (jiwa per km²):
  1. DKI Jakarta - 15.978
  2. Jawa Barat - 1.379
  3. Banten - 1.248
  4. DI Yogyakarta - 1.155
  5. Jawa Tengah - 1.120
- 5 Provinsi dengan Kepadatan Terendah (jiwa per km²):
  1. Kalimantan Utara - 9
  2. Papua Barat - 10
  3. Papua - 15
  4. Kalimantan Tengah - 28
  5. Kalimantan Timur - 28

3. Pola atau Tren yang Ditemukan
- Konsentrasi Ekstrem di Pulau Jawa: Terdapat ketimpangan yang sangat signifikan, di mana 5 provinsi terpadat berada di Pulau Jawa. Kepadatan DKI Jakarta puluhan kali lipat lebih tinggi dari provinsi lainnya.
- Wilayah Luar Jawa Sangat Jarang: Provinsi di luar Jawa, terutama di Kalimantan dan Papua, memiliki tingkat kepadatan penduduk yang sangat rendah, menunjukkan luasnya wilayah yang belum tergarap secara maksimal.

AI Support Explanation

AI (Large Language Model) dari IBM Granite digunakan untuk memperkaya analisis melalui:

1.  Summarization (Peringkasan): Membuat ringkasan naratif dari temuan kunci. Contoh: "Analisis menunjukkan DKI Jakarta sebagai provinsi terpadat dengan angka 15.978 jiwa/km², sementara Kalimantan Utara menjadi yang terjarang dengan hanya 9 jiwa/km²."
2.  Classification (Klasifikasi): Mengelompokkan provinsi ke dalam kategori kepadatan untuk segmentasi, misalnya: Sangat Padat (>1000), Padat (500-1000), Sedang (100-500), dan Jarang (<100).
3.  Insight Generation (Pembuatan Wawasan Lanjutan): Mengajukan pertanyaan analitis. Contoh: "Bagaimana korelasi antara kepadatan penduduk dengan tingkat pembangunan ekonomi di setiap provinsi?"
