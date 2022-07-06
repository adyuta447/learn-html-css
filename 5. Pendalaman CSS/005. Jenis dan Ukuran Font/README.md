# Jenis dan Ukuran Font 
## Font Styling
Ketika kita membuat sebuah dokumen teks, termasuk dokumen cetak, langkah awal biasanya adalah menentukan jenis font yang akan digunakan. Pada pengembangan website pun seperti itu. Dalam CSS, Font ditentukan dengan menggunakan beberapa paket porperti font. Kita bisa atur tipe font, ukuran, ketebalan, dan gaya. 

- font-family : Menetapkan jenis font yang akan diterapkan pada target.
- font-size : Menentukan ukuran pada teks.
- font-weight : Menentukan ketebalan pada teks.
- font-style : Menetapkan styling yang diterapkan pada teks.
- font-variant : Menentukan teks untuk menggunakan gaya <i>small caps</i>(huruf kepital kecil).
- font : Shorthand dari properti font yang ada.

## Font-family
Pada pengenalan CSS kita sudah mencoba menggunakan <i>font-properties</i> untuk mengubah standar font yang ditampilkan pada browser dengan menggunakan ```font-family``` pada elemen ```<body>```.

```css
body {
    font-family: sans-serif;
}
```
Pada rule tersebut kita mengubah standar font yang digunakan browser dengan font '<i>sans-serif</i>'. Sebenarnya untuk nilai dari properti ini dapat lebih dari satu biasa dikenal sebagai <i>font stack</i>. Tujuannya adalah sebagai <i>fallback</i> jika terjadi kegagalan dalam menggunakan font yang kita gunakan. Untuk menuliskan lebih dari satu font, berikut ini aturan yang harus kita perhatikan adalah: 

<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/5.%20Pendalaman%20CSS/img/Screenshot%202022-07-02%20221450.png" alt="screenshot">
</p>

