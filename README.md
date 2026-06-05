# Postes-Kelompok-6-PrakAlprog-2026
# 🏠 Dashboard Analisis Data Housing

## Deskripsi Proyek

Proyek ini merupakan implementasi analisis data menggunakan Python terhadap dataset harga rumah (*Housing Dataset*). Analisis dilakukan menggunakan library Pandas untuk pengolahan data dan Matplotlib untuk visualisasi.

Program menghasilkan sebuah dashboard interaktif yang terdiri dari empat visualisasi utama untuk memberikan gambaran mengenai karakteristik dan distribusi harga rumah berdasarkan beberapa variabel pada dataset.

---

## Tujuan Proyek

- Mengolah dan menganalisis data harga rumah menggunakan Python.
- Menampilkan informasi statistik dalam bentuk visualisasi yang mudah dipahami.
- Menganalisis hubungan antara jumlah lantai, jumlah ruangan, dan harga rumah.
- Mengelompokkan harga rumah ke dalam kategori tertentu berdasarkan distribusi data.
- Menyajikan hasil analisis dalam bentuk dashboard yang informatif.

---

## Dataset

Dataset yang digunakan adalah **Housing Dataset** yang berisi data karakteristik rumah dan harga jualnya.

### Deskripsi Atribut

| Kolom | Deskripsi |
|---------|---------|
| price | Harga rumah |
| area | Luas rumah |
| bedrooms | Jumlah kamar tidur |
| bathrooms | Jumlah kamar mandi |
| stories | Jumlah lantai rumah |
| mainroad | Akses ke jalan utama |
| guestroom | Ketersediaan ruang tamu |
| basement | Ketersediaan basement |
| hotwaterheating | Ketersediaan pemanas air |
| airconditioning | Ketersediaan AC |
| parking | Jumlah tempat parkir |
| prefarea | Lokasi pada area favorit |
| furnishingstatus | Status furnitur rumah |

Dataset terdiri dari **545 data** dengan **13 atribut** yang digunakan untuk melakukan analisis terhadap karakteristik dan harga rumah.

---

## Analisis yang Dilakukan

### 1. Standar Deviasi Harga Rumah Berdasarkan Jumlah Lantai

Program menghitung standar deviasi harga rumah pada setiap kategori jumlah lantai (*stories*).

Tujuan:
- Mengetahui tingkat variasi harga rumah pada setiap kelompok jumlah lantai.
- Mengidentifikasi kategori rumah yang memiliki penyebaran harga terbesar.

Visualisasi:
- Bar Chart

---

### 2. Sebaran Rumah Berdasarkan Jumlah Lantai

Grafik menunjukkan jumlah rumah yang memiliki luas bangunan di atas rata-rata dan harga di bawah rata-rata, kemudian dikelompokkan berdasarkan jumlah lantai.

Tujuan:
- Mengidentifikasi rumah yang memiliki nilai ekonomis lebih baik.
- Mengetahui distribusi rumah berdasarkan jumlah lantai.

Visualisasi:
- Bar Chart

---

### 3. Pengaruh Total Ruangan terhadap Harga Rumah

Program membuat variabel baru:

```python
total_rooms = bedrooms + bathrooms
```

Kemudian dilakukan analisis hubungan antara total ruangan dengan harga rumah.

Tujuan:
- Mengetahui hubungan antara jumlah ruangan dan harga rumah.
- Mengamati pola kenaikan harga berdasarkan jumlah ruangan.

Visualisasi:
- Scatter Plot

---

### 4. Distribusi Harga Rumah Berdasarkan Kuantil

Harga rumah dibagi menjadi tiga kategori menggunakan metode kuantil:

| Kategori | Keterangan |
|-----------|-----------|
| Murah | 33,33% harga terendah |
| Sedang | 33,33% harga menengah |
| Mewah | 33,33% harga tertinggi |

Tujuan:
- Mengetahui proporsi rumah pada setiap kategori harga.
- Mempermudah interpretasi distribusi harga rumah.

Visualisasi:
- Pie Chart

---

## Teknologi yang Digunakan

- Python
- Pandas
- Matplotlib
- CSV Dataset

---

## Kontribusi Anggota Tim

Proyek ini dikerjakan secara kolaboratif oleh seluruh anggota tim dengan pembagian tugas sebagai berikut:

| Nama | Peran | Deskripsi Tanggung Jawab |
|------|------|--------------------------|
| **Aqil** | Programmer & Data Analyst | Mengembangkan program menggunakan Python, melakukan pengolahan dan analisis data, serta membuat visualisasi yang digunakan dalam dashboard analisis housing. |
| **Kian** | Infographic Designer | Mendesain dan menyusun infografis berdasarkan hasil analisis data agar informasi dapat disampaikan secara efektif dan mudah dipahami. |
| **Nadya** | LinkedIn Content Designer | Mengembangkan desain infografis yang dioptimalkan untuk publikasi di LinkedIn serta membantu penyajian hasil proyek kepada audiens profesional. |
| **Ryva** | GitHub Repository Manager | Mengelola repositori GitHub proyek, mengorganisasi struktur file, mengunggah dokumentasi dan source code, serta memastikan seluruh komponen proyek terdokumentasi dengan baik. |

---

## Struktur Proyek

```text
├── Kelas C_Housing.csv
├── housing_dashboard.py
├── README.md
└── hasil_visualisasi.png
```

---

## Cara Menjalankan Program

### 1. Install Library

```bash
pip install pandas matplotlib
```

### 2. Jalankan Program

```bash
python housing_dashboard.py
```

### 3. Hasil Program

Program akan menampilkan dashboard analisis yang terdiri dari:

- Grafik standar deviasi harga rumah berdasarkan jumlah lantai.
- Grafik sebaran rumah berdasarkan jumlah lantai.
- Scatter plot hubungan total ruangan dan harga rumah.
- Pie chart distribusi kategori harga rumah.

---

## Hasil Visualisasi

Dashboard disusun dalam format 2×2 yang menampilkan empat visualisasi berbeda untuk membantu memahami pola dan karakteristik data housing secara lebih komprehensif.

---

## Kesimpulan

Program berhasil mengolah dan memvisualisasikan data housing melalui empat jenis analisis yang berbeda. Hasil visualisasi menunjukkan variasi harga rumah berdasarkan jumlah lantai, distribusi rumah berdasarkan karakteristik tertentu, hubungan antara jumlah ruangan dan harga rumah, serta persebaran kategori harga rumah. Dashboard yang dihasilkan mampu menyajikan informasi secara ringkas, informatif, dan mudah dipahami sehingga dapat digunakan sebagai media analisis data yang efektif.
