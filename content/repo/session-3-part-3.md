---
date: 2025-09-27T10:00:00+07:00
draft: false
title: "Latihan operator aritmatika dalam perhitungan JavaScript"
short: "Operator"
thumb:
    image: "cover.jpg"
    anima: ""
    video: ""
layout: "module"
weight: 3
lister: 3
format:
    media: "article"
    model: "practical"
    datum:
        data: "Operator dan Ekspresi"
outcome:
    - prop: ""
      name: "Konseptual"
      icon: ""
      desc: "Memahami peran operator aritmatika dalam membangun logika program."
    - prop: ""
      name: "Praktik"
      icon: ""
      desc: "Mampu melakukan perhitungan sederhana menggunakan operator aritmatika dalam kasus nyata perpustakaan."
require:
    - prop: "Dasar Variabel"
      name: "Variabel & Tipe Data"
      icon: "code"
      desc: "Diperlukan pemahaman variabel untuk menyimpan nilai yang akan dihitung."
metadata:
    index: false
    thumb: "cover.jpg"
    group: []
    author: ["Al Muhdil Karim"]
description: "Modul ini memberikan latihan praktis penggunaan operator aritmatika dalam JavaScript dengan studi kasus sistem perpustakaan."
---

### Pendahuluan

Pernahkah Anda mencoba menghitung jumlah buku yang dipinjam dalam sebuah sistem perpustakaan, namun hasilnya tidak sesuai harapan? Situasi ini sering terjadi ketika operator aritmatika tidak digunakan dengan benar. Dalam dunia pemrograman, kesalahan kecil dalam urutan operasi dapat menimbulkan hasil yang jauh berbeda dari yang diharapkan. Misalnya, menghitung denda keterlambatan dengan urutan operasi yang salah bisa menghasilkan angka yang lebih besar dari seharusnya, sehingga merugikan anggota perpustakaan.  

Bayangkan seorang pustakawan yang harus menghitung denda dari 5 buku yang terlambat dikembalikan, masing-masing 3 hari. Jika ia salah menempatkan tanda kurung atau operator, hasil yang seharusnya Rp15.000 mungkin menjadi Rp150.000. Kasus sederhana ini menunjukkan bahwa logika matematis dalam kode tidak boleh dianggap remeh. JavaScript menyediakan operator aritmatika untuk membantu proses ini, tetapi cara kita menggunakannya akan menentukan ketepatan hasil.  

Dalam modul ini, kita akan berlatih menggunakan operator aritmatika dasar dengan pendekatan kasus nyata di perpustakaan. Anda akan menemukan bagaimana operator `+`, `-`, `*`, `/`, dan `%` dapat digunakan untuk berbagai skenario, mulai dari menghitung jumlah buku hingga denda keterlambatan. Latihan ini akan mempersiapkan Anda agar tidak terjebak pada kesalahan sederhana yang bisa berdampak besar. Mari kita mulai dengan memahami konsep dasar operator sebelum masuk ke tahap instruksi perhitungan.  

![pendahuluan](session-3-part-3/pendahuluan.png)  

### Konsep Dasar Operator Aritmatika

Operator aritmatika adalah simbol yang digunakan untuk melakukan perhitungan matematis dalam JavaScript. Secara umum, terdapat lima operator dasar yaitu `+` (tambah), `-` (kurang), `*` (kali), `/` (bagi), dan `%` (modulo/sisa bagi). Masing-masing operator memiliki aturan penggunaan yang jelas serta urutan prioritas (operator precedence) yang menentukan bagaimana ekspresi dievaluasi. Misalnya, perkalian dan pembagian memiliki prioritas lebih tinggi dibandingkan penjumlahan dan pengurangan【50†sourc...

Dalam kasus perpustakaan, operator ini dapat digunakan untuk menghitung berbagai data. Sebagai contoh, `+` bisa menjumlahkan total buku yang dipinjam oleh anggota, sedangkan `-` digunakan untuk menghitung sisa kuota peminjaman. Operator `*` bermanfaat saat menghitung denda berdasarkan jumlah hari keterlambatan, sementara `/` dapat dipakai untuk menghitung rata-rata buku yang dipinjam setiap minggu. Adapun `%` sangat berguna dalam menentukan pola, misalnya mengecek apakah jumlah peminjaman genap at...

