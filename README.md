# Postes-Kelompok-6-PrakAlprog-2026
# 🏠 Dashboard Analisis Data Housing

## Deskripsi Proyek

Proyek ini merupakan implementasi analisis data menggunakan Python terhadap dataset harga rumah (Housing Dataset). Analisis dilakukan dengan memanfaatkan library Pandas untuk pengolahan data dan Matplotlib untuk visualisasi.

Program menghasilkan sebuah dashboard yang terdiri dari empat grafik berbeda yang bertujuan untuk memberikan gambaran mengenai karakteristik dan distribusi harga rumah berdasarkan beberapa variabel pada dataset.

---

## Tujuan Proyek

- Mengolah data housing menggunakan Python.
- Menampilkan informasi statistik dalam bentuk visualisasi.
- Menganalisis hubungan antara jumlah lantai, jumlah ruangan, dan harga rumah.
- Mengelompokkan harga rumah berdasarkan kategori harga menggunakan metode kuantil.
- Menyajikan hasil analisis dalam bentuk dashboard yang informatif.

---

## Dataset

Dataset yang digunakan adalah **Housing Dataset** yang berisi data karakteristik rumah dan harga jualnya.

### Atribut Dataset

| Kolom | Deskripsi |
|---------|---------|
| price | Harga rumah |
| area | Luas rumah |
| bedrooms | Jumlah kamar tidur |
| bathrooms | Jumlah kamar mandi |
| stories | Jumlah lantai rumah |
| mainroad | Akses jalan utama |
| guestroom | Ketersediaan ruang tamu |
| basement | Ketersediaan basement |
| hotwaterheating | Ketersediaan pemanas air |
| airconditioning | Ketersediaan AC |
| parking | Jumlah tempat parkir |
| prefarea | Lokasi pada area favorit |
| furnishingstatus | Status furnitur rumah |

Jumlah data pada dataset sebanyak **545 baris data** dengan **13 atribut utama**.

---

## Analisis yang Dilakukan

### 1. Standar Deviasi Harga Rumah Berdasarkan Jumlah Lantai

Program menghitung standar deviasi harga rumah untuk setiap kategori jumlah lantai (stories).

Tujuan analisis:
- Mengetahui tingkat variasi harga rumah pada setiap jumlah lantai.
- Mengidentifikasi kelompok rumah yang memiliki penyebaran harga terbesar.

Visualisasi:
- Bar Chart

---

### 2. Sebaran Rumah dengan Luas di Atas Rata-rata dan Harga di Bawah Rata-rata

Grafik menampilkan jumlah rumah yang memenuhi kriteria:

- Luas rumah di atas rata-rata.
- Harga rumah di bawah rata-rata.

Data kemudian dikelompokkan berdasarkan jumlah lantai.

Tujuan analisis:
- Menemukan rumah yang memiliki nilai ekonomis tinggi.
- Membandingkan distribusi rumah berdasarkan jumlah lantai.

Visualisasi:
- Bar Chart

---

### 3. Pengaruh Total Ruangan terhadap Harga Rumah

Program membuat variabel baru:

```python
total_rooms = bedrooms + bathrooms
