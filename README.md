# Web Prediksi Nilai Ujian Akhir

## Deskripsi
Web Prediksi Nilai Ujian Akhir adalah aplikasi web berbasis client-side yang digunakan untuk memprediksi nilai ujian akhir untuk berbagai mata pelajaran. Pengguna memasukkan nama, rata-rata nilai rapor, serta daftar mata pelajaran, lalu aplikasi akan menghasilkan nilai prediksi secara acak berdasarkan logika tertentu.

Aplikasi ini sepenuhnya menggunakan HTML, CSS, dan JavaScript tanpa backend server. Seluruh logika prediksi dijalankan di sisi browser sehingga aplikasi dapat dijalankan langsung menggunakan GitHub Pages.

---

## Fitur
- Prediksi nilai ujian untuk setiap mata pelajaran.
- Rentang nilai prediksi berdasarkan rata-rata nilai rapor:
  - Rata-rata ≥ 75 menghasilkan nilai antara 75–100.
  - Rata-rata < 75 menghasilkan nilai antara 25–74.
- Nilai prediksi konsisten untuk setiap mata pelajaran dalam satu sesi.
- Perhitungan nilai rata-rata dari seluruh mata pelajaran.
- Pesan hasil otomatis berdasarkan nilai rata-rata.
- Pesan hasil hanya dihasilkan satu kali per sesi.
- Minimal 5 mata pelajaran untuk menampilkan hasil.
- Penambahan mata pelajaran secara dinamis.
- Tampilan responsif untuk desktop dan perangkat mobile.

---

## Teknologi yang Digunakan
- HTML5
- CSS3
- JavaScript (Client-side)
- localStorage (pengganti session)

---

## Persyaratan
- Browser modern dengan JavaScript aktif
- Tidak memerlukan PHP, database, atau backend server

---

## Cara Penggunaan

1. Masukkan nama pengguna.
2. Masukkan rata-rata nilai rapor.
3. Masukkan minimal 5 mata pelajaran.
4. Klik tombol tambah untuk menambahkan mata pelajaran lainnya jika diperlukan.
5. Klik tombol **Prediksi Hasil**.
6. Lihat hasil prediksi nilai, rata-rata, dan pesan hasil.

---

## Struktur File

* `index.html` : File utama aplikasi berisi HTML, CSS, dan JavaScript.
* `CHANGELOG.md` : Riwayat perubahan proyek.
* `README.md` : Dokumentasi proyek.

---

## Logika Utama Aplikasi

### Prediksi Nilai

Nilai prediksi dihasilkan secara acak dengan rentang berikut:

* Jika rata-rata nilai rapor ≥ 75, maka nilai berada pada rentang 75–100.
* Jika rata-rata nilai rapor < 75, maka nilai berada pada rentang 25–74.

Nilai disimpan menggunakan `localStorage` agar tetap konsisten selama sesi berlangsung.

---

### Perhitungan Nilai Rata-rata

Rata-rata nilai dihitung dari seluruh mata pelajaran yang diprediksi dan digunakan untuk menentukan pesan hasil.

---

## Kustomisasi

* Pesan hasil dapat diubah pada array `successMessages` dan `errorMessages` di dalam file `index.html`.
* Tampilan dapat disesuaikan melalui bagian `<style>` di dalam file HTML.
* Logika prediksi dapat dimodifikasi langsung pada script JavaScript jika diperlukan.
