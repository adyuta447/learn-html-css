# Mengenal Styling CSS Lebih Dalam 
Ada banyak jenis <i>Selector</i> untuk menargetkan aturan ke elemen tertentu dalam dikumen HTML. Pada materi sebelumnya, kita sudah mengetahui salah satu cara dasar dalam menggunakan <i>selector</i>. Sekarang mari kita bahas lebih detail mengenai berbagai maca <i>Selector</i> yang ada.

## Selector Basic
Pada materi sebelumnya kita sudah mengetahui apa itu selector, dan menggunakannya. Yang kita gunakan tersebut merupakan <i>selector basic</i>. Sebenarnya terdapat beberapa macam dari <i>selector basic,</i> yakni:

- Type Selector
- Class Selector
- ID Selector
- Attribute Selector
- Universal Selector

## Type Selector 
<i>Type Selector</i> menggunakan nama elemen sebagai terget untuk diterapkannya rule. Dengan kata lain, ketika menggunakan <i>selector</i> ini tentu akan diterapkan pada seluruh elemen target yang ada pada dokumen HTML. Coba kita lihat contoh berikut ini:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        span {
            color: red;
        }
    </style>
</head>
<body>
    <span>Ini merupakan sebuah teks yang berada pada elemen span. Seharusnya elemen ini ditampilkan dengan warna teks merah. </span>
    <p>Ini merupakan sebuah teks yang berada pada elemen paragraf, teks ini tidak akan terpengaruh oleh rule.</p>
    <span>Ini merupakan sebuah teks yang berada pada elemen span lainnya. Seharusnya ditampilkan dengan warna teks merah juga.</span>
</body>
</html>
```

Jika berkas tersebut dibuka pada sebuah browser, maka teks yang berada pada setiap elemen ```<span>``` akan berwarna merah.

<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/5.%20Pendalaman%20CSS/img/Screenshot%202022-05-20%20135118.png" alt="screenshot">
</p>

## Class Selector 

Class Selector menetapkan target elemen berdasarkan nilai dari atribut class html yang diterapkan pada elemennya. Untuk penulisan <i> selector</i>, diawali dengan tanda titik(.) kemudian lanjutkan dengan nama class nya. Lihatlah pada contoh berikut ini:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        .green {
            color: green;
        }
        .purple-bg {
            background-color: purple;
        }
        .fancy {
            font-weight: bold;
            text-shadow: 4px 4px 3px #000;
        }
    </style>
</head>
<body>
    <p class="green">Paragraf ini berwarna hijau</p>
    <p class="purple-bg">Paragraf ini berwarna ungu</p>
    <p class="fancy">Paragraf ini bergaya fancy</p>
    <p> Paragraf yang menampilkan teks dengan warna standar tanpa menerapkan styling</p>
</body>
</html>
```
Jika file/berkas tersebut dibuka pada browser, maka akan tampak seperti ini:

<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/5.%20Pendalaman%20CSS/img/Screenshot%202022-05-20%20141120.png" alt="screenshot">
</p>

Class juga bersifat shareable, sehingga dapat diterapkan pada banyak elemen dengan tipe elemen yang berbeda. Misalkan sebuah class ```green``` dapat diterapkan pada elemen paragraf dan juga heading untuk menampilkan teks berwarna hijau
```html
    <h2 class="green">Heading ini berwarna hijau</p>
    <p class="green">Paragraf ini berwarna hijau</p>
```
Tidak hanya itu, sebuah elemen juga mungkin memiliki banyak nilai class, sehingga kita dapat menerapkan lebih dari satu rule atau gabungan rule pada elemen target. Untuk menggunakannya, pada atribut ```class``` kita cukup tuliskan nama kelasnya dan pisahkan tiap kelasnya dengan spasi.

```html
    <h2 class="green purple-bg">Heading ini berwarna hijau dengan background ungu</p>
    <p class="green purple-bg">Paragraf ini berwarna hijau dengan background ungu</p>
```

Kita juga bisa menargetkan elemen secara spesifik yang memiliki sebuah class. Bagaimana jika kita ingin menerapkan gaya yang berbeda ketike menggunakan class fancy pada sebuah paragraf? Untuk melakukan itu, pada selector mari kita tuliskan nama elemen target diikuti dengan titik(.) kemudian nama kelasnya. Coba perhatikan pada contoh berikut ini:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        p.fancy {
            font-weight: bold;
            text-shadow: 4px 4px 3px #000;
        }
        .fancy {
            font-weight: bold;
            text-shadow: 4px 4px 3px #242F9B;           
        }
    </style>
</head>
<body>
    <h1 class="fancy">Ini merupakan heading yang bergaya fancy</h1> 
    <p class="fancy">Paragraf ini bergaya fancy</p>
</body>
</html>
```

Jika file/berkas tersebut dibuka pada browser, maka gaya ```fancy``` yang diterapkan pada elemen heading dan elemen paragraf akan berbeda.

<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/5.%20Pendalaman%20CSS/img/Screenshot%202022-05-20%20151306.png" alt="screenshot">
</p>