Salah satu hal penting yang perlu diingat adalah penggunaan tanda kurung `( )`. Tanda kurung berfungsi untuk mengubah urutan evaluasi agar sesuai dengan kebutuhan logika. Sebagai contoh, jika ingin menghitung total denda dengan rumus `(jumlahBuku * hariTerlambat) * tarifDenda`, maka tanda kurung memastikan perkalian jumlah buku dengan hari keterlambatan dilakukan lebih dulu sebelum dikalikan dengan tarif. Jika tanda kurung diabaikan, hasil bisa jadi berbeda dari yang diharapkan【50†source】.  

Para peneliti menekankan bahwa memahami operator dasar adalah langkah penting sebelum melangkah ke ekspresi kompleks (Flanagan, 2020; Haverbeke, 2018). Pengetahuan ini membantu programmer menulis kode yang tidak hanya benar tetapi juga mudah dipahami. Operator aritmatika, meskipun terlihat sederhana, adalah fondasi dari logika perhitungan dalam hampir semua aplikasi, termasuk sistem perpustakaan【50†source】.  

![konsep-dasar](session-3-part-3/konsep-dasar.png)  

### Instruksi Perhitungan Dasar

Tujuan akhir dari praktik ini adalah mengajarkan Anda bagaimana menggunakan operator aritmatika JavaScript untuk menghitung data numerik sederhana dalam sistem perpustakaan. Dengan mengikuti instruksi berikut, Anda akan mampu menghitung sisa stok buku, total denda keterlambatan, serta rata-rata peminjaman anggota. Latihan ini disusun secara sistematis agar Anda terbiasa menulis kode yang benar, jelas, dan mudah dipelihara.  

**Langkah 1: Menghitung Sisa Buku di Perpustakaan**  
Buat variabel untuk menyimpan jumlah buku awal dan jumlah buku yang dipinjam, kemudian gunakan operator `-` untuk menghitung sisa buku. Instruksi ini berlaku sama pada Windows, Linux, dan Mac karena JavaScript dijalankan dalam Node.js maupun browser tanpa perbedaan sintaks.  

```javascript
// Windows / Linux / Mac
let totalBuku = 120;
let dipinjam = 35;
let sisaBuku = totalBuku - dipinjam;

console.log("Sisa buku di perpustakaan:", sisaBuku);
```  

Kode ini memperlihatkan penggunaan operator pengurangan `-`. Jika total buku adalah 120 dan 35 dipinjam, maka hasilnya adalah 85. Konsep sederhana ini penting karena operator pengurangan adalah salah satu alat paling sering dipakai dalam logika sistem pengelolaan data【43†source】.  

**Langkah 2: Menghitung Total Denda Keterlambatan**  
Hitung total denda berdasarkan jumlah hari keterlambatan dan tarif per hari. Operator perkalian `*` digunakan untuk menggabungkan ketiga variabel tersebut.  

```javascript
// Windows / Linux / Mac
let hariTerlambat = 4;
let tarifDenda = 2000;
let jumlahBukuTerlambat = 3;

let totalDenda = jumlahBukuTerlambat * hariTerlambat * tarifDenda;
console.log("Total denda keterlambatan:", totalDenda);
```  

Kode ini akan menghasilkan Rp24.000 jika 3 buku terlambat 4 hari dengan tarif Rp2.000 per hari. Operator perkalian bekerja sesuai aturan prioritas, namun penggunaan tanda kurung dapat memberi kejelasan tambahan. Seperti yang disampaikan oleh Haverbeke (2018), tanda kurung membantu developer menuliskan ekspresi yang mudah dipahami sekaligus mencegah kesalahan logika【50†source】.  

**Langkah 3: Menghitung Rata-Rata Peminjaman Buku per Anggota**  
Gunakan operator pembagian `/` untuk menghitung rata-rata buku yang dipinjam setiap anggota perpustakaan.  

```javascript
// Windows / Linux / Mac
let totalAnggota = 7;
let rataPinjam = dipinjam / totalAnggota;

console.log("Rata-rata buku dipinjam per anggota:", rataPinjam);
```  

Jika 35 buku dipinjam oleh 7 anggota, maka hasilnya adalah 5 buku per anggota. Operator pembagian sangat bermanfaat untuk analisis data, misalnya memahami pola peminjaman rata-rata anggota. Flanagan (2020) menjelaskan bahwa operator pembagian merupakan fondasi dari kalkulasi analitik sederhana hingga lanjutan dalam aplikasi JavaScript【50†source】.  

