---
layout: post
title: Install Jekyll dan Membuat index.html
---

Install jekyll dan membuat index.html


- Clone repository ke lokal
- Masuk ke dalam folder repository kemudian install jekyll => gem install jekyll bundler
- jalankan perintah => bundle init 
maka menghasilkan file baru dengan naman Gemfile
- Edit file Gemfile, tambahkan => gem "jekyll"
- buat file dengan nama "index.html" kemudian isi => 
#### <!DOCTYPE html>
####                <html lang="en">
####                <head>
####                    <meta charset="UTF-8">
####                    <meta name="viewport" content="width=device-width, initial-scale=1.0">
####                    <title>Document</title>
####                </head>
####                <body>
####                    
####                </body>
####                </html>
- jalankan => jekyll build
sehingga menghasilkan directory _site
- jalankan perintah => "jekyll serve" dan klik url http://localhost;4000
- jika web berhasil dibuka, edit file Gemfile.lock, tambahkan => x86_64-linux
- Kemudian push ke GitHub dengan perintah => git add .
   git commit -m "tampilan pertama"
   git push