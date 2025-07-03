---
layout: post
title: "HTML link dan list"
---

penjelasan tentang link dan list pada Html:
Dalam HTML, link (juga dikenal sebagai hyperlink) digunakan untuk menghubungkan satu halaman web ke halaman web lain, atau bahkan ke bagian lain dari halaman yang sama. Sementara list digunakan untuk menyajikan informasi dalam format terstruktur, bisa berupa daftar berurut (ordered list) atau tidak berurut (unordered list). 


Link (Hyperlink)

Link dibuat menggunakan tag <a> dengan atribut href yang menentukan URL tujuan. 

Contoh: <pre><code><a href="https://www.example.com">Klik di sini</a></code></pre> 

Ketika diklik, link akan mengarahkan pengguna ke halaman atau lokasi yang ditentukan oleh atribut href. 
Link juga bisa mengarah ke bagian lain dalam halaman yang sama, dengan menggunakan id pada elemen tujuan dan menyertakan id tersebut pada atribut href link. 

List (Daftar)

Unordered List (Daftar Tidak Berurut):

Menggunakan tag <ul> untuk memulai daftar dan tag <li> untuk setiap item dalam daftar. 
Contoh:<pre><code><ul><li>Item 1</li><li>Item 2</li></ul></code></pre> 
Item-item ini biasanya ditampilkan dengan bullet points. 

Ordered List (Daftar Berurut):

Menggunakan tag <ol> untuk memulai daftar dan tag <li> untuk setiap item.

Contoh: <pre><code><ol><li>Langkah 1</li><li>Langkah 2</li></ol><code><pre>

Item-item ini ditampilkan dengan nomor atau huruf sesuai urutan. 

Description List (Daftar Deskripsi):

Menggunakan tag <dl>, <dt> (istilah), dan <dd> (deskripsi). 

Contoh: <pre><code><dl><dt>Istilah 1</dt><dd>Deskripsi istilah 1</dd></dl><code><pre>

Contoh penggunaan:


![HTML link dan list](/assets/images/link_dan_list.png)


Dalam contoh di atas, ada sebuah link yang mengarahkan ke situs Example.com. Juga terdapat unordered list dan ordered list yang masing-masing menampilkan item dengan bullet points dan nomor urut, contoh kode ini merujuk pada kode yang dihasilkan pada contoh tersebut. 