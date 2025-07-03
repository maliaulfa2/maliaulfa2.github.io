---
layout: post
title: Membuat Web Dengan Jekyll serve
---

Jekyll adalah static site generator (pembuat situs statis) yang sering digunakan dengan GitHub Pages. Jekyll mengubah file Markdown, HTML, dan konfigurasi menjadi website statis yang siap digunakan.

# Struktur Proyek Jekyll
.
├── _config.yml         ← File konfigurasi utama
├── _posts/             ← Folder untuk posting blog (format: YYYY-MM-DD-nama.md)
├── _layouts/           ← Template layout (HTML)
├── _includes/          ← Komponen HTML yang bisa disisipkan
├── index.md / index.html
└── assets/             ← Gambar, CSS, JS, dll


# Langkah-Langkah Membuat Web dengan jekyll
1. Install Ruby dan Jekyll
    -Install Ruby dari https://rubyinstaller.org
    -Buka terminal (cmd atau PowerShell) ketik:
            gem install jekyll bundler

2. Membuat Proyek Baru Jekyll
    masih diterminal ketik:
            jekyll new nama-proyek-ku
            cd nama-proyek-ku

3. Jalankan Server Jekyll
    masih diterminal ketik:
            bundle exec jekyll serve

    setelah itu buka browser ke:
            http://localhost:4000
            
4. Struktur Dasar File index.md / index.html
    index.md:
        ---
        layout: default
        title: Halaman Utama
        ---

        # Selamat Datang di Web Saya!
        Ini adalah halaman yang dibuat dengan Jekyll.

    _layouts/default.html:
        <!DOCTYPE html>
        <html>
        <head>
            <meta charset="UTF-8">
            <title>{{ page.title }}</title>
        </head>
        <body>
            {{ content }}
        </body>
        </html>

5. Edit File _config.yml
    title: Web Jekyll Saya
    description: Ini adalah deskripsi web saya
    author: Naila
    theme: minima

Kamu bisa mengubah tema, menambah link, atau membuat halaman blog otomatis dari file Markdown.

# Tips Tambahan
- Untuk mengatur blog, buat file di folder _posts/:
    2025-07-03-selamat-datang.md

- Isi file markdown-nya:
    ---
    layout: post
    title: "Selamat Datang"
    ---

    Ini adalah posting blog pertamaku!

- Jalankan ulang jekyll serve jika ada perubahan besar di file config.

# Deploy ke GitHub Pages
1. Push ke repo GitHub.
2. Aktifkan GitHub Pages di Settings → Pages.
3. Jika pakai GitHub Pages, jekyll akan otomatis dibangun oleh GitHub.

