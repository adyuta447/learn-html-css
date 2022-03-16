# Praktik Menerapkan Anchor pada Navigasi Halaman Profile

Pada praktik [sebelumnya](https://github.com/adyuta447/learn-html-css/tree/main/3.%20Pendalaman%20HTML/5.%20Praktik%20Menambah%20List%20pada%20Halaman%20Profile) sudah ada sebuah list sebagai navigasi. Namun demikian, karena belum ada elemen anchor ```<a>```, maka navigasi tersebut belum dapat kita gunakan. Oleh karena itu, mari kita tambahkan elemen anchor pada tiap item <i>list</i>-nya.

Silahkan buka kembali berkas <b>index.html</b> pada <i>teks editor</i>. Tambahkan elemen anchor di setiap item <i>list</i>.

```html
<ul>
    <li><a href="#">Sejarah</a></li>
    <li><a href="#">Geografis</a></li>
    <li><a href="#">Wisata</a></li>
</ul>
 
```

Setelah menambahkan elemen <i>anchor</i> pada item <i>list</i>, maka tampilan item list akan nampak menjadi <i>hyperlink</i>.

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-16_22-18.png)

Namun ketika salah satu item dipilih, tidak akan terjadi apa apa, Itu karena pada atribut ```<href>``` kita belum menetapkan sebuah target. Nilai <i>href</i> dapat berupa sebuah URL untuk mengarahkan ke sebuah halaman yang berbeda. Selain itu juga berupa tanda pagar (#) diikuti dengan id elemen untuk mengarahkan tampilan pada elemen sesuai id yang ditentukan (masih dalam satu halaman).

Maka dari itu, mari kita berikan atribut ```<id>``` pada sebuah elemen yang akan menjadi target navigasi. Berikan atribut ```<id>``` pada seluruh elemen ```<h2>``` dengan id sesuai dengan kontennya.

```html
<body>
--------
   <ul>
       <li><a href="#">Sejarah</a></li>
       <li><a href="#">Geografis</a></li>
       <li><a href="#">Wisata</a></li>
   </ul>
   <h2 id="sejarah">Sejarah</h2>
--------
 
   <h2 id="geografis">Geografis</h2>
--------
 
   <h2 id="wisata">Wisata</h2>
--------
</body>
```
Kemudian tuliskan juga id elemen target setelah pagar (#) pada tiap elemen <i>anchor</i> yang terdapat pada item <i>list</i>

```html
<body>
  .......
   <ul>
       <li><a href="#sejarah">Sejarah</a></li>
       <li><a href="#geografis">Geografis</a></li>
       <li><a href="#wisata">Wisata</a></li>
   </ul>
   <h2 id="sejarah">Sejarah</h2>
 .......
 
   <h2 id="geografis">Geografis</h2>
 .......
 
   <h2 id="wisata">Wisata</h2>
 .......
</body>
```
Setelah menuliskan id elemen pada target anchor, maka <i>hypertext</i> di navigasi sudah dapat digunakan. Yang terakhir sebagai pemanis kita tambahkan gambar dibagian sejarah.

```html
<body>
   .......
<h2 id="sejarah">Sejarah</h2>
<img src="https://media.suara.com/pictures/653x366/2019/10/14/14093-tugu-pal-putih-atau-tugu-yogyakarta-suaraeleonora-pew.jpg" alt="sejarah">
   .......
</body>
```

jadi seperti inilah keseluruhan kode <b>index.html</b> yang sudah kita buat tadi:

```html
<!DOCTYPE html>
<html>
<head>
</head>
<body>
<h1>Yogyakarta</h1>
<p>Kota Yogyakarta adalah ibu kota dan pusat pemerintahan Daerah Istimewa Yogyakarta, Indonesia.</p> 

<ul>
    <li><a href="#sejarah">Sejarah</a></li>
    <li><a href="#geografis">Geografis</a></li>
    <li><a href="#wisata">Wisata</a></li>
</ul>
 
<h2 id="sejarah">Sejarah</h2>
<img src="https://media.suara.com/pictures/653x366/2019/10/14/14093-tugu-pal-putih-atau-tugu-yogyakarta-suaraeleonora-pew.jpg" alt="sejarah">
<p>Ryadi Goenawan dan Darto Harnoko dalam buku Sejarah Sosial Daerah, Daerah Istimewa Yogyakarta (1993) menjelaskan, ada pihak yang menyatakan bahwa nama Kota Yogyakarta berasal dari kata "Ayodya" yang berarti kemenangan dan "Karta" yang berarti kota. Lalu sebuah buku yang dikarang oleh C.F. Winter (1928), menyatakan bahwa Ngayogyakarta itu berasal dari kata "Jogja" yang berarti baik, sedangkan "Karta" berarti aman dan makmur.</p>
 
 
<h2 id="geografis">Geografis</h2>
<p>Komponen fisiografi yang menyusun Propinsi Daerah Istimewa Yogyakarta terdiri dari 4 (empat) satuan fisiografis yaitu Satuan Pegunungan Selatan (Dataran Tinggi Karst) dengan ketinggian tempat berkisar antara 150 - 700 meter, Satuan Gunungapi Merapi dengan ketinggian tempat berkisar antara 80 - 2.911 meter, Satuan Dataran Rendah yang membentang antara Pegunungan Selatan dan Pegunungan Kulonprogo pada ketinggian 0 - 80 meter, dan Pegunungan Kulonprogo dengan ketinggian hingga 572 meter.
Propinsi Daerah Istimewa Yogyakarta mempunyai luas 3.185,80 km, terdiri dari 4 kabupaten dan 1 Kota, yaitu Kota Yogyakarta, Kabupaten Sleman, Kabupaten Bantul, Kabupaten Gunungkidul, dan Kabupaten Kulonprogo. Setiap kabupaten/kota mempunyai kondisi fisik yang berbeda sehingga potensi alam yang tersedia juga tidak sama. Perbedaan kondisi fisik ini ikut menentukan dalam rencana pengembangan daerah.</p>
 
 
<h2 id="wisata">Wisata</h2>
<p>Yogyakarta atau kerap disebut dengan Jogja menjadi salah satu kota besar di Provinsi Daerah Istimewa Yogyakarta yang tidak pernah sepi.
Bagaimana tidak? Kota yang tetap dan terus mengangkat budaya jawa ini menghadirkan banyak tempat wisata yang menjadi daya tarik. Tempat wisata yang ada pun tergolong hits dan instagramable, sehingga banyak anak muda yang menjadikan kota ini destinasi wisata wajib dikunjungi.
Lantas, tempat wisata hits apa saja yang ada di Jogja? Untuk lebih jelasnya, simak ulasan berikut ini.</p>
 
 
<h3>Tugu Pal Putih</h3>

<p>Lokasinya ada ti tengah Kota Yogyakarta yang selalu ramai dilewati kendaraan. Jaraknya dari Malioboro adalah 1 - 2 kilometer(km) dan dapat ditemput dengan jalan kaki mulai dari 15 menit.
Pengunjung yang datang menjadikan tempat ini sebagai tempat nongkrong dan berfoto.
Monumen yang didominasi warna putih itu memiliki nilai simbolis dan merupakan bangunan yang menghubungkan Pantai Parangtritis, Panggung Krapyak, Keraton Yogyakarta, dan Gunung Merapi.</p> 
 
<h3>Jogja National Museum</h3>

<p>Jogja National Museum atau biasa disingkat JNM adalah sebuah tempat wisata sejarah yang ada dekat kawasan Malioboro.  Jaraknya dari Malioboro adalah 2 km dengan waktu berkendara kira-kira 11 menit.  Museum ini dulunya adalah area kompleks gedung Akademi Seni Rupa Indonesia (ASRI) dan Fakultas Seni Rupa dan Desain (FSRD) yang kini sudah berdiri sendiri menjadi Institut Seni Indonesia (ISI) Yogyakarta. Setelah bertahun-tahun tak terurus gedung ini akhirnya dijadikan museum pada tahun 2006 dan digunakan untuk ruang aktivitas seni dan budaya untuk publik.</p>

</body>
</html>

```

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-16_23-38.png)