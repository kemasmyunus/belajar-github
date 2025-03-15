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
Perintah ini mengirimkan commit ke repository GitHub pada branch `main`. Jika menggunakan branch lain, gantilah `main` dengan nama branch yang sesuai. Opsi `-u` digunakan untuk menetapkan branch upstream, sehingga pada push berikutnya cukup menggunakan `git push`.

## Perintah Tambahan

### Melihat Status Repository
```bash
git status
```
Perintah ini menampilkan informasi tentang perubahan yang belum di-commit dan status file dalam repository. Ini membantu Anda untuk melihat apa yang telah diubah dan apa yang masih perlu di-commit.

### Melihat Log Commit
```bash
git log --oneline
```
Menampilkan daftar commit dalam format singkat untuk memudahkan tracking perubahan. Setiap commit ditampilkan dalam satu baris dengan hash commit dan pesan commit.

### Mengambil Perubahan dari Remote Repository
```bash
git pull origin main
```
Digunakan untuk mengambil update terbaru dari branch `main` di repository remote dan menyelaraskannya dengan lokal. Ini memastikan bahwa Anda memiliki versi terbaru dari kode sebelum melakukan perubahan lebih lanjut.

## Perintah Lanjutan

### Membuat Branch Baru
```bash
git checkout -b nama-branch
```
Perintah ini digunakan untuk membuat branch baru dan langsung berpindah ke branch tersebut. Gantilah `nama-branch` dengan nama branch yang diinginkan.

### Menggabungkan Branch
```bash
git merge nama-branch
```
Digunakan untuk menggabungkan perubahan dari branch lain ke branch saat ini. Pastikan Anda berada di branch yang ingin digabungkan, lalu gantilah `nama-branch` dengan nama branch yang akan digabungkan.

### Menghapus Branch
```bash
git branch -d nama-branch
```
Perintah ini menghapus branch yang sudah tidak diperlukan. Gantilah `nama-branch` dengan nama branch yang ingin dihapus. Gunakan opsi `-D` untuk memaksa penghapusan branch yang belum di-merge.

### Melihat Daftar Branch
```bash
git branch
```
Menampilkan daftar semua branch yang ada di repository lokal. Branch yang aktif akan ditandai dengan tanda bintang (*).

### Membatalkan Perubahan di Staging Area
```bash
git reset nama_file
```
Perintah ini digunakan untuk menghapus file dari staging area, sehingga perubahan pada file tersebut tidak akan di-commit. Gantilah `nama_file` dengan nama file yang ingin dihapus dari staging area.

## Materi Tambahan

### Menghapus File dari Repository
```bash
git rm nama_file
```
Perintah ini digunakan untuk menghapus file dari repository dan staging area. Gantilah `nama_file` dengan nama file yang ingin dihapus.

### Mengembalikan File ke Keadaan Sebelumnya
```bash
git checkout -- nama_file
```
Perintah ini digunakan untuk mengembalikan file yang telah diubah ke keadaan sebelumnya (sebelum diubah). Gantilah `nama_file` dengan nama file yang ingin dikembalikan.

### Melihat Perbedaan Antar Commit
```bash
git diff commit1 commit2
```
Perintah ini digunakan untuk melihat perbedaan antara dua commit. Gantilah `commit1` dan `commit2` dengan hash commit yang ingin dibandingkan.

### Mengubah Pesan Commit Terakhir
```bash
git commit --amend -m "pesan-commit-baru"
```
Perintah ini digunakan untuk mengubah pesan commit terakhir. Gantilah `"pesan-commit-baru"` dengan pesan commit yang baru.

### Menghapus Commit Terakhir
```bash
git reset --hard HEAD~1
```
Perintah ini digunakan untuk menghapus commit terakhir dan mengembalikan repository ke keadaan sebelum commit tersebut.

### Membuat Tag
```bash
git tag -a v1.0 -m "versi 1.0"
```
Perintah ini digunakan untuk membuat tag dengan nama `v1.0` dan pesan "versi 1.0". Tag digunakan untuk menandai titik penting dalam sejarah proyek.

### Menghapus Tag
```bash
git tag -d v1.0
```
Perintah ini digunakan untuk menghapus tag dengan nama `v1.0`.

### Mengunggah Tag ke Remote
```bash
git push origin v1.0
```
Perintah ini digunakan untuk mengunggah tag `v1.0` ke repository remote.

