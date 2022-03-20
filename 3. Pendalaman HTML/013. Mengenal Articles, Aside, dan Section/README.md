# Mengenal Aticles, Aside, dan Section

## Articles

Elemen ```<article>``` bertindak sebagai <i>container</i> untuk independen konten pada sebuah halaman, artinya konten utuh yang tidak terkait dengan konten lain. Bisa saja konten yang dimaksud berupa artikel blog, komentar, forum post, dan konten lainnya.

Jika sebuah halam terdapat beberapa artikel, maka tiap artikel tersebut seharusnya berada pada elemen <i>article</i>-nya masing-masing.

```html
<article>
    <h2 id="sejarah">Sejarah</h2>
    <img src="https://media.suara.com/pictures/653x366/2019/10/14/14093-tugu-pal-putih-atau-tugu-yogyakarta-suaraeleonora-pew.jpg" alt="sejarah">
    <p>Ryadi Goenawan dan Darto Harnoko dalam buku Sejarah Sosial Daerah, Daerah Istimewa Yogyakarta (1993) menjelaskan, ada pihak yang menyatakan bahwa nama Kota Yogyakarta berasal dari kata "Ayodya" yang berarti kemenangan dan "Karta" yang berarti kota. Lalu sebuah buku yang dikarang oleh C.F. Winter (1928), menyatakan bahwa Ngayogyakarta itu berasal dari kata "Jogja" yang berarti baik, sedangkan "Karta" berarti aman dan makmur.</p>
</article>
 
<article>
    <h2 id="geografis">Geografis</h2>
    <img src="https://3.bp.blogspot.com/-vhPuIo9j9CY/XHxAv9LcybI/AAAAAAAAKEg/Y2fJEnyZAPAU0QUb-WKeqyZG1hme4MJDwCLcBGAs/s1600/3%2Bpeta%2Byogya.jpg" alt="geografis">
    <p>Komponen fisiografi yang menyusun Propinsi Daerah Istimewa Yogyakarta terdiri dari 4 (empat) satuan fisiografis yaitu Satuan Pegunungan Selatan (Dataran Tinggi Karst) dengan ketinggian tempat berkisar antara 150 - 700 meter, Satuan Gunungapi Merapi dengan ketinggian tempat berkisar antara 80 - 2.911 meter, Satuan Dataran Rendah yang membentang antara Pegunungan Selatan dan Pegunungan Kulonprogo pada ketinggian 0 - 80 meter, dan Pegunungan Kulonprogo dengan ketinggian hingga 572 meter.
Propinsi Daerah Istimewa Yogyakarta mempunyai luas 3.185,80 km, terdiri dari 4 kabupaten dan 1 Kota, yaitu Kota Yogyakarta, Kabupaten Sleman, Kabupaten Bantul, Kabupaten Gunungkidul, dan Kabupaten Kulonprogo. Setiap kabupaten/kota mempunyai kondisi fisik yang berbeda sehingga potensi alam yang tersedia juga tidak sama. Perbedaan kondisi fisik ini ikut menentukan dalam rencana pengembangan daerah.</p>
</article>
 
<article>
    <h2 id="wisata">Wisata</h2>
    <img src="https://akcdn.detik.net.id/visual/2020/10/21/candi-prambanan_169.jpeg?w=650" alt="wisata">
    <p>Yogyakarta atau kerap disebut dengan Jogja menjadi salah satu kota besar di Provinsi Daerah Istimewa Yogyakarta yang tidak pernah sepi.
Bagaimana tidak? Kota yang tetap dan terus mengangkat budaya jawa ini menghadirkan banyak tempat wisata yang menjadi daya tarik. Tempat wisata yang ada pun tergolong hits dan instagramable, sehingga banyak anak muda yang menjadikan kota ini destinasi wisata wajib dikunjungi.
Lantas, tempat wisata hits apa saja yang ada di Jogja? Untuk lebih jelasnya, simak ulasan berikut ini.</p>
</article>
 
```

Elemen ```<article>``` dapat berada pada elemen ```<article>``` lainnya (<i>nested</i>) selama artikel tersebut berkaitan dengan induk elemen ```<article>``` yang menampungnya.

