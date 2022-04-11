# Spanning Cell
Terkadang kita membutuhkan sebuah sel yang mencakup untuk dua kolom ataupun dua baris sekaligus. Dalam aplikasi seperti Microsoft Word, hal ini biasa kita kenal sebagai <i>merging cell</i> atau menggabungkan dua atau lebih sebuah sel. Ini memang menjadi sebuah fitur dasar dalam membuat sebuah tabel. Sehingga, pada HTML pun kita dapat melakukan hal tersebut.

Pada HTML hal ini lebih dikenal sebagai <i>Spanning cell</i> yang artinya menjangkau atau merentangkan sebuah ukuran sel lebih dari ukuran yang biasanya. Dengan <i>spanning cell</i> kita dapat membuat sebuah tabel yang lebih kompleks, tetapi akan membuat markup yang kita tulis menjadi sedikit sulit dibaca.

## Column Spans

Untuk merentangkan sebuah kolom (<i>column spanning</i>) kita bisa menggunakan atribut ```cosplan``` pada elemen ```<td>``` atau ```<th>```. Berikut contoh untuk penggunaan atribut ```cosplan``` sehingga sebuah <i>header</i> mencakup dua kolom.

```html
<table>
   <tr>
       <th>18:00</th>
       <th>19:00</th>
       <th>20:00</th>
   </tr>
   <tr>
       <td colspan="2">Avenger Infinity Wars</td>
       <td>It Chapter 2</td>
   </tr>
   <tr>
       <td>One Piece: Stampede</td>
       <td>Weathering With You</td>
       <td>Gundala</td>
   </tr>
   <tr>
       <td>Gundala</td>
       <td colspan="2">Avenger Infinity Wars</td>
   </tr>
</table>
```

Maka sebuah eleman yang menggunakan atribut ```colspan``` akan mencakup ruang kolom sesuai nilai dari atribut itu sendiri.

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/Screenshot%202022-04-10%20183936.png)

Untuk lebih jelasnya, kita bisa tambahkan atribut ```border``` pada elemen ```<table>``` agar terdapat garis pada tepi selnya. Value yang diberikan pada atribut ini berupa <i>integer</i> dalam pixel.

```html
<table border="1">
   <tr>
       <th>18:00</th>
       <th>19:00</th>
       <th>20:00</th>
   </tr>
   <tr>
       <td colspan="2">Avenger Infinity Wars</td>
       <td>It Chapter 2</td>
   </tr>
   <tr>
       <td>One Piece: Stampede</td>
       <td>Weathering With You</td>
       <td>Gundala</td>
   </tr>
   <tr>
       <td>Gundala</td>
       <td colspan="2">Avenger Infinity Wars</td>
   </tr>
</table>
```

Tampilkan pada browser:

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/Screenshot%202022-04-11%20163026.png)

## Row Spans

Untuk merentangkan sebuah baris(<i>row spanning</i>) kita dapat menggunakan atribut <i>rowspan</i>. Sama seperti <i>column spanning</i>, tetapi atribut ini akan merentangkan sebuah sel ke bawah. Berikut contohnya:

```html
<table border="1">
   <tr>
       <th rowspan="3">18:00</th>
       <td>Avenger Infinity Wars</td>
   </tr>
   <tr>
       <td>One Piece: Stampede</td>
   </tr>
   <tr>
       <td>Gundala</td>
   </tr>
</table>
```

Perhatikan elemen ```<th>``` yang diberi nilai atribut ```rowspan```. Elemen tersebut berada pada baris pertama dan akan memanjang menjadi tiga baris ke bawahnya. Jadi pada baris tersebut kita membuatuhkan dua buah elemen (```<th>``` dan ```<td>```) dan pada baris selanjutnya (baris dua dan tiga) kita hanya perlu satu buah elemen ```<td>``` saja di dalam elemen ```<tr>``` setelahnya. Sehingga jika dilihat pada <i>browser</i> akan nampak seperti ini:

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/Screenshot%202022-04-11%20202936.png)