# Mengenal Attribute Dalam HTML
Elemen dituliskan dengan awalan tag pembuka <> dan diakhiri dengan tag penutup </>. Ada satu hal lagi yang bisa kita tuliskan pada sebuah elemen, lebih tepatnya tag pembuka, yaitu <b>Attribute</b>. Atribut ini berfungsi memberikan informasi tambahan pada sebuah elemen. Atribut dituliskan pada tag pembuka sebuah elemen setelah nama dari elemennya tersebut ditulis. Contohnya:
```html
<p lang="id">Yogyakarta mendapat berbagai macam julukan seperti Kota Pelajar, Kota Gudeg, Kota Perjuangan, maupun Kota Budaya</p>
```
Contoh kode tersebut, kita bisa menetapkan atribut bahasa(dengan penulisan lang) dengan nilai <b>"id"</b> atau Indonesia pada sebuah elemen paragraf. Kode bahasa lainnya bisa kita explore pada link berikut:
[https://www.w3schools.com/tags/ref_language_codes.asp](https://www.w3schools.com/tags/ref_language_codes.asp)

Untuk menuliskan sebuah atribut kita memerlukan nama dari atribut itu diikuti dengan nilai atribut tersebut dalam bentuk <i>string</i>(Ditulis dalam tanda kutip dua). Untuk lebih jelasnya, coba kita lihat gambar berikut:

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-06_19-21.png)

Atribut pada elemen juga dapat dituliskan lebih dari satu. Kita bisa menuliskan struktur atribut di samping atribut yang sudah ada. Seperti contoh berikut ini:

```html
<p lang="id" translate="no">Yogyakarta mendapat berbagai macam julukan seperti Kota Pelajar, Kota Gudeg, Kota Perjuangan, maupun Kota Budaya</p>
```
Dengan menambah atribut ```translate``` dan memberikan nilai <b>"no"</b> pada elemen paragraf tsb, maka konten dari elemen yang dimaksud tidak akan diterjemahkan oleh layanan sistem translate seperti <b>Google Translate</b>.

Pada HTML terdapat dua jenis atribut, yaitu <b>Global Attribute</b> dan atribut yang hanya bisa digunakan pada elemen tertentu. Untuk atribut yang spesifik pada sebuah elemen, kita akan mengulasnya pada pembahasan elemen tsb. Untuk Global Attribute, berikut daftar yang kita bisa gunakan di seluruh elemen HTML.

| Attribute | Fungsi |
| :--------- | :-----: |
| accesskey | Menentukan tombol shortcut untuk mengaktifkan/memfokuskan pada sebuah element. |
| class | Menentukan satu atau lebih classname untuk sebuah elemen. |
| contenteditable | Menentukan konten dari elemen merupakan konten yang dapat diubah atau tidak. |
| data-* | Digunakan untuk menyimpan sebuah data pribadi khusus ke halaman atau aplikasi. |
| dir | Menentukan arah teks untuk konten pada suatu elemen. |
| draggable | Menentukan apakah suatu elemen dapat di-drag atau tidak. |
| dropzone | Menentukan apakah data yang di-drag adalah data yang disalin, dipindahkan, atau ditautkan saat dijatuhkan. |
| hidden | Menentukan apakah suatu elemen ditampilkan atau tidak pada browser. |
| id | Menetapkan id pada elemen. |
| lang | Menentukan bahasa pada konten elemen. |
| spellcheck | Menentukan apakah elemen harus diperiksa ejaannya dan tata bahasanya atau tidak. |
| style | Menentukan styling secara satu baris untuk suatu elemen. |
| tabindex | Menentukan urutan dari suatu elemen. |
| title | Menentukan informasi tambahan tentang suatu elemen. |
| translate | Menentukan apakah konten elemen harus diterjemahkan atau tidak. |