> **Tip:** Jalankan setiap kode langkah demi langkah, bukan sekaligus, agar lebih mudah memahami perbedaan fungsi tiap operator.  

![instruksi](session-3-part-3/instruksi.png)  

### Studi Kasus Sosial Media  

Operator aritmatika tidak hanya relevan dalam sistem perpustakaan, tetapi juga sangat penting dalam pengembangan aplikasi sosial media. Pada platform seperti Facebook atau Instagram, setiap postingan biasanya memiliki interaksi berupa "like", "love", atau "wow" yang bisa dihitung secara matematis. Untuk memahami keterlibatan pengguna, kita perlu menjumlahkan semua reaksi ini agar mendapatkan data yang jelas tentang performa sebuah konten. Dengan memanfaatkan operator penjumlahan `+`, total interaksi ...

```javascript
// Windows / Linux / Mac
let like = 120;
let love = 80;
let wow = 25;

let totalReaksi = like + love + wow;
console.log("Total reaksi postingan:", totalReaksi);
```  

Kode di atas menjumlahkan tiga kategori reaksi yang berbeda menjadi satu nilai total. Jika ditambahkan hasilnya menjadi 225, angka ini bisa dipakai untuk mengevaluasi popularitas postingan. Menurut Flanagan (2020), operator aritmatika berfungsi sebagai pondasi dasar dalam pengolahan data numerik, yang kemudian digunakan untuk pengambilan keputusan di level aplikasi【50†source】. Dengan cara ini, kita bisa mengetahui konten mana yang lebih menarik dibandingkan lainnya.  

Selain menjumlahkan, operator pembagian `/` juga berperan penting dalam menganalisis data interaksi. Misalnya, seorang pengembang ingin mengetahui rata-rata reaksi per pengguna untuk menilai keterlibatan. Dengan membagi total reaksi dengan jumlah pengguna, informasi yang lebih mendalam dapat diperoleh.  

```javascript
let jumlahPengguna = 25;
let rataReaksi = totalReaksi / jumlahPengguna;

console.log("Rata-rata reaksi per pengguna:", rataReaksi);
```  

Kode ini menghasilkan rata-rata 9 reaksi per pengguna. Informasi ini bisa dipakai untuk menentukan apakah keterlibatan pengguna sudah sesuai ekspektasi. Dengan pendekatan ini, tim pengembang dapat mengatur strategi konten agar lebih efektif. Analisis rata-rata menggunakan operator pembagian sangat umum dilakukan pada sistem analitik sosial media.  

Operator modulo `%` juga memiliki kegunaan dalam konteks sosial media, terutama untuk melakukan pengujian pola data. Misalnya, kita ingin mengetahui apakah total reaksi adalah bilangan genap atau ganjil. Informasi sederhana ini bisa berguna untuk menguji algoritma statistik atau sekadar untuk validasi logika.  

```javascript
if (totalReaksi % 2 === 0) {
  console.log("Total reaksi adalah angka genap");
} else {
  console.log("Total reaksi adalah angka ganjil");
}
```  

Dengan hasil ini, aplikasi bisa menampilkan pesan tambahan atau bahkan menyesuaikan strategi tampilan konten. Operator modulo memang terlihat sederhana, tetapi sering menjadi bagian dari logika validasi di balik layar aplikasi. Menurut Haverbeke (2018), operator seperti `%` berperan penting dalam pengendalian alur program berbasis data numerik【50†source】. Hal ini membuktikan bahwa setiap operator, sekecil apa pun perannya, memiliki dampak nyata pada analisis data.  

![studi-kasus-sosial-media](session-3-part-3/studi-kasus-sosial-media.png)  

### Validasi & Debugging  

Setelah menyelesaikan perhitungan dengan operator aritmatika, langkah penting berikutnya adalah melakukan validasi hasil. Validasi berarti memastikan bahwa nilai yang dihitung sesuai dengan ekspektasi logika sistem. Misalnya, ketika menghitung rata-rata reaksi per pengguna, hasil tidak boleh lebih besar dari total reaksi itu sendiri. Tanpa validasi, kesalahan kecil dapat lolos dan menghasilkan output yang menyesatkan. Oleh karena itu, validasi adalah jembatan penting antara logika perhitungan dan...

