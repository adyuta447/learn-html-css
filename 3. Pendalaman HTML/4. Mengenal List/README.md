# List
Seperti yang sudah disebutkan pada pembahasan paragraf, tidak semua teks dibungkus oleh paragraf, salah satunya list. Kita pun terbiasa membuat list dalam kehidupan sehari-hari, baik membuat to-do list atau daftar yang terstruktur sekalipun.<br>

Pada HTML terdapat tiga tipe list, yaitu:
- Unordered lists : daftar yang ditampilkan tidak memiliki urutan. 
- Ordered lists : daftar yang ditampilkan secara terurut.
- Description lists : daftar yang terbuat dari beberapa istilah diikuti dengan deskripsi dari istilah tersebut.

## Unordered List ```<ul>```
Seperti namanya, unordered list merupakan daftar yang tidak mementingkan urutan. Standarnya, unordered list menampilkan bullet pada tiap item list-nya (tetapi kita bisa mengubahnya dengan styling). <br/>

Untuk menetapkan konten sebagai unordered list kita gunakan ```<ul></ul>``` kemudian di dalam elemen tersebut kita gunakan tags ```<li></li>``` untuk menetapkan item pada list tsb. Contoh penerapannya sebagai berikut:

```html
<ul>
   <li>Item 1</li>
   <li>Item 2</li>
   <li>Item 3</li>
   <li>Item 4</li>
</ul>
```
Ketika kita membukanya pada browser, maka akan nampak seperti ini:

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-07_22-20.png)

Di antara <i>tag</i> elemen ```<li>```, kita dapat mengisikan konten apapun termasuk elemen HTML lain. Contohnya kita dapat memasukkan sebuah <i>heading</i> atau paragraf pada item.

```html
<ul>
   <li><h1>Sebuah Heading sebagai item list</h1></li>
   <li><h2>Sebuah Heading level 2 sebagai item list</h2></li>
   <li><p>Sebuah paragraf sebagai item list</p></li>
</ul>
```
Seperti yang kita sudah ketahui, maka list item akan menampilkan seperti format <b>header</b>.

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-07_22-31.png)

Kita juga bisa menyimpan kembali elemen ```<ul>``` untuk membuat sebuah nested list.

```html
<ul>
   <li>List item 1</li>
   <li>List item 2</li>
   <li>List item 3
       <ul>
           <li>List item 3.1</li>
           <li>List item 3.2</li>
           <li>List item 3.3</li>
       </ul>
   </li>
   <li>List item 4</li>
</ul>
```
## Ordered List ```<ol>```
Ordered list digunakan untuk membuat list yang mementingkan urutan. Contohnya, membuat daftar instruksi langkah demi langkah sehingga dibutuhkan urutan yang sesuai. Ordered list bekerja seperti unordered list, namun perbedaanya pada tiap item menampilkan angka bukan sebuah bullet. Angka yang ditampilkan, otomatis berurut tiap itemnya, sehingga kita tidak perlu menuliskan secara kasar urutan nomornya. Hal ini tentu mempermudah kita untuk mengorganisir tiap itemnya.

Untuk menetapkan konten sebagai ordered list kita gunakan ```<ol></ol>```. Sama seperti Unordered list, tiap item dalam list ditetapkan dengan menggunakan tags ```<li></li>```.

```html
<ol>
   <li>Langkah pertama</li>
   <li>Langkah kedua</li>
   <li>Langkah ketiga</li>
   <li>Langkah selanjutnya</li>
</ol>
```
Ketika kita membukanya pada browser, maka akan nampak seperti ini:

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-07_22-52.png)

Sama seperti pada unordered list, di antara tag elemen ```<li>``` kita dapat mengisikan konten apapun termasuk elemen HTML lain.<br />

Pada ordered list, tipe urutan angkanya dapat kita atur melalui sebuah atribut ```type```. Contohnya, selain nomor ururtan angka dapat menggunakan alfabet ataupun angka romawi.

```html
<ol type="I">
   <li>Langkah pertama</li>
   <li>Langkah kedua</li>
   <li>Langkah ketiga</li>
   <li>Langkah selanjutnya</li>
</ol>
 
<ol type="A">
   <li>Langkah pertama</li>
   <li>Langkah kedua</li>
   <li>Langkah ketiga</li>
   <li>Langkah selanjutnya</li>
</ol>
```

ketika kita membuka browser maka akan seperti ini:

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-08_19-45.png)

Berikut merupakan nilai - nilai yang dapat digunakan pada atribut ```<type>``` pada elemen ```<ol>```:

| Nilai | Deskripsi |
|:-------|:---------:|
| 1 | Menggunakan angka dalam urutan item(default) |
| a | Menggunakan huruf kecil dalam urutan item |
| A | Menggunakan huruf besar dalam urutan item |
| i | Menggunakan huruf romawi kecil dalam urutan item |
| I | Menggunakan huruf romawi besar dalam ururtan item |

Selain tipe angka pada urutan, kita juga bisa menerapkan nilai awal pada sebuah ordered list dengan menggunakan atribut ```start```. Contohnya, pada saat kita ingin memulai sebuah list dari angka 7, maka kita tetapkan atribut ```start``` dengan nilai 7 pada elemen ```<ol>```.

```html
<ol start="7">
   <li>Langkah ketujuh</li>
   <li>Langkah kedelapan</li>
   <li>Langkah kesembilan</li>
   <li>Langkah selanjutnya</li>
</ol>
```
Maka hasil yang ditampilkan akan dimulai dengan nilai urutan ke-7.

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-08_19-55.png)

Normalnya ururtan list diawali dengan urutan paling tendah dengan menambahkan atribut ```reversed``` pada elemen ```<ol>```, urutan dalam sebuah list akan dibalik. Atribut ini berbeda dengan atribut yang lain (yang sudah dibahas sebelumnya), atribut ini tidak memerlukan sebuah nilai ketika menggunakannnya. Atribut ini hanya menandakan sebuah <b>list</b> untuk membalikkan urutan angka pada tiap itemnya.

```html
<ol reversed>
   <li>Langkah keempat</li>
   <li>Langkah ketiga</li>
   <li>Langkah kedua</li>
   <li>Langkah kesatu</li>
</ol>
```
Jika kita buka pada browser maka jadi seperti ini:

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-08_20-11.png)
