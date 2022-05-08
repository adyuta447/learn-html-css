# Latihan Membuat Berkas CSS

Sekarang coba tika latihan beberapa styling dasar pada halaman profil yang sudah kita buat dari beberapa materi sebelumnya. Latihan pada kali ini akana mencakup tahapan seperti pembuatan berkas CSS, menuliskan <i>rule</i> pada berkas CSS, hingga menghubungkan berkas CSS dengan HTML. Silahkan buka kembali project yang telah kita buat dan buka folder <b>assets</b>. Jika anda baru / langsung loncat ke materi ini langsung saja download projectnya di [disini](https://www.mediafire.com/file/5oljx5cowiqqdh4/WebDasar.zip/).

<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/4.%20Pengenalan%20CSS/img/Screenshot%202022-05-07%20105105.png" alt="screenshot">
</p>

Jika kita sudah selesai mengikuti latihan pada beberapa materi sebelumnya, maka di dalam folder <b>assets</b> akan terdapat folder <i>image</i>. Sekarang, mari kita coba tambahkan folder baru dan beri dengan nama <b>styles</b>.

<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/4.%20Pengenalan%20CSS/img/Screenshot%202022-05-08%20044114.png" alt="screenshot">
</p>

Folder styles ini akan kita gunakan untuk menyimpakn berkas CSS. Maka selahkan buka folder tersebut dan buat berkas baru dan beri nama <b>style.css</b>.

<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/4.%20Pengenalan%20CSS/img/Screenshot%202022-05-08%20050025.png" alt="screenshot">
</p>

Kita bisa coba tuliskan sebuah rule styling pada beberapa elemen HTML yang ada pada latihan sebelumnya. Yang pertama, kita tetapkan font 'sans-serif'  sebagai font yang digunakan pada seluruh elemen yang ada di dalam ```<body>```. Silahkan buka berkas <b>style.css</b> yang sudah kita buat dan tuliskan kode berikut:

```css
body {
    font-family: sans-serif;
}
```

Kemudian, kita tetapkan juga warna pada setiap elemen ```<h2>``` dan ```<h3>``` yang digunakan pada berkas HTML dengan menuliskan kode sebagai berikut:

```css
h2 {
   color: #00a2c6
}
 
h3 {
   color: #00a2c6
}
```

Dan yang terakhir, kita coba ubah warna backgorund dan warna teks pada elemen ```<footer>```, tidak lupa beri sebuah <i>padding</i>.

```css
footer {
    padding: 20px;
    color: white;
    background-color: #00a2c6;
}
```

Sehingga seluruh kode pada <b>style.css</b> akan seperti ini:

```css
body {
    font-family: sans-serif;
}

h2 {
   color: #00a2c6
}
 
h3 {
   color: #00a2c6
}

footer {
    padding: 20px;
    color: white;
    background-color: #00a2c6;
}
```
## Menghubungkan Berkas CSS dengan HTML
Setelah kita menuliskan <i>rules</i> pada berkas style.css, kita perlu menghubungkan berkas tersebut dengan berkas HTML sebagai <i>stylesheet</i> agar elemen HTML yang ditampilkan dapat menerapkan rules CSS yang kita terapkan. Buka kembali berkas <b>index.html</b>, kemudian tambahkan kode berikut di dalam elemen ```<head>```:

```html
<link rel="stylesheet" href="assets/styles/style.css">
```

Sehingga keseluruhan kode pada elemen ```<head>``akan nampak seperti ini:

```html
<head>
    <title>Kota Yogyakarta</title>
    <link rel="stylesheet" href="assets/styles/style.css">
</head>
```

Kemudian save perubahan pada berkas index.html, kemudian coba buka berkas tersebut menggunakan browser.