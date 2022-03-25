# Mengorganisasikan konten pada Halaman Profil

Kita sudah mengenal beberapa elemen yang digunakan untuk mengorganisasikan halaman, seperti ```<header>```,```<footer>```,```<article>```, dan yang lainnya. Dan juga kita sudah mengenal generic elemen yang digunakan untuk mengelompokkan elemen secara umum. Sekarang saatnya kita mengorganisasikan pada halaman profil yang sudah kita buat sebelumnya.

Sebelum mengorganisasikan konten mari kita tambahkan sebuah konten untuk diterapkan pada elemen ```<aside>``` nantinya. Unduh terlebih dahulu aset gambar yang akan digunakan pada tautan berikut: 

https://seeklogo.com/images/D/Daerah_Istimewa_Jogjakarta-logo-19A73BFE95-seeklogo.com.png

Simpanlah gambar tersebut pada folder assets -> images dan beri nama Jogja-badge.png

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-25_19-58.png)

Kemudian tuliskan konten berikut di dalam elemen ```<body>``` (tuliskan tepat sebelum penutup tag ```</body>```).

```html
<body>

    .......

    <h1>Yogyakarta</h1>
    <p>Kota Yogyakarta adalah ibu kota dan pusat pemerintahan Daerah Istimewa Yogyakarta, Indonesia.</p> 
    <figure>
        <img src="assets/images/Jogja-badge.png" alt="">
        <figcaption>Lambang</figcaption>
    </figure>


</body>
```

Tuliskan juga konten copyright berikut tepat setelah tag penutup ```</figure>```.

```html
<body>

.......

   </figure>
   <p>Belajar desain website bersama K0oceng</p>
</body>

```

Setelah menambahkan beberapa konten tersebut, mari saatnya kita organisasikan konten-konten yang ada agar dapat tercipta struktur halaman yang baik.

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-25_20-57.png)