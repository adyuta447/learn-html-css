# Mengenal Gambar
Tanpa gambar sebuah website tentu tidak akan menarik. Ada beberapa alasan mengapa website perlu sebuah gambar. Contohnya kita perlu menampilkan logo perusahaan, ilustrasi, diagram, dan sebagainya.

Pada HTML untuk menampilkan sebuah gambar kita bisa menggunakan tag ```<img>```. Berbeda dengan elemen lain, elemen ```<img>``` tidak menuliskan konten di antara tag pembuka dan tag penutup. Tetapi untuk menetapkan gambar yang ditampilkan kita gunakan sebuah atribut. Contohnya seperti ini:

```html
<img src="https://i.ibb.co/5vLpTw9/Group.png" alt="github">
```
Maka gambar akan ditampilkan pada browser seperti ini:

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-10_21-33.png)

Pada contoh kode di atas, perlu kita perhatikan nih bahwa sebuah elemen ```<img>``` merupakan sebuah elemen kosong(tidak memiliki konten sehingga tidak ada closing tag ```</>```).
Selain itu, yang perlu kita perhatikan adalah atribut yang ada pada elemen tsb, terdapat dua elemen yang harus kita gunakan ketika menggunakan ```<img>```, nah disini saya akan jelaskan fungsi-fungsinya.

Yang pertama, atribut ```src```. Atribut ini berfungsi sebagai sumber dari gambar yang ditampilkan. Atribut ini dapat bernilai url gambar atau path gambar lokal dari sebuah gambar yang digunakan.

Selanjutnya adalah atribut ```alt```. Atribut ini sebenarnya tidak wajib untuk diterapkan, hanya saja atribut ini akan sangat berguna ketika gambar tidak berhasil ditampilkan. Nilai atribut ini akan sangat berguna ketika gambar tidak berhasil ditampilkan. Nilai atribut ini merupakan sebuah gambaran dari gambar yang ditampilkan. Nilai atribut ini merupakan gambaran dari gambar yang ditampilkan dalam bentuk tulisan. Sehingga ketika gambar gagal ditampilkan maka akan memunculkan teks alternatif yang dapat mewakili arti dari gambar tersebut.  

Selnajutnya terdapat atribut lain yang bisa Anda gunakan pada elemen ini, contohnya ```title```. <b>Title</b> berfungsi sebagai informasi tambahan untuk sebuah gambar. Informasi tsb akan muncul ketika kita mengarahkan sebuah cursor pada gambar yang ditampilkan.

## Jenis format gambar

| Nama | Ekstensi Format File | Keterangan |
|:-----|:--------------------:|:-----------|
| Graphics Interchange Format | .gif | Dapat digunakan untuk gambar animasi. Ukuran file biasanya kecil. Kualitas gambar terbatas. |
| Joint Photographic Expert Group image | .jpg, .jpeg, .jfif, .pjpeg, .pjp | Kualitas text pada gambar dapat menjadi buruk. Ukuran file lumayan kecil. Pada website biasanya digunakan untuk gambar yang tidak banyak text. |
| Portable Network Graphics | .png | Text lebih bisa terbaca dibandingkan jenis Jpeg. Ukuran file dapat menjadi besar sehingga mengurangi kecepatan memuat situs. |
| WebP | .webp | Dibandingkan dengan gambar berkualitas sama pada jpeg atau png, ukuran file pada webp dapat menjadi lebih kecil. Namun tidak semua web browser dapat membaca webp. |
| Scalable Vector Graphics | .svg | Kualitas gambar terjaga dan ukuran file kecil. Namun tidak cocok untuk gambar yang terlalu kompleks seperti foto. Pada website biasanya digunakan untuk logo atau icon. |

## Mengatur ukuran pada gambar
Untuk mengatur ukuran gambar yang ditampilkan juga tentunya menggunakan sebuah atribut. Untuk menentukan lebar gambar kita gunakan atribut width, dan untuk menentukan tinggi tentu gunakan atribut height.

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-10_22-35.png)

Ketika menggunakan atribut ini disarankan hanya gunakan salah satunya. Terkecuali kita menentukan nilai lebar dan tingginya sesuai dengan rasio dari ukuran gambar aslinya. Gambar tentu  lebih perlu waktu untuk tampil di browser, sehingga tentukanlah ukuran sesuai kebutuhan.