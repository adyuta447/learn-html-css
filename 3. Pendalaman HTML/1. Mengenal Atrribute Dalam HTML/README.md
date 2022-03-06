# Mengenal Attribute Dalam HTML
Elemen dituliskan dengan awalan tag pembuka <> dan diakhiri dengan tag penutup </>. Ada satu hal lagi yang bisa kita tuliskan pada sebuah elemen, lebih tepatnya tag pembuka, yaitu Attribute. Atribut ini berfungsi memberikan informasi tambahan pada sebuah elemen. Atribut dituliskan pada tag pembuka sebuah elemen setelah nama dari elemennya tersebut ditulis. Contohnya:
```html
<p lang="id">Yogyakarta mendapat berbagai macam julukan seperti Kota Pelajar, Kota Gudeg, Kota Perjuangan, maupun Kota Budaya</p>
```
Contoh kode tersebut, kita bisa menetapkan atribut bahasa(dengan penulisan lang) dengan nilai <b>"id"</b> atau Indonesia pada sebuah elemen paragraf. Kode bahasa lainnya bisa kita explore pada link berikut:
![https://www.w3schools.com/tags/ref_language_codes.asp](https://www.w3schools.com/tags/ref_language_codes.asp)

Untuk menuliskan sebuah atribut kita memerlukan nama dari atribut itu diikuti dengan nilai atribut tersebut dalam bentuk <i>string</i>(Ditulis dalam tanda kutip dua). Untuk lebih jelasnya, coba kita lihat gambar berikut:
![screenshot](gambar)

Atribut pada elemen juga dapat dituliskan lebih dari satu. Kita bisa menuliskan struktur atribut di samping atribut yang sudah ada. Seperti contoh berikut ini:

```html
<p lang="id" translate="no">Yogyakarta mendapat berbagai macam julukan seperti Kota Pelajar, Kota Gudeg, Kota Perjuangan, maupun Kota Budaya</p>
```
Dengan menambah atribut ```translate``` dan memberikan nilai <b>"no"</b> pada elemen paragraf tsb, maka konten dari elemen yang dimaksud tidak akan diterjemahkan oleh layanan sistem translate seperti <b>Google Translate</b>.