Salah satu cara validasi paling dasar dalam JavaScript adalah dengan menggunakan `console.log()`. Metode ini memungkinkan pengembang menampilkan hasil sementara ke layar sehingga dapat dibandingkan dengan perhitungan manual. Jika hasil berbeda, berarti terdapat kesalahan pada logika operator atau urutan operasi. Validasi sederhana dengan `console.log()` sangat efektif digunakan pada tahap awal belajar JavaScript, sebelum beralih ke teknik debugging yang lebih kompleks【43†source】.  

```javascript
// Windows / Linux / Mac
let totalBuku = 100;
let dipinjam = 25;
let sisaBuku = totalBuku - dipinjam;

console.log("Sisa buku dihitung manual:", 75);
console.log("Sisa buku hasil program:", sisaBuku);
```  

Dalam contoh ini, kita membandingkan hasil manual (75) dengan output program. Jika hasilnya sama, berarti operator berfungsi dengan benar. Jika berbeda, maka developer harus menelusuri apakah ada kesalahan pada deklarasi variabel atau penggunaan operator. Cara sederhana ini membantu menghindari kesalahan logika yang bisa merembet ke fitur lain.  

Selain validasi, debugging juga memegang peran penting. Debugging adalah proses menemukan dan memperbaiki bug, yaitu kesalahan yang membuat hasil perhitungan tidak sesuai harapan. Salah satu strategi debugging adalah memecah ekspresi kompleks menjadi beberapa langkah lebih kecil. Dengan demikian, setiap bagian dapat diperiksa hasilnya satu per satu. Teknik ini sesuai dengan prinsip "divide and conquer" yang umum dipakai dalam rekayasa perangkat lunak (Fowler, 2018)【50†source】.  

> **Info Penting:** Jangan mengandalkan tebakan dalam debugging. Selalu gunakan alat bantu seperti `console.log`, breakpoint di DevTools, atau bahkan kalkulasi manual untuk membuktikan benar-tidaknya hasil.  

![validasi-debugging](session-3-part-3/validasi-debugging.png)  

### Kesalahan Umum  

Penggunaan operator aritmatika dalam JavaScript sering kali menimbulkan masalah jika tidak dipahami dengan benar. Banyak pemula yang tidak menyadari bahwa ekspresi matematis memiliki aturan prioritas tertentu. Akibatnya, hasil perhitungan bisa jauh berbeda dari yang diinginkan. Selain itu, kesalahan dalam memilih operator juga sering membuat logika program tidak berjalan sesuai harapan. Pemahaman yang kurang matang terhadap operator ini dapat menimbulkan bug tersembunyi yang sulit dilacak. Oleh k...

**1. Salah Urutan Operasi**  
Kesalahan ini terjadi ketika developer lupa menambahkan tanda kurung pada ekspresi yang kompleks.  

```javascript
// Salah
let hasil1 = 10 + 5 * 2; // Hasil: 20

// Benar
let hasil2 = (10 + 5) * 2; // Hasil: 30
```  

Tanpa tanda kurung, JavaScript akan mendahulukan perkalian sebelum penjumlahan sesuai aturan *operator precedence*. Hal ini membuat hasil tidak sesuai dengan maksud programmer. Flanagan (2020) menekankan bahwa tanda kurung secara eksplisit membantu meningkatkan keterbacaan kode dan mencegah kesalahan perhitungan【50†source】. Banyak bug kritis pada aplikasi besar justru bermula dari kesalahan sederhana seperti ini. Untuk menghindarinya, biasakan selalu menambahkan tanda kurung meskipun Anda sudah ha...

**2. Menggunakan `=` Alih-alih `==` atau `===`**  
Kesalahan lain yang sangat sering adalah salah menggunakan operator assignment saat ingin melakukan perbandingan.  

```javascript
// Salah
let nilai = 0;
if (nilai = 5) {
  console.log("Nilai sama dengan 5");
}

// Benar
if (nilai === 5) {
  console.log("Nilai sama dengan 5");
}
```  

