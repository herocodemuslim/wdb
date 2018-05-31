## 02 - Pengenalan Front End Development
### Objective
1. Menginstall Tools yang Diperlukan
2. Memahami Perbedaan Front-end, Back-end, dan Full-stack
3. Memahami Peran HTML, CSS, dan JavaScript

### 1. Menginstall Tools yang Diperlukan
- Text Editor: Tempat kita menulis kode (VSCode, Sublime, Atom)
- Web Browser: Tempat kita melihat hasil kode (Chrome, Firefox)

#### Cara Kerja Internet in a High Level
1. Menemukan Alamat yang Tepat
  - Query kita akan di submit ke DNS 
  - DNS akan mengkonversikan nama domain nya menjadi alamat IP

2. Going to That Address
  - Request yang kita minta akan dikirim ke alamat IP bersangkutan
  - Request kita akan mencari jalur tercepat untuk sampai ke komputer server tersebut
  - Loncat dari satu server ke server lainnya

3. Server Memberikan Respon
  - Server tersebut akan mencari tahu apa yang sedang kita inginkan atau akses
  - Server akan menyiapkan konten untuk kita, seringkali mengambil data dari database
  - Server mengirimkan respons dalam bentuk kombinasi HTML, CSS, dan JavaScript

4. Browser Magic!
  - Browser kita mengkonversikan kode-kode tersebut ke sesuatu yang dapat kita lihat


### 2. Memahami Perbedaan Front-end, Back-end, dan Full-stack
1. Front-end adalah hal-hal yang kita lihat dan interaksi. HTML, CSS, dan JavaScript
2. Back-end itu luas! Ada banyak teknologi. NodeJS, MongoDB, Python, Ruby

Ketika kita mengakses Facebook.com di browser, melakukan HTTP Request dan Server mengembalikan respon, tampilan nya itu adalah FRONT-END atau CLIENT-SIDE. Tetapi yang menentukan teman-teman siapa saja yang kita punya, postingan yang paling atas, history chat kita, posting status, upload foto, dan sejumlah fungsional tersebut di handle oleh teknologi BACK-END atau SERVER-SIDE.

#### Static VS Dynamic Site
Ada website yang bersifat statis atau jarang sekali dilakukan update dan ada pula yang secara konstan di update atau dinamis.

Web Statis biasanya hanya menggunakan teknologi FRONT-END, yaitu HTML, CSS, dan JavaScript. Contohnya yaitu website berikut: https://www.lazybearsf.com/ yang hanya menampilkan informasi tentang restaurant mereka.

Sedangkan Web Dinamis konten nya akan secara konstan di update, contohnya website berita: https://news.google.com/?hl=en-US&gl=US&ceid=US:en, web tersebut menggunakan kode-kode server side untuk membuat web nya dinamis. 

Jadi, bisa dibilang pada website dinamis, FRONT-END NYA DI CONSTRUCT OLEH BACK-END.

3. Analogi sederhananya: The back-end is everything that happens in the kitchen, the front-end is what plated and sent to your table.

#### HTML
- HyperText Markup Language
- Mendefinsikan struktur halaman web
  - Ini header
  - Ini footer
  - Ini paragraph
  - Ini list
- Disebut juga "noun" atau "skeleton"

#### CSS
- Cascading Style Sheet
- Mendefinisikan style untuk HTML
  - Buat semua text warna biru
  - Buat tombol ini punya border kuning
  - Posisikan logo ke sudut kiri atas
- Disebut juga "adjective" atau "skin"

#### JavaScript
- Menambahkan logic ke website
- Menambahkan interaktifitas
  - Do some math
  - Ganti warna background ketika tombol di klik
- Disebut juga "verbs" atau "behavior"

---

## 03 -  Pengenalan HTML
### Objectives
1. Mampu menulis struktur HTML dengan benar
2. Memahami Tag-tag HTML, Closing dan Self-closing Tag
3. Membuat Ulang Website yang Diperintahkan

### History of HTML
- Dibuat tahun 1989/1990
- Memungkinkan untuk mempublikasikan dan saling mempertukarkan dokumen teknikal dan scientific
- Memungkinkan untuk menghubungkan ke e-document lain melalui hyperlink

### General Rule
`<namaTag>Konten</namaTag>`

### Pengenalan MDN
MDN atau Mozilla Developer Network adalah sebuah website yang sangat bermanfaat sekali buat kamu yang ingin mencari referensi Web Development, terutama HTML, CSS, dan JavaScript. Web: https://developer.mozilla.org/en-US/

Untuk memahami sekilas tentang HTML, kamu bisa baca artikel berikut: https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML

