# Menuliskan Aturan Styling

Sebuah <i>style sheet</i> dibuat terdiri dari satu atau lebih atura styling (biasa disebut dengan <i>rules</i> atau <i>rule-sets</i>) yang mendeskripsikan bagaimana sebuah elemen atau sebuah kelompok elemen ditampilkan dalam jendela browser.

Langkah awal belajar CSS adalah dengan memahami sebuah bagian rule. Berikut ini dua contoh rules yang dituliskan dalam sebuah CSS. Rule yang pertama menerapkan sebuah warna hijau pada elemen ```<h1>``` dan rule yang kedia menetapkan ukuran font dan tipe font pada sebueh elemen paragraf.

```css
h1 { color: blue; }

p {
    font-size: 2rem;
    font-family: sans-serif;
}
```
Dalam penggunaan CSS, terdapat dua bagian dalam sebuah rule. Yang pertama adalah identitas elemen atau elemen yang akan menerapkan <i>rule</i> (Singkatnya kita akan sebut <b>selector</b>) dan yang kedua adalah deklarasi atau insturksi yang akan diterapkan pada sebuah <b>selector</b>.

<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/4.%20Pengenalan%20CSS/img/Screenshot%202022-04-27%20012000.png" alt="screenshot">
<p>

## Selector
Pada contoh diatas, <i>h1</i> dan <i>p</i> digunakan sebagai selector. Selector ini dipanggil melalui tipe elemennya, dan ini merupakan teknik dasar dari pemanggilan selector. Properti dan nilainya yang terdapat pada <i>declaration/declaration block</i> akan diterapkan pada seluruh elemen ```<h1>``` dan ```<p>``` yang ada pada dokumen HTML. Pada materi selanjutnya kita akan mengetahui berbagai cara lainnya untuk menetapkan <i>selector</i> dengan lebih canggih lagi.

## Declarations
Bagian deklarasi terdiri dari pasangan properti dengan nilainya. Kita bisa menetapkan lebih dari satu deklarasi pada satu <i>rule</i>, contohnya seperti pada selector <i>p</i> di atas. Kita menetapkan lebih dari satu deklarasi pada <i>declaration block</i>. Nah setiap deklarasinya harus diakhiri dengan (;) sebagai tanda diakhirinya sebuah deklarasi.

Karena CSS tidak memperhatikan spasi(sama seperti bahasa pemograman pada umumnya), sebaiknya penulisan deklarasi selalu diawali dengan garis baru supaya mudah dibaca dan juga mudah untuk dipahami.

```css
p {
    font-size: 2rem;
    font-family: sans-serif;
    /* Mendeklarasikan nilai properti lainnya pada garis baru */
}
```
Tapi ingat, walaupun CSS tidak memperhatikan spasi, untuk satuan nilai seperti px, em, rem dan lainnya harus dituliskan tanpa spasi pada nilainya. Lihatlah pada contoh berikut:

```css
p {
    font-size: 2rem;
}
```

Jika kita menambhakan spasi di antara satuan dan nilai, maka seklarasi tersebut tidak akan berfungsi. Seperti pada contoh berikut ini:

```css 
p {
    font-size: 2 rem; /*Deklarasi tidak akan berfungsi karena terdapat spasi antara nilai dan satuan*/
}
```

## CSS Comments
CSS comments digunakan untuk menjelaskan kode dan dapat membantu ketika Anda mengedit kode sumber di lain waktu. Apa yang tertulis akan diabaikan oleh browser dan tidak ditampilkan di browser, Sehingga dapat menjadi opsi baik untuk memberi catatan atau informasi dokumentasi pada kode.

Seperti contoh yang beberapa kali telah Anda lihat di atas, CSS commentts ditempatkan pada elemen ```<style>``` dengan cara penulisan dimulai dengan /* dan diakhiri */ seoerti contoh berikut:

```css
p {
    /* Ini merupalakan CSS comments */
    font-size: 2rem;
    font-family: sans-serif;
}
```






