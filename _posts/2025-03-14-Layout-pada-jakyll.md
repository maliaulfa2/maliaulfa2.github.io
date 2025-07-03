---
layout: post
title: Layout Pada Jakyll
---

Layout di Jekyll adalah template HTML yang digunakan untuk membungkus konten dari halaman atau postingan.

1. apa itu layout di jakyll?

    Layout di Jekyll adalah template HTML yang digunakan untuk membungkus konten dari halaman atau postingan.
    layout disimpan di folder _layouts/

2. MENGGUNAKAN LAYOUT DI POSTINGAN

    File Markdown di folder _posts/ wajib punya front matter, dan kamu bisa tentukan layout-nya
    <pre>
        <code>    ---
            layout: post
            title: "Belajar Jekyll"
            date: 2025-07-03
            ---

            Ini isi konten blog saya.
        </code>
    </pre>        

    Berarti, kontennya akan dibungkus oleh layouts/post.html.

3. MENGGUNAKAN LAYOUT DI HALAMAN (PAGE)

    Misalnya kamu punya halaman about.md:

    <pre>
        <code>
            ---
            layout: default
            title: Tentang Saya
            ---

            # Halo!
            Saya seorang pelajar yang sedang belajar Jekyll.
        </code>
    </pre>

    Berarti isi file ini akan dibungkus oleh layouts/default.html.


Jadi baik post maupun halaman bisa pakai layout — tinggal kamu atur di bagian --- paling atas (front matter).



