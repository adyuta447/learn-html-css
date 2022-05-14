# Konsep pada penulisan CSS

## Inheritance

Styling HTML bersifat <i>inheritance</i> yang artinya dapat mewarisi properti <i>style</i> "tertentu" pada elemen yang ada di dalamnya. Contohnya pada rules yang kita tuliskan untuk elemen ```<body>``` akan diterapkan pada seluruh elemen yang ada di dalama elemennya (```body```). Contoh lainnya, pada rules yang diterapkan pada elemen ```<footer>``` dengan properti color yang bernilai white, akan diterapkan pada seluruh elemen yang ada di dalam ```<footer>```. Hal ini menjadi alasan mengapa memahami struktur itu penting.

<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/4.%20Pengenalan%20CSS/img/Screenshot%202022-05-12%20131514.png" alt="screenshot">
</p>

## Group Selector
Di CSS kita dapat menyatukan selector tersebut sehingga dapat meminimalisir penulisan kode yang berulang. Contohnya pada styling yang sudah kita buat sebelumnya, terdapat rule yang serupa antara ```h2``` dan ```h3```.

```css
h2 {
   color: #00a2c6;
}
 
h3 {
   color: #00a2c6;
}
```

Jika terdapat kasus ini, kita dapat menuliskan dua selector sekaligus dalam satu struktur <i>rule</i>. Gunakan tanda kome (,) untuk memisahkan tiap selectornya. Silahkan kita buka kembali file <b>style.css</b> dan gabungkan rule untuk elemen ```<h2>``` dan ```<h3>``` menjadi seperti ini:

```css
h2, h3 {
    color: #00a2c6;
}
```

## Rule Order

alur kerja dari CSS dalam membaca kode dari atas ke bawah. Maka dari itu kita harus memperhatikan urutan dalam penulisan rules, terutama saat terjadi sebuah konflik. Konflik dapat terjadi karena kita dapat menerapkan styling pada satu dokumen HTML. Contohnya, apa yang seharusnya ditampilkan pada browser ketika eksternal css mengharuskan elemen ```<p>``` menampilkan warna merah, tetapi pada <i>embedded css</i> ```<p>``` harus menampilkan warna biru? Kembali pada alur kerja CSS yang membaca dari atas ke bawah, sehingga warna yang akan diterapkan adalah warna yang paling akhir didefinisikan. Coba kita lihat contoh berikut:

```html
<!doctype html>
<html lang="en">
<head>
   <title>Judul Berkas</title>
   <style>
       p {
           color: red;
       }
 
       p {
           color: blue;
       }
   </style>
</head>
<body>
<p>Sesuai dengan namanya cascading yang artinya <q>mengalir</q>, alur kerja CSS dalam membaca kode pun seperti itu.
   Mengalir dari atas ke bawah sehingga kita harus memperhatikan urutan dalam penulisan rules <i>styling</i></p>
</body>
</html>
```
Maka pada browser elemen ```<p>``` menerapkan warna biru pada tulisannya.

<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/4.%20Pengenalan%20CSS/img/Screenshot%202022-05-14%20090030.png" alt="screenshot">
</p>

Tetapi kita bisa membuat sebuah property styling agar dianggap penting untuk diterapkan oleh browser dan tidak memperhatikan urutannya. Kita bisa menambahkan keyword ```!important``` diakhir nilai pada property tersebut.

```html
<!doctype html>
<html lang="en">
<head>
   <title>Judul Berkas</title>
   <style>
       p {
           color: red !important;
       }
 
       p {
           color: blue;
       }
   </style>
</head>
<body>
<p>Sesuai dengan namanya cascading yang artinya <q>mengalir</q>, alur kerja CSS dalam membaca kode pun seperti itu.
   Mengalir dari atas ke bawah sehingga kita harus memperhatikan urutan dalam penulisan rules <i>styling</i></p>
</body>
</html>
```

Sehingga warna yang diterapkan pada teks paragraf adalah merah.

<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/4.%20Pengenalan%20CSS/img/Screenshot%202022-05-14%20090030.png" alt="screenshot">
</p>

Gunakan ```!important``` ketika memang dibutuhkan saja. Sebaiknya kita pahami aturan urutan pada CSS dengan baik sehingga meminimalisir penggunaan tanda tersebut.


Catatan yang sudah kita pelajari sejauh ini tentang styling agar tidak lupa:

- Rule : Sebuah aturan styling yang harus diterapkan pada elemen HTML. Dalam sebuah rule terdapat selector dan deklarasi properti styling.
- Selector : Sebuah bagian rule, yang mengidentifikasikan terget elemen untuk menetapkan sebuah rule.
- Declaration : Sebuah bagian dari rule, yang terdiri dari pasangan properti dan nilainya.
- External Style Sheet : Berkas/file terpisah yang didalamnya hanya terdapat sebuah rules yang akan digunakan pada web.
- Embedded Style Sheet : Kumpulan rules yang dituliskan dalam berkas HTML dengan menggunakan elemen ```<style>```.
- Inline Style : Styling yang diterapkan pada elemen HTML dengan menggunakan atribut style.
