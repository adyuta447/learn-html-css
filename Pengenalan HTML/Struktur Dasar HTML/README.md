# Struktur Dasar HTML
Website serupa dengan berkas dokumen yang ada seperti koran, majalah, atau buku. Serupa dalam hal memiliki struktur konten layaknya dokumen sehari-hari yang kita baca. Pada sebuah majalah terdapat judul, gambar yang ditampilkan dan teks dalam bentuk paragraf. Terkadang, jika konten tersebut panjang terdapat sub-judul untuk memisahkannya menjadi beberapa bagian.<br/>

Judul dan subjudul pada sebuah dokumen menggambarkan suatu hierarki dari informasi. Misalnya, judul dengan ukuran besar merupakan judul utama dalam sebuah konten. Kemudian diikuti dengan judul kecil di bawahnya yang menjelaskan informasi dengan lebih mendetail lagi.<br/>

Berkas HTML dasarnya memiliki struktur yang nampak seperti ini:

```html
<!DOCTYPE html>
<html>
    <head>
    <title>Judul Halaman</title>
    </head>
    <body>
        <h1>Heading Utama</h1>
        <p>Sebuah Paragraph.</p>
    </body>
</html>
```

Kita dapat melihat bahwa struktur dasar HTML dituliskan dari beberapa elemen. Pada setiap elemen HTML terdapat dua tag, yaitu pembuka tag <> dan penutup tag </>. <br/> 

## Elemen <html>
Hierarki elemen teratas pada berkas HTML adalah elemen HTML-nya itu sendiri. Elemen ini digunakan untuk memberitahu kepada browser bahwa ini merupakan sebuah berkas HTML sekaligus menjadi root dari sebuah berkasnya itu. Seluruh elemen lainnya tentunya dituliskan pada konten elemen ini.

## Elemen <head>
Elemen <head> pada berkas HTML berfungsi sebagai tempat disimpannya informasi dari dokumen HTML. Informasi dapat berupa elemen meta, style, atau link. Dan juga pada elemen ini judul dari dokumen HTML didefinisikan dengan menggunakan elemen <title>. Berikut contoh elemen yang berada pada konten head:
- <title>
- <style>
- <base>
- <link>
- <meta>
- <script>
- <noscript>

Pada HTML versi 4.01, elemen <head> wajib ada di dalam sebuah berkas HTML.<br/> Tetapi semenjak HTML5, penggunaan <head> dapat dihilangkan. Sehingga struktur dasar berkas HTML menjadi seperti ini:

```html
<!DOCTYPE html>
<html>
    <meta charset="utf-8">
    <title>Judul halaman</title>
    <style> Style </style>
    <body>
        <h1>Heading Utama</h1>
        <p>Sebuah Paragraph.</p>
    </body>
</html>
```
## Elemen <body> 

Seluruh konten yang terdapat pada elemen ini akan ditampilkan pada halaman website. Maka dari itu, elemen ini digunakan untuk menampung seluruh konten atau elemen yang ditampilkan ke dalam jendela browser. Silakan coba tuliskan kode berikut(Jangan Copas ya masa programer copas hehe)

```html
<html>
    <head>
        <title>Judul dari dokumen HTML</title>
    </head>
    <body>
        <h1>header yang diletakan di dalam elemen body</h1>
        <p>Ini merupakan sebuah paragraph yang juga diletakan pada sebuah konten body, sehingga konten ini dapat dilihat oleh pengguna pada jendela browser.</p>
    </body>
</html>
```