1. Mengapa memilih konfigurasi col- tertentu untuk tiap breakpoint?

Konfigurasi col- dipilih agar layout tetap responsif sesuai ukuran layar.

Pada layar kecil (≤576px), digunakan col-12 agar setiap postingan memenuhi lebar layar sehingga lebih mudah dilihat di perangkat mobile.

Pada layar sedang (≥768px), digunakan col-md-4 sehingga dalam satu baris bisa 2–3 postingan, menjaga keseimbangan antara ukuran gambar dan jumlah kolom.

Pada layar besar (≥992px), digunakan col-lg-3 atau col-xl-2 agar bisa menampilkan 4–6 postingan per baris.
Pendekatan ini menjaga konsistensi tampilan, keterbacaan, dan kenyamanan pengguna di berbagai perangkat.

2. Bagaimana memastikan tombol Follow/Edit Profile tetap mudah dijangkau di mobile? Jelaskan pendekatannya.

Tombol diletakkan dengan pendekatan mobile-first. Pada layar kecil, tombol ditempatkan di bawah username secara vertikal atau dalam barisan horizontal yang terpusat. Hal ini dilakukan dengan memanfaatkan kelas Bootstrap seperti d-flex, flex-wrap, dan justify-content-center. Dengan cara ini, tombol tetap terlihat jelas, tidak saling berhimpitan, dan mudah dijangkau oleh pengguna menggunakan jari.

3. Jika postingan bertambah jadi 50, apa potensi masalah dan bagaimana solusi gridmu mengatasinya?

Potensi masalah: jumlah postingan yang sangat banyak dapat membuat halaman lebih panjang, waktu muat lebih lama, dan tampilan terasa padat.
Solusi: sistem grid Bootstrap yang digunakan tetap responsif sehingga meskipun jumlah gambar bertambah, tata letaknya otomatis menyesuaikan ukuran layar tanpa merusak proporsi. Untuk mengoptimalkan performa, dapat ditambahkan fitur pagination atau lazy loading agar gambar tidak di-load sekaligus.

Penjelasan singkat:

A. struktur file
struktur project ini dibagi menjadi beberapa folder utama:

├── index.html # Halaman utama Instagram Profile
├── assets
│ ├── css
│ │ └── custom.css # File CSS tambahan untuk styling khusus
│ └── img # Kumpulan gambar profil, highlight, dan postingan
│ ├── ppp.jpg
│ ├── 1.jpg
│ ├── 2.jpg
│ ├── ...
│ └── 12.jpg

Keterangan:

1. index.html berisi struktur utama halaman (header, bio, highlights, grid postingan, footer).
2. assets/css/custom.css dipakai untuk styling tambahan di luar Bootstrap.
3. assets/img/ menyimpan seluruh gambar profil, highlight, dan postingan feed.

B. Build/Run

Tidak diperlukan proses build karena project ini berbasis HTML statis. Untuk menjalankan:

1. Unduh atau clone project ke komputer lokal.
2. Pastikan semua gambar ada di folder assets/img.
3. Buka file index.html menggunakan browser modern (misalnya Chrome, Edge, atau Firefox).
4. Halaman akan langsung tampil dengan dukungan Bootstrap dari CDN.

C. Dependensi

Project ini menggunakan dependensi berikut:

1. Bootstrap 5.3.2 (CSS & JS) → digunakan untuk sistem grid, layout responsif, dan komponen tombol.
   - CDN: https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css
2. Bootstrap Icons → digunakan untuk ikon (misalnya ikon tiga titik dan tambah orang).
   - CDN: https://cdn.jsdelivr.net/npm/bootstrap-icons/font/bootstrap-icons.css
3. Custom CSS (custom.css) → untuk styling tambahan seperti highlight, post-img, tab-menu, dan footer.
   Tidak ada dependensi tambahan yang perlu diinstal melalui package manager (seperti npm atau yarn).
