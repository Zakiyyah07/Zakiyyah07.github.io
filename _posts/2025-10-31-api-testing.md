---
title: 6. API Testing
date: 2025-10-31
categories: [Artikel, Software Testing and Quality Assurance]
tags: [Artikel]
image:
  path: assets/img/post/article/api_testing_illustration.png
  alt: api Testing Thumbnail
---

# API Testing

---

## 1. Apa Itu API Testing?

API Testing adalah kegiatan pengujian pada **Application Programming Interface (API)** dengan tujuan memverifikasi bahwa:

* API berfungsi sesuai dengan spesifikasi yang ditetapkan.
* API mampu mengelola berbagai skenario input dan output secara tepat.
* API memberikan hasil yang sesuai saat menerima input tertentu.

Sasaran utamanya adalah memelihara kualitas, keandalan, serta keamanan sistem yang memanfaatkan API.

---

## 2. Keunggulan API Testing

* Memverifikasi bahwa fungsi API sesuai spesifikasi dan menghasilkan output yang akurat.
* Meningkatkan keandalan sistem melalui deteksi bug di tahap awal.
* Melindungi API dari akses tidak terotorisasi dan potensi celah keamanan.
* Mengevaluasi performa API dalam kondisi beban tertentu.
* Mempercepat siklus pengembangan melalui pengujian otomatis.
* Menjadi fondasi krusial untuk integrasi antarsistem.

---

## 3. Tools API Testing

### a. Postman

**Alasan penggunaan:**

* Memiliki antarmuka yang ramah pengguna (user-friendly)
* Mendukung beragam metode HTTP (GET, POST, PUT, DELETE, dan lainnya)
* Mendukung autentikasi, environment, serta variabel
* Mendukung otomatisasi pengujian dan dokumentasi API

**Fitur utama Postman:**

* Mengirim permintaan HTTP
* Mengelola environment
* Pengujian otomatis
* Collection dan dokumentasi API
* Mock server serta monitoring

**Contoh Request di Postman:**

```http
GET https://api.example.com/users
Authorization: Bearer <token>
```

**Contoh Response:**

```json
{
  "status": "success",
  "data": [
    {"id": 1, "name": "John Doe"},
    {"id": 2, "name": "Jane Doe"}
  ]
}
```

---

### b. SOAPUI

**Kelebihan:**

* Mendukung pengujian SOAP maupun REST API.
* Dapat dimanfaatkan untuk functional, security, dan load testing.
* Mendukung data-driven testing (pengambilan data dari Excel atau database).
* Ideal untuk pengujian enterprise dengan skenario yang kompleks.

---

## 4. Anatomi Request & Response API

### Anatomi Request

Request merupakan **permintaan dari client ke server** untuk mengakses atau memanipulasi data.

| Komponen | Deskripsi |
| ------------------ | ------------------------------------------------------ |
| Method (HTTP Verb) | Tipe aksi: `GET`, `POST`, `PUT`, `DELETE`              |
| URL | Alamat sumber daya yang akan diakses                   |
| Header             | Informasi tambahan, seperti otorisasi atau tipe data   |
| Body               | Data yang dikirimkan (umumnya dalam `POST` atau `PUT`) |

**Contoh:**

```http
POST https://api.example.com/users
Content-Type: application/json

{
  "name": "Alice",
  "email": "alice@example.com"
}
```

---

### Anatomi Response

Response merupakan **jawaban dari server** setelah memproses permintaan.

| Komponen    | Deskripsi                                                                    |
| ----------- | ---------------------------------------------------------------------------- |
| Status Code | Kode hasil eksekusi, misalnya: `200 OK`, `404 Not Found`, `401 Unauthorized` |
| Headers     | Informasi tambahan dari server                                               |
| Body        | Konten respon berupa data, umumnya dalam format JSON atau XML                |

**Contoh:**

```json
{
  "status": "success",
  "message": "User created successfully"
}
```

---

## 5. Kesimpulan

API Testing merupakan langkah vital dalam pengembangan perangkat lunak modern. Dengan memanfaatkan tools seperti **Postman** dan **SOAPUI**, pengujian dapat dilaksanakan secara efisien untuk menjamin kualitas, performa, dan keamanan API yang digunakan dalam aplikasi.

---