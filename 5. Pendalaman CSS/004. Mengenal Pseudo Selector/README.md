# Mengenal Jenis-jenis Pseudo Selector
## Pseudo Selector
Selain beberapa <i>selector</i> yang sudah kita pelajari, CSS masih memiliki dua selector lagi yang dapat kita manfaatkan untuk membantu menyeleksi elemen dalam menerapkan sebuah <i>rule</i>, yaitu <b>Pseudo-class</b> dan <b>Pseudo-element</b>. Perlu kita ketahui <b>pseudo selector</b> berbeda dari selector yang sudah dibahas sebelumnya, selector ini menarget elemen pada bagian yang tidak terlihat seperti sifat pada elemen, sehingga untuk menetapkannya, kita tidak bisa menggunakan selector biasa. Salah satu contoh yang paling sering kita terapkan adalah ```:hover```, Pseudo Selector tersebut kita gunakan untuk menetapkan rule ketika cursor diarahkan ke target elemen.

```css
button:hover {
    color: green;
}
```
Contoh kode di atas merupakan salah satu pseudo-class dimana elemen anchor akan menerapkan warna biru ketika cursor diarahkan pada elemen tersebut. 

## Pseudo-class Selector
Pseudo-class merupakan sebuah class <b>semu</b> yang sebenarnya ada pada tiap elemen HTML. Pada contoh sebelumnya kita sudah mengetahui salah satu pseudo-class selector, dengan menggunakan selector ini kita dapat memilih elemen berdasarkan <i>class</i> yang tidak nampak pada dokumen. Kita bisa menetapkan rule hanya ketika sebuah tautan telah dikunjungi (```:visited```) atau ketika sebuah elemen diarahkan dengan cursor (```:hover```). Untuk menggunakan pseudo-class kita gunakan tanda titik dua (:) pada <i>basic selector</i> kemudian diikuti dengan pseudo-class nya. Berikut ini adalah contoh penerapan beberapa pseudo-class pada sebuah elemen anchor:

```css
/* rule akan diterapkan pada sebuah tautan yang belum pernah dikunjungi */
a:link {
   color: red;
}
 
/* rule akan diterapkan pada sebuah tautan yang sudah pernah dikunjungi */
a:visited {
   color: green;
}
 
/* rule akan diterapkan pada sebuah tautan ketika diarahkan dengan kursor */
a:hover {
   color: pink;
}
 
/* rule akan diterapkan pada sebuah tautan ketika ditekan */
a:active {
   color:orange;
}
```

Tidak hanya yang dicontohkan di atas ada banyak sekali class semu yang menjadi standar <i>pseudo-classes</i> dalam CSS.

## Pseudo-elemen Selector
Sama seperti <i>pseudo-class</i>, pseudo-elemen merupakan sebuah elemen <b>semu</b> yang sebenarnya ada tetapi tidak tampak secara tertulis pada berkas HTML. Selector ini biasa digunakan ketika ingin menambahkan sebuah konten tepat sebelum dan setelah sebuah elemen paragraf. Jadi kita tidak perlu menuliskan sturktur elemen tersebut pada berkas HTML. Cukup manfaatkan pseudo-elemen ```::before``` dan ```::after``` kemudian tuliskan konten tersebut cukup pada CSS. Contohnya kita ingin menambahkan tanda kutip sebelum dan sesudah elemen <i>blockquote</i>. Perhatikan contoh berikut ini dan cara penulisannya:

```css
blockquote::before,
blockquote::after {
   content: '"';
   font-size: 24px;
   font-style: italic;
   font-weight: bold;
}
```
Dengan menuliskan rule tersebut, elemen ```<blockquote>``` memiliki tanda kutip pada awal dan akhir elemennya.

```html
<blockquote>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aut eius error explicabo ipsum molestiae necessitatibus nesciunt possimus reprehenderit sed voluptates. Aliquam aspernatur autem est nobis officia praesentium quas recusandae rem.</blockquote>
```
<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/5.%20Pendalaman%20CSS/img/Screenshot%202022-06-23%20192006.png" alt="null">
</p>

Untuk menggunakan pseudo-elemen kita gunakan dua buah tanda titik dua(::) kemudian diikuti dengan pseudo-elemen nya. Kita bisa menggunakan satu buah tanda tanda titik dua (:) namun kita perlu membedakannya dengan pseudo-class. Karena itu sebaiknya ketika menggunakan pseudo elemen, gunakanlah dua buah titik dia (::). Pseudo-elemen tidak hanya ```::before``` dan ```::after```. Dengan pseudo-elemen kita juga dapat menentukan rule pada awal karakter konten elmemen.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        p::first-letter {
            font-size: 32px;
            font-weight: 400;
            color: blue;
        }
    </style>
</head>
<body>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Architecto deserunt, dicta laudantium quae quam sequi
        soluta vitae! A, architecto beatae, consequuntur et eveniet fuga laudantium molestias praesentium temporibus, unde
        velit.</p>
</body>
</html>
```
<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/5.%20Pendalaman%20CSS/img/Screenshot%202022-06-23%20194113.png" alt="null">
</p>

