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