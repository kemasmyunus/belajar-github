
# Jenis Commit Message (Conventional/Angular Style)

## 1. Type yang Umum
- **feat** → menambahkan fitur baru  
  Contoh: `feat: add search bar in header`

- **fix** → memperbaiki bug  
  Contoh: `fix: prevent crash on empty user input`

- **docs** → perubahan dokumentasi  
  Contoh: `docs: update README with setup steps`

- **style** → perubahan gaya kode tanpa memengaruhi logika  
  (misalnya format, indentasi, spasi, tanda baca)  
  Contoh: `style: format code with Prettier`

- **refactor** → merapikan atau restrukturisasi kode tanpa mengubah perilaku  
  Contoh: `refactor: simplify authentication logic`

- **perf** → perbaikan performa  
  Contoh: `perf: optimize image rendering`

- **test** → menambah atau memperbarui pengujian  
  Contoh: `test: add unit tests for login service`

- **chore** → tugas rutin yang tidak memengaruhi kode produksi  
  (misalnya update dependency, konfigurasi build, tool dev)  
  Contoh: `chore: update dependencies`

---

## 2. Type Tambahan (Tetap Standar, Walau Jarang Dipakai)

- **build** → perubahan pada sistem build atau dependency eksternal  
  Contoh: `build: update webpack config for production`

- **ci** → perubahan terkait *continuous integration* (GitHub Actions, Travis, dsb.)  
  Contoh: `ci: fix GitHub Actions node version`

- **revert** → membatalkan commit sebelumnya  
  Contoh:  
```

revert: "feat: add search bar"

```

- **BREAKING CHANGE** → dipakai jika ada perubahan besar yang tidak kompatibel ke belakang  
Biasanya ditulis di body/footer commit.  
Contoh:  
```

feat: upgrade API to v2

BREAKING CHANGE: old endpoints /v1/\* are no longer supported.

```

- **build(deps)** *(dari Angular style)* → spesifik menandakan update dependency  
Contoh: `build(deps): bump axios from 0.19.2 to 0.21.1`

- **ci(lint)** *(dari Angular style)* → memperjelas ruang lingkup perubahan di pipeline/CI  
Contoh: `ci(lint): add ESLint check in GitHub Actions`

---

## Catatan (Angular Style)
- Angular guideline memakai format:  
```

<type>(<scope>): <short summary>

```
- **scope** → bagian aplikasi yang terpengaruh (opsional).  
- Contoh:  
- `feat(auth): add JWT authentication`  
- `fix(ui): align button text properly`  
