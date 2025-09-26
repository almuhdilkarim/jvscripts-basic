---
date: "2025-09-27T09:00:00+07:00"
draft: false
title: "Pahami tipe data primitif dalam JavaScript dengan studi kasus nyata"
short: "Primitif"
thumb:
    image: "cover.jpg"
    anima: ""
    video: ""
layout: "module"
weight: 2
lister: 4
format:
    media: "article"
    model: ""
    datum:
        data: "2025-09-27"
outcome:
    - prop: "concept"
      name: "Konseptual"
      icon: "book"
      desc: "Mengenali tipe data primitif seperti Number, String, Boolean, Null, Undefined, Symbol, dan BigInt dalam JavaScript."
    - prop: "practice"
      name: "Praktik"
      icon: "code"
      desc: "Mampu mengidentifikasi dan menggunakan tipe data primitif dalam studi kasus sederhana sistem perpustakaan."
require:
    - prop: "basic"
      name: "Dasar Variabel"
      icon: "database"
      desc: "Pemahaman variabel var, let, dan const dibutuhkan sebelum mempelajari tipe data primitif."
metadata:
    index: false
    thumb: "cover.jpg"
    group: ["Variabel & Data"]
    author: ["Al Muhdil Karim"]
description: "Modul ini membahas konsep tipe data primitif dalam JavaScript dengan pendekatan sistematis dan studi kasus kontekstual di perpustakaan."
---


## Pendahuluan  

Bayangkan sebuah perpustakaan digital yang menyimpan ribuan buku dalam sistemnya. Setiap buku memiliki judul, jumlah halaman, status ketersediaan, hingga kode identifikasi unik. Semua informasi tersebut tidak bisa disimpan sembarangan, melainkan harus ditempatkan dalam bentuk yang jelas dan konsisten. Di sinilah konsep *tipe data* berperan, karena komputer hanya bisa memahami informasi jika sudah diubah ke dalam bentuk data yang sesuai.  

Kisah menarik terjadi ketika seorang pengembang junior mencoba membuat sistem katalog buku tanpa memahami tipe data. Ia menyimpan jumlah halaman sebagai teks, status ketersediaan sebagai angka, dan kode buku sebagai kombinasi sembarangan. Akibatnya, sistem sering salah menghitung jumlah halaman, menolak input, bahkan gagal mengenali buku yang seharusnya ada. Dari sini kita bisa melihat bahwa memahami tipe data adalah pondasi agar sistem tidak berantakan.  

Dalam pemrograman JavaScript, konsep *tipe data primitif* menjadi dasar dari semua pengelolaan data. Tipe data ini sederhana, tidak bisa dipecah lagi, namun sangat penting dalam membangun logika yang benar. Sama seperti dalam perpustakaan, buku, rak, dan kode katalog harus memiliki format yang konsisten agar mudah diproses. Maka dari itu, kita perlu menelusuri lebih jauh apa itu tipe data primitif dan bagaimana ia menjadi fondasi bagi pengembang untuk membangun aplikasi yang rapi dan efisien.  

![Pendahuluan](session-2-part-4/pendahuluan.png)  


## Konsep Dasar  

Tipe data primitif adalah kategori data paling sederhana dalam JavaScript yang merepresentasikan nilai tunggal tanpa struktur tambahan. Disebut “primitif” karena data ini tidak dapat dipecah menjadi elemen yang lebih kecil dan tidak memiliki properti maupun method bawaan. Contoh tipe data primitif mencakup *Number*, *String*, *Boolean*, *Null*, *Undefined*, *Symbol*, dan *BigInt*, yang masing-masing memiliki peran penting dalam menyusun logika program. Jika seorang pengembang memahami perbedaan mendasar antar tipe data ini, maka kemungkinan terjadinya kesalahan logika dapat ditekan seminimal mungkin. Flanagan (2020) menegaskan bahwa mengenali karakteristik dasar setiap tipe data adalah langkah awal menuju kode yang aman dan dapat dipelihara dalam jangka panjang【43†source】. Dengan kata lain, penguasaan tipe data primitif menjadi fondasi sebelum beranjak ke konsep lanjutan seperti objek atau array.  

Untuk memahami konsep ini, bayangkan sistem perpustakaan yang menggunakan data berbeda untuk mengelola buku. Judul buku direpresentasikan sebagai *String*, jumlah halaman sebagai *Number*, status ketersediaan sebagai *Boolean*, dan kode katalog besar dapat menggunakan *BigInt*. Jika pustakawan mencampuradukkan kategori ini, maka pencarian, perhitungan, dan pelaporan akan terganggu. Analogi ini sejalan dengan Haverbeke (2018) yang menjelaskan bahwa data dalam program perlu diatur dalam wadah yang sesuai agar dapat digunakan dengan konsisten【43†source】. Oleh karena itu, memahami tipe data primitif bukan hanya masalah teknis, tetapi juga cara berpikir sistematis untuk memastikan integritas data dalam aplikasi sehari-hari.  

> Peringatan: Banyak pemula sering bingung antara *Undefined* dan *Null*, padahal keduanya memiliki makna yang berbeda secara fundamental.  

![Konsep Dasar](session-2-part-4/konsep-dasar.png)  


## Number dalam JavaScript  

Dalam JavaScript, *Number* digunakan untuk merepresentasikan nilai numerik, baik bilangan bulat maupun bilangan desimal. Keunikan JavaScript adalah semua angka, baik integer maupun float, disimpan dalam format *double-precision 64-bit binary* sesuai standar IEEE 754. Hal ini berarti angka 10 dan 10.5 berada dalam tipe data yang sama meskipun berbeda bentuk. Dengan pendekatan ini, JavaScript dapat menyederhanakan penulisan kode, namun juga menghadirkan tantangan berupa keterbatasan presisi. Sebagai cont...

Bayangkan sebuah perpustakaan yang menyimpan data jumlah halaman buku dalam sistem katalog digital. Jika seorang pustakawan ingin menjumlahkan halaman dari dua buku, sistem akan menggunakan tipe data *Number*. Namun, jika sistem harus menghitung total halaman dari banyak buku dengan angka desimal tertentu, seperti perhitungan rata-rata halaman, maka presisi angka menjadi sangat penting. Flanagan (2020) menyebutkan bahwa memahami karakteristik tipe data *Number* membantu programmer menghindari kesalahan d...

Selain itu, *Number* dalam JavaScript memiliki nilai khusus seperti `Infinity`, `-Infinity`, dan `NaN` (*Not a Number*). Nilai `Infinity` muncul ketika angka melebihi batas maksimum representasi, sedangkan `NaN` muncul ketika operasi matematika dilakukan pada data yang tidak valid, seperti `parseInt("buku")`. Dalam konteks perpustakaan, jika sistem mencoba menghitung jumlah halaman dari data yang salah input, hasilnya bisa berupa `NaN`. Haverbeke (2018) menekankan bahwa programmer harus berhati-hati men...

> Tips: Gunakan fungsi `Number.isNaN()` atau `isFinite()` untuk menghindari bug yang disebabkan oleh perhitungan angka yang tidak valid.  

![Number](session-2-part-4/number.png)  


## String dalam JavaScript  

*String* adalah tipe data primitif yang digunakan untuk merepresentasikan teks dalam JavaScript. Nilai string ditulis di antara tanda kutip tunggal (`'...'`), tanda kutip ganda (`"..."`), atau backtick (`` `...` ``) yang memungkinkan penggunaan *template literal*. Template literal memberi fleksibilitas lebih, misalnya menyisipkan ekspresi atau variabel langsung ke dalam teks. Dengan kata lain, string bukan hanya sekadar kumpulan huruf, melainkan alat utama untuk menampilkan informasi kepada pengguna. Fl...

Bayangkan sebuah perpustakaan digital yang ingin menampilkan judul dan nama penulis dalam katalog. Informasi tersebut akan disimpan sebagai string, misalnya `"Belajar JavaScript"` atau `"Jane Doe"`. Jika sistem salah memperlakukan string sebagai angka, tentu akan terjadi kesalahan saat menampilkan data. Haverbeke (2018) menjelaskan bahwa string dalam JavaScript bersifat immutable, artinya setiap kali kita memodifikasi string, sebenarnya kita membuat string baru【43†source】. Fakta ini penting agar pengemb...

