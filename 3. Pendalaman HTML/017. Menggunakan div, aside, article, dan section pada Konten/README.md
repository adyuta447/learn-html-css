# Menggunakan ```<div>```, ```<aside>```, ```<article>```, dan ```<section>``` pada Konten

Kita sudah membagi konten pada elemen ```<body>``` secara besar menjadi tiga bagian. Tetapi belum sampai disitu ya, pada salah satu bagiannya yaitu pada elemen ```<main>```, masih terdapat konten yang dapat kita kelompokan. Di sini kita akana menerapkan generic elemen seperti ```<div>``` dan <i>semantic</i> elemen lainnya seperti ```<aside>```, ```<article>```, dan ```<section>``` dalam mengelompokkan elemennya.

Sebelum itu kalian harus download asset yang sudah disediakan oleh penulis yang terdiri dari ```index.html``` dan juga beberapa gambar lainnya. Kasian bisa mendownloadnya [disini](https://www.mediafire.com/file/ahwfp2p5z1ygo1e/WebDasar.zip/file)

Dimulai dari hierarki teratas, dalam elemen ```<main>``` kita bagi konten menjadi dua bagian, yang pertama sebuah konten utama yang dikelompokan menggunakan ```<div>``` dan konten samping yang dikelompokkan menggunakan ```<aside>```.

```html
<main>
    <div>
        <h2 id="sejarah">Sejarah</h2>
        <img src="assets/images/sejarah.jpg" alt="sejarah">
        <p>Ryadi Goenawan dan Darto Harnoko dalam buku Sejarah Sosial Daerah, Daerah Istimewa Yogyakarta (1993) menjelaskan, ada pihak yang menyatakan bahwa nama Kota Yogyakarta berasal dari kata "Ayodya" yang berarti kemenangan dan "Karta" yang berarti kota. Lalu sebuah buku yang dikarang oleh C.F. Winter (1928), menyatakan bahwa Ngayogyakarta itu berasal dari kata "Jogja" yang berarti baik, sedangkan "Karta" berarti aman dan makmur.</p>
        
        
        <h2 id="geografis">Geografis</h2>
        <img src="assets/images/geografis.png" alt="geografis">
        <p>Komponen fisiografi yang menyusun Propinsi Daerah Istimewa Yogyakarta terdiri dari 4 (empat) satuan fisiografis yaitu Satuan Pegunungan Selatan (Dataran Tinggi Karst) dengan ketinggian tempat berkisar antara 150 - 700 meter, Satuan Gunungapi Merapi dengan ketinggian tempat berkisar antara 80 - 2.911 meter, Satuan Dataran Rendah yang membentang antara Pegunungan Selatan dan Pegunungan Kulonprogo pada ketinggian 0 - 80 meter, dan Pegunungan Kulonprogo dengan ketinggian hingga 572 meter.
        Propinsi Daerah Istimewa Yogyakarta mempunyai luas 3.185,80 km, terdiri dari 4 kabupaten dan 1 Kota, yaitu Kota Yogyakarta, Kabupaten Sleman, Kabupaten Bantul, Kabupaten Gunungkidul, dan Kabupaten Kulonprogo. Setiap kabupaten/kota mempunyai kondisi fisik yang berbeda sehingga potensi alam yang tersedia juga tidak sama. Perbedaan kondisi fisik ini ikut menentukan dalam rencana pengembangan daerah.</p>
        
        
        <h2 id="wisata">Wisata</h2>
        <p>Yogyakarta atau kerap disebut dengan Jogja menjadi salah satu kota besar di Provinsi Daerah Istimewa Yogyakarta yang tidak pernah sepi.
        Bagaimana tidak? Kota yang tetap dan terus mengangkat budaya jawa ini menghadirkan banyak tempat wisata yang menjadi daya tarik. Tempat wisata yang ada pun tergolong hits dan instagramable, sehingga banyak anak muda yang menjadikan kota ini destinasi wisata wajib dikunjungi.
        Lantas, tempat wisata hits apa saja yang ada di Jogja? Untuk lebih jelasnya, simak ulasan berikut ini.</p>
        
        
        <h3>Tugu Pal Putih</h3>
        <img src="assets/images/tugu-pal-putih.jpeg" alt="">
        <p>Lokasinya ada ti tengah Kota Yogyakarta yang selalu ramai dilewati kendaraan. Jaraknya dari Malioboro adalah 1 - 2 kilometer(km) dan dapat ditemput dengan jalan kaki mulai dari 15 menit.
        Pengunjung yang datang menjadikan tempat ini sebagai tempat nongkrong dan berfoto.
        Monumen yang didominasi warna putih itu memiliki nilai simbolis dan merupakan bangunan yang menghubungkan Pantai Parangtritis, Panggung Krapyak, Keraton Yogyakarta, dan Gunung Merapi.</p> 
        
        <h3>Jogja National Museum</h3>
        <img src="assets/images/Museum-National-Jogja.jpg" alt="">
        <p>Jogja National Museum atau biasa disingkat JNM adalah sebuah tempat wisata sejarah yang ada dekat kawasan Malioboro. 
            Jaraknya dari Malioboro adalah 2 km dengan waktu berkendara kira-kira 11 menit. 
            Museum ini dulunya adalah area kompleks gedung Akademi Seni Rupa Indonesia (ASRI) dan Fakultas Seni Rupa dan Desain (FSRD) yang kini sudah berdiri sendiri menjadi Institut Seni Indonesia (ISI) Yogyakarta. Setelah bertahun-tahun tak terurus gedung 
            ini akhirnya dijadikan museum pada tahun 2006 dan digunakan untuk ruang aktivitas seni dan budaya untuk publik.
        </p>
    </div>
    
    <aside>
        <h2>Yogyakarta</h2>
        <p>Kota Pelajar</p>
        <figure>
            <img src="assets/images/Jogja-badge.png" alt="">
            <figcaption>Lambang</figcaption>
        </figure>
    </aside>
</main>
```

Dengan begitu, konten elemen ```<main>``` terbagi menjadi dua, yaitu elemen ```<div>``` dan ```<aside>```. Selanjutnya, kita mulai kelompokkan konten lebih detail lagi pada elemen ```<div>```.

Kita bisa lihat, di dalam elemen ```<div>``` terdapat konten yang dapat digolongkan sebagai artikel. Pertama memuat konten mengenai sejarah, yang kedua mengenai geografi dan selanjutnya mengenai wisata. Dengan hasil identifikasi tersebut, maka kita memerlukan tiga buah elemen ```<article>``` untuk mengelompokkan masing-masing konten yang terkait. Masing-masing elemen ```<article>``` akan terdiri dari <i>heading</i>, gambar dan paragraf.

```html
 <div>
        <article>
            <h2 id="sejarah">Sejarah</h2>
            <img src="assets/images/sejarah.jpg" alt="sejarah">
            <p>Ryadi Goenawan dan Darto Harnoko dalam buku Sejarah Sosial Daerah, Daerah Istimewa Yogyakarta (1993) menjelaskan, ada pihak yang menyatakan bahwa nama Kota Yogyakarta berasal dari kata "Ayodya" yang berarti kemenangan dan "Karta" yang berarti kota. Lalu sebuah buku yang dikarang oleh C.F. Winter (1928), menyatakan bahwa Ngayogyakarta itu berasal dari kata "Jogja" yang berarti baik, sedangkan "Karta" berarti aman dan makmur.</p>
        </article>
        
        <article>
            <h2 id="geografis">Geografis</h2>
            <img src="assets/images/geografis.png" alt="geografis">
            <p>Komponen fisiografi yang menyusun Propinsi Daerah Istimewa Yogyakarta terdiri dari 4 (empat) satuan fisiografis yaitu Satuan Pegunungan Selatan (Dataran Tinggi Karst) dengan ketinggian tempat berkisar antara 150 - 700 meter, Satuan Gunungapi Merapi dengan ketinggian tempat berkisar antara 80 - 2.911 meter, Satuan Dataran Rendah yang membentang antara Pegunungan Selatan dan Pegunungan Kulonprogo pada ketinggian 0 - 80 meter, dan Pegunungan Kulonprogo dengan ketinggian hingga 572 meter.
            Propinsi Daerah Istimewa Yogyakarta mempunyai luas 3.185,80 km, terdiri dari 4 kabupaten dan 1 Kota, yaitu Kota Yogyakarta, Kabupaten Sleman, Kabupaten Bantul, Kabupaten Gunungkidul, dan Kabupaten Kulonprogo. Setiap kabupaten/kota mempunyai kondisi fisik yang berbeda sehingga potensi alam yang tersedia juga tidak sama. Perbedaan kondisi fisik ini ikut menentukan dalam rencana pengembangan daerah.</p>
        </article>
        
        <article>
            <h2 id="wisata">Wisata</h2>
            <p>Yogyakarta atau kerap disebut dengan Jogja menjadi salah satu kota besar di Provinsi Daerah Istimewa Yogyakarta yang tidak pernah sepi.
            Bagaimana tidak? Kota yang tetap dan terus mengangkat budaya jawa ini menghadirkan banyak tempat wisata yang menjadi daya tarik. Tempat wisata yang ada pun tergolong hits dan instagramable, sehingga banyak anak muda yang menjadikan kota ini destinasi wisata wajib dikunjungi.
            Lantas, tempat wisata hits apa saja yang ada di Jogja? Untuk lebih jelasnya, simak ulasan berikut ini.</p>
    
            <h3>Tugu Pal Putih</h3>
            <img src="assets/images/tugu-pal-putih.jpeg" alt="Tugu Pal Putih">
            <p>Lokasinya ada ti tengah Kota Yogyakarta yang selalu ramai dilewati kendaraan. Jaraknya dari Malioboro adalah 1 - 2 kilometer(km) dan dapat ditemput dengan jalan kaki mulai dari 15 menit.
            Pengunjung yang datang menjadikan tempat ini sebagai tempat nongkrong dan berfoto.
            Monumen yang didominasi warna putih itu memiliki nilai simbolis dan merupakan bangunan yang menghubungkan Pantai Parangtritis, Panggung Krapyak, Keraton Yogyakarta, dan Gunung Merapi.</p> 
        
            <h3>Jogja National Museum</h3>
            <img src="assets/images/Museum-National-Jogja.jpg" alt="">
            <p>Jogja National Museum atau biasa disingkat JNM adalah sebuah tempat wisata sejarah yang ada dekat kawasan Malioboro. 
                Jaraknya dari Malioboro adalah 2 km dengan waktu berkendara kira-kira 11 menit. 
                Museum ini dulunya adalah area kompleks gedung Akademi Seni Rupa Indonesia (ASRI) dan Fakultas Seni Rupa dan Desain (FSRD) yang kini sudah berdiri sendiri menjadi Institut Seni Indonesia (ISI) Yogyakarta. Setelah bertahun-tahun tak terurus gedung 
                ini akhirnya dijadikan museum pada tahun 2006 dan digunakan untuk ruang aktivitas seni dan budaya untuk publik.
            </p>
        </article>
    </div>

```

Coba kita lihat pada elemen ```<article>``` terakhir, konten tersebut memiliki subjudul lainnya yaitu membahas tentang wisata Farm House dan Observatorium Bosscha. Maka pada konten ini kita dapat mengelompokkan juga subjudul beserta kontennya dengan menggunakan elemen ```<section>```. Sehingga seluruh konten yang berada pada elemen ```<div>``` memiliki struktur seperti ini:

```html
 <div>
        <article>
            <h2 id="sejarah">Sejarah</h2>
            <img src="assets/images/sejarah.jpg" alt="sejarah">
            <p>Ryadi Goenawan dan Darto Harnoko dalam buku Sejarah Sosial Daerah, Daerah Istimewa Yogyakarta (1993) menjelaskan, ada pihak yang menyatakan bahwa nama Kota Yogyakarta berasal dari kata "Ayodya" yang berarti kemenangan dan "Karta" yang berarti kota. Lalu sebuah buku yang dikarang oleh C.F. Winter (1928), menyatakan bahwa Ngayogyakarta itu berasal dari kata "Jogja" yang berarti baik, sedangkan "Karta" berarti aman dan makmur.</p>
        </article>
        
        <article>
            <h2 id="geografis">Geografis</h2>
            <img src="assets/images/geografis.png" alt="geografis">
            <p>Komponen fisiografi yang menyusun Propinsi Daerah Istimewa Yogyakarta terdiri dari 4 (empat) satuan fisiografis yaitu Satuan Pegunungan Selatan (Dataran Tinggi Karst) dengan ketinggian tempat berkisar antara 150 - 700 meter, Satuan Gunungapi Merapi dengan ketinggian tempat berkisar antara 80 - 2.911 meter, Satuan Dataran Rendah yang membentang antara Pegunungan Selatan dan Pegunungan Kulonprogo pada ketinggian 0 - 80 meter, dan Pegunungan Kulonprogo dengan ketinggian hingga 572 meter.
            Propinsi Daerah Istimewa Yogyakarta mempunyai luas 3.185,80 km, terdiri dari 4 kabupaten dan 1 Kota, yaitu Kota Yogyakarta, Kabupaten Sleman, Kabupaten Bantul, Kabupaten Gunungkidul, dan Kabupaten Kulonprogo. Setiap kabupaten/kota mempunyai kondisi fisik yang berbeda sehingga potensi alam yang tersedia juga tidak sama. Perbedaan kondisi fisik ini ikut menentukan dalam rencana pengembangan daerah.</p>
        </article>
        
        <article>
            <h2 id="wisata">Wisata</h2>
            <p>Yogyakarta atau kerap disebut dengan Jogja menjadi salah satu kota besar di Provinsi Daerah Istimewa Yogyakarta yang tidak pernah sepi.
            Bagaimana tidak? Kota yang tetap dan terus mengangkat budaya jawa ini menghadirkan banyak tempat wisata yang menjadi daya tarik. Tempat wisata yang ada pun tergolong hits dan instagramable, sehingga banyak anak muda yang menjadikan kota ini destinasi wisata wajib dikunjungi.
            Lantas, tempat wisata hits apa saja yang ada di Jogja? Untuk lebih jelasnya, simak ulasan berikut ini.</p>
            
            <section>
                <h3>Tugu Pal Putih</h3>
                <img src="assets/images/tugu-pal-putih.jpeg" alt="Tugu Pal Putih">
                <p>Lokasinya ada ti tengah Kota Yogyakarta yang selalu ramai dilewati kendaraan. Jaraknya dari Malioboro adalah 1 - 2 kilometer(km) dan dapat ditemput dengan jalan kaki mulai dari 15 menit.
                Pengunjung yang datang menjadikan tempat ini sebagai tempat nongkrong dan berfoto.
                Monumen yang didominasi warna putih itu memiliki nilai simbolis dan merupakan bangunan yang menghubungkan Pantai Parangtritis, Panggung Krapyak, Keraton Yogyakarta, dan Gunung Merapi.</p> 
            </section>

            <section>
                <h3>Jogja National Museum</h3>
                <img src="assets/images/Museum-National-Jogja.jpg" alt="">
                <p>Jogja National Museum atau biasa disingkat JNM adalah sebuah tempat wisata sejarah yang ada dekat kawasan Malioboro. 
                    Jaraknya dari Malioboro adalah 2 km dengan waktu berkendara kira-kira 11 menit. 
                    Museum ini dulunya adalah area kompleks gedung Akademi Seni Rupa Indonesia (ASRI) dan Fakultas Seni Rupa dan Desain (FSRD) yang kini sudah berdiri sendiri menjadi Institut Seni Indonesia (ISI) Yogyakarta. Setelah bertahun-tahun tak terurus gedung 
                    ini akhirnya dijadikan museum pada tahun 2006 dan digunakan untuk ruang aktivitas seni dan budaya untuk publik.
                </p>
            </section>
        </article>
    </div>

```

Sebelumnya, kita sudah menetapkan atribut ```id``` pada elemen heading untuk dijadikan target navigasi, setelah mengorganisasikan konten seperti ini, pindahkan atribut ```id``` dari heading ke halaman ```<article>``` lebih menunjukkan keseluruhan dari konten artikelnya.

Kemudian pada elemen ```<div>``` kita juga bisa tambahkan atribut ```id``` dan beri nilai "<i>content</i>." Hal ini nantinya akan digunakan dalam membantu penyusunan tata letak(layouting) menggunakan CSS.

```html
    <div id="content">
        <article id="sejarah">
            <h2>Sejarah</h2>
            <img src="assets/images/sejarah.jpg" alt="sejarah">
            <p>Ryadi Goenawan dan Darto Harnoko dalam buku Sejarah Sosial Daerah, Daerah Istimewa Yogyakarta (1993) menjelaskan, ada pihak yang menyatakan bahwa nama Kota Yogyakarta berasal dari kata "Ayodya" yang berarti kemenangan dan "Karta" yang berarti kota. Lalu sebuah buku yang dikarang oleh C.F. Winter (1928), menyatakan bahwa Ngayogyakarta itu berasal dari kata "Jogja" yang berarti baik, sedangkan "Karta" berarti aman dan makmur.</p>
        </article>
        
        <article id="geografis">
            <h2>Geografis</h2>
            <img src="assets/images/geografis.png" alt="geografis">
            <p>Komponen fisiografi yang menyusun Propinsi Daerah Istimewa Yogyakarta terdiri dari 4 (empat) satuan fisiografis yaitu Satuan Pegunungan Selatan (Dataran Tinggi Karst) dengan ketinggian tempat berkisar antara 150 - 700 meter, Satuan Gunungapi Merapi dengan ketinggian tempat berkisar antara 80 - 2.911 meter, Satuan Dataran Rendah yang membentang antara Pegunungan Selatan dan Pegunungan Kulonprogo pada ketinggian 0 - 80 meter, dan Pegunungan Kulonprogo dengan ketinggian hingga 572 meter.
            Propinsi Daerah Istimewa Yogyakarta mempunyai luas 3.185,80 km, terdiri dari 4 kabupaten dan 1 Kota, yaitu Kota Yogyakarta, Kabupaten Sleman, Kabupaten Bantul, Kabupaten Gunungkidul, dan Kabupaten Kulonprogo. Setiap kabupaten/kota mempunyai kondisi fisik yang berbeda sehingga potensi alam yang tersedia juga tidak sama. Perbedaan kondisi fisik ini ikut menentukan dalam rencana pengembangan daerah.</p>
        </article>
        
        <article id="wisata">
            <h2>Wisata</h2>
            <p>Yogyakarta atau kerap disebut dengan Jogja menjadi salah satu kota besar di Provinsi Daerah Istimewa Yogyakarta yang tidak pernah sepi.
            Bagaimana tidak? Kota yang tetap dan terus mengangkat budaya jawa ini menghadirkan banyak tempat wisata yang menjadi daya tarik. Tempat wisata yang ada pun tergolong hits dan instagramable, sehingga banyak anak muda yang menjadikan kota ini destinasi wisata wajib dikunjungi.
            Lantas, tempat wisata hits apa saja yang ada di Jogja? Untuk lebih jelasnya, simak ulasan berikut ini.</p>
            
            <section>
                <h3>Tugu Pal Putih</h3>
                <img src="assets/images/tugu-pal-putih.jpeg" alt="Tugu Pal Putih">
                <p>Lokasinya ada ti tengah Kota Yogyakarta yang selalu ramai dilewati kendaraan. Jaraknya dari Malioboro adalah 1 - 2 kilometer(km) dan dapat ditemput dengan jalan kaki mulai dari 15 menit.
                Pengunjung yang datang menjadikan tempat ini sebagai tempat nongkrong dan berfoto.
                Monumen yang didominasi warna putih itu memiliki nilai simbolis dan merupakan bangunan yang menghubungkan Pantai Parangtritis, Panggung Krapyak, Keraton Yogyakarta, dan Gunung Merapi.</p> 
            </section>

            <section>
                <h3>Jogja National Museum</h3>
                <img src="assets/images/Museum-National-Jogja.jpg" alt="">
                <p>Jogja National Museum atau biasa disingkat JNM adalah sebuah tempat wisata sejarah yang ada dekat kawasan Malioboro. 
                    Jaraknya dari Malioboro adalah 2 km dengan waktu berkendara kira-kira 11 menit. 
                    Museum ini dulunya adalah area kompleks gedung Akademi Seni Rupa Indonesia (ASRI) dan Fakultas Seni Rupa dan Desain (FSRD) yang kini sudah berdiri sendiri menjadi Institut Seni Indonesia (ISI) Yogyakarta. Setelah bertahun-tahun tak terurus gedung 
                    ini akhirnya dijadikan museum pada tahun 2006 dan digunakan untuk ruang aktivitas seni dan budaya untuk publik.
                </p>
            </section>
        </article>
    </div>
```

Selanjutnya kita perhatika konten yang berada pada elemen ```<aside>```. Konten ini tidak terlalu kompleks seperti pada elemen ```<div>```. Sehingga saat ini, kita cukup mengelompokkan dengan menggunakan satu elemen ```<article>```.

```html
    <aside>
        <article>
            <h2>Yogyakarta</h2>
            <p>Kota Pelajar</p>
            <figure>
                <img src="assets/images/Jogja-badge.png" alt="">
                <figcaption>Lambang</figcaption>
        </figure>
        </article>
    </aside>
```

Good job! Sekrang konten sudah terorganisir dengan baik.
