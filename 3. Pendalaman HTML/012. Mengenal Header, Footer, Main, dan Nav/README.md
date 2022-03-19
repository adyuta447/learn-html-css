# Mengenal Header, Footer, Main dan Nav

## Header dan Footer

Elemen ini dapat kita gunakan untuk:

- Sebuah <i>header</i> dan <i>Footer</i> utama muncul pada awal dan akhir di sebuah halaman ```<body>```.

- Header digunakan sebagai pembuka konten dalam sebuah elemen ```<article>``` atau ```<section>```.

- Footer digunakan sebagai catatan kaki pada sebuah elemen ```<article>``` atau ```<section>```.

Pada contoh dibawah ini elemen ```<header>``` digunakan untuk menampilkan nama situs dan navigasi utama.

```html
<header>
<h1>Yogyakarta</h1>
<p>Kota Yogyakarta adalah ibu kota dan pusat pemerintahan Daerah Istimewa Yogyakarta, Indonesia.</p> 
    <nav>
        <ul>
            <li><a href="#sejarah">Sejarah</a></li>
            <li><a href="#geografis">Geografis</a></li>
            <li><a href="#wisata">Wisata</a></li>
        </ul>
    </nav>
</header>

```
Dan elemen ```<footer>``` digunakan sebagai informasi hak cipta.

```html
<body>
<header>
<h1>Yogyakarta</h1>
<p>Kota Yogyakarta adalah ibu kota dan pusat pemerintahan Daerah Istimewa Yogyakarta, Indonesia.</p> 
    <nav>
        <ul>
            <li><a href="#sejarah">Sejarah</a></li>
            <li><a href="#geografis">Geografis</a></li>
            <li><a href="#wisata">Wisata</a></li>
        </ul>
    </nav>
</header>
<footer>
    &copy; 2019, Ether Linux
</footer>
</body>
```

Selain itu, elemen ```<header>``` dan ```<footer>``` dapat digunakan pada sebuah elemen ```<article>``` atau ```<section>```. Header biasanya menampung judul dan penulis, footer dapat menampung link untuk membagikan artikel pada sebuah sosial media.

```html
<article>
   <header>
       <h1>Judul Artikel</h1>
       <h2>Oleh: K0oceng</h2>
   </header>
   <p>....... Konten artikel dimulai dari sini ......</p>
   <footer>
       <p>Bagikan artikel ini melalui</p>
       <ul>
           <li>Instagram</li>
           <li>Whatsapp</li>
           <li>......</li>
       </ul>
   </footer>
</article>
```
Disini perlu kita ketahui bahwa elemen ```<header>``` dan ```<footer>``` tidak boleh ditulis di dalam elemen ```<header>``` dan ```<footer>``` lainnya (bertumpuk/nested).

## Main

Element ```<main>``` digunakan untuk menampung/mewadahi konten utama(dominan) dalam ```<body>```. Konten main dapat terdiri dari banyak section, ataupun artikel, atau konten apapun di dalam elemen main, selama termasuk konten utama yang dimiliki oleh website.

```html
<body>
    <header>
        <!-- Konten header website -->
    </header>
    <main>
        <section>
            <article>
                <p>Sebuah article</p>
            </article>
        </section>
        <article>
            <p>Sebuah article lain</p>
        </article>
    </main>
    <footer>
        <!-- Konten footer website -->
    </footer>
</body>
```


Note: ```<!-- -->``` merupakan tag komentar pada HTML, teks yang terdapat di antara tag tersebut, tidak akan ditampilkan pada website. Fungsinya untuk memberikan komentar / catatan.

Karena elemen ```<main>``` merupakan berisi dari inti konten pada website, jangan gunakan elemen main lebih dari satu pada berkas HTML.

## Nav

Elemen ```<nav>``` digunakan untuk menampung sebuah navigasi yang sifatnya penting(major), contohnya navigasi utama pada sebuah website.

Tapi tidak menjamin pada sebuah website hanya ada satu navigasi. Contohnya, sebuah akhir artikel pada blog terdapat tautan navigasi menuju artikel yang dianggap relevan dengan artikel yang telah kita baca. Navigasi tersebut tidak dianggap sebagai navigasi yang penting, sehingga kita perlu menggunakan elemen ```<nav>``` untuk menampilkannya.

```html
<nav>
   <ul>
       <li><a href="#sejarah">Sejarah</a></li>
       <li><a href="#geografis">Geografis</a></li>
       <li><a href="#wisata">Wisata</a></li>
   </ul>
</nav>
```

Sebuah navigation pada dasarnya sangat berguna untuk aksesibilitas website kita. Contohnya ketika pengguna website kita menggunakan <i>screen reader</i> dalam mengunjungi website, pengguna akan mudah mencari bagian yang dia inginkan tanpa harus menelusuri seluruh konten website.


