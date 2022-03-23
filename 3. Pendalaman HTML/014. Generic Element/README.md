# Generic Element 
Setelah mengenal beberapa elemen yang ada, bagaimana jika tidak terdapat elemen sesuai yang mempu menggambarkan konten kita? Dalam dunia nyata, jenis informasi sangat beragam dan mungkin tidak semua semantik elemen yang kalian ketahui dapat menggambarkan jenis informasinya. Untungnya, HTML menyediakan dua tipe elemen umum (generic element) yang bisa kita kustomisasi untuk menggambarkan konten kita dengan tepat.

Terdapat dua generic elemen yang dapat kita manfaatkan.

## Div

Yang pertama elemen ```<div>```, elemen ini merupakan sebuah wadah (container) yang bersifat umum untuk menampung beberapa konten. Elemen ini tidak akan memberikan efek apapun pada konten atau layout sebelum menerapkan sebuah style menggunakan CSS.

```html
 <div>Paragraf ini berada di dalam elemen div, namun akan ditampilkan sama seperti paragraf biasanya.</div>
```

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-23_16-17.png)

Sebagai sebuah wadah yang murni, elemen ```<div>``` tidak merepresentasikan apapun. Elemen ini lebih sering digunakan untuk mengelompokkan sebuah konten sehingga dapat memudahkan <i>styling</i> dengan menggunakan atribut ```class``` atau ```id```.

```html
<!DOCTYPE html>
<html>
 
<head>
   <title>Div Element</title>
   <style>
       .shadowbox {
           width: 15em;
           border: 1px solid #333;
           box-shadow: 8px 8px 5px #444;
           padding: 8px 12px;
           background-color: #F3E9DD; 
           border-radius: 1rem;
       }
   </style>
</head>
 
<body>
   <div class="shadowbox">
       <p>Paragraf ini berada di dalam elemen div, namun akan ditampilkan sama seperti paragraf biasanya. Elemen ini lebih sering digunakan untuk mengelompokkan sebuah konten sehingga dapat memudahkan styling dengan menggunakan atribut class atau id.
       </p>
   </div>
</body>
 
</html>

```
Jika kita menerapkan styling seperti di atas, maka akan terlihat efek dari penggunaan ```<div>``` ini.

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-23_20-36.png)

## Span 

Yang kedua elemen ```<span>```, elemen ini memberikan manfaat yang sama seperti ```<div>```, bedanya elemen ini digunakan sebagai <b>pharse elements</b> dan tidak terdapat <i>line breaks</i> ketika menggunakannya. Sederhananya, ```<span>``` merupakan sebuah ```<div>``` yang digunakan dalam sebuah baris teks yang dapat diwadahi oleh paragraf, list, heading atau lainnya.

Mari kita ambil contoh. Tidak ada elemen pada inline element yang memiliki arti untuk menampung sebuah informasi telepon. Maka dari itu, tiap item pada nomor telepon bisa ditampung dalam elemen ```<span>``` dan diklasifikasikan(menggunakan atribut <i>class</i>) dengan nilai <b>"phone"</b>.

```html
<ul>
   <li>Agil: <span class="phone">08123xxx</span></li>
   <li>Widy: <span class="phone">08222xxx</span></li>
   <li>Gilang: <span class="phone">08333xxx</span></li>
</ul>
```
Dengan menggunakan elemen ```<span>```, kita dapat menentukan sebuah <i>styling</i> pada teks tsb.

```html
<!DOCTYPE html>
<html>
 
<head>
   <title>Div Element</title>
   <style>
        .phone {
            font-weight: bold;
        }
   </style>
</head>
 
<body>
    <ul>
        <li>Rehan: <span class="phone">08123xxx</span></li>
        <li>Dhimas: <span class="phone">08222xxx</span></li>
        <li>Gilang: <span class="phone">08333xxx</span></li>
     </ul>
</body>
 
</html>
```
Jika kita coba lihat pada browser, akan tampak seperti ini:

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-23_21-04.png)

Contoh lainnya, kita juga bisa gunakan elemen ```<span>``` dalam sebuah paragraf.

```html
<!DOCTYPE html>
<html>
 
<head>
   <title>Div Element</title>
   <style>
       .bahan {
       color: red;
   }
   </style>
</head>
 
<body>
<p>Untuk membuat sebuah bakso kita membutuhkan <span class="bahan">daging sapi</span>, <span
       class="bahan">tepung tapioka</span>, <span class="bahan">bawang merah</span> dan <span class="bahan">bawang
putih</span> kemudian satu sendok makan <span class="bahan">gula</span> dan <span class="bahan">garam.</span></p>
</body>
 
</html>
```
Jika kita coba lihat pada browser, akan tampak seperti ini:

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-23_21-16.png)