- Seluruh font yang bukan merupakan <i>generic font families</i> harus dituliskan secara kapital. Seperti "Arial" bukan dituliskan "arial".
- Gunakan tanda koma (,) untuk memisahkan antar nilai <i>font</i> yang digunakan. 
- Selalu tanda kutip (") untuk membungkus nilai font yang memiliki spasi pada namanya 

Mungkin ada pertanyaan seperti ini mengapa sih kita perlu memberikan lebih dari satu nilai pada font-family? Hal tersebut penting karena tidak semua browser mendukung semua jenis font. Memberikan lebih dari satu nilai font dapat menawarkan alternatif tampilan font pada browser. Terutama jika font utama yang diterapkan tidak didukung oleh browser yang digunakan. Jadi font pertama didukung oleh browser, maka browser akan menggunakannya. Namun jika tidak, maka browser akan memeriksa nilai <i>font</i> yang kedua dan menggunakannya, demikian dan seterusnya.

Dalam memilih jenis font terdapat istilah yang dinamakan <b>web safe font</b>. Web safe font adalah jenis font yang umumnya sudah pasti tersedia di sebagian besar komputer. Sehingga dapat dipastikan bahwa web akan terlihat sebagaimana mestinya pada browser. Berikut merupakan beberapa contoh font yang masuk ke kategori ini adalah:

- Arial (sans-serif)
- Verdana (sans-serif)
- Helvetica (sans-serif)
- Tahoma (sans-serif)
- Trebuchet MS (sans-serif)
- Times New Roman (serif)
- Georgia (serif)
- Garamond (serif)
- Courier New (monospace)
- Brush Script MT (cursive)

## Font-size
Mengubah nilai font pada sebuah dokumen adalah hal yang sangat wajar terjadi, begitu pula dengan website. Untuk menetapkan ukuran font, kita perlu menerapkan properti <i>font-size</i>. Kita bisa menetapkan nilai dari properti ini dengan menuliskan langsung nilai dan satuannya. Contohnya seperti ini:

```css
h1 {
    font-size: 2px
}

/** Contoh penulisan yang salah **/
h1 {
    font-size: 2 px;
    /* Rule tidak akan diterapkan pada target karena kesalahan penulisan nilai properti */
}
```
Satuan dalam menetapkan ukuran font terdapat dua jenis. Yang pertama <i>relative</i>, yakni satuan yang nilainya tergantung pada sesuatu hal, contohnya ukuran dari <i>viewport</i>, induk elemen ataupun ukuran teks standar. Dan yang kedua adalah <i>absolute</i>, yakni satuan yang nilainya telah ditentukan atau digunakan dalam dunia nyata.

### Absolute unit

|Satuan|Fungsi|
|:-----|:----:|
|px | Menetapkan nilai font berdasarkan ukuran pixel |
|pt | Menetapkan nilai font berdasarkan points (1/72 inch di CSS2.1) |
|pc | Menetapkan nilai font berdasarkan picas(1 pica = 12pt) |
|mm | Menetapkan nilai font berdasarkan milimeters | 
|cm | Menetapkan nilai font berdasarkan centimeters |
|in | Menetapkan nilai font berdasarkan inches |  

### Relative unit

|Satuan|Relative pada|Fungsi|
|:----|:-------------|:-----|
|em | Font size | Satuan relatif terhadap ukuran font yang sedang digunakan pada elemen |
|ex | Font height | Satuan relatif terhadap tinggi font saat ini, satuan snagat jarang sekali digunakan |
|rem | Font size | Mirip seperti em, tetapi rem merupakan satuan relatif terhadap ukuran font dari root elemen |
|ch | Font width | Satuan relatif terhadap 1% lebar viewport. Contoh 1vw = 1% dari lebar viewport. Satuan ini tidak didukung pada browser IE8 ke bawah |
|vw | Viewport width | Satuan relatif terhadap 1% lebar viewport. Contoh 1vw = 1% dari lebar viewport. Satuan ini tidak didukung pada browser IE8 ke bawah |
|vh | Viewport height | Satuan relatif terhadap 1% tinggi viewport. Contoh 1vh - 1% dari tinggi viewport. Satuan ini tidak didukung pada browser IE8 ke bawah |

### Browser support
|Satuan|Chrome|Edge|Firefox|Safari|Opera|
|-----:|:----:|:--:|:-----:|:----:|:---:|
| em, ex, %, px, cm, mm, in, pt, pc | 1.0 | 3.0 | 1.0 | 1.0 | 3.5 |
| ch | 27.0 | 9.0 | 1.0 | 7.0 | 20.0 |
| rem | 4.0 | 9.0 | 3.6 | 4.1 | 11.6 |
| vh, vw | 20.0 | 9.0 | 19.0 | 6.0 | 20.0 |

Selain dengan menetapkan nilai dan satuannya secara langsung, untuk mengatur ukuran font kita juga bisa gunakan nilai persentase.

```css
body {
    font-size: 16px;
}

h1 {
    font-size: 150px;  /* 150% dari 16 = 24px */ 
}
```
Pada contoh ini ukuran  font dari elemen ```<h1>```  yang seharusnya memiliki ukuran 16px karena mewarisi dari induk elemennya (body). Namun, di bawahnya terdapat rule yang menargetkan secara spesifik untuk elemen ```<h1>``` untuk menerapkan ukuran font sebesar 150% dari ukuran induknya sehingga elemen ```<h1>``` akan nampak 50% lebih besar dari elemen lain yang ada di dalam ```<body>```.

<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/5.%20Pendalaman%20CSS/img/Screenshot%202022-07-06%20174630.png" alt="null">
</p>

Dan yang terakhir kita juga bisa menentukan ukuran <i>font</i> dengan menuliskan kata kunci secara spesifik yang tersedia pada CSS. Kata kunci itu adalah: <i>xx-small, x-small, small, medium, large, x-large, dan xx-large</i>. Kata kunci tersebut tidak ada kaitannya dengan pengukuran tertentu (bukan ukuran yang absolute) tetapi nilainya diubah secara konsisten satu sama lain. 
