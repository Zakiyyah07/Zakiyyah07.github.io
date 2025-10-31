---
title: 1. Strategi Testing
date: 2025-10-31
categories: [Artikel, Software Testing and Quality Assurance]
tags: [Artikel]
image:
  path: assets/img/post/article/test_strategy_illustration.png
  alt: Strategy Testing Thumbnail
---

# Testing Strategi
---

## 1. Pengertian Testing
Testing adalah kegiatan untuk mengevaluasi perangkat lunak dengan tujuan menemukan kesalahan (*bug*) dan memastikan sistem memenuhi kebutuhan fungsional maupun non-fungsional.  
Fokus utama pengujian adalah menjaga mutu perangkat lunak, memperkuat keamanan, memastikan pengalaman pengguna yang baik, serta menekan biaya perbaikan di kemudian hari.

| **Aspek**             | **Penjelasan**                                                                 |
|------------------------|--------------------------------------------------------------------------------|
| **Tujuan Testing**     | Mendeteksi bug dan memastikan sistem bekerja sesuai persyaratan.              |
| **Manfaat**            | Meminimalkan risiko kegagalan, meningkatkan kepercayaan pemangku kepentingan, serta efisiensi biaya. |
| **Hasil Akhir**        | Produk perangkat lunak yang berkualitas, aman, stabil, dan sesuai kebutuhan pengguna.    |

---

## 2. Software Testing Life Cycle (STLC)
STLC adalah rangkaian tahapan terstruktur yang digunakan untuk memastikan kualitas perangkat lunak secara konsisten.

| **Tahap**                       | **Deskripsi**                                                                  | **Hasil Utama**                            |
|---------------------------------|--------------------------------------------------------------------------------|--------------------------------------------|
| **1. Test Planning**            | Menetapkan strategi, jadwal, anggaran, lingkungan, dan pembagian peran pengujian. | Dokumen rencana pengujian.                |
| **2. Test Design**              | Menyusun *test case*, menyiapkan data uji, dan merancang skenario pengujian.     | Kumpulan test case & RTM (*Requirement Traceability Matrix*). |
| **3. Test Execution**           | Melaksanakan pengujian pada tingkat unit, integrasi, sistem, dan acceptance.     | Hasil pelaksanaan pengujian.              |
| **4. Test Reporting & Analysis**| Mengevaluasi hasil pengujian, mencatat bug, dan memberikan rekomendasi perbaikan. | Laporan hasil pengujian dan rekomendasi.  |

---

## 3. Jenis Pengujian Berdasarkan Abstraksi

| **Jenis Testing**     | **Tujuan**                                                | **Contoh**                                      |
|------------------------|-----------------------------------------------------------|-------------------------------------------------|
| **Unit Testing**       | Memverifikasi fungsi atau metode individual agar output sesuai harapan.      | Menguji fungsi perhitungan diskon.              |
| **Integration Testing**| Memastikan integrasi dan aliran data antar modul berjalan semestinya.        | Modul login yang terhubung dengan modul profil. |
| **System Testing**     | Menguji keseluruhan sistem terhadap spesifikasi yang ditetapkan.           | Pengujian aplikasi e-commerce untuk skenario 1000 pengguna. |
| **Acceptance Testing** | Validasi akhir oleh pengguna atau klien sebelum rilis produk.              | Persetujuan klien sebelum peluncuran aplikasi.  |

---

## 4. Jenis Pengujian Berdasarkan Fungsi

| **Jenis**               | **Fokus**                                      | **Contoh**                                   | **Tujuan**                               |
|--------------------------|------------------------------------------------|-----------------------------------------------|-------------------------------------------|
| **Fungsional Testing**   | Menguji fitur utama untuk memastikan sesuai kebutuhan. | Login, reset password, pembayaran online.     | Memastikan fungsi bekerja dengan benar.    |
| **Non-Fungsional Testing**| Menguji aspek seperti performa, keamanan, dan keandalan. | Uji beban saat flash sale, pengukuran waktu respon. | Menilai kualitas dan ketahanan sistem.   |

---

## 5. Jenis Pengujian Berdasarkan Domain

| **Jenis Testing**      | **Fokus**                              | **Contoh**                                      | **Tujuan**                                      |
|-------------------------|-----------------------------------------|-------------------------------------------------|-------------------------------------------------|
| **Performance Testing** | Mengukur kinerja dan stabilitas di bawah beban. | Menguji situs web saat lonjakan traffic.           | Menjamin respons dan kestabilan sistem.         |
| **Security Testing**    | Mencari dan menutup celah keamanan.     | Pengujian terhadap serangan SQL injection, XSS.   | Melindungi data pengguna dan integritas sistem. |
| **Usability Testing**   | Menilai kemudahan penggunaan oleh pengguna. | Evaluasi navigasi dan elemen antarmuka.           | Memastikan pengalaman pengguna intuitif.        |

---

## 6. Jenis Pengujian Berdasarkan Struktur

| **Jenis Testing**     | **Penjelasan**                                                  | **Kelebihan**                                         | **Kekurangan**                                       |
|------------------------|----------------------------------------------------------------|--------------------------------------------------------|------------------------------------------------------|
| **Black-Box Testing**  | Penguji tidak melihat struktur internal, hanya mengevaluasi input–output. | Mudah dilakukan dan merepresentasikan perspektif pengguna. | Sulit mendeteksi cacat pada logika internal.         |
| **White-Box Testing**  | Penguji memahami struktur kode dan logika internal program.     | Mampu menemukan bug tersembunyi dan meningkatkan kualitas kode. | Memerlukan waktu lebih banyak dan keahlian teknis.   |

---

## 7. Pelaporan & Analisis Testing
Setelah pengujian dilaksanakan, hasil dianalisis untuk menilai kualitas sistem dan menentukan langkah perbaikan yang diperlukan.

| **Komponen**         | **Isi Pelaporan**                                                                 |
|-----------------------|-----------------------------------------------------------------------------------|
| **Ringkasan Hasil**   | Jumlah test case yang lulus, gagal, atau belum dijalankan.                       |
| **Evaluasi Kualitas** | Penilaian apakah sistem memenuhi spesifikasi fungsional dan non-fungsional.      |
| **Identifikasi Bug**  | Klasifikasi kesalahan, tingkat keparahan, dan status perbaikannya.              |
| **Rekomendasi**       | Usulan perbaikan untuk performa, keamanan, dan stabilitas.                      |
| **Analitik & Grafik** | Visualisasi tren pengujian seperti jumlah bug dan rasio keberhasilan dari waktu ke waktu. |

---

## 8. Kesimpulan
Pengujian adalah langkah penting dalam SDLC (Software Development Life Cycle) yang memastikan perangkat lunak memenuhi standar kualitas, aman, dan andal sebelum digunakan oleh pengguna.  
Dengan penerapan pengujian yang tepat, tim pengembang dapat:

- Mengurangi risiko dan menekan biaya perbaikan pada tahap akhir,  
- Menjamin performa dan keamanan sistem,  
- Meningkatkan kepuasan serta kepercayaan pengguna.

| **Aspek Utama**        | **Dampak**                                                |
|-------------------------|-----------------------------------------------------------|
| **Kualitas Produk**     | Perangkat lunak menjadi lebih stabil, aman, dan minim bug. |
| **Kepercayaan Pengguna**| Meningkatkan kepuasan dan loyalitas pengguna.             |
| **Efisiensi Proyek**    | Waktu perbaikan lebih singkat dan biaya lebih terkendali. |