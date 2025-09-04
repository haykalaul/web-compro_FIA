# Female in Action (FIA) — Company Profile Website

Deskripsi singkat
-----------------
Project ini adalah website company profile untuk Female in Action (FIA) yang bergerak dalam industri perlindungan wanita dan mental health. Tujuan utama situs adalah menampilkan profil organisasi, layanan korporat, program Fiacare, berita, dan informasi kontak dengan tata letak responsif dan aset multimedia.

Latar belakang
--------------
Website dibuat untuk menyediakan identitas daring bagi FIA, memudahkan pengunjung memahami misi, layanan, dan update berita organisasi. Struktur file dan penggunaan library populer membuat situs mudah dipelihara dan dikembangkan lebih lanjut.

Teknologi & dependensi
----------------------
- HTML (struktur halaman)
- CSS (custom styles di `assets/css/main.css`)
- JavaScript (interaksi di `assets/js/main.js`)
- Vendor / library yang disertakan di `assets/vendor/`:
  - Bootstrap (grid dan utilitas)
  - AOS (animate on scroll)
  - Swiper (slider)
  - GLightbox (lightbox)
  - Isotope (layout/filtering)
  - PureCounter (hit counter)
- Assets: gambar di `assets/images/` dan `assets/img/`

Struktur proyek (ringkasan)
--------------------------
- `index.html`, `aboutus.html`, `corporate.html`, `fiacare.html`, `berita.html`
- `assets/css/` — stylesheet utama
- `assets/js/` — script utama (`main.js`)
- `assets/vendor/` — library pihak ketiga
- `assets/images/`, `assets/img/` — aset gambar
- `forms/` — endpoint PHP sederhana (`contact.php`, `newsletter.php`)

Langkah setup (lokal)
---------------------
Pilihan A — Jalankan dengan Laragon (direkomendasikan pada Windows):

1. Letakkan folder proyek di direktori web server Laragon (contoh: `C:/laragon/www/`).
2. Buka Laragon dan start Apache (atau start All).
3. Akses situs melalui browser: http://localhost/<folder-proyek>

Pilihan B — Server statis cepat (menggunakan Python, bila tidak menggunakan Laragon):

Jalankan dari root proyek (`C:/laragon/www/Fia Website`) di PowerShell:

```powershell
# masuk ke folder proyek
Set-Location -Path 'C:/laragon/www/Fia Website'

# jika menggunakan Python 3.x
python -m http.server 8000

# buka http://localhost:8000 di browser
```

Catatan untuk formulir PHP
-------------------------
Formulir kontak dan newsletter mengirim ke endpoint PHP di folder `forms/`. Untuk mengujinya secara penuh gunakan Laragon/XAMPP atau server yang sudah mengaktifkan PHP. Jika hanya membuka file via static server (Python/file://) fungsi PHP tidak akan berjalan.

Tips pengembangan & troubleshooting
----------------------------------
- Pastikan jalur relatif ke `assets/` tidak dirubah jika memindahkan file.
- Jika stylesheet atau skrip vendor tidak dimuat, periksa konsol browser (DevTools) untuk 404 dan sesuaikan path.
- Untuk perubahan cepat pada CSS, lihat `assets/css/main.css`.

Kontribusi
----------
Kami menyambut kontribusi untuk memperbaiki konten, memperbarui aset, atau menambah fitur kecil.

Cara berkontribusi singkat:

- Buka issue untuk mendiskusikan perubahan besar atau bug sebelum mengerjakan.
- Buat branch baru dari cabang utama dengan nama yang jelas, mis. `fix/header-path` atau `feat/news-filter`.
- Lakukan perubahan di branch Anda, sertakan commit message yang singkat dan jelas.
- Jika ada perubahan pada CSS/JS, sertakan keterangan singkat di PR tentang area yang terpengaruh dan cara mengetesnya.
- Buka Pull Request ke cabang utama dan tautkan issue terkait (jika ada).

Panduan singkat kualitas:

- Jaga struktur folder dan path relatif ke `assets/`.
- Beri komentar pada perubahan JS yang non-trivial.
- Untuk teks/terjemahan, pastikan konsistensi bahasa.

Pengujian lokal:

- Jalankan situs secara lokal seperti dijelaskan di atas (Laragon atau server statis) dan verifikasi halaman utama serta formulir (jika menguji PHP menggunakan Laragon/XAMPP).

Terima kasih atas kontribusinya — setiap perbaikan kecil membantu menjaga situs tetap relevan.

Lisensi & kredit
-----------------
Dokumentasi ini ditulis untuk repositori internal; tambahkan lisensi (mis. MIT) jika ingin membagikan secara publik.

Kontak
------
Untuk pertanyaan tentang repo ini, hubungi maintainer proyek atau catat issue di sistem kontrol versi yang Anda gunakan.
