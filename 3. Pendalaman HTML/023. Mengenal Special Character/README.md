# Special Character
Terdapat beberapa karakter special seperti <i>copyright symbol ©</i> yang tidak termasuk ke dalam standar kelompok ASCII characters, di mana ASCII characters hanya menyediakan karakter seperti huruf, nomor, dan beberapa simbol dasar. Karakter lain seperti lebih dari (>) atau kurang dari (<) walaupun tersedia dalam <i>ASCII character</i>, karakter tersebut tidak dapat digunakan secara langsung sebagai konten pada HTML. Hal tersebut dikarenakan karakter tersebut akan terbaca sebagai sebuah <i>tag</i>.

Untuk menampilkan karakter seperti yang disebutkan tadi, HTML memerlukan sebuah "<i>escaped</i>" karakter. <i>Escaping</i> artinya adalah tidak menyliskan karakter itu sendiri, melainkan menggantinya dengan nilai <i>numeric</i> atau <i>character reference</i> pada karakternya.

Terdapat dua cara untuk melakukannya, yakni dengan menetapkan nilai numerik(numeric entity) atau menggunakan nama singkatan yang sudah ditetapkan untuk masing-masing  karakternya (named entity). Semua referensi karakter dimulai dengan "&" dan diakhiri dengan ";"

Contohnya untuk menggunakan simbol copyright, kita dapat menggunakan "&copy"

```html
<p>Copyright &copy;2021 Ether Linux</p>
```

atau "&#169"

```html
<p>Copyright &#169;2021 Ether Linux</p>
```
Alhasil tampilannya sama.

<p align="center">
<img src="https://github.com/adyuta447/learn-html-css/blob/main/3.%20Pendalaman%20HTML/img/2022-04-18_16-49.png" alt="screenshot">
</p>

Berikut daftar karakter spesial dengan karakter referensinya.

| Karakter | Deskripsi | Named Entity | Numeric Entity |
|:---------|:----------|:-------------|:---------------|
|      | non-breaking space | ```&nbsp;``` | ```&#160;``` |
| & | Ampersand | ```&amp;``` | ```&#038;``` |
| ’ | Apostrophe | ```&apos;``` | ```&#039;``` |
| < | Kurang dari (less-than) | ```&lt;``` | ```&#060``` |
| > | Lebih dari (greater-than) | ```&gt``` | ```&#062;``` |
| © | Hak cipta(copyright) | ```&copy``` | ```&#169;``` |
| ® | Merek dagang terdaftar (registered trademark) | ```&reg;``` | ```&#174;``` |
| ™ | Merek dagang (trademark) | ```&trade;``` | ```&#8482;``` |
| £ | Pound | ```&pound;``` | ```&#163;``` |
| ¥ | Yen | ```&yen;``` | ```&#165;``` |
| € | Euro | ```&euro;``` | ```&#8364;``` |
| - | En-dash | ```&ndash;``` | ```&#8211;``` |
| — | Em-dash | ```&mdash;``` | ```&#8212;``` |
| ‘ | Kutip tunggal kiri | ```&lsquo;``` | ```&#8216;``` |
| ’ | Kutip tunggal kanan | ```&rsquo;``` | ```&#8217;``` |
| “ | Kutip ganda kiri | ```&ldquo;``` | ```&#8221;``` |
| ” | Kutip ganda kanan | ```&rdquo;``` | ```&#8221;``` |
| • | Bullet | ```&bull;``` | ```&#8226;``` |
| ... | Horizontal ellipsis | ```&hellip;``` | ```&#8230;```