### HTML Boilerplate
Dokumen mempunyai struktur dasar yang harus ada pada setiap yang kita tulis. Kita sebut HTML Boilerplate. Berita gembiranya adalah pertama struktur nya tetap sama, kedua text editor modern sekarang sudah memudahkan kita untuk membuat boilerplate ini, dengan mengetikkan html kemudian tab, maka boilerplate nya akan tercipta.

```html
<!DOCTYPE html>
<html>
  <head>
    <!-- metadata kita letakkan disini -->
    <meta charst="utf-8">
    <title>Website Pertama Saya</title>
  </head>
  <body>
    <!-- konten kita letakkan disini -->
    <h1>Halo, Saya Fadli. Ini adalah Website pertama saya.</h1>
  </body>
</html>
```

`<!DOCTYPE html>` adalah kode untuk ngasih tahu sama si Browser bahwa kita menggunakan HTML versi terbaru yaitu HTML5.

`<html>..</html>` disebut sebagai root element, dimana kita meletakkan semua tag-tag HTML lainnya di dalamnya. Hanya ada dua element yang boleh ada secara langsung di dalam element `<html>` ini, yakni element `<head>` dan `<body>`.

`<head>..</head>` tempat dimana kita meletakkan kode-kode informasi mengenai web kita yang tidak tampil di halaman web nya. Contohnya deskripsi, keyword, author, link ke file CSS, JavaScript, dan informasi lainnya, yang kita sebut metadata.

`<meta charst="utf-8">` kode ini kita gunakan untuk menyatakan bahwa kumpulan karakter yang kita gunakan ini adalah UTF-8 dimana mencakup hampir seluruh cara penulisan yang ada di dunia.

`<title>Website Pertama Saya</title>` sudah bisa di tebak, kode ini digunakan untuk menetapkan judul dari website kita, bisa kita lihat pada tab di browser. Ini juga berguna ketika seseorang melakukan bookmark pada website kita, maka judul inilah yang akan disimpan, begitupun dengan search engine, jadi ketika seseorang mengetikkan website kita, maka title inilah yang akan dimunculkan.

`<body>..</body>` tempat dimana konten kita akan tampil di halaman web, mulai dari penjudulan, paragraf, gambar, table, link, dan lainnya.

#### HTML Comments
Sama seperti pada bahasa pemrograman, kita juga bisa memberikan komentar pada kode kita atau menonaktifkan kode kita dengan komentar. Komentar berguna untuk memberikan informasi kepada kita tentang kode yang kita tulis misalnya. Juga memberikan informasi kepada developer lain ketika kita bekerja secara team. Bahkan kita bisa ada reminder jika setelah enam bulan tidak ngoding.

`<!-- ini adalah komentar pada HTML -->`

### HTML Basic Tags

Ada banyak sekali tag-tag yang ada di HTML, tapi ini bukan masalah 'main' hafal-hafalan, sejujurnya dari sekian banyak itu, hanya 10-15 tag saja yang sering kita gunakan. Berikut referensi element pada HTML: https://developer.mozilla.org/en-US/docs/Web/HTML/Element

1. Heading: penjudulan
Terdapat 6 tingkat level penjudulan, sehingga layaknya menulis sebuah buku, sebaiknya kita menggunakannya dengan tepat.

```html
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
```

2. Paragraph: membuat paragraf
```html
<h1>HeroCodeMuslim</h1>
<p>Situs belajar pemrograman online</p>

<p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quis consectetur delectus quibusdam est natus ex corrupti magnam dolorem ea cumque?</p>
```

3. Bold dan Italic atau Strong dan Emphasis
```html
<p>
<b>Lorem ipsum</b> dolor, <i>sit amet</i> consectetur adipisicing elit. <strong>Quis consectetur</strong> delectus <em>quibusdam est</em> natus ex corrupti magnam dolorem ea cumque?
</p>
```
Tag `<b>` dan `<i>` sebenarnya setatus nya sudah deprecated atau sebaiknya tidak digunakan lagi, meskipun tetap bisa digunakan. Karena pada konsep HTML adalah struktur sedangkan untuk style kita serahkan pada teknologi CSS. 

Tag tersebut lebih kepada style bukan struktur, `<strong>` dan `<em>` sendiri menekankan pada struktur atau meaning. Tag-tag yang memiliki 'meaning' ini disebut SEMANTIC TAG. Artinya, ia menggambarkan konten di dalamnya atau apa yang di lakukannya bukan menggambarkan 'how it looks'. Contohnya tag `<p>, <img>, <header> <strong>, <em>` dan masih banyak lagi.

Jika kita lihat tag `<h1>-<h6>` dan `<p>` akan membuat baris baru sebelum dan sesudahnya. Ini disebut BLOCK LEVEL ELEMENT, sedangkan untuk tag `<strong> dan <em>` berada pada posisi yang sama, ini disebut INLINE LEVEL ELEMENT.

### HTML List
Ada dua tipe list pada HTML, Ordered List dan UnOrdered List. Sudah bisa kita tebak bahwa list pertama membutuhkan urutan, sedangkan yang kedua tidak.

Ordered List akan tampil seperti berikut:
1. HTML
2. CSS
3. JavaScript
Sedangkan Unordered List sama saja, bedanya bukan angka melainkan lingkaran hitam kecil.

```html
<h2>Film Favorit Saya</h2>
<ol>
  <li><strong>IP Man 1,2,3</strong></li>
  <li>Harry Potter Series
    <ul>
      <li>Harry Potter 1</li>
      <li>Harry Potter 2
        <ol>
          <li>Harry Potter Scence 1</li>
          <li>Harry Potter Scence 2</li>
        </ol>
      </li>
      <li>Harry Potter 3</li>
    </ul>
  </li>
  <li>Ayat-Ayat Cinta</li>
</ol>

<h2>Buku Startup Rekomendasi</h2>
<ul>
  <li>Startupedia</li>
  <li>Startupreneur</li>
  <li>The Lean Startup</li>
</ul>
```
Secara default, list akan ditampilkan oleh style nya browser, kita juga bisa mengganti dari nomor menjadi alfabet, huruf romawi dengan menggunakan CSS.

Kita biasanya membuat menu navigasi menggunakan Unordered List.


### Divs dan Spans
Kita akan benar-benar bisa memahami dan merasakan efek penggunaan Div dan Span ketika kita belajar CSS.

Div singkatan dari division, div sebagai generic kontainer atau pembungkus kita gunakan untuk mengelompokkan sekumpulan element. Contohnya kita mengelompokkan sekumpulan elemen div untuk banner, div untuk header, div untuk profil author, dan seterusnya.

Span, sebagai kontainer untuk konten yang lebih kecil, contohnya ada huruf yang kita ingin lebih besar dari yang lainnya. 

Bedanya, Div: block level, sedangkan span: inline-level.

Sekali lagi, kita akan baru benar-benar merasakannya ketika kita belajar CSS, dimana kita bisa menargetkan suatu div atau span dengan attribut nya, class ataupun id, yang akan kita segera pelajari.

```html
<div>
  <h1>HeroCodeMuslim</h1>
  <p>Tempat belajar coding online!</p>
</div>

<p>
  Ayo buruan daftar!
</p>
```

### HTML Attributes
Atribute digunakan untuk menambahkan informasi tambahan pada element HTML. Berikut format dasar untuk menambahkan atribut pada element HTML.

`<namaTag name="value">Konten</namaTag>`

Berikut beberapa contoh element pada HTML yang menggunakan atribut.

```html
<img src="cat.jpg">

<a href="tentang.html">Halaman Tentang</a>

<p class="long-copy">
  Ini adalah paragraf
</p>

<link rel="stylesheet" type="text/css" href="css/style.css">
```

Ada banyak sekali atribut yang ada pada HTML, list nya bisa dilihat di link berikut: https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes

Sama seperti sebelumnya, mungkin hanya 15 atribut saja yang akan sering kita gunakan. 

Ada atribut yang khusus untuk satu element saja, ada yang 2-5 element bisa menggunakannya, ada yang hampir semua element bisa menggunakannya.

### Images dan Link
```html
<img src="cat.jpg">

<img src="http://www.cutestpaw.com/wp-content/uploads/2011/11/To-infinity-and-beyond.jpeg" alt="Super Hero Cat">

<a href="tentang.html">Tentang</a>

<a href="https://www.instagram.com/herocodemuslim/" target="_blank">
```

Untuk menyisipkan gambar kita bisa menggunakan tag `<img>` ditambah dengan atribut `src="value"` dimana atribut `src` atau source menentukan dimana lokasi dari gambar tersebut, nilainya bisa berupa lokasi di dalam project folder kita ataupun gambar dari internet.

Ada lagi atribut `alt` dimana digunakan untuk sebagai teks alternatif jika suatu saat gambar gagal dimuat karena suatu kendala ataupun untuk screenreader.

Untuk membuat link, kita gunakan tag anchor `<a>`. Tidak cukup sampai disitu kita perlu atribut `href` dimana nilainya menentukan akan kemana link itu kita arahkan. Nilainya bisa mengarah ke halaman lain website kita, halaman di luar website kita misalnya instagram, facebook, dan lainnya ataupun alamat nya berupa file.

---

## 04 - Intermediate HTML
### Objectives
1. Mampu Membuat Table
2. Mampu Membuat Form