Selain itu, string memiliki berbagai *method* bawaan yang memudahkan manipulasi data teks. Misalnya `toUpperCase()`, `toLowerCase()`, dan `slice()` digunakan untuk memodifikasi atau mengambil bagian dari string. Dalam konteks perpustakaan, method ini dapat dipakai untuk membuat pencarian buku tidak sensitif terhadap huruf kapital, atau memotong judul buku yang terlalu panjang untuk ditampilkan. Osmani (2012) menekankan bahwa kemampuan memanfaatkan method string dengan benar meningkatkan kualitas pengala...

> Info: Gunakan template literal dengan backtick untuk membuat teks dinamis lebih mudah dibaca dibandingkan concatenation dengan `+`.  

![String](session-2-part-4/string.png)  


## Boolean dalam JavaScript  

*Boolean* adalah tipe data primitif yang hanya memiliki dua kemungkinan nilai: `true` atau `false`. Sederhananya, boolean digunakan untuk merepresentasikan kondisi logika biner yang menjadi dasar dalam pengambilan keputusan program. Dalam JavaScript, boolean sering muncul pada hasil operasi perbandingan, misalnya `5 > 3` yang bernilai `true` atau `2 === 4` yang bernilai `false`. Flanagan (2020) menegaskan bahwa boolean adalah inti dari kontrol alur program, karena setiap percabangan logika bergantung...

Bayangkan sebuah perpustakaan yang ingin memeriksa status keanggotaan seseorang. Jika anggota masih aktif, maka nilai boolean `true` akan dipakai untuk mengizinkan peminjaman buku. Sebaliknya, jika masa aktif sudah habis, sistem akan memberikan nilai `false` sehingga transaksi peminjaman ditolak. Haverbeke (2018) menjelaskan bahwa boolean tidak hanya mengontrol percabangan, tetapi juga menjadi dasar evaluasi kondisi dalam iterasi seperti *looping*【43†source】. Dengan contoh ini, kita dapat melihat baga...

Selain hasil perbandingan, JavaScript juga mengenal konsep *truthy* dan *falsy*, yaitu cara interpreter memperlakukan nilai non-boolean dalam konteks logika. Misalnya, string kosong `""`, angka nol `0`, `null`, `undefined`, dan `NaN` semuanya dianggap `false`. Sebaliknya, string `"buku"` atau angka `5` dianggap `true`. Menurut Crockford (2008), pemahaman tentang truthy dan falsy penting agar pengembang tidak terjebak dalam bug yang sulit dilacak【43†source】. Dengan memanfaatkan pengetahuan ini, sistem pe...

> Peringatan: Banyak pemula terjebak saat menganggap string kosong (`""`) berbeda dengan `false`, padahal keduanya akan dievaluasi sebagai falsy dalam kondisi if-else.  

![Boolean](session-2-part-4/boolean.png)  


## Null dalam JavaScript  

*Null* adalah tipe data primitif yang merepresentasikan ketiadaan nilai secara eksplisit dalam JavaScript. Artinya, *null* digunakan ketika seorang programmer dengan sengaja ingin menyatakan bahwa sebuah variabel tidak memiliki isi. Hal ini berbeda dengan `undefined` yang menandakan variabel belum diinisialisasi atau tidak memiliki nilai yang didefinisikan. Menurut Flanagan (2020), perbedaan ini sangat penting karena kesalahan memahami *null* dan `undefined` dapat menimbulkan bug yang sulit dilacak【43†...

Bayangkan seorang pustakawan digital yang mengelola data perpustakaan. Ketika sebuah buku hilang atau tidak ditemukan, sistem bisa menandai data lokasi buku tersebut sebagai `null`. Dengan cara ini, pustakawan tahu bahwa lokasi buku tidak ada, bukan sekadar belum dimasukkan ke sistem. Haverbeke (2018) menekankan bahwa *null* memiliki makna semantik yang jelas dan penting dalam desain sistem【43†source】. Misalnya, sebuah kolom database bisa berisi nilai *null* untuk menunjukkan ketiadaan informasi.  

