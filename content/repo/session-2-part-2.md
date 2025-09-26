---
date: "2025-09-27T09:00:00+07:00"
draft: false
title: "Kenali Konsep Variabel untuk Data Dinamis pada JavaScript"
short: "variabel"
thumb:
    image: "cover.jpg"
    anima: ""
    video: ""
layout: "module"
weight: 2
lister: 2
format:
    media: "article"
    model: "concept"
    datum:
        data: "Konsep Variabel dalam JavaScript"
outcome:
    - prop: ""
      name: "Konseptual"
      icon: "book"
      desc: "Memahami konsep dasar variabel, perbedaan var, let, dan const serta kaitannya dengan block scope dan hoisting."
    - prop: ""
      name: "Praktik"
      icon: "code"
      desc: "Mampu memilih tipe deklarasi variabel yang tepat untuk kasus nyata dalam aplikasi sederhana."
require:
    - prop: "Dasar"
      name: "Struktur Program"
      icon: "file"
      desc: "Diperlukan pemahaman dasar struktur program JavaScript agar mudah memahami konsep variabel."
metadata:
    index: false
    thumb: "cover.jpg"
    group: []
    author: ["Al Muhdil Karim"]
description: "Modul ini membahas konsep variabel dalam JavaScript, mulai dari definisi, aturan penamaan, hingga perbedaan penggunaan var, let, dan const. Pembahasan dilengkapi dengan studi kasus sederhana pada sistem perpustakaan."
---


## Pendahuluan

Bayangkan Anda sedang mengelola sebuah toko online, di mana setiap produk, pembeli, dan transaksi membutuhkan wadah penyimpanan informasi sementara agar sistem dapat berjalan lancar. Dalam dunia pemrograman, wadah penyimpanan ini disebut dengan *variabel*. Sama seperti rak gudang yang menampung berbagai stok barang, variabel menampung data yang berbeda-beda sesuai kebutuhan program. Kisah pengelolaan data ini menarik, karena tanpa variabel, kode hanya akan menjadi kumpulan instruksi yang kaku tanpa fleksibilitas.  

Mari kita ambil contoh sederhana: ketika seorang pelanggan menambahkan produk ke keranjang, sistem harus tahu nama produk, jumlah yang dipesan, dan total harga. Semua informasi ini harus disimpan di memori agar aplikasi dapat memprosesnya lebih lanjut. Jika tidak ada variabel, setiap kali informasi tersebut dipanggil, programmer harus menuliskan ulang nilainya secara manual. Tentu saja hal ini tidak efisien, sama seperti kasir yang harus menuliskan ulang daftar belanjaan setiap kali transaksi terjadi.  

Keterkaitan ini menimbulkan rasa penasaran tentang bagaimana variabel bekerja di balik layar, serta bagaimana *JavaScript* menyediakan berbagai cara untuk mendefinisikan dan mengatur data. Dari `var` yang sudah lama ada, hingga `let` dan `const` yang diperkenalkan pada standar modern, setiap pendekatan memiliki peran dan kelebihan. Pada titik inilah kita akan mulai masuk ke pembahasan yang lebih dalam, yaitu mengenai **konsep dasar variabel**.  

![Pendahuluan](session-2-part-2/pendahuluan.png)  


## Konsep Dasar

Variabel dalam JavaScript adalah sebuah *identifier* atau penanda yang digunakan untuk menyimpan nilai di dalam memori program. Dengan definisi ini, variabel berfungsi sebagai simbol yang memungkinkan programmer menyimpan data sementara, sehingga program dapat memproses informasi secara dinamis tanpa menuliskan ulang nilai berulang kali. Misalnya, dalam toko online, variabel digunakan untuk menyimpan jumlah produk di keranjang agar sistem dapat menghitung total belanja otomatis. Konsep ini sama seperti catatan kasir yang menampung harga sementara hingga pembayaran selesai diproses. Variabel dengan demikian bukan hanya sekadar tempat menyimpan data, tetapi juga menjadi jembatan antara logika program dan kebutuhan aplikasi nyata. Pemahaman definisi ini sangat penting, karena seluruh alur pemrograman modern tidak akan berjalan tanpa variabel yang konsisten. 【43†source】  

