# Struktur Dasar Sebuah Tabel

Tabel pada HTML disusun dari tiga buah elemen, yaitu ```<table>```, ```<tr>``` sebagai "<i>table row</i>", dan ```<td>``` sebagai "<i>table data</i>" atau ```<th>``` sebagai "Table head". Elemen ```<table>``` digunakan untuk menandakan dimulai dan diakhirinya sebuah konten tabel dan juga sebagai wadah untuk tabel itu sendiri. Kemudian, elemen ```<tr>``` digunakan untuk membuat sebuah baris baru yang di dalamnya terdapat elemen ```<td>``` atau ```<th>``` sehingga menghasilkan sebuah  <i>cell</i>.

Elemen ```<td>``` yang berarti "<i>table data</i>" selain membuat <i>cell</i> elemen ini juga merupakan tempat di mana data pada tabel ditampung. Selanjutnya untuk elemen ```<th>``` atau "<i>table header</i>" digunakan untuk menentukan sebuah header pada kolom datanya. Untuk lebih jelasnya perhatikan ilustrasi berikut:

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/ilustrasi01.png)

Cukup mudah dimengerti kan? Sekarang mari kita ubah menjadi penerapan elemen HTML

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/ilustrasi02.png)

Berdasarkan ilustrasi di atas, kita dapat menuliskan sebuah struktur dasar tabel pada html sepeti berikut:

```html
<h1>Pemenang Piala Dunia tiga tahun terakhir</h1>
 
<table>
   <tr>
       <th>Tahun</th>
       <th>Juara 1</th>
       <th>Juara 2</th>
       <th>Juara 3</th>
   </tr>
   <tr>
       <td>2018</td>
       <td>Prancis</td>
       <td>Kroasia</td>
       <td>Belgium</td>
   </tr>
   <tr>
       <td>2014</td>
       <td>Jerman</td>
       <td>Argentina</td>
       <td>Belanda</td>
   </tr>
   <tr>
       <td>2010</td>
       <td>Spanyol</td>
       <td>Belanda</td>
       <td>Jerman</td>
   </tr>
</table>
```

Jika dibuka pada browser, maka akan tampak seperti ini:

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/Screenshot%202022-04-09%20163417.png)

Perlu kita ingat bahwa seluruh konten atau data dituliskan pada elemen ```<td>``` ataupun ```<th>```. Kita bisa memberikan konten apa saja di dalamnya seperti teks, gambar, atau tabel lainnya.