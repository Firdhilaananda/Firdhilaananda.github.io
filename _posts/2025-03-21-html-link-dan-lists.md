---
layout: post
title: "HTML Link dan List"
---

Penjelasan tentang Link dan List pada HTML.




### 1. HTML Link

  HTML Link digunakan untuk membuat hyperlink ke halaman lain, sintaksnya:
  ```
  <a href="URL">
  ```
  Contohnya : 
  ```
  <a href="https://www.instagram.com/firdhilas?igsh=MTFnZmNrcWZnNjI5cg==">Coba Buka</a>
  ```
  Hasilnya : <a href="https://www.instagram.com/firdhilas?igsh=MTFnZmNrcWZnNjI5cg==">Coba Buka</a>

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

### Menambahkan Link dan List ke website Friends
- Edit file index.html menjadi
```
  <h2>Berikut teman-teman saya di kelas: </h2>
  <ul>
    <li><a href ="https://lepii1.github.io/" target="blank">Ahmad Aulia Fahlevi</a></li>
    <li><a href ="https://bunga-hub.github.io/" target="blank">Bunga Alfa Zahrah</a></li>
    <li><a href ="https://devarisny.github.io" target="blank">Deva Risny</a></li>
    <li><a href ="https://firdhilaananda.github.io" target="blank">Firdhila Ananda Syahputri</a></li>
  </ul>
```
- Kemudian buat file baru dengan nama friends.md dan isi file tersebut seperti dibawah ini dengan link yang sama seperti di file index.html:
```
    # Friends page

    Berikut teman-teman saya di kelas:
    1. [Ahmad Aulia Fahlevi](https://lepii1.github.io/)
    2. [Bunga Alfa Zahrah](https://bunga-hub.github.io/)
    3. [Deva Risny](https://devarisny.github.io)
    4. [Firdhila Ananda Syahputri](https://firdhilaananda.github.io)
```
