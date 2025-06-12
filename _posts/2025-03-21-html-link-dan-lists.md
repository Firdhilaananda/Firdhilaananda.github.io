---
layout: post
title: "HTML Link dan List"
---

Penjelasan tentang Link dan List pada HTML.




### 1. HTML Link
```
HTML Link digunakan untuk membuat hyperlink ke halaman lain, sintaksnya: <a href="URL">Linknya</a>
```
contohnya : <a href="https://www.instagram.com/firdhilas?igsh=MTFnZmNrcWZnNjI5cg==">Coba Buka</a>

### 2. HTML List

1. Tidak Berurutan (Unorded List)

Menggunakan <ul> dan dengan daftar item dimulai dengan <li>
Contohnya:
```
<ul>
  <li>Baju</li>
  <li>Celana</li>
  <li>Anting</li>
</ul>
```

Hasilnya: 

<ul>
  <li>Baju</li>
  <li>Celana</li>
  <li>Anting</li>
</ul>

2. Daftar Berurutan (Ordered List)

Menggunakan <ol> dan dengan daftar item dimulai dengan <li>
Contohnya:
```
<ol>
  <li>Baju</li>
  <li>Celana</li>
  <li>Anting</li>
</ol>
```
Hasilnya: 
<ol>
  <li>Baju</li>
  <li>Celana</li>
  <li>Anting</li>
</ol>

# Membuat Link dan List ke website Friends
- Edit file index.html menjadi
```
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
    </head>
    <body>
        <h1>Nama: Firdhila Ananda Syahputri</h1>
        <p>Deskripsi Diri: Saya merupakan mahasiswa semester 2 jurusan Teknologi Informasi dan Komputer prodi Teknik Informatika di Politeknik Negeri Lhokseumawe.<br> 
            Saya lahir di Lhokseumawe pada 18 Mei 2006.</p>
        <h2>Berikut teman-teman saya di kelas: </h2>
        <ul>
            <li><a href ="https://lepii1.github.io/" target="blank">Ahmad Aulia Fahlevi</a></li>
            <li><a href ="https://alvi0syahril.github.io/" target="blank">Alvi Syahril</a></li>
            <li><a href ="https://bunga-hub.github.io/" target="blank">Bunga Alfa Zahrah</a></li>
            <li><a href ="https://devarisny.github.io" target="blank">Deva Risny</a></li>
            <li><a href ="https://faizul-abrar.github.io/" target="blank">Faizul Abrar</a></li>
            <li><a href ="https://faqriyadiandika.github.io" target="blank">Faqriyadi Andika</a></li>
            <li><a href ="https://fathan-mubina.github.io/" target="blank">Fathan Mubina</a></li>
            <li><a href ="https://firdhilaananda.github.io" target="blank">Firdhila Ananda Syahputri</a></li>
        </ul>
    </body>
    </html>
```
- Kemudian buat file baru dengan nama friends.md dan isi file tersebut seperti dibawah ini dengan link yang sama seperti di file index.html:
```
    # Friends page

    Berikut teman-teman saya di kelas:
    1. [Ahmad Aulia Fahlevi](https://lepii1.github.io/)
    2. [Alvi Syahril](https://alvi0syahril.github.io/)
    3. [Bunga Alfa Zahrah](https://bunga-hub.github.io/)
    4. [Deva Risny](https://devarisny.github.io)
    5. [Faizul Abrar](https://faizul-abrar.github.io/)
    6. [Faqriyadi Andika](https://faqriyadiandika.github.io)
    7. [Fathan Mubina](https://fathan-mubina.github.io/)
    8. [Firdhila Ananda Syahputri](https://firdhilaananda.github.io)
```
