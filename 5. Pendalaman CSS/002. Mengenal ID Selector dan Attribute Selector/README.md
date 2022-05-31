# Mengenal ID Selector dan Attribute Selector

## ID Selector
ID selector menetapkan target elemen berdasarkan nilai dari atribut ```id``` yang diterapkan pada elemennya. Sama seperti class, atribut ```id``` dapat diterapkan pada seluruh elemen HTML, dan kebanyakan atribut ini digunakan untuk memberikan sebuah arti pada generic elemen seperti ```<div>``` dan ```<span>```. Namun atribut id ini tidak bersifat shareable, yang artinya nilai ```id``` tersebut harus unik dan digunakan pada satu elemen saja. Untuk menetapkan selector dengan menggunakan id, kita gunakan tanda (#). Perhatikan contoh berikut ini:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        #special {
            background-color: skyblue;
        }
    </style>
</head>
<body>
    <div id="special">
        <p>Ini meruapkan konten di dalam sebuah div yang diberi id special</p>
    </div>
    <div>
        <p>Ini merupakan konten di dalam sebuah div biasa.</p>
    </div>
</body>
</html>
```
Jika kode di atas dibuka pada browser, maka tampilannya akan seperti ini:

<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/5.%20Pendalaman%20CSS/img/Screenshot%202022-05-28%20233254.png" alt="screenshot">
</p>

Yang harus kita perhatikan kembali adalah id ini bersifat unik. Jika kita ingin menerapkan sebuah rule pada banyak elemen, sebaiknya gunakan atribut ```class```, bukan dengan ```id```. Berikut ini contoh penerapan yang salah:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        #special {
            background-color: skyblue;
        }
    </style>
</head>
<body>
    <div id="special">
        <p>Ini meruapkan konten di dalam sebuah div yang diberi id special</p>
    </div>
    <div id="special"> <!-- ini merupakan contoh yang salah dalam penerapan id -->
        <p>Ini merupakan konten di dalam sebuah div biasa.</p>
    </div>
</body>
</html>
```
## Attribute Selector 
Attribute selector merupakan cara menetapkan target elemen berdasarkan sebuah atribut yang digunakan atau bahkan bisa lebih spesifik dengan nilainya. Seperti contoh berikut ini:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        /* <a> element yang menerapkan href attribut */
        a[href] {
            color: blue;
        }
        /* <a> element yang menerapkan nilai href attribut */
        a[href^="#"] {
            background-color: gold;
        }

       /* <a> element yang menerapkan nilai pada href yang mengandung teks "example" */
       a[href*="example"] {
           background-color: silver;
       }
 
       /* <a> element yang menerapkan nilai pada href yang mengandung teks "insensitive" tidak mementingkan huruf kapital*/
       a[href*="insensitive" i] {
           color: cyan;
       }
 
       /* <a> element yang menerapkan nilai pada href dengan akhiran ".org" */
       a[href$=".org"] {
           color: red;
       }
    </style>
</head>
<body>
    <ul>
        <ul>
            <li><a href="#internal">ini adalah Internal link</a></li>
            <li><a href="https://example.com">ini adalah Example link</a></li>
            <li><a href="#InSensitive">ini adalah Insensitive internal link</a></li>
            <li><a href="https://example.org">ini adalah Example org link</a></li>
        </ul>
    </ul>
</body>
</html>
```
<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/5.%20Pendalaman%20CSS/img/Screenshot%202022-05-29%20003515.png" alt="screenshot">
</p>

Dari kode di atas terlihat banyak sekali kondiri yang dapat diterapkan pada atribut <i>selector</i>. Supaya kita lebih memahami lagi, coba kita rangkum dalam sebuah tabel berikut.

| Syntax | Fungsi |
|:-----|----------|
| [attr] | Menargetkan elemen yang menerapkan atribut attr. |
| [attr=value] | Menargetkan elemen yang menerapkan atribut attr dengan nilai value. |
| [attr~=value] | Menargetkan elemen yang menerapkan atribut attr dengan salah satu nilainya adalah value |
| [attr^=value] | Menargetkan elemen yang menerapkan atribut attr yang nilainya diawali dengan nilai value. |
| [attr$=value] | Menargetkan elemen yang menerapkan atribut attr yang nilainya diakhiri dengan value. |
| [attr*=value] | Menargetkan elemen yang menerapkan attr yang nilainya mengandung value |

## Universal Selector(Tambahan)
Universal selector digunakan juga untuk diterapkan pada seluruh elemen. Tetapi selector ini juga bisa secara spesifik menargetkan sebuah elemen yang menggabungkan bersama selector yang lain. Untuk lebih jelasnya coba kita lihat contoh berikut:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <style>
        /* Menargetkan seluruh tipe elemen */
        * {
            color: blue;
        }

        /* Menargetkan seluruh tipe elemen yang mengandung nilai "en" pada atribut lang */
        * [lang^=en] {
            font-style: italic;
        }

         /* Menargetkan seluruh tipe elemen yang memiliki nilai "warning" pada atribut class */
         *.warning {
             color: red;
         }

         /* Menargetkan seluruh tipe elemen yang memiliki nilai "content" pada atribut id */
         *#content {
             border: 1px solid blue;
             padding: 20px;
         }
    </style>
</body>
<p>
    Ini adalah paragraf biasa atau tidak menetapkan atribut apapun. Maka teks ini berwarna biru
</p>
<p lang="en-us">This is an English paragraph contains en-us value of lang attribue, so this text will be blue and italic </p>

<h1>Ini adalah header biasa</h1>
<h1 lang="en-us">This is an English Header</h1>
<p class="warning">Perhatikan paragraf ini! Paragraf ini adalah paragraf yang memiliki kelas bernilai warning,
   sehingga teks dari paragraf ini akan berwarna merah</p>
 
<div id="content">
   <p>Ini merupakan sebuah teks di dalam sebuah div yang memiliki id bernilai "content", seharusnya paragraf ini
       dibungkus dalam border yang memiliki padding 20px</p>
</div>
</html>
```
<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/5.%20Pendalaman%20CSS/img/Screenshot%202022-06-01%20010632.png" alt="screenshot">
</p>
