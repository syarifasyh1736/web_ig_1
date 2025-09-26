# Instagram Profile Page - Bootstrap 5 Grid

## 📌 Deskripsi

Proyek ini adalah implementasi halaman profil Instagram responsif menggunakan Bootstrap 5. Fokus utamanya adalah penggunaan **Bootstrap Grid System** (container → row → col) beserta fitur lanjutan seperti breakpoints, order, offset, dan nesting.

## 📂 Struktur Folder

## 🚀 Cara Build/Run

1. Clone/download repository.
2. Buka file `index.html` di browser.
3. Pastikan folder `assets/img/` berisi gambar yang digunakan.

## 📦 Dependencies

- [Bootstrap 5](https://getbootstrap.com) (CDN)
- Custom CSS opsional

---

## ❓ Pertanyaan README

### 1. Mengapa memilih konfigurasi col tertentu untuk tiap breakpoint?

Karena kebutuhan **responsif** berbeda:

- Mobile → layar sempit, jadi hanya **1 kolom**.
- Tablet → layar sedang, **2–3 kolom**.
- Desktop → layar lebar, **4–6 kolom**.

### 2. Bagaimana memastikan tombol Follow/Edit Profile tetap mudah dijangkau di mobile?

Menggunakan kombinasi **utility classes Bootstrap** seperti `order-*` dan `d-flex flex-wrap`.

- Di mobile, tombol ditampilkan bertumpuk agar mudah ditekan.
- Di desktop, tombol berdampingan untuk efisiensi ruang.

### 3. Jika postingan bertambah jadi 50, apa potensi masalah grid dan bagaimana solusinya?

Masalah: loading berat, tampilan memanjang.  
Solusi: gunakan **pagination**, **lazy loading**, atau **infinite scroll** + optimasi gambar (thumbnail).

---

## 👨‍💻 Kontributor

Nama Lengkap - NIM  
Mata Kuliah: [Nama Mata Kuliah]  
Dosen Pengampu: [Nama Dosen]
