# Mengenal Font Weight, Font Style, dan Font Variant

## font-weight 
Selanjutnya ada juga <i>font-weight</i> yang digunakan untuk mengatur ketebalan dari <i>font</i> yang ditampilkan. Nilai dari properti ini dapat ditentukan dengan menggunakan <i>numeric values</i>(100 sampai 900) atau dengan menggunakan <i>descriptive terms</i> (normal, bold, bolder, dan lighter). Properti <i>font-weight</i> dapat diaplikasikan ke seluruh elemen yang ada di HTML dan nilainya dapat diturunkan pada elemen turunannya.

## font-style
Properti selanjutnya adalah <i>font-style</i>. Properti ini digunakan untuk menentukan postur dari teks yang ditampilkan, apakah bentuknya vertikal (normal) atau miring (italic dan oblique).

<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/5.%20Pendalaman%20CSS/img/Screenshot%202022-07-22%20215932.png" alt="null">
</p>

<i>italic</i> dan <i>oblique</i> keduanya menampilkan teks yang miring. Perbedaanya adalah <i>italic</i> menerapkan tipe miring(<i>italic font version</i>)
dari suatu font sedangkan <i>oblique</i> adalah font normal yang hanya dibuat miring.

Properti <i>font-style</i> dapat diaplikasikan ke seluruh elemen yang ada di HTML dan nilainya dapat diturunkan pada elemen turunannya.

## font-variant
Kita terbiasa dnegan aplikasi <i>document editor (rich text)</i> seperti Microsoft Word, tentu tahu atau sudah mencoba fitur <i>small caps</i>. Fitur ini dapat membuat teks menjadi kapital tetapi dituliskan secara kecil dan merapat, seperti ini:

<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/5.%20Pendalaman%20CSS/img/Screenshot%202022-07-24%20132327.png" alt="null">
</p>

Untuk membuat tulisan seperti gambar di atas, kita bisa memanfaatkan properti ```font-variant``` dengan nilai small-caps pada propertinya. Properti <i>font-variant</i> dengan nilai small-caps pada propertinya. Properti <i>font-variant</i> dapat diaplikasikan ke seluruh elemen yang ada di HTML dan nilainya dapat diturunkan pada elemen turunannya.

## Shorthand
Menspesifikasikan masing-masing nilai properti font akan menghasilkan banyak sekali kode repetitif. Dengan begitu CSS memberikan suatu "jalan pintas" untuk menuliskan properti-properti tersebut ke dalam satu properti yaitu font. Dengan menggunakan properti font kita dapat menuliskan beberapa properti hanya dalam satu properti pada satu rule.

<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/5.%20Pendalaman%20CSS/img/Screenshot%202022-07-24%20133743.png" alt="null">
</p>

Nilai dari <i>properti font</i> merupakan nilai dari seluruh properti dari font yang sudah kita bahas. Tiap nilai dipisahkan dengan menggunakan spasi. Pada properti ini urutan nilai merupakan hal yang penting, sehingga jangan sampai salah urutan dalam menuliskannya. Kesalahan penulisan atau urutan menyebabkan seluruh struktur rule menjadi tidak valid. Walaupun bagitu kita bisa tidak menuliskan seluruh nilai properti yang ada, tetapi nilai dari properti <i>font-size</i> dan <i>font-family</i> wajib ada ketika menggunakan properti ini. Berikut contohnya penulisan minimal ketika menggunakan properti ```font```:

```css
p {
    font: 1em sans-serif;
}
```