Namun, penggunaan *null* juga dapat memunculkan masalah jika tidak dikelola dengan baik. Banyak pemula sering keliru menganggap *null* sama dengan nilai nol (`0`) atau string kosong (`""`). Padahal, secara teknis keduanya adalah data yang valid, bukan ketiadaan data. Osmani (2012) menjelaskan bahwa kesalahan ini sering menyebabkan aplikasi gagal mengenali kondisi sebenarnya【43†source】. Oleh karena itu, programmer harus hati-hati membedakan antara data kosong, data nol, dan *null*.  

> Tips: Gunakan pemeriksaan ketat dengan `=== null` untuk memastikan bahwa variabel benar-benar bernilai *null*, bukan sekadar falsy lain seperti `0` atau `undefined`.  

![Null](session-2-part-4/null.png)  


## Undefined dalam JavaScript  

*Undefined* adalah tipe data primitif yang merepresentasikan variabel yang telah dideklarasikan tetapi belum diberi nilai. Berbeda dengan *null* yang diberikan secara sengaja, *undefined* muncul secara otomatis ketika JavaScript tidak menemukan nilai dalam suatu variabel. Misalnya, ketika kita menuliskan `let buku;`, maka variabel `buku` akan memiliki nilai *undefined* secara default. Flanagan (2020) menjelaskan bahwa kondisi ini penting untuk dibedakan karena *undefined* menandakan ketiadaan inisial...

Dalam sebuah perpustakaan digital, bayangkan seorang pustakawan menambahkan data buku baru ke sistem, tetapi belum sempat mengisi kolom judulnya. Pada titik ini, nilai judul akan berupa *undefined*, karena sistem mengetahui ada kolom tersebut, namun belum berisi data. Haverbeke (2018) menekankan bahwa *undefined* sering menjadi penyebab bug tersembunyi, terutama ketika pengembang lupa melakukan inisialisasi variabel sebelum digunakan【43†source】. Akibatnya, operasi yang seharusnya berjalan normal bisa g...

