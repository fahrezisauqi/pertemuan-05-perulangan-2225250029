# Pertemuan 05 Perulangan Python

**Nama:** Fahrezi Sauqi Alghani
**NIM:** 2225250029
**Kelas:** 3E
**Mata Kuliah:** Algoritma dan Pemrograman, S1 Pendidikan Matematika FKIP Untirta
**Dosen Pengampu:** Dr. Aan Hendrayana, S.Si., M.Pd.

## Tujuan

Menggunakan perulangan `for` dan `while` untuk menyelesaikan masalah iteratif, menelusuri perubahan nilai variabel (tracing), menguji kondisi berhenti, serta mengumpulkan hasil kerja melalui Git dan GitHub.

## Struktur Repositori

```
pertemuan-05-perulangan-NIM/
|-- README.md
|-- .gitignore
|-- latihan/
|   |-- 01_tabel_perkalian.py
|   |-- 02_jumlah_bilangan.py
|   |-- 03_validasi_input.py
|   `-- 04_hitung_genap.py
`-- kuis/
    `-- kuis2_deret_aritmetika.py
```

## Cara Menjalankan

Buka folder proyek di VS Code, lalu jalankan dari terminal di root folder.
Pada Windows gunakan `python`; pada macOS/Linux gunakan `python3`.

```bash
python3 latihan/01_tabel_perkalian.py
python3 latihan/02_jumlah_bilangan.py
python3 latihan/03_validasi_input.py
python3 latihan/04_hitung_genap.py
python3 kuis/kuis2_deret_aritmetika.py
```

## Algoritma Kuis 2

Program menerima suku pertama `a`, beda `d`, dan banyak suku `n`, lalu menampilkan `n` suku pertama deret aritmetika dan jumlahnya tanpa memakai rumus jumlah deret.

1. Baca `a` dan `d` sebagai `float`.
2. Baca `n` sebagai `int`. Selama `n <= 0`, tampilkan pesan dan minta `n` lagi (`while`, karena jumlah pengulangan input tidak diketahui sejak awal).
3. Set `total = 0` **sebelum** loop supaya tidak ter-reset pada setiap iterasi.
4. Ulangi `for i in range(n)`, yaitu tepat `n` kali (i = 0 sampai n - 1).
5. Di setiap iterasi: hitung `suku = a + i * d`, tambahkan ke `total`, lalu tampilkan nomor suku dan nilainya.
6. Setelah loop selesai, tampilkan `total` dengan dua angka di belakang koma.

> Catatan: tulis ulang langkah di atas dengan bahasa Anda sendiri sebelum dikumpulkan.

## Hasil Pengujian

### Kuis 2: Deret Aritmetika

| No | Input (a, d, n) | Keluaran yang diharapkan | Keluaran aktual | Status |
|----|-----------------|--------------------------|-----------------|--------|
| 1 | 2, 3, 5 | Suku: 2, 5, 8, 11, 14; Jumlah = 40.00 | ... | ... |
| 2 | 10, -2, 4 | Suku: 10, 8, 6, 4; Jumlah = 28.00 | ... | ... |
| 3 | 1.5, 0.5, 3 | Suku: 1.50, 2.00, 2.50; Jumlah = 6.00 | ... | ... |
| 4 | 2, 3, lalu n = 0, -2, 5 | Menolak 0 dan -2, lalu menerima 5; Jumlah = 40.00 | ... | ... |

### Latihan

| Latihan | Input | Keluaran yang diharapkan | Keluaran aktual | Status |
|---------|-------|--------------------------|-----------------|--------|
| 1 Tabel perkalian | n = 4 | 4 x 1 = 4 sampai 4 x 10 = 40 (10 baris) | ... | ... |
| 1 Tabel perkalian | n = -3 | -3 x 1 = -3 sampai -3 x 10 = -30 (10 baris) | ... | ... |
| 2 Jumlah 1 sampai n | n = 1 | Jumlah = 1 | ... | ... |
| 2 Jumlah 1 sampai n | n = 5 | Jumlah = 15 | ... | ... |
| 2 Jumlah 1 sampai n | n = 10 | Jumlah = 55 | ... | ... |
| 3 Validasi input | 120, -5, 75 | Menolak 120 dan -5, lalu menerima 75 | ... | ... |
| 4 Bilangan genap | n = 1 | 0 | ... | ... |
| 4 Bilangan genap | n = 2 | 1 | ... | ... |
| 4 Bilangan genap | n = 5 | 2 | ... | ... |
| 4 Bilangan genap | n = 10 | 5 | ... | ... |

## Tracing Singkat (Kuis 2, test case 1: a = 2, d = 3, n = 5)

| Iterasi | i | suku | total sebelum | total sesudah |
|---------|---|------|---------------|---------------|
| 1 | 0 | 2 | 0 | 2 |
| 2 | 1 | 5 | 2 | 7 |
| 3 | 2 | 8 | 7 | 15 |
| 4 | 3 | 11 | 15 | 26 |
| 5 | 4 | 14 | 26 | 40 |

Loop berhenti setelah `i = 4` karena `range(5)` tidak menghasilkan nilai 5.

## Refleksi

Tuliskan satu kesalahan perulangan yang Anda temukan saat mengerjakan (misalnya batas `range` kurang satu, `total = 0` salah tempat, atau lupa memperbarui variabel pada `while`), bagaimana Anda menemukannya (tracing atau breakpoint), dan bagaimana Anda memperbaikinya.

...

## Sumber dan Bantuan

Cantumkan sumber atau bantuan yang memengaruhi solusi (dokumentasi Python, VS Code, GitHub Docs, diskusi dengan teman, atau alat bantu lain) secara jujur.

- ...
-