JavaScript menyediakan tiga cara utama dalam deklarasi variabel: `var`, `let`, dan `const`. `var` adalah cara lama yang memiliki sifat *hoisting*, artinya deklarasi akan dipindahkan ke atas lingkup eksekusi sehingga kadang membingungkan bagi pemula. `let` diperkenalkan dalam ES6 untuk mendukung *block scope*, sehingga nilai hanya berlaku di dalam blok tertentu seperti `{}`. `const` digunakan untuk nilai yang tidak berubah setelah dideklarasikan, misalnya *tax rate* atau *API key*. Perbedaan mendasar ini memberi fleksibilitas bagi programmer untuk memilih pendekatan yang sesuai dengan kasus. Sebagai contoh, jumlah stok barang dapat menggunakan `let` karena sifatnya berubah, sementara nilai pajak penjualan lebih tepat memakai `const`. Pengetahuan ini membantu menulis kode yang lebih aman, terstruktur, dan mudah dipelihara. 【43†source】  

![Konsep Dasar](session-2-part-2/konsep-dasar.png)  


## Var dan Hoisting

`var` adalah cara paling awal untuk mendeklarasikan variabel di JavaScript, dan memiliki perilaku unik yang dikenal sebagai *hoisting*. Hoisting berarti deklarasi variabel dengan `var` akan dipindahkan ke bagian atas lingkup fungsi atau global sebelum kode dijalankan. Konsep ini sering membuat bingung pemula, karena variabel bisa digunakan sebelum dideklarasikan. Misalnya, dalam toko online, jika programmer mendefinisikan `var totalHarga` di akhir fungsi tetapi memanggilnya di awal, JavaScript tetap mengen...

```javascript
console.log(totalHarga); // undefined
var totalHarga = 50000;
console.log(totalHarga); // 50000
```

Penggunaan `var` dalam kasus nyata sering menimbulkan bug tersembunyi. Misalnya, dalam sistem e-commerce, jika ada dua fungsi berbeda yang sama-sama menggunakan `var totalHarga`, nilai yang satu dapat menimpa nilai yang lain karena lingkupnya tidak terbatas pada blok. Hal ini bisa menyebabkan perhitungan diskon atau pajak menjadi salah, sehingga laporan penjualan tidak akurat. Dengan demikian, meskipun `var` masih didukung, banyak developer modern menghindari penggunaannya untuk mengurangi risiko konflik d...

Sebuah fakta menarik adalah bahwa hoisting hanya memindahkan deklarasi, bukan inisialisasi. Artinya, nilai baru hanya akan diberikan setelah baris inisialisasi dijalankan. Kesalahpahaman ini sering terjadi pada pemula yang mengira hoisting juga berlaku untuk nilai. Jika kita ingin menjaga kejelasan logika program, maka penggunaan `var` harus disertai pemahaman mendalam mengenai bagaimana JavaScript mengeksekusi kode di balik layar. Pengetahuan ini memperlihatkan mengapa standar modern memperkenalkan `let` ...

![Var dan Hoisting](session-2-part-2/var-dan-hoisting.png)  


## Let dan Block Scope

Setelah memahami `var` dengan segala keterbatasannya, muncul `let` sebagai solusi modern dalam ES6. `let` memperkenalkan konsep *block scope*, yaitu lingkup variabel yang terbatas hanya pada blok kode yang membungkusnya, biasanya ditandai dengan tanda kurung kurawal `{}`. Dengan pendekatan ini, variabel yang dideklarasikan di dalam sebuah blok tidak dapat diakses dari luar blok tersebut. Misalnya, pada toko online, variabel `let diskon` yang hanya berlaku di dalam perhitungan promosi musiman tidak akan ...

```javascript
if (true) {
  let diskon = 0.2;
  console.log(diskon); // 0.2
}
console.log(diskon); // ReferenceError
```

Penggunaan `let` juga memberikan keuntungan dalam hal keterbacaan kode. Karena lingkupnya jelas terbatas, programmer tidak perlu khawatir variabel dengan nama sama akan menimpa nilai di luar blok. Dalam sistem e-commerce, hal ini berarti variabel jumlah produk dalam satu fungsi checkout tidak akan berbenturan dengan variabel jumlah produk di fungsi manajemen stok. Dengan kata lain, `let` memberikan kepastian ruang lingkup yang memudahkan debugging sekaligus memperkecil kemungkinan kesalahan logika. Perb...

Fakta menarik adalah bahwa `let` tidak mendukung hoisting dengan cara yang sama seperti `var`. Meskipun secara teknis deklarasi tetap diangkat, variabel berada dalam *temporal dead zone* sampai benar-benar diinisialisasi. Artinya, memanggil `let` sebelum baris deklarasi akan menghasilkan error, bukan `undefined`. Hal ini melindungi programmer dari bug tersembunyi yang sering muncul saat menggunakan `var`. Konsep *temporal dead zone* ini menegaskan bahwa JavaScript modern dirancang untuk menghindari ambigu...

![Let dan Block Scope](session-2-part-2/let-dan-block-scope.png)  


## Const dan Nilai Tetap

Selain `var` dan `let`, JavaScript juga menyediakan `const` untuk mendeklarasikan variabel dengan nilai yang tidak bisa diubah setelah inisialisasi. Konsep ini mirip dengan label harga tetap pada sebuah produk di toko online yang tidak bisa diubah oleh kasir. Begitu nilai sudah diberikan pada `const`, maka setiap percobaan untuk mengubahnya akan menghasilkan error. Hal ini menjadikannya sangat berguna untuk data yang sifatnya konstan, seperti *tax rate*, URL API, atau kode kupon diskon yang sudah diten...

```javascript
const pajak = 0.1;
pajak = 0.2; // TypeError: Assignment to constant variable
```

Namun, penting untuk dipahami bahwa `const` tidak berarti membuat data menjadi benar-benar tidak berubah. Jika nilai yang disimpan adalah objek atau array, maka isi di dalamnya masih bisa dimodifikasi. Sebagai contoh, dalam sistem e-commerce, sebuah array `const keranjang` dapat diubah isinya dengan menambahkan produk baru, meskipun variabel `keranjang` sendiri tidak dapat diarahkan ke array lain. Hal ini sering membingungkan pemula, tetapi sekaligus menunjukkan fleksibilitas JavaScript dalam menangani str...

```javascript
const keranjang = ["Buku", "Pulpen"];
keranjang.push("Tas");
console.log(keranjang); // ["Buku", "Pulpen", "Tas"]
```

Fakta menarik lainnya adalah bahwa `const` secara otomatis mendorong penulisan kode yang lebih aman dan terstruktur. Dengan membiasakan diri menggunakan `const` untuk nilai yang tidak berubah, programmer akan terhindar dari bug yang muncul karena variabel diubah tanpa sengaja. Dalam pengembangan aplikasi besar seperti e-commerce dengan ribuan transaksi, praktik ini menjaga konsistensi dan stabilitas sistem. Dengan demikian, `const` bukan sekadar fitur tambahan, melainkan sebuah pendekatan pemrograman yan...

![Const dan Nilai Tetap](session-2-part-2/const-dan-nilai-tetap.png)  


## Aturan Penamaan Variabel

Setelah memahami cara mendeklarasikan variabel dengan `var`, `let`, dan `const`, langkah berikutnya adalah mengenal aturan penamaan variabel dalam JavaScript. Penamaan variabel bukan sekadar formalitas, melainkan hal yang memengaruhi keterbacaan dan kualitas kode. Dalam sebuah toko online, variabel seperti `totalHarga` atau `jumlahProduk` lebih mudah dipahami dibandingkan `x` atau `y`. JavaScript mewajibkan nama variabel diawali huruf, underscore `_`, atau tanda dolar `$`, tetapi tidak boleh dimulai den...

```javascript
let totalHarga = 100000;  // benar
let 2produk = 5;          // salah, nama tidak boleh diawali angka
```

Selain aturan sintaks, penamaan variabel juga mengikuti konvensi gaya penulisan. Konvensi yang paling umum dalam JavaScript adalah *camelCase*, di mana kata pertama huruf kecil dan kata berikutnya diawali huruf besar, misalnya `jumlahPesanan`. Dalam sistem e-commerce, gaya ini memastikan nama variabel mudah dibaca meskipun terdiri dari beberapa kata. Hindari penggunaan nama variabel yang terlalu umum seperti `data` atau `info`, karena tidak memberikan makna yang jelas. Sebaliknya, nama yang deskriptif a...

Fakta menarik adalah bahwa JavaScript memiliki daftar kata kunci (*reserved words*) yang tidak boleh digunakan sebagai nama variabel, seperti `class`, `return`, atau `function`. Jika digunakan, program akan menghasilkan error atau perilaku yang tidak terduga. Kesalahan ini sering dilakukan pemula yang mencoba menyingkat kode tanpa memerhatikan aturan. Dalam aplikasi besar seperti e-commerce dengan banyak modul, aturan penamaan yang jelas sangat penting agar variabel tidak tumpang tindih. Dengan menerapk...

![Aturan Penamaan Variabel](session-2-part-2/aturan-penamaan.png)  


## Mutabilitas dan Imutabilitas

Konsep penting lain dalam variabel adalah *mutabilitas* (dapat diubah) dan *imutabilitas* (tidak dapat diubah). Dalam JavaScript, variabel yang dideklarasikan dengan `let` bersifat mutable, artinya nilainya bisa diganti setelah inisialisasi. Sebaliknya, `const` dianggap immutable untuk referensi, meskipun isi objek atau array yang disimpan di dalamnya masih bisa diubah. Misalnya, dalam sistem e-commerce, variabel `let jumlahProduk` dapat diperbarui setiap kali pembeli menambah barang, sementara `const...

```javascript
let jumlahProduk = 2;
jumlahProduk = 5; // nilai berhasil diubah

const pajak = 0.1;
pajak = 0.2; // Error: Assignment to constant variable
```

Fakta menarik adalah bahwa meskipun `const` tidak dapat diganti referensinya, isi dari objek atau array yang ditampung tetap dapat dimodifikasi. Dalam toko online, jika keranjang belanja didefinisikan sebagai `const`, pelanggan tetap bisa menambah produk baru ke dalamnya. Hal ini menunjukkan bahwa imutabilitas di JavaScript bersifat terbatas hanya pada referensi, bukan pada isi data yang kompleks. Kesalahan memahami hal ini sering menyebabkan bug ketika developer mengira `const` melindungi seluruh isi data...

```javascript
const keranjang = ["Buku"];
keranjang.push("Pulpen"); // berhasil menambah
console.log(keranjang);   // ["Buku", "Pulpen"]
```

Dalam konteks aplikasi berskala besar, pemahaman tentang mutabilitas dan imutabilitas sangat penting untuk menjaga stabilitas data. Variabel mutable seperti `let` sangat berguna untuk nilai yang sering berubah, misalnya jumlah stok produk atau total belanja sementara. Sementara itu, variabel immutable seperti `const` lebih tepat digunakan untuk data yang konsisten, seperti tarif pajak atau alamat API. Dengan membedakan keduanya, kode menjadi lebih terorganisir dan meminimalkan resiko kesalahan. Pendekat...

![Mutabilitas dan Imutabilitas](session-2-part-2/mutabilitas-dan-imutabilitas.png)  


## Perbandingan Var, Let, dan Const

Untuk memahami kelebihan masing-masing deklarasi variabel, penting dilakukan perbandingan antara `var`, `let`, dan `const`. `var` mewakili pendekatan lama yang fleksibel tetapi rawan bug karena sifat hoisting dan cakupannya yang global atau fungsi. `let` memperkenalkan block scope, membuat variabel lebih aman dan tidak saling menimpa. Sementara itu, `const` digunakan ketika nilai harus tetap konsisten sepanjang program. Dalam sistem e-commerce, `var` mungkin dipakai pada kode lama untuk menyimpan tota...

```javascript
var total = 1000;   // bisa berubah, global/fungsi scope
let jumlah = 5;     // block scope, bisa berubah
const pajak = 0.1;  // block scope, tidak bisa berubah
```

Jika dilihat dari sisi keamanan kode, `let` dan `const` jelas lebih unggul dibandingkan `var`. `let` mencegah kebingungan akibat hoisting yang sering menjerat pemula, sementara `const` menjaga integritas data yang sifatnya konstan. Studi kasus dalam e-commerce menunjukkan bahwa bug perhitungan sering terjadi jika `var` digunakan untuk data transaksi, karena variabel dapat ditimpa secara tidak sengaja di blok berbeda. Dengan beralih ke `let` atau `const`, kode menjadi lebih prediktif dan mudah dirawat. Ha...

Fakta menarik adalah bahwa komunitas developer modern lebih menyarankan penggunaan `const` secara default, dan hanya beralih ke `let` jika nilainya benar-benar berubah. `var` jarang digunakan kecuali untuk kompatibilitas dengan kode lama. Dalam aplikasi besar, pendekatan ini mengurangi kebingungan dan mendorong praktik pemrograman yang konsisten. Dalam konteks toko online dengan ribuan data produk, pemilihan yang tepat antara `let` dan `const` menjaga agar data tidak bercampur. Perbandingan ini membukti...

![Perbandingan Var, Let, dan Const](session-2-part-2/perbandingan-var-let-const.png)  


## Studi Kasus Variabel pada E-Commerce

Untuk memahami penggunaan variabel dalam skenario nyata, mari kita lihat studi kasus pada aplikasi e-commerce. Ketika pelanggan menambahkan barang ke keranjang, sistem perlu menyimpan nama produk, jumlah, dan harga. Variabel digunakan sebagai tempat penyimpanan sementara agar informasi ini dapat diolah untuk perhitungan total belanja. Misalnya, `let jumlahProduk` digunakan untuk menampung kuantitas barang, sementara `const pajak` tetap digunakan untuk menghitung tambahan biaya sesuai aturan yang berlaku...

```javascript
let jumlahProduk = 3;
const pajak = 0.1;
let hargaSatuan = 50000;
let total = jumlahProduk * hargaSatuan;
let totalDenganPajak = total + (total * pajak);
console.log(totalDenganPajak); // 165000
```

Selain menyimpan data transaksi, variabel juga penting untuk mengelola status pengguna. Misalnya, variabel `let isLoggedIn` digunakan untuk melacak apakah pelanggan sudah masuk ke akun atau belum. Jika nilainya `true`, maka sistem menampilkan tombol checkout, jika `false`, maka pengguna diarahkan ke halaman login. Dengan menggunakan variabel boolean sederhana, aplikasi dapat mengubah perilaku sesuai kondisi nyata. Studi kasus ini menunjukkan bagaimana variabel mendukung logika bisnis yang kompleks dalam e...

```javascript
let isLoggedIn = false;
if (isLoggedIn) {
  console.log("Lanjutkan ke checkout");
} else {
  console.log("Silakan login terlebih dahulu");
}
```

Fakta menarik adalah bahwa meskipun variabel terlihat sederhana, pengelolaannya bisa memengaruhi performa aplikasi. Dalam e-commerce dengan ribuan transaksi per menit, deklarasi variabel yang tepat membantu mengurangi potensi bug dan menjaga stabilitas sistem. Misalnya, penggunaan `const` untuk data tetap seperti kurs mata uang mencegah perubahan yang bisa merusak laporan keuangan. Sementara itu, `let` memberikan fleksibilitas untuk data yang terus berubah, seperti stok produk. Studi kasus ini menegaskan...

![Studi Kasus Variabel pada E-Commerce](session-2-part-2/studi-kasus-ecommerce.png)  


## Kesimpulan

Variabel adalah fondasi utama dalam JavaScript karena menjadi wadah penyimpanan data yang dibutuhkan hampir di setiap baris program. Melalui pemahaman `var`, kita belajar mengenai fleksibilitas sekaligus risiko hoisting yang sering menimbulkan bug. Dengan `let`, kita mendapatkan kontrol yang lebih baik melalui block scope yang membatasi cakupan variabel agar tidak saling menimpa. `const` hadir untuk menjaga nilai tetap, meskipun masih memungkinkan perubahan isi data kompleks seperti array atau objek. A...



## Referensi

- Flanagan, D. (2020). *JavaScript: The Definitive Guide*. O’Reilly Media.  
- Haverbeke, M. (2018). *Eloquent JavaScript*. No Starch Press.  
- Freeman, E. (2014). *Head First JavaScript Programming*. O’Reilly Media.  
- Crockford, D. (2008). *JavaScript: The Good Parts*. O’Reilly Media.  
- Mozilla Developer Network. (2022). *MDN Web Docs – JavaScript Guide*.  