Operator `=` menetapkan nilai baru, bukan membandingkan. Akibatnya, kondisi `if` selalu bernilai benar, dan logika program menjadi tidak valid. Fowler (2018) menekankan pentingnya penggunaan `===` karena membandingkan nilai sekaligus tipe data sehingga mengurangi potensi bug【50†source】. Kesalahan ini biasanya muncul pada tahap awal belajar karena simbolnya terlihat mirip. Cara terbaik menghindarinya adalah dengan mengaktifkan *linting tools* seperti ESLint yang dapat memberikan peringatan otomatis...

**3. Salah Menafsirkan Modulo `%`**  
Banyak pemula mengira operator `%` hanya mengembalikan nilai 0 atau 1.  

```javascript
// Salah
console.log(10 % 3); // Hasil: 1, tapi sering disangka boolean

// Benar
console.log(12 % 5); // Hasil: 2
```  

Operator `%` menghitung sisa pembagian, bukan sekadar menentukan genap atau ganjil. Kesalahan pemahaman ini bisa berakibat fatal saat membagi data ke dalam kelompok. Haverbeke (2018) menjelaskan bahwa modulo merupakan bagian penting dalam algoritma pembagian data dan pola perhitungan berulang【50†source】. Kesalahan memahami `%` biasanya muncul karena asumsi berlebihan dari pengalaman sehari-hari, misalnya hanya melihat genap-ganjil. Untuk menghindarinya, selalu lakukan uji coba kecil pada konsol d...

Dengan memahami ketiga kesalahan umum ini, Anda dapat mengantisipasi masalah lebih awal dalam menulis program. Kesalahan kecil yang terlihat sepele sering kali menjadi sumber bug besar di kemudian hari. Membiasakan diri untuk menggunakan tanda kurung, memahami perbedaan assignment dan comparison, serta menguji operator modulo akan meningkatkan kualitas kode secara signifikan. Kebiasaan ini juga akan mempersiapkan Anda untuk menulis program yang lebih kompleks dengan tingkat kesalahan yang lebih min...

![kesalahan-umum](session-3-part-3/kesalahan-umum.png)  

### Best Practice  

Setelah memahami kesalahan umum, langkah berikutnya adalah menerapkan praktik terbaik agar kode lebih aman dan efisien. Best practice bukan hanya tentang menulis program yang bisa berjalan, tetapi juga tentang membuatnya mudah dipahami, mudah diperbaiki, dan minim risiko bug. Dalam konteks operator aritmatika, praktik terbaik membantu developer menuliskan ekspresi yang jelas, akurat, dan konsisten. Dengan cara ini, kode Anda akan lebih siap digunakan dalam skala proyek yang lebih besar maupun dalam...

**1. Gunakan Tanda Kurung untuk Kejelasan**  
Tanda kurung `( )` memberikan kejelasan tentang urutan operasi dalam sebuah ekspresi.  

```javascript
// Lebih baik
let hasil = (10 + 5) * 2;
console.log("Hasil yang jelas:", hasil);
```  

Tanpa tanda kurung, pembaca kode harus mengingat aturan prioritas operator untuk memahami maksud program. Penambahan tanda kurung memastikan logika terlihat eksplisit dan mencegah salah tafsir. Flanagan (2020) menekankan bahwa penggunaan tanda kurung meningkatkan keterbacaan dan mengurangi bug yang disebabkan oleh salah urutan operasi【50†source】. Dengan membiasakan diri menambahkan tanda kurung, kode akan lebih aman terutama saat dikerjakan dalam tim yang beragam tingkat pemahamannya.  

**2. Selalu Gunakan `===` untuk Perbandingan**  
Menggunakan operator identik `===` memberikan hasil yang lebih ketat dibandingkan `==`.  

```javascript
// Lebih baik
let umur = "25";
if (umur === 25) {
  console.log("Umur sama persis dengan 25");
} else {
  console.log("Tidak sama");
}
```  

Operator `===` memaksa JavaScript membandingkan nilai dan tipe data sekaligus. Hal ini penting untuk menghindari bug yang tidak terlihat, terutama dalam aplikasi yang memproses input dari pengguna. Fowler (2018) menyatakan bahwa `===` adalah standar emas dalam penulisan kode modern karena mengurangi potensi kesalahan akibat *type coercion*【50†source】. Dengan mengutamakan `===`, Anda melatih diri untuk selalu berhati-hati terhadap perbedaan tipe data dalam JavaScript.  

