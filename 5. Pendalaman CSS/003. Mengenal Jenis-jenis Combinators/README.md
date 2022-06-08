# Jenis-jenis Combinators
Tak terasa kita sudah mengetahui beberapa <i>basic selector</i> yang ada pada CSS. Kita juga tidak lupa akan CSS Selector yang berisi lebih dari satu basic selector. Di antara basic selector, kita dapat mempelajari sebuah kombinator. Ada empat kombinator yang dapat kita gunakan yaitu: <i>Adjacent Sibling Selector</i>, <i>General Sibling Selector</i>, <i>Child Selector</i>, dan juga <i>Descedant Selector</i>. Mari kita bahas satu persatu, terutama kita akan membahas Adjacent Sibling Selector dan General Sibling Selector.

## Adjacent Sibling Selector (+)

<i>Adjacent Sibling Selector</i> merupakan gabungan dua buah basic selector dengan menggunakan tanda + di antara keduanya.

```css
h1 + p {
    color: blue;
}
```
</i>Adjacent Sibling Selector<i> terdiri dari dua buah target elemen, namun hanya elemen kedua yang menerapkan rule selama elemen tersebut ditulisakan langsung setelah elemen pertama pada berkas HTML. Selain itu kedua elemen tersebut harus berada di dalam induk elemen yang sama. Pada contoh di atas rule yang akan diterapkan pada elemen paragraf yang berada tepat setelah elemen gambar.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        h1 + p {
            color: blue;
        }
    </style>
</head>
<body>
    <p>Ini merupakan paragraf pertama. Rule styling tidak akan diterapkan pada elemen paragraph ini.</p>   
    <h1>Ini meruparakan header1. Maka Rule styling tidak akan diterapkan</h1>
    <p>Ini merupakan paragraph dan ditetapkan setelah header1. Maka Maka paragraf ini seharusnya menerapkan rule dengan menampilkan teks berwarna biru</p>
</body>
</html>
```
<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/5.%20Pendalaman%20CSS/img/Screenshot%202022-06-08%20022407.png" alt="screenshot">
</p>

General Sibling Selector (~)
 
Mirip seperti Adjacent Sibling Selector namun rules akan diterapkan pada seluruh elemen kedua yang berada setelah elemen pertama. Dengan catatan, indukny sama, walaupun posisi dari elemen kedua tidak berada tepat setelahnya. General Sibling Selector menggunakan tanda (~) untuk menetapkan elemennya.

```css
img ~ p {
    color: blue;
}
```
Rule di atas akan diterapkan pada elemen paragraf yang berada setelah elemen img selama masih di dalam induk yang sama.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        h1 ~ p {
            color: blue;
        }
    </style>
</head>
<body> 
    <h1>Ini meruparakan header1. Maka Rule styling tidak akan diterapkan</h1>
    <p>Ini merupakan paragraph dan ditetapkan setelah header1. Maka paragraf ini seharusnya menerapkan rule dengan menampilkan teks berwarna biru</p>
    <div>
        <p>Ini merupakan paragraph dan tidak ditetapkan rule styling</p>
    </div>
    <p>Ini merupakan paragraph. Maka paragraf ini seharusnya menerapkan rule dengan menampilkan teks berwarna biru</p>
</body>
</html>
```

<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/5.%20Pendalaman%20CSS/img/Screenshot%202022-06-09%20014814.png" alt="screenshot">
</p>