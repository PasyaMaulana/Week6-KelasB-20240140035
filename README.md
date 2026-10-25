# LugnerKart - Katalog Produk & Pendaftaran Member (Tugas Fetch API & Form DOM / Event Handling)

Dua halaman statis (HTML + CSS + JavaScript native, tanpa library) yang dihubungkan lewat navigasi.

## Tampilan Aplikasi
index.html
<img width="1919" height="1027" alt="image" src="https://github.com/user-attachments/assets/e5310638-82f0-4408-8528-4ab6aa584d8c" />
<img width="1917" height="1028" alt="image" src="https://github.com/user-attachments/assets/c651e597-208b-4fd7-945e-7c85a986b4fb" />
form.html
<img width="1920" height="1028" alt="image" src="https://github.com/user-attachments/assets/b90fce72-c7aa-480e-8ecf-0ad541dc14b5" />
<img width="1918" height="1027" alt="image" src="https://github.com/user-attachments/assets/e8e1bdf6-bd1b-4fce-a137-2454966a3193" />

## Fitur

### 1. Katalog Produk (`index.html`) - Fetch API
- Mengambil data dari `https://dummyjson.com/products` dengan `fetch()`.
- Menampilkan nama, harga, kategori, dan gambar produk lewat DOM.
- Status **loading** saat data diambil, pesan **error** + tombol "Coba lagi" bila gagal.
- Cek `response.ok` agar status 404/500 juga dianggap error.
- Pencarian produk (nama / kategori) memakai event `input`.

### 2. Pendaftaran Member (`form.html`) - DOM & Event Handling
- Kolom: nama, email, password, konfirmasi password, minat, persetujuan.
- Event: `input`, `blur`, `change`, `click`, `submit`, `reset`.
- Validasi langsung saat mengetik, pesan error muncul di bawah kolom.
- Indikator kekuatan password, tombol tampilkan/sembunyikan password.
- Hasil pendaftaran tampil dinamis sebagai kartu ringkasan.

| Kolom | Aturan |
|---|---|
| Nama | wajib, minimal 3 karakter, hanya huruf dan spasi |
| Email | wajib, format email valid |
| Password | wajib, minimal 8 karakter, mengandung huruf dan angka |
| Konfirmasi | wajib, sama dengan password |
| Persetujuan | wajib dicentang |

## Struktur Folder

```
tugas-fetch-form/
├── index.html
├── form.html
├── css/
│   ├── style.css
│   └── form.css
├── js/
│   ├── products.js
│   └── form.js
├── assets/
│   ├── favicon.svg
└── README.md
```

## Cara Menjalankan

Buka `index.html` di browser. Halaman produk membutuhkan koneksi internet.
