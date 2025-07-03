---
layout: post
title: Belajar Buat Post
---

membuat post di website statis menggunakan Jekyll dan Markdown — cocok untuk kamu yang sedang mengembangkan website di GitHub Pages seperti maliaulfa2.github.io.


#  Struktur Post Jekyll

    - Untuk membuat sebuah post blog di Jekyll, kamu perlu:

    - Menaruh file di folder: _posts

    - Menggunakan format nama file: YYYY-MM-DD-nama-post.md

        Contoh: 2025-07-03-halo-dunia.md 


# Isi File Post (Markdown)

File post ditulis menggunakan Markdown (.md) dengan bagian atas disebut Front Matter (---).

Contoh Satu Post

<pre>
    <code>
        ---
        layout: post
        title: "Halo Dunia!"
        date: 2025-07-03 20:00:00 +0700
        categories: [blog, personal]
        ---

        Ini adalah post pertama saya di blog ini.  
        Saya sedang belajar membuat web menggunakan **Jekyll dan GitHub Pages**!

        Terima kasih telah membaca. 😊
    </code>
</pre>

Penjelasan:

    layout: post → menggunakan template khusus postingan

    title: → judul artikel

    date: → tanggal dan waktu terbit

    categories: → tag/kelompok (bisa satu atau lebih)


# Menampilkan Post di Web

Pastikan di file index.html atau default.html ada bagian seperti ini:

<pre>
    <code>
        {% for post in site.posts %}
        <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
        <p>{{ post.date | date: "%d %B %Y" }}</p>
        <p>{{ post.excerpt }}</p>
        {% endfor %}
    </code>
</pre>

# Cara Cek Hasil Post

    - Jalankan: jekyll serve

    - Akses di browser: http://localhost:4000

    - Atau lihat langsung di GitHub Pages:
        https://maliaulfa2.github.io

# Markdown Singkat

    - # Judul Besar

    -  Subjudul

    - **teks tebal**

    - *teks miring*

    - [link](https://example.com)

    - ![gambar](path/gambar.jpg)