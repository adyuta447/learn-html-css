# Mengenal Teks Terformat
Sejauh ini, Kita sudah mengenal paragraf, heading dan juga list pada HTML. Tapi sabar, masih ada beberapa lagi yang meruapakan spesial teks format yang dapat kita gunakan yaitu ```<blockqoute>```, ```<pre>```, dan ```<figure>```.

## Long quotations
Jika pada konten kita memiliki sebuah kutipan ataupun sebuah testimonial, kita dapat gunakan format long quotations dengan menggunakan tags ```<blockquote>```. Konten di dalam elemen ```<blockquote>``` ini dapat berupa sebuah paragraf, heading, ataupun list.

```html
    <blockquote>
        <p>Situs web (bahasa Inggris: website) adalah sekumpulan halaman web yang saling berhubungan yang umumnya   berada pada peladen yang sama berisikan kumpulan informasi yang disediakan secara perorangan, kelompok, atau organisasi.</p>
    </blockquote>
```
Berikut ini tampilanm standar ketika sebuah konten berada di dalam ```<blockquote>```.

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-11_23-35.png)

Pada elemn ini tidapa dapat menggunakan atribut <i>cite</i> untuk menentukan sumber URL dari sebuah kutipan ( Jika kutipan tersebut bersumbar dari sebuah situs website).

```html
<blockquote cite="https://id.wikipedia.org/wiki/Situs_web">
   <p>Situs web (bahasa Inggris: website) adalah sekumpulan halaman web yang saling berhubungan yang umumnya berada pada peladen yang sama berisikan kumpulan informasi yang disediakan secara perorangan, kelompok, atau organisasi.</p>
</blockquote>
```
## Preformatted text
Pada materi sebelumnya, kita sudah mengetahui bahwa HTML akan mengabaikan penulisan spasi yang dituliskan secara berulang dan juga <i>line breaks</i> (baris baru). Tetapi pada beberapa tipe konten seperti contoh kode atau puisi hal tersebut dapat kita gunakan unutk menampilkan konten sesuai yang kita tulis pada text editor. Untuk menggunakannya, kita gunakan elemen ```<pre>``` sebagai pembungkus kontennya. Perhatikan contoh berikut ini:

```html
<pre>
   SAJAK PUTIH
 
Bersandar pada tari warna pelangi
Kau depanku bertudung sutra senja
Di hitam matamu kembang mawar dan melati
Harum rambutmu mengalun bergelut senda
 
Sepi menyanyi, malam dalam mendoa tiba
Meriak muka air kolam jiwa
Dan dalam dadaku memerdu lagu
Menarik menari seluruh aku
 
Hidup dari hidupku, pintu terbuka
Selama matamu bagiku menengadah
Selama kau darah mengalir dari luka
Antara kita Mati datang tidak membelah...
 
                   Karya : Chairil Anwar
</pre>
```
Sehingga pada browser akan menampilkan hasil yang sama seperti yang kita tuliskan.

![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-12_00-25.png)

## Figure

Elemen ini digunakan untuk merepresentasikan konten tersendiri (<i>self-contained content</i>) seperti ilustrasi, diagram, foto atau bisa juga sebuah baris kode. Banyak hal yang dapat digunakan dalam elemen ini.

Elemen ini digunakan untuk mengklompokkan blok konten yang dapat dipindahkan posisinya dari blok utama sebuah dokumen tanpa mempengaruhi arti dari induk dokumen.

Di dalam elemen figure kita dapat menuliskan elemen ```<figcaption>``` sebagai sebuah caption (judul) untuk konten tersebut. Berikut ini adalah contoh penggunaan figure pada sebuah konten gambar.

```html
<p>Ether Linux is a Linux derivative of Debian. Originating from Indonesia which makes penetration testing and security professionals. Ether Linux is the second Linux in Indonesia that focuses on penetration testing and security professionals. Ether Linux provides more than 100 tools for penetration testing which are of course free.</p>
<figure>
    <img src="https://i.ibb.co/3sJC2db/Ether-Linux.png" alt="ether" width="200px">
    <figcaption>Ether Linux</figcaption>
</figure>
<p>We also focus on these debian-derived distros for pentesters and security professionals. Ether Linux does provide ready-to-use automated tools. But we made it not for script kiddies.</p>
```
![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-12_01-09.png)

Pada contoh lainnya, <b>figure</b> ini dapat kita gunakan untuk <i>markup</i> sebuah konten puisi.

```html
<figure>
   <pre>
           SAJAK PUTIH
 
       Bersandar pada tari warna pelangi
       Kau depanku bertudung sutra senja
       Di hitam matamu kembang mawar dan melati
       Harum rambutmu mengalun bergelut senda
 
       Sepi menyanyi, malam dalam mendoa tiba
       Meriak muka air kolam jiwa
       Dan dalam dadaku memerdu lagu
       Menarik menari seluruh aku
 
       Hidup dari hidupku, pintu terbuka
       Selama matamu bagiku menengadah
       Selama kau darah mengalir dari luka
       Antara kita Mati datang tidak membelah...
   </pre>
   <figcaption>Sajak Putih oleh Charil Anwar</figcaption>
</figure>
```
![screenshot](https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-03-12_01-23.png)
