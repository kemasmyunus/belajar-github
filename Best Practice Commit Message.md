# Best Practice Commit Message (Git/GitHub)

## 1. Struktur Commit Message
Format umum:

```

<type>: <short summary>

<body>

<footer>
```

* **type** → menjelaskan jenis perubahan (mengikuti *conventional commits*).
* **short summary** → ringkas, maksimal ±50 karakter.
* **body** (opsional) → penjelasan detail perubahan, alasan, atau konteks (wrap di 72 karakter per baris).
* **footer** (opsional) → referensi issue, breaking change, atau catatan tambahan.

---

## 2. Jenis *type* yang Umum

* `feat` → fitur baru
* `fix` → perbaikan bug
* `docs` → dokumentasi
* `style` → perubahan gaya kode (spasi, format, indentasi, tanpa logika)
* `refactor` → perubahan kode tanpa mengubah perilaku
* `perf` → peningkatan performa
* `test` → menambah/ubah pengujian
* `chore` → perubahan kecil/pekerjaan rutin (update dependency, build script)

---

## 3. Contoh Commit Message

```
feat: add search bar to header

Implement a search bar with autocomplete suggestions.
This helps users quickly find products without browsing categories.

Closes #42
```

```
fix: prevent crash on empty user input

The login form was throwing an error if submitted with no data.
Now it validates the fields before making a request.
```

```
docs: update README with installation steps
```

---

## 4. Tips Tambahan

* Gunakan **imperative mood** (contoh: "add feature", bukan "added feature").
* Jangan terlalu panjang di summary (maksimal 50 karakter).
* Pisahkan *summary* dengan *body* menggunakan satu baris kosong.
* Jika ada issue/PR terkait, referensikan di footer (`Closes #123`).
* Konsisten sepanjang proyek.
