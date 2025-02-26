# Menyimpan dan Mengirim Perubahan ke GitHub

Git adalah sistem kontrol versi yang banyak digunakan untuk mengelola proyek perangkat lunak. Berikut adalah langkah-langkah dasar untuk menyimpan dan mengunggah perubahan ke repository GitHub.

## Langkah-langkah

### 1. Menambahkan Perubahan ke Staging Area
```bash
git add .
```
Perintah ini akan menambahkan semua perubahan yang telah dibuat dalam direktori kerja ke staging area. Jika ingin menambahkan file tertentu, gunakan:
```bash
git add nama_file
```

### 2. Membuat Commit
```bash
git commit -m "belajar-javascript-dasar-hari2-commit2"
```
Commit digunakan untuk menyimpan perubahan secara lokal dengan pesan deskriptif. Pastikan mengganti `"belajar-javascript-dasar-hari2-commit2"` dengan pesan yang lebih jelas mengenai perubahan yang dilakukan.

### 3. Mengunggah Perubahan ke Repository Remote
```bash
git push -u origin main
```
Perintah ini mengirimkan commit ke repository GitHub pada branch `main`. Jika menggunakan branch lain, gantilah `main` dengan nama branch yang sesuai.

## Perintah Tambahan

### Melihat Status Repository
```bash
git status
```
Perintah ini menampilkan informasi tentang perubahan yang belum di-commit dan status file dalam repository.

### Melihat Log Commit
```bash
git log --oneline
```
Menampilkan daftar commit dalam format singkat untuk memudahkan tracking perubahan.

### Mengambil Perubahan dari Remote Repository
```bash
git pull origin main
```
Digunakan untuk mengambil update terbaru dari branch `main` di repository remote dan menyelaraskannya dengan lokal.

Dengan memahami perintah-perintah dasar ini, Anda bisa lebih efisien dalam mengelola proyek menggunakan Git. 🚀

