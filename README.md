# 📘 Laporan Tugas Version Control dengan Git

> **username:** anotherzar  
> **NIM:** 012  
> **Repository:** [tugas-version-control](https://github.com/anotherzar/tugas-version-control)  

---

## 📋 Deskripsi Tugas

Melakukan pengelolaan versi proyek menggunakan **Git** dan **GitHub**, mencakup pembuatan commit bertahap, manajemen branch, merge, serta sinkronisasi ke remote repository.

---

## 🗂️ Struktur File Proyek

```
tugas-git/
├── index.html   → Struktur halaman web
├── style.css    → Styling tampilan
└── main.js      → Logika / skrip interaktif
```

---

## ⚙️ Tech Stack

| Teknologi                                                                                                | Kategori          | Kegunaan                          |
| -------------------------------------------------------------------------------------------------------- | ----------------- | --------------------------------- |
| ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)                | Frontend          | Struktur dan konten halaman web   |
| ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)                   | Frontend          | Styling dan tampilan visual       |
| ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black) | Frontend          | Logika interaktif dan skrip       |
| ![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)                      | Version Control   | Manajemen versi kode secara lokal |
| ![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)             | Remote Repository | Hosting dan kolaborasi kode       |

### 🔧 Tools yang Digunakan

- **Git**: Version control system untuk tracking perubahan kode
- **GitHub**: Platform remote repository dan kolaborasi
- **PowerShell**: Terminal untuk menjalankan perintah Git di Windows
- **VS Code**: Code editor untuk menulis `index.html`, `style.css`, dan `main.js`

---

## 🔄 Alur Pengerjaan

### 1️⃣ Inisialisasi & Commit Pertama

```bash
git add .
git commit -m "menambahkan file html tugas Bu Malisa"
```

> ✅ Membuat commit pertama dengan 1 file (`index.html`) — 29 baris kode ditambahkan.

---

### 2️⃣ Modifikasi File HTML

```bash
git add .
git commit -m "mengubah title html"
```

> ✅ Mengubah judul (title) pada file `index.html` (1 baris diubah).

---

### 3️⃣ Menambahkan File CSS

```bash
git add .
git commit -m "menambahkan styling"
```

> ✅ Menambahkan file `style.css` dengan 65 baris styling.

---

### 4️⃣ Menambahkan File JavaScript

```bash
git add .
git commit -m "menambahkan skrip"
```

> ✅ Menambahkan file `main.js` dengan 86 baris logika / skrip.

---

### 5️⃣ Rename Branch ke `main`

```bash
git branch -M main
```

> ✅ Mengganti nama branch default dari `master` menjadi `main`.

---

### 6️⃣ Membuat Branch `dev`

```bash
git checkout -b dev
```

> ✅ Membuat dan berpindah ke branch baru bernama `dev` untuk keperluan pengembangan.

---

### 7️⃣ Commit di Branch `dev`

```bash
git add .
git commit -m "mengubah html untuk development"
```

> ✅ Melakukan perubahan pada `index.html` khusus untuk versi development.

---

### 8️⃣ Merge Branch `dev` ke `main`

```bash
git checkout main
git merge dev
```

> ✅ Kembali ke branch `main` dan menggabungkan perubahan dari `dev`.  
> Mode merge: **Fast-forward** (1 file berubah, 17 baris dihapus).

---

### 9️⃣ Menambahkan Remote Repository

```bash
git remote add origin https://github.com/anotherzar/tugas-version-control.git
git remote -v
```

> ✅ Menghubungkan repository lokal ke GitHub.

```
origin  https://github.com/anotherzar/tugas-version-control.git (fetch)
origin  https://github.com/anotherzar/tugas-version-control.git (push)
```

---

### 🔟 Push Branch `main` ke Remote

```bash
git push -u origin main
```

> ✅ Mengunggah seluruh commit ke GitHub (15 objek, 2.77 KiB).  
> Branch `main` sekarang melacak `origin/main`.

---

### 1️⃣1️⃣ Push Branch `dev` ke Remote

```bash
git checkout dev
git push -u origin dev
```

> ✅ Branch `dev` berhasil dikirim ke GitHub.  
> Branch `dev` sekarang melacak `origin/dev`.

---

## 📊 Ringkasan Commit History

| #   | Pesan Commit                          | Branch | File Terdampak     |
| --- | ------------------------------------- | ------ | ------------------ |
| 1   | menambahkan file html tugas Bu Malisa | master | `index.html` (+29) |
| 2   | mengubah title html                   | master | `index.html` (~1)  |
| 3   | menambahkan styling                   | master | `style.css` (+65)  |
| 4   | menambahkan skrip                     | master | `main.js` (+86)    |
| 5   | mengubah html untuk development       | dev    | `index.html` (-17) |

---

## 🌿 Manajemen Branch

```
main  ──●──●──●──●──────●  (merge dari dev)
                          ↑
dev   ────────────────────●  (push ke origin/dev)
```

| Branch | Status  | Remote Tracking |
| ------ | ------- | --------------- |
| `main` | ✅ Aktif | `origin/main`   |
| `dev`  | ✅ Aktif | `origin/dev`    |

---

## 🔗 Link Repository

|              | Link                                                                                               |
| ------------ | -------------------------------------------------------------------------------------------------- |
| 🐙 Repository | [github.com/anotherzar/tugas-version-control](https://github.com/anotherzar/tugas-version-control) |