# 📑 Notes App

Note Apps adalah proyek backend sederhana menggunakan **Hapi.js** yang dibuat sebagai bagian dari latihan kelas **Belajar Belajar Back-End Pemula dengan JavaScript** di Dicoding.

API ini memungkinkan pengguna untuk:
- Menambahkan note
- Melihat seluruh note
- Melihat detail note
- Mengubah data note
- Menghapus note

## 🚀 Teknologi yang Digunakan

- [Node.js](https://nodejs.org/)
- [Hapi.js](https://hapi.dev/)
- [ESLint](https://eslint.org/) + [eslint-config-dicodingacademy](https://www.npmjs.com/package/eslint-config-dicodingacademy)
- [NanoID](https://github.com/ai/nanoid) — untuk generate ID unik

## 🗂️ Struktur Direktori

```
📁 NOTE-APPS-DICODING
├── 📁 notes-app-backend
│   ├── 📁 src
│       ├── handler.js
│       ├── notes.js
│       ├── routes.js
│       └── server.js
│   ├── .gitignore
│   ├── .eslintrc.config.mjs
│   ├── package-lock.json
│   └── package.json
├── 📁 notes-app-frontend-1
└── README.md
```

## 📌 Cara Menjalankan Aplikasi

### 1. Clone repositori

```bash
git clone https://github.com/kandikaprima/note-apps-dicoding.git
cd NOTE-APPS-DICODING
```

### 2. Install dependencies

```bash
npm install
```

### 3. Jalankan server

```bash
npm run start
```

Server akan berjalan pada: `http://localhost:5000`

---

## ⚙️ Endpoint API

### ✅ Menambahkan Note
- **Method:** POST  
- **URL:** `/notes`

**Request Body:**
```json
{
 "title": "Judul Catatan",
 "tags": ["Tag 1", "Tag 2"],
 "body": "Konten catatan"
}
```

### ✅ Mendapatkan Semua Note
- **Method:** GET  
- **URL:** `/notes`

### ✅ Mendapatkan Note berdasarkan ID
- **Method:** GET  
- **URL:** `/notes/{id}`

### ✅ Mengubah Note berdasarkan ID
- **Method:** PUT  
- **URL:** `/notes/{id}`

### ✅ Menghapus Note berdasarkan ID
- **Method:** DELETE  
- **URL:** `/notes/{id}`

---

## ✅ ESLint & Style Guide

Proyek ini menggunakan ESLint dengan konfigurasi `eslint-config-dicodingacademy` agar gaya penulisan kode lebih konsisten.

- Jalankan ESLint:
```bash
npm run lint
```
---
