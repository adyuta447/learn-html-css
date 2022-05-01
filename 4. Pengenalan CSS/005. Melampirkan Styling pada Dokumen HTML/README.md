# Melampirkan Styling pada Dokumen HTML.

Setelah kita menuliskan <i>rules</i>, maka tahapan selanjutnya adalah melampirkan atau menerapkan aturan tersebut pada berkas HTML. Sebenarnya, terdapat tiga cara untuk menerapkan <i>styling</i> pada elemen HTML.

## External Style Sheet

<i>External Style Sheet</i> merupakan berkas terpisah yang di dalamnya hanya terdapat sebuah rules. Berkas ini harus berekstensi <b>.css</b>, dan berkas ini nantinya dihubungkan pada dokumen HTML. Cara ini merupakan yang paling powerful dalam menerapkan <i>styling</i>. Karena dengan cara ini, satu berkas <i>styling</i> (.css) dapat digunakan oleh banyak berkas HTML.

Kemudian, untuk menyambungkan berkas .css dengan dokumen HTML, kita dapat menggunakan elemen ```<link>``` pada ```<head>``` berkas HTML. Contohnya:

```html
<head>
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
</head>
```

Pada elemen ```<link>``` tersebut, kita tetapkan berkas CSS yang digunakan dengan menggunakan atribut ```href``` dan beri nilai "stylesheet" pada atribut ```rel``` sebagai relationship (hubungan) antara berkas <i>style.css</i> dengan dokumen HTML.

Pada contoh di atas kita tahu bahwa berkas css yang digunakan merupakan berkas lokal (berkas yang berada pada komputer/server kita sendiri). Nilai atribut href juga dapat berupa berkas .css yang tersedia melalui sebuah URL.

Contohnya, banyak pengembang menggunakan <i>bootstrap</i> untuk membantu penyusunan <i>layout</i> website-nya. Kita bisa menggunakannnya pada berkas HTML dengan langsung menuliskan URL untuk berkas tersebut.

```html
<head>
    <title>Document</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css">
</head>
```
## Embedded Style Sheet

<i>Embedded Style Sheet</i> merupakan rules yang dituliskan dalam berkas HTML dengan menggunakan elemen ```<style>```. Dengan begitu rules yang dituliskan hanya dapat dicakup oleh satu berkas HTML. Penulisan rules harus dituliskan dalam elemen ```<style>``` dan ditempatkan di dalam ```<head>``` dari berkas HTML.

```html
<head>
   <title>Document</title>
   <style>
       h1 {
           color: green;
       }
   </style>
</head>
```

## Inline Style

<i>Inline Style</i> merupakan <i>styling</i> yang diterapkan pada elemen HTML dengan menggunakan atribut ```style```. Contohnya seperti berikut:

```html
<h1 style="color: green">Kota Malang</h1>
```

Untuk menambahkan multiple properties, kita tuliskan dengan menggunakan <i>semicolon</i> (;) sebagai pemisah antar <i>styling propertiesnya</i>.

```html
<h1 style="color: green; margin-left: 2rem">Kota Malang </>
```

<i>Inline Styles</i> hanya diterapkan pada elemen di mana atribut ```style``` diterapkan. Teknik ini seharusnya dihindari kecuali memang benar-bener diperlukan untuk menggantikan sebuah <i>styling</i> yang ditetapkan pada <i>Embedded Style Sheet</i> atau <i>External Style Sheet</i>

## Commenting in Style

Pada contoh kode di atas, kita sudah melihat sebuah teks pada rule yang dimulai dari /* dan diakhiri dengan */. Teks tersebut merupakan <i>commenting line</i> di dalam sebuah CSS. Sama seperti <i>commenting</i> pada HTML dan bahasa pemograman lainnya, Teks yang dijadikan sebuah komentar tidak akan diproses oleh browser(sebagai compiler) atau lebih tepatnya diabaikan.

```css
/* Ini merupakan sebuah komentar satu baris */

/* Ini merupakan sebuah komentar lebih dari satu baris, 
entah bagaimana bahwa
aku sangat ganteng kata mamaku */
```
