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
Gantilah `nama_file` dengan nama file yang ingin Anda tambahkan.

### 2. Membuat Commit
```bash
git commit -m "pesan-commit"
```
Commit digunakan untuk menyimpan perubahan secara lokal dengan pesan deskriptif. Pastikan mengganti `"pesan-commit"` dengan pesan yang lebih jelas mengenai perubahan yang dilakukan. Pesan commit yang baik membantu dalam memahami sejarah perubahan proyek.

### 3. Mengunggah Perubahan ke Repository Remote
```bash
git push -u origin main
```


## Perintah Tambahan

### Melihat Status Repository
```bash
git status
```


### Melihat Log Commit
```bash
git log --oneline
```


### Mengambil Perubahan dari Remote Repository
```bash
git pull origin main
```

Dengan memahami perintah-perintah dasar ini, Anda bisa lebih efisien dalam mengelola proyek menggunakan Git. 🚀