## Aside

Elemen ```<aside>``` memiliki dua tujuan, tergantung kita menempatkannya di sebuah elemen ```<article>``` atau tidak.

Katika elemen ini ditempatkan di dalam elemen ```<article>```, pada elemen ini dapat berisikan informasi yang berhubungan dengan artikel tersebut, tetapi bukan bagian dari konten artikelnya itu sendiri (dipisahkan dari konten utama).

Ketika elemen ini ditempatkan di luar dari elemen ```<article>```, pada elemen ini dapar berisi informasi yang berhubungan pada keseluruhan halaman.

Elemen ```<aside>``` biasanya terletak di samping dari sebuah elemen yang menampungnya.

```html
<main>
   <article>
       ......
   </article>
   <aside>
       <article>
           <header>
               <h2>Daerah Istimewa Yogyakarta</h2>
               <p>Kota Pelajar</p>
               <figure>
                   <img src="img/jogja.png">
                   <figcaption>Lambang</figcaption>
               </figure>
           </header>
       </article>
   </aside>
</main>
```
## Section

Sebuah elemen yang memiliki kesamaan konten dan memiliki sebuah <i>heading</i> di dalamnya dapat dikelompokkan dengan menggunakan elemen ```<section>```. Dengan begitu elemen ini dapat digunakan pada sebuah elemen ```<article>``` yang memiliki konten panjang dan berpotensi untuk dikelompokkan.

Di dalam sebuah ```<section>``` sebaiknya terdapat elemen heading (h1 - h6), yang menjadi elemen pertama yang dituliskan pada sebuah section untuk menunjukkan judul atau tema dari bagian konten yang dikelompokkan.

```html
<article>
    <section>
        <h2 id="wisata">Wisata</h2>
        <img src="https://akcdn.detik.net.id/visual/2020/10/21/candi-prambanan_169.jpeg?w=650" alt="wisata">
        <p>Yogyakarta atau kerap disebut dengan Jogja menjadi salah satu kota besar di Provinsi Daerah Istimewa Yogyakarta yang tidak pernah sepi.
    Bagaimana tidak? Kota yang tetap dan terus mengangkat budaya jawa ini menghadirkan banyak tempat wisata yang menjadi daya tarik. Tempat wisata yang ada pun tergolong hits dan instagramable, sehingga banyak anak muda yang menjadikan kota ini destinasi wisata wajib dikunjungi.
    Lantas, tempat wisata hits apa saja yang ada di Jogja? Untuk lebih jelasnya, simak ulasan berikut ini.</p>
    </section>

    <section>
        <h3>Tugu Pal Putih</h3>
        <p>Lokasinya ada ti tengah Kota Yogyakarta yang selalu ramai dilewati kendaraan. Jaraknya dari Malioboro adalah 1 - 2 kilometer(km) dan dapat ditemput dengan jalan kaki mulai dari 15 menit.
        Pengunjung yang datang menjadikan tempat ini sebagai tempat nongkrong dan berfoto.
        Monumen yang didominasi warna putih itu memiliki nilai simbolis dan merupakan bangunan yang menghubungkan Pantai Parangtritis, Panggung Krapyak, Keraton Yogyakarta, dan Gunung Merapi.</p> 
        
        <h3>Jogja National Museum</h3>

        <p>Jogja National Museum atau biasa disingkat JNM adalah sebuah tempat wisata sejarah yang ada dekat kawasan Malioboro.  Jaraknya dari Malioboro adalah 2 km dengan waktu berkendara kira-kira 11 menit.  Museum ini dulunya adalah area kompleks gedung Akademi Seni Rupa Indonesia (ASRI) dan Fakultas Seni Rupa dan Desain (FSRD) yang kini sudah berdiri sendiri menjadi Institut Seni Indonesia (ISI) Yogyakarta. Setelah bertahun-tahun tak terurus gedung ini akhirnya dijadikan museum pada tahun 2006 dan digunakan untuk ruang aktivitas seni dan budaya untuk publik.</p>
    </section>
</article>

```