# Mengenal Citation, Defining Terms, Subscript, Superscript, Highlighted Text, dan Line Break

## Citation ```<cite>```
Selain sebuah atribut, ```<cite>``` juga merupakan sebuah elemen yang digunakan untuk sebuah rujukan pada sebuah dokumen, contohnya sebuah buku, majalah, artikel dan lainnya.

```html
 <p>Kalian bisa download iso ether linux disini <cite><a href="https://ether-linux.org">ether-linux.org</a></cite>.</p> 

```

Standarnya pada sebuah browser sebuah teks yang diberi <i>markup</i> ```<cite>``` akan ditempilkan dengan garis miring (<i>italic</i>).

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-15_22-55.png)

## Defining terms ```<dfn>```
Elemen ```<dfn>``` digunakan ketika mendefinisikan sebuah istilah (<i>term</i>). Elemen ini haruslah terletak pada elemen lain yang menaunginya. Contohnya pada sebuah elemen ```<p>``` atau elemen ```<section>```. Berikut ini adalah contoh penggunaanya:

```html
<p><dfn>Website</dfn> merupakan halaman yang menampilkan informasi melalui teks atau gambar. Website dapat diakses melalui internet dengan menggunakan browser.</p>
```

Standar pada browser yakni sebuah teks yang diberi markup ```<dfn>``` akan ditampilkan dengan garis miring(<i>italic</i>).

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-15_23-02.png)

## Subscript ```<sub>``` dan Superscript ```<sup>```

<i>Subscript</i> ```<sub>``` dan <superscript> ```<sup>``` merupakan elemen yang dapat membuat teks yang ditampilkan tampak kecil, dengan posisi dibawah (<b>sub</b>) atau di atas (<b>sup</b>) dari teks biasanya. Elemen ini digunakan untuk menunjukan sebuah rumus kimia ataupun matematika.

```html
<p>Sukrosa merupakan suatu disakarida yang dibentuk dari monomer-monomernya yang berupa unit glukosa dan fruktosa,dengan rumus molekul C<sub>12</sub>H<sub>22</sub>O<sub>11</sub>.</p>
 
<p>Salah satu persamaan paling umum dalam semua fisika adalah E=MC<sup>2</sup></p> 

```
Jika kita lihat pada browser, tampilan akan tampak seperti ini:

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-15_23-10.png)

## Highlighted text ```<mark>```

Untuk menandai atau menyorot sebuah teks kita bisa menggunakan elemen ```<mark>```. Elemen ini digunakan ketika terdapat sebuah teks yang memiliki peran penting, biasanya teks tersebut merupakan bagian yang paling relevan atau panting dalam sebuah konteks kalimat.

```html
<p>Ini adalah periode perang saudara. Pesawat ruang angkasa pemberontak, menyerang dari pangkalan tersembunyi, telah
memenangkan kemenangan pertama mereka melawan Kekaisaran Galactic yang jahat. Selama pertempuran,
<mark>mata-mata
Pemberontak berhasil mencuri rencana rahasia
</mark>
ke senjata pamungkas Kekaisaran, STAR DEATH, stasiun ruang angkasa
berlapis baja dengan kekuatan yang cukup untuk menghancurkan seluruh planet.
</p>
```
Standarnya pada browser teks yang diberi markup ```<mark>``` akan ditampilkan dengan background kuning dan teks hitam.

Jika kita lihat pada browser, tampilan akan tampak seperti ini:

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-15_23-17.png)

## Line Break ```<br>```

Terkadang kita mungkin perlu menambahkan sebuah baris baru pada sebuah bari teks (termasuk di dalam paragraf), tetapi kita mengetahui bahwa browser akan mengabaikan sebuah penulisan spasi ganda atau garis baru, Nah untuk itulah kita memerlukan sebuah tanda yang dapat digunakan untuk memberitahu browser untuk "Tambahkan garis baru disini".

<i>Inline line break elemen</i> atau ```<br>``` dapat digunakan untuk memberitahu browser untuk memberikan sebuah garis baru pada baris teks. Sama seperti gambar, elemen ini merupakan elemn kosong sehingga kita tidak membutuhkan sebuah <i>tag</i> penutup.

```html
<p>
    Jakarta, <br>
    15 Maret 2022<br>
    Aku ganteng<br>
    Ibu sedang mencuci baju
</p>
```

Jika kita lihat pada browser, maka tampilan akan tampak seperti ini:

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-15_23-37.png)