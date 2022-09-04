# Text Styling

Sebelumnya kita terfokus pada formating bentuk karakter yang ditampilkan dengan menggunakan beberapa properti <i>font</i> yang ada. Sekarang kita akan mempelajari bagaimana seorang developer bisa memberikan formatting pada keseluruhan teks yang ada pada baris paragraf, seperti menetapkan <i>indent</i>, jarak antar baris, kata dan huruf , dan sebagainya. Maka dari itu, mari kita bahas satu persatu.

## Line Height
Properti ```line-height``` digunakan untuk mengatur jarak minimal dari garis dasar ke garis dasar dalam menampilkan teks pada halaman. Jika kita terbiasa dengan <i>software</i> document editor (rich text) seperti Microsoft Word, properti ini mirip dengan fungsi <i>line and paragraph spacing</i>

<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/5.%20Pendalaman%20CSS/img/ilustrasi.png" alt="ilustrasi">
</p>

Pada penjelasan diatas disebutkan "minimal", karena jika terdapat sebuah karakter yang tinggi atau besar dalam sebuah baris, maka tinggi dari baris pun akan menyesuaikan agar jarak tetap mengakomodirnya. Ini merupakan contoh tiga cara berbeda dalam menerapkan tinggi barus dua kali tinggi ukuran font:

```css
p {
    line-height: 2;
}

p {
    line-height: 200%;
}

p {
    line-height: 2em;
}
```

Cara pertama merupakan cara yang paling mudah digunakan, karena kita dapat menentukan nilai hanya dengan satu angka, di mana angka tsb nantinya dikalikan dengan nilai ```font-size``` sebelum diterapkan pada nilai properti ```line-height```. Contohnya, ukuran font standar pada paragraf adalah 16 pixel. Kita definisikan properti ```line-height``` dengan nilai 2, maka nilai properti ```line-height``` seharusnya adalah <b>16 pixel = 32 pixel(dua kali lebih besar dari ukuran font).</b> Properti ```line-height``` dapat diaplikasikan ke seluruh elemen yang ada pada HTML dan nilainya dapat diturunkan pada elemen turunannya.

## Text Indent
Dalam membuat sebuah dokumen tidak jarang kita membutuhkan jarak di awal paragraf. Hal tersebut dapat dilakukan pada website dengan menerapkan properti ```text-indent```. Kita dapat menentukan nilai properti ini melalui perhitungan panjang dalam ```px```, ```em```, dan ```in``` atau bisa menggunakan nilai persentase (%). Nilai persentase dihitung berdasarkan lebar dari induk elemen. Berikut merupakan contoh penggunaannya:

```css
p#first {
   text-indent: 2em;
}
 
p#second {
   text-indent: 25%;
}
 
p#third {
   text-indent: -35px;
}
```

Jika elemen menerapkan <i>rule</i> tersebut, akan tampak seperti ini:

<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/5.%20Pendalaman%20CSS/img/ilustrasi-text-indent.png" alt="ilustrasi" /></p>

Pada contoh ke-tiga kita bisa melihat bahwa pada nilai properti ini dapat diberikan nilai negatif. Jika kita menggunakannya, maka baris pertama pada paragraf akan keluar dari batas elemen yang menampungnya (ini biasa disebut <b>hanging indent</b>). Perlu diingat kembali, bahwa properti ini hanya berpengaruh pada awal baris paragraf. Jika kita ingin menetapkan untuk seluruh baris kita dapat gunakan <i>margin</i> atau <i>padding</i>.


## Text Alignment
Kita bisa mengatur <i>text alignment</i> (perataan teks) pada <i>website</i> seperti kita melakukannya pada aplikasi Microsoft Word dengan menggunakan properti ```text-align```. Untuk asalnya, properti ini bernilai <i>left</i> atau biasa disebut rata kiri. Namun jika kita ingin mengubah preataan teks ini berada di posisi lainnya, maka kita dapat mengubah valuenya menjadi value yang sesuai dengan keinginan kita.

| Nilai Properti | Fungsi |
|:---------------|:-------|
| text-align: <b>left</b> | Membuat perataan teks pada ujung kiri | 
| text-align: <b>right</b> | Membuat teks pada ujung kanan |
| text-align: <b>center</b> | Membuat teks secara menengah |
| text-align: <b>justify</b> | Membuat perataan teks yang setara pada ujung kiri dan kanannya |

Berikut ini merupakan contoh penggunaan dari properti ```text-align```:

```css
p#first {
    text-align: left;
}
 
p#second {
    text-align: right;
}
 
p#third {
    text-align: center;
}
 
p#fourth {
    text-align: justify;
}
```

Jika elemen menerapkan rule tersebut, akan tampak seperti ini:

<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/5.%20Pendalaman%20CSS/img/Screenshot%202022-09-04%20103404.png" alt="null" >
</p>