Selain itu, JavaScript memiliki perbedaan penting antara *undefined* dan *null* yang kerap membingungkan pemula. Jika sebuah fungsi tidak mengembalikan nilai (*return*), maka hasil eksekusinya akan berupa *undefined*. Osmani (2012) menegaskan bahwa kesalahpahaman antara *null* dan *undefined* dapat memicu kesalahan logika yang serius dalam program【43†source】. Oleh karena itu, pengembang harus membiasakan diri melakukan pemeriksaan kondisi dengan `typeof` atau pengecekan eksplisit menggunakan `=== unde...

> Info: Gunakan operator `??` (*nullish coalescing*) untuk memberikan nilai default ketika variabel bernilai *null* atau *undefined*.  

![Undefined](session-2-part-4/undefined.png)  


## Symbol dalam JavaScript  

*Symbol* adalah tipe data primitif yang diperkenalkan pada ECMAScript 2015 (ES6) untuk merepresentasikan identitas unik. Setiap kali kita membuat sebuah symbol dengan `Symbol()`, hasilnya selalu unik meskipun deskripsi yang diberikan sama. Tidak seperti *String* atau *Number*, nilai symbol tidak dapat dibandingkan secara langsung untuk kesetaraan kecuali berasal dari referensi yang sama. Flanagan (2020) menjelaskan bahwa symbol terutama digunakan untuk membuat properti objek yang tidak akan berbentura...

Bayangkan sebuah sistem perpustakaan digital yang dikelola oleh banyak pengembang. Satu tim menambahkan properti objek `id` untuk buku, sementara tim lain menggunakan nama properti yang sama. Hal ini bisa menimbulkan konflik data. Dengan menggunakan symbol sebagai key, konflik tersebut dapat dihindari karena setiap symbol dijamin unik. Haverbeke (2018) menegaskan bahwa penggunaan symbol sangat bermanfaat dalam membangun sistem berskala besar, terutama ketika ada banyak modul dan pustaka eksternal yang s...

Selain itu, symbol juga digunakan dalam fitur-fitur khusus JavaScript yang disebut *well-known symbols*. Contohnya adalah `Symbol.iterator` yang memungkinkan sebuah objek diiterasi dengan `for...of`. Osmani (2012) menjelaskan bahwa fitur ini membuka jalan bagi pengembang untuk membuat struktur data kustom yang tetap kompatibel dengan mekanisme iterasi standar【43†source】. Dengan demikian, symbol bukan hanya alat untuk menghindari konflik, tetapi juga bagian penting dari ekosistem modern JavaScript.  

> Tips: Gunakan symbol ketika Anda ingin membuat properti objek yang benar-benar privat dan tidak mudah diakses secara tidak sengaja oleh kode lain.  

![Symbol](session-2-part-4/symbol.png)  


## BigInt dalam JavaScript  

*BigInt* adalah tipe data primitif yang diperkenalkan pada ECMAScript 2020 untuk merepresentasikan bilangan bulat dengan ukuran yang lebih besar dari batas aman *Number*. Dalam JavaScript, *Number* menggunakan format IEEE 754 dengan presisi hingga `2^53 - 1`, sehingga angka yang melebihi batas ini berisiko kehilangan akurasi. Dengan *BigInt*, pengembang dapat menangani angka yang sangat besar hanya dengan menambahkan akhiran `n`, misalnya `9007199254740991n`. Flanagan (2020) menekankan bahwa fitur i...

Bayangkan sebuah perpustakaan digital yang memiliki kode identifikasi unik untuk setiap buku dengan panjang angka sangat besar. Jika menggunakan *Number*, sistem mungkin tidak dapat membedakan dua kode yang mirip karena keterbatasan presisi. Namun dengan *BigInt*, angka sebesar apa pun dapat disimpan dan diproses tanpa risiko kesalahan. Haverbeke (2018) menekankan bahwa representasi numerik yang akurat sangat penting untuk menjaga konsistensi data dalam sistem berskala besar【43†source】. Dengan kata lai...

Namun, penggunaan *BigInt* juga memiliki keterbatasan. Tipe ini tidak dapat dicampur langsung dengan *Number* tanpa konversi eksplisit, dan beberapa fungsi bawaan JavaScript tidak mendukungnya. Osmani (2012) mengingatkan bahwa pengembang harus berhati-hati saat memutuskan kapan menggunakan *BigInt* agar tidak menimbulkan bug tak terduga【43†source】. Dalam konteks perpustakaan, jika sistem hanya butuh angka kecil seperti jumlah buku, penggunaan *BigInt* justru akan memperumit kode. Oleh karena itu, *BigI...

> Tips: Gunakan *BigInt* hanya jika Anda benar-benar memerlukan angka yang melampaui batas aman *Number*, dan selalu konversi tipe secara eksplisit saat berinteraksi dengan fungsi bawaan.  

![BigInt](session-2-part-4/bigint.png)  


## Kesimpulan  

Tipe data primitif dalam JavaScript merupakan fondasi utama yang wajib dipahami sebelum melangkah ke konsep lanjutan. *Number* menyediakan representasi numerik, namun memiliki batasan presisi yang diselesaikan oleh *BigInt*. *String* digunakan untuk merepresentasikan teks dan komunikasi antar manusia dengan sistem. *Boolean* menjadi saklar logika yang menentukan alur pengambilan keputusan program. *Null* dan *Undefined* sering membingungkan pemula, tetapi perbedaan keduanya sangat penting untuk menjaga...


## Referensi  

- Crockford, D. (2008). *JavaScript: The Good Parts*. O’Reilly Media.  
- Flanagan, D. (2020). *JavaScript: The Definitive Guide* (7th ed.). O’Reilly Media.  
- Haverbeke, M. (2018). *Eloquent JavaScript* (3rd ed.). No Starch Press.  
- Mozilla Developer Network. (2022). *MDN Web Docs – JavaScript Guide*. Retrieved from https://developer.mozilla.org/  
- Osmani, A. (2012). *Learning JavaScript Design Patterns*. O’Reilly Media.  