# Inline Formatting Text
Standarnya elemen HTML memiliki dua sifat yaitu <i>block</i> dan <i>inline</i>. Elemen yang memiliki sifat block selalu membuat garis baru ketika menampilkannya, contohnya seperti elemen paragraf, list, heading, dan lainnya. Berlawanan dengan elemen yang memiliki sifat inline, elemen ini tidak menambah baris baru ketika dibuat. Apa saja elemen tersebut? Mari kita bahas satu persatu ya.

## Anchor
Anchor(jangkar) merupakan elemen yang digunakan untuk membuat sebuah <i>hyperlink</i> ke halaman atau website lain, file, alamat email, atau URL lainnya. Untuk menggunakan elemen ini kita gunakan tag ```<a>...</a>``` bersama dengan atribut ```href``` untuk menetapkan sebuah target yang akan dituju.

```html
<p>Hubungi kami di</p>
<ul>
   <li><a href="https://example.com">Website</a></li>
   <li><a href="mailto:info@example.com">Email</a></li>
   <li><a href="tel:+62123456">Telepon</a></li>
   <li><a href="#address">Alamat</a></li>
</ul>
```
Selain atribut ```href```, terdapat eberapa atribut khusus yang dapat digunakan pada elemen ini, antara lain:

| Atribut | Nilai | Fungsi |
|:--------|:------|:-------|
| download | filename | Menginstruksikan browser untuk mengunduh pada URL yang ditetapkan daripada mengarahkannya.  |
| href | URL | Menetapkan target yang akan diarahkan/unduh ketika pengguna menekan hyperlink. |
| hreflang | language_code | Menetapkan bahasa dari dokumen target. |
| ping | list_of_URLs | Menetapkan URL yang akan diberitahu dengan mengirimkan post request ping pada body oleh browser (berjalan di belakang layar) ketika target URL pada hyperlink ditekan. Biasanya atribut ini digunakan untuk pelacakan. | 
| referrerpolicy | no-referrer, no-referrer-when-downgrade, origin, origin-when-cross-origin, unsafe-url | Menetapkan referensi untuk dikirim pada target. |
| rel | alternate, author, bookmark, external, help, license, next, nofollow, noreferrer, noopener, | Menetapkan hubungan antara halaman yang ditampilkan dengan target. |
| target | _blank, _parent, _self, _top | Menetapkan lokasi ketika membuka target contohnya pada sebuah tab, window atau pada tab itu sendiri. |
| media | media_type | Menetapkan tipe media yang digunakan pada target. |

## Emphasized text

Gunakan elemen ```<em>``` untuk menunjukan bagian kata yang perlu kita tekankan. Elemen ini menunjukan stress emphasis atau konten/kata yang perlu mendapatkan penekanan atau perhatian khusus. Berikut ini adalah contoh penggunaannya.

```html
<p><em>Oding</em> adalah seorang pelajar</p>
<p>Dia adalah seorang <em>pelajar</em></p>
```
Pada kalimat pertama, penekanan terdapat pada “siapa” seorang pelajar. Sedangkan pada kalimat kedua, penekanan terdapat pada “apa” yang sedang ditekuni oleh Oding.

Standarnya pada browser sebuah kata yang ditekankan akan ditampilkan dalam gaya miring pada teks nya.




![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-13_23-07.png)

## Short quotations
Gunakan elemen ```<q>``` untuk menandai sebuah kutipan dalam sebuah teks. Elemen short quations berbeda dengan ```<blockquote>```. Elemen ini digunakan untuk kutipan pendek yang terletak di dalam baris (inline). Berikut ini adalah contohnya:

```html
<p>Sebelum pulang kerja, ia berkata kepadaku: <q>Maaf saya tidak bisa hadir dalam pertemuan nanti</q></p>
```
Standarnya pada browser sebuah teks yang diberi markup ```<q>``` akan ditampilkan di dalam tanda kutip (Quotation marks).

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-13_23-12.png)
