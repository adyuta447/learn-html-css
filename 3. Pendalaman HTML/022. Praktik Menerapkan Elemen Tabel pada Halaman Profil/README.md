# Menerapkan Elemen Tabel pada Halaman Profil

Setelah kita mengetahui cara menerapkan tabel pada <i>website</i>, mari kita perkaya kembali konten pada halaman profil, khususnya konten pada elemen ```<aside>``` yang sudah kita buat. Kita akan menambahkan detail informasi dari kota Bandung seperti negara, luar, bahasa daerah, dan kode telepon.

Tapi sebelum itu mari kita atur kembali struktur elemen yang di dalam elemen ```<aside>``` tersebut. Saat ini elemen ```<aside>``` memiliki struktur seperti ini:

<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/Screenshot%202022-04-14%20195355.png" alt="ilustrasi">
</p>

Karena kita akan menambahkan konten lain, maka kita perlu mengelompokkan kembali seluruh elemen di dalam elemen ```<article>```. Kelompokan atau bungkus seluruh elemen yanf ada di dalam elemen ```<article>``` dengan elemen ```<header>```, dan buat elemen baru yaitu ```<section>``` pada level yang setara dengan elemen ```<header>``` tsb. Pada elemen ```<section>``` ini konten tabel akan ditempatkan. Silahkan buka kembali berkas <b>index.html</b> dan sesuaikan struktur dalam elemen ```<aside>``` seperti berikut ini.

```html
    <aside>
        <article>
            <header>
                <h2>Yogyakarta</h2>
                <p>Kota Pelajar</p>
                <figure>
                    <img src="assets/images/Jogja-badge.png" alt="">
                    <figcaption>Lambang</figcaption>
                </figure>
            </header>
            <section></section>
        </article>
    </aside>
```

Sehingga struktur pada elemen ```<aside>``` akan menjadi seperti ini:

<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/Screenshot%202022-04-15%20194528.png" alt="screenshot">
</p>

Selanjutnya pada elemen ```<section>``` kita masukkan konten berikut:

```
Informasi Lainnya

Negara 
Indonesia 

Hari jadi 
13 Maret 1755

Luas Total
3.185,80 km2

Bahasa Daerah 
Jawa

Kode Telepon
0274
```

Sesuaikan konten tersebut dengan menerapkan elemen yang sesuai, salah satunya gunakan elemen tabel untuk menampung sebagian kontennya. Sehingga kode tersebut menjadi seperti ini:

```html
            <section>
                <h3>Informasi Lainnya</h3>
                <table>
                    <tr>
                        <th>Negara</th>
                        <td>Indonesia</td>
                    </tr>
                    <tr>
                        <th>Hari jadi</th>
                        <td>13 Maret 1755</td>
                    </tr>
                    <tr>
                        <th>Luas Total</th>
                        <td>3.185,80 km<sup>2</sup></td>
                    </tr>
                    <tr>
                        <th>Bahasa Daerah</th>
                        <td>Jawa</td>
                    </tr>
                    <tr>
                        <th>Kode Telepon</th>
                        <td>0274</td>
                    </tr>
                </table>
            </section>
```

Sehingga jika kita buka pada browser maka akan seperti ini:

<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/Screenshot%202022-04-15%20203753.png" alt="screenshot">
</p>
