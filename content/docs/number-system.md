---
title: "Sistem Bilangan"
weight: 3
---

# Jenis-jenis Sistem Angka

Dalam dunia ilmu komputer dan elektronika digital, **sistem bilangan** (atau sistem angka) adalah cara kita mewakili dan menuliskan nilai matematika. Jika manusia terbiasa menghitung dengan 10 jari, komputer memiliki cara yang berbeda untuk memproses dan menyimpan angka. 

Setiap sistem bilangan memiliki **Basis** (atau *Radix*), yaitu jumlah digit atau simbol unik yang digunakan dalam sistem tersebut sebelum angkanya berulang. Berikut adalah penjelasan lengkap mengenai jenis-jenis sistem angka yang paling sering digunakan.

---

## Desimal (Basis 10)

Sistem bilangan **Desimal** adalah sistem angka yang paling umum dan kita gunakan setiap hari. Sistem ini disebut Basis 10 karena menggunakan 10 simbol angka yang berbeda.

* **Digit yang digunakan:** 0, 1, 2, 3, 4, 5, 6, 7, 8, dan 9.
* **Cara kerja:** Setiap posisi digit dalam bilangan desimal mewakili kelipatan 10 (satuan, puluhan, ratusan, ribuan, dst). Semakin ke kiri, nilainya semakin besar.

**Contoh Pemahaman:**
Angka desimal 256 (basis 10) dapat diuraikan secara matematis sebagai berikut:
* 256 = (2 x 100) + (5 x 10) + (6 x 1)
* 256 = 200 + 50 + 6

---

## Biner (Basis 2)

Sistem bilangan **Biner** adalah bahasa dasar dari semua komputer dan perangkat digital. Komputer menggunakan sinyal listrik yang hanya memiliki dua keadaan: hidup (arus mengalir) atau mati (tidak ada arus). Oleh karena itu, sistem ini hanya menggunakan 2 simbol.

* **Digit yang digunakan:** 0 dan 1. (Setiap digit biner disebut sebagai **Bit** atau *Binary Digit*).
* **Cara kerja:** Setiap posisi digit mewakili kelipatan 2 (1, 2, 4, 8, 16, 32, dst dari kanan ke kiri).

**Contoh Pemahaman:**
Angka biner 1010 (basis 2) jika dikonversi menjadi desimal adalah:
* 1010 = (1 x 8) + (0 x 4) + (1 x 2) + (0 x 1)
* 1010 = 8 + 0 + 2 + 0 
* Hasil = 10 (basis 10)
Jadi, biner `1010` sama dengan desimal `10`.

---

## Heksadesimal (Basis 16)

Membaca angka biner yang sangat panjang (misalnya `1101001110110101`) sangat menyulitkan dan rentan terhadap kesalahan manusia. Di sinilah **Heksadesimal** (sering disingkat *Hex*) berperan. Sistem ini digunakan oleh programmer untuk meringkas angka biner agar lebih mudah dibaca, seperti pada pengalamatan memori komputer atau kode warna (contoh: `#FF5733`).

Karena membutuhkan 16 simbol tetapi angka standar hanya ada 10 (0-9), sistem ini meminjam enam huruf pertama dari alfabet.

* **Digit yang digunakan:** 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, dan F.
    * *Catatan:* A = 10, B = 11, C = 12, D = 13, E = 14, F = 15.
* **Cara kerja:** Satu digit heksadesimal secara tepat mewakili **4 bit** dari angka biner. Ini membuatnya sangat efisien untuk merangkum biner.

**Contoh Pemahaman:**
Angka heksadesimal 1A (basis 16) jika dikonversi menjadi desimal:
* 1A = (1 x 16) + (10 x 1)
* 1A = 16 + 10 
* Hasil = 26 (basis 10)

---

## Tabel Perbandingan dan Konversi

Untuk mempermudah pemahaman konversi antar sistem angka, berikut adalah tabel perbandingan nilai dari angka 0 hingga 15 dalam sistem Desimal, Biner, dan Heksadesimal.

| Desimal| Biner | Heksadesimal | Penjelasan |
| :---: | :---: | :---: | :--- |
| **0** | `0000` | **0** | Titik awal semua sistem bilangan. |
| **1** | `0001` | **1** | |
| **2** | `0010` | **2** | Biner bergeser ke kiri (nilai 2). |
| **3** | `0011` | **3** | |
| **4** | `0100` | **4** | Nilai biner posisi ketiga adalah 4. |
| **5** | `0101` | **5** | |
| **6** | `0110` | **6** | |
| **7** | `0111` | **7** | |
| **8** | `1000` | **8** | Nilai biner posisi keempat adalah 8. |
| **9** | `1001` | **9** | Angka terakhir pada sistem desimal tunggal. |
| **10** | `1010` | **A** | **Hex mulai menggunakan huruf!** A = 10. |
| **11** | `1011` | **B** | B = 11. |
| **12** | `1100` | **C** | C = 12. |
| **13** | `1101` | **D** | D = 13. |
| **14** | `1110` | **E** | E = 14. |
| **15** | `1111` | **F** | Nilai maksimum untuk 4-bit biner (semua menyala). |

> **Tips Cepat Konversi:**
> Jika Anda memiliki angka biner yang panjang seperti `10101111`, bagilah menjadi kelompok 4-bit dari kanan: `1010` dan `1111`. 
> Lihat tabel di atas: `1010` adalah **A**, dan `1111` adalah **F**. 
> Jadi, biner `10101111` sama dengan heksadesimal **AF**. Sangat mudah, bukan?