**3. Uji Coba Operator Modulo pada Berbagai Kasus**  
Modulo `%` sebaiknya tidak hanya dipahami sebatas menentukan bilangan genap atau ganjil.  

```javascript
// Pola pembagian data
for (let i = 1; i <= 10; i++) {
  if (i % 3 === 0) {
    console.log(i, "kelipatan 3");
  }
}
```  

Penggunaan modulo pada kasus nyata jauh lebih luas, misalnya membagi data ke dalam kelompok atau membuat pola perulangan tertentu. Haverbeke (2018) menekankan bahwa `%` adalah operator penting dalam membangun algoritma berbasis pola【50†source】. Dengan menguji berbagai input, Anda dapat memahami perilaku modulo lebih dalam. Latihan ini juga melatih Anda untuk berpikir kreatif dalam memanfaatkan operator aritmatika sederhana.  

Dengan menerapkan praktik terbaik di atas, kode JavaScript Anda akan lebih mudah dipahami, lebih aman, dan lebih andal. Best practice membantu developer menghindari kesalahan sejak awal, sekaligus memperkuat disiplin menulis kode yang profesional. Kode yang jelas, konsisten, dan rapi adalah kunci untuk membangun aplikasi yang tahan lama dan mudah dikelola dalam jangka panjang.  

![best-practice](session-3-part-3/best-practice.png)  

### Mini Aplikasi  

Untuk menguatkan pemahaman Anda mengenai operator aritmatika, mari kita membangun sebuah mini aplikasi sederhana. Aplikasi ini akan menampilkan laporan ringkas dari sistem sosial media berupa jumlah reaksi, rata-rata reaksi per pengguna, dan status genap atau ganjil dari total reaksi. Tujuan utamanya adalah menggabungkan konsep penjumlahan, pembagian, dan modulo dalam satu alur logika. Dengan demikian, Anda akan lebih mudah memahami bagaimana operator aritmatika bekerja secara bersamaan.  

``...

Kode di atas menyatukan beberapa operator sekaligus: `+` untuk penjumlahan reaksi, `/` untuk menghitung rata-rata, dan `%` untuk memeriksa status genap atau ganjil. Fungsi `laporanReaksi` menampilkan informasi yang mirip dengan dashboard analitik sosial media. Menurut Flanagan (2020), latihan menggabungkan operator dalam satu fungsi membantu pemula mengembangkan pola berpikir logis yang lebih sistematis【50†source】.  

Selain itu, mini aplikasi ini bisa dikembangkan lebih jauh. Misalnya, Anda bisa menambahkan fitur validasi untuk memastikan jumlah pengguna tidak nol agar tidak terjadi kesalahan pembagian. Anda juga dapat memperluasnya dengan menampilkan persentase setiap jenis reaksi. Dengan cara ini, Anda tidak hanya melatih operator aritmatika, tetapi juga belajar menyusun alur program kecil yang bermanfaat.  

> **Tip:** Cobalah ubah nilai input dalam pemanggilan fungsi untuk melihat bagaimana hasil laporan berubah. Eksperimen seperti ini adalah cara terbaik untuk melatih intuisi Anda dalam penggunaan operator.  

![mini-aplikasi](session-3-part-3/mini-aplikasi.png)  

### Kesimpulan  

Modul ini memperlihatkan bagaimana operator aritmatika berfungsi sebagai fondasi penting dalam membangun logika program yang jelas dan akurat. Dimulai dari pemahaman konsep dasar, Anda telah berlatih menghitung data sederhana menggunakan instruksi langkah demi langkah. Studi kasus sosial media membantu memperluas perspektif tentang penerapan operator dalam situasi nyata yang dekat dengan kehidupan sehari-hari. Validasi dan debugging memberikan bekal keterampilan untuk memastikan hasil perhitungan s...

### Referensi  

- Flanagan, D. (2020). *JavaScript: The Definitive Guide*. O’Reilly Media.  
- Haverbeke, M. (2018). *Eloquent JavaScript*. No Starch Press.  
- Fowler, M. (2018). *Refactoring: Improving the Design of Existing Code*. Addison-Wesley.  
- Freeman, E., & Robson, E. (2014). *Head First JavaScript Programming*. O’Reilly Media.  
- Mozilla Developer Network. (2022). *MDN Web Docs – JavaScript Guide*.  
