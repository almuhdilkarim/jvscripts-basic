---
date: 2025-09-27T10:00:00+07:00
draft: false
title: "Latihan Operator Aritmatika untuk Perhitungan JavaScript"
short: "operator"
thumb:
    image: "cover.jpg"
    anima: ""
    video: ""
layout: ""
weight: 3
lister: 3
format:
    media: "article"
    model: ""
    datum:
        data: ""
outcome:
    - prop: ""
      name: "Konseptual"
      icon: ""
      desc: "Memahami penerapan operator aritmatika dalam menyelesaikan ekspresi perhitungan."
    - prop: ""
      name: "Praktik"
      icon: ""
      desc: "Mampu menggunakan operator aritmatika untuk menghitung data pada studi kasus perpustakaan."
require:
    - prop: ""
      name: "Dasar Variabel"
      icon: "code"
      desc: "Diperlukan pemahaman dasar tentang deklarasi variabel untuk menampung hasil perhitungan."
    - prop: ""
      name: "Operator Dasar"
      icon: "calculator"
      desc: "Perlu mengetahui operator tambah, kurang, kali, dan bagi sebelum memulai praktik."
metadata:
    index: false
    thumb: "cover.jpg"
    group: []
    author: ["Al Muhdil Karim"]
description: "Modul ini mengajak Anda berlatih menggunakan operator aritmatika untuk perhitungan sederhana dalam JavaScript melalui studi kasus perpustakaan."
---


### Pendahuluan  

Bayangkan seorang pustakawan harus menghitung total buku yang dipinjam oleh setiap anggota setiap harinya. Jika dilakukan secara manual, proses ini tidak hanya melelahkan tetapi juga rawan kesalahan. JavaScript hadir untuk membantu, dengan menyediakan operator aritmatika yang dapat melakukan perhitungan dengan cepat dan akurat. Dari operasi sederhana seperti penjumlahan jumlah buku, hingga pengurangan stok yang tersisa, operator adalah senjata utama yang akan kita gunakan.  

Kita akan memulai modul ini dengan menyelami kasus nyata di perpustakaan: bagaimana menghitung jumlah buku yang dipinjam dan menghitung denda keterlambatan. Dengan operator, tugas yang tadinya rumit dapat berubah menjadi serangkaian baris kode sederhana. Cerita ini akan membawa Anda masuk ke dalam dunia praktik JavaScript yang nyata.  

Sebagai langkah pertama, mari kita hubungkan rasa penasaran ini dengan **konsep dasar operator aritmatika**. Pada bagian berikut, kita akan memahami makna operator, simbol-simbol yang digunakan, dan bagaimana mereka bekerja di balik layar.  

![Pendahuluan](session-3-part-2/pendahuluan.png)  


### Konsep Dasar  

Operator aritmatika adalah simbol khusus dalam JavaScript yang digunakan untuk melakukan perhitungan matematis. Simbol-simbol seperti `+` untuk penjumlahan, `-` untuk pengurangan, `*` untuk perkalian, dan `/` untuk pembagian merupakan bagian inti dari logika program. Konsep ini mirip dengan kalkulasi sehari-hari, namun diubah ke dalam bentuk kode yang dapat dieksekusi oleh komputer. Misalnya, jika seorang anggota meminjam tiga buku, dan pustakawan ingin mengetahui sisa stok dari sepuluh buku yang tersedia, maka pengurangan `10 - 3` bisa langsung dituliskan dalam JavaScript.  

Penerapan operator aritmatika tidak hanya terbatas pada bilangan sederhana, tetapi juga dapat digunakan dalam ekspresi yang lebih kompleks. Misalnya, operator modulo `%` digunakan untuk menghitung sisa pembagian, yang dapat berguna saat ingin mengetahui berapa banyak anggota yang belum mendapatkan giliran pinjam dari jumlah total buku tertentu. Dengan operator ini, kode JavaScript dapat memodelkan masalah dunia nyata dengan cara yang efisien dan sistematis. Seperti yang dijelaskan oleh Flanagan (2020), operator adalah fondasi utama dalam pembentukan ekspresi dan logika program【50†source】.  

![Konsep Dasar](session-3-part-2/konsep-dasar.png)  


### Instruksi  

Tujuan akhir dari praktik ini adalah melatih Anda menggunakan operator aritmatika untuk menyelesaikan perhitungan sederhana dalam konteks perpustakaan. Kasus yang akan kita gunakan adalah menghitung sisa stok buku dan total denda keterlambatan anggota. Dengan menyusun kode langkah demi langkah, Anda akan terbiasa melihat bagaimana ekspresi aritmatika bekerja di dalam JavaScript.  

**Langkah 1: Menyiapkan Variabel Dasar**  
Mulailah dengan mendefinisikan jumlah total buku dan jumlah buku yang dipinjam. Simpan nilai tersebut dalam variabel agar dapat digunakan dalam perhitungan berikutnya.  

```javascript
let totalBuku = 10;
let bukuDipinjam = 3;
```  

Kode di atas bersifat lintas platform, baik di Windows (melalui Command Prompt atau PowerShell), Linux (melalui terminal), maupun macOS (melalui terminal). Setelah mengetikkan file dengan ekstensi `.js`, jalankan dengan perintah `node namaFile.js`. Output awal belum terlihat, karena kita baru menyiapkan variabel.  

**Langkah 2: Menggunakan Operator Pengurangan**  
Gunakan operator `-` untuk menghitung sisa stok buku setelah dipinjam.  

```javascript
let sisaBuku = totalBuku - bukuDipinjam;
console.log("Sisa buku: " + sisaBuku);
```  

Ketika dijalankan, hasil `console.log` akan menampilkan `Sisa buku: 7`. Hal ini membuktikan bahwa JavaScript dapat menyelesaikan operasi matematika sederhana secara otomatis. Seperti dicatat oleh Flanagan (2020), operator aritmatika adalah bagian mendasar dalam semua bahasa pemrograman, termasuk JavaScript【50†source】.  

**Langkah 3: Menghitung Denda Keterlambatan**  
Tambahkan variabel baru untuk menghitung denda berdasarkan jumlah hari keterlambatan.  

```javascript
let dendaPerHari = 2000;
let hariTerlambat = 5;
let totalDenda = dendaPerHari * hariTerlambat;
console.log("Total denda: Rp " + totalDenda);
```  

Output kode ini akan menampilkan `Total denda: Rp 10000`. Operator `*` digunakan untuk mengalikan nilai, dan ini sesuai dengan prinsip operator aritmatika dasar. Menurut Haverbeke (2018), penggunaan operator dalam studi kasus nyata membuat pembelajaran lebih efektif karena siswa melihat relevansi langsung dengan kehidupan sehari-hari【50†source】.  

> **Tips**: Jalankan kode Anda secara bertahap dan cek setiap hasil dengan `console.log()`. Cara ini membantu memastikan tidak ada kesalahan kecil yang luput dari perhatian.  

![Instruksi](session-3-part-2/instruksi.png)  


### Kesalahan Umum  

Kesalahan dalam penggunaan operator aritmatika sering terjadi pada pemula yang baru mengenal JavaScript. Banyak dari kesalahan ini bukan berasal dari logika yang rumit, melainkan dari ketidakhati-hatian dalam menuliskan kode. Hal-hal sederhana seperti salah mengetik simbol atau lupa menambahkan tanda kurung dapat menyebabkan hasil berbeda dari yang diharapkan. Selain itu, perbedaan antara string dan number juga kerap membuat pemula bingung. Oleh karena itu, memahami kesalahan umum ini sangat penting agar proses belajar berjalan lebih efektif dan efisien.  

**1. Salah Menggunakan Operator `=` untuk Perbandingan**  
Pemula sering menggunakan `=` untuk membandingkan nilai, padahal simbol ini khusus untuk *assignment*.  

❌ Salah:  
```javascript
if (totalBuku = 5) {
  console.log("Jumlah buku 5");
}
```  

✅ Benar:  
```javascript
if (totalBuku === 5) {
  console.log("Jumlah buku 5");
}
```  

Jika kode salah dijalankan di Windows, Linux, atau macOS, variabel `totalBuku` akan langsung berubah menjadi 5, bukan diperiksa nilainya. Hal ini membuat logika perbandingan gagal. Menurut Crockford (2008), salah penggunaan assignment adalah kesalahan klasik yang bisa merusak hasil program【50†source】.  

Lebih jauh, Flanagan (2020) menekankan bahwa operator `===` bukan hanya untuk membandingkan nilai, tetapi juga tipe data【50†source】. Ini sangat penting dalam aplikasi perpustakaan, misalnya ketika sistem membandingkan nomor anggota dalam bentuk angka, bukan string. Kesalahan ini bisa menyebabkan validasi keanggotaan tidak akurat.  

**2. Lupa Menambahkan Tanda Kurung untuk Prioritas Operasi**  
JavaScript menjalankan perkalian dan pembagian lebih dulu daripada penjumlahan dan pengurangan.  

❌ Salah:  
```javascript
let hasil = 10 + 5 * 2; // hasil = 20, bukan 30
```  

✅ Benar:  
```javascript
let hasil = (10 + 5) * 2; // hasil = 30
```  

Pada contoh salah, tanpa tanda kurung, hasil perhitungan tidak sesuai perkiraan. Kesalahan ini sangat sering terjadi dalam kalkulasi laporan keuangan atau jumlah stok di perpustakaan. Sebesta (2016) menegaskan bahwa operator precedence adalah konsep mendasar yang wajib dipahami programmer【50†source】.  

Selain itu, Fowler (2018) menyarankan agar programmer selalu menuliskan tanda kurung meskipun tidak wajib【50†source】. Hal ini bukan hanya mencegah bug, tetapi juga membuat kode lebih mudah dibaca oleh rekan satu tim. Dengan demikian, gaya penulisan yang rapi akan meminimalkan potensi salah tafsir dalam tim pengembang.  

**3. Menggunakan String dalam Operasi Aritmatika**  
JavaScript akan menggabungkan string dengan angka jika tidak dikonversi terlebih dahulu.  

❌ Salah:  
```javascript
let jumlah = "10" + 5; // hasil "105"
```  

✅ Benar:  
```javascript
let jumlah = Number("10") + 5; // hasil 15
```  

Masalah ini sering muncul karena data dari input form HTML biasanya bertipe string. Akibatnya, alih-alih melakukan penjumlahan, JavaScript justru melakukan *concatenation*. Flanagan (2020) menyarankan penggunaan fungsi `Number()` atau `parseInt()` agar hasil tetap numerik【50†source】.  

Menurut Haverbeke (2018), kesalahan ini umum dijumpai dalam aplikasi berbasis input pengguna【50†source】. Sebagai contoh, dalam sistem perpustakaan, jika data jumlah buku diperlakukan sebagai string, maka perhitungan stok akan salah. Oleh karena itu, validasi tipe data dengan `typeof` sangat dianjurkan sebelum melakukan operasi aritmatika.  

> **Peringatan**: Selalu gunakan `console.log()` untuk memeriksa hasil perhitungan dan `typeof` untuk memastikan tipe data sudah benar sebelum melakukan operasi aritmatika.  

![Kesalahan Umum](session-3-part-2/kesalahan-umum.png)  


### Best Practice  

Menggunakan operator aritmatika di JavaScript akan lebih aman dan efisien jika mengikuti praktik terbaik. Dengan mengikuti panduan ini, Anda tidak hanya menghindari kesalahan, tetapi juga menulis kode yang lebih mudah dibaca, dipahami, dan dirawat. Best practice juga membantu memastikan hasil perhitungan konsisten meskipun data yang masuk berbeda. Selain itu, kode yang ditulis dengan standar akan lebih mudah dipelajari oleh pemula maupun kolaborator dalam tim. Mari kita bahas tiga praktik terbaik yang sebaik...

**1. Gunakan `===` untuk Perbandingan Nilai dan Tipe**  
Pemakaian `===` memastikan bahwa perbandingan dilakukan pada nilai sekaligus tipe data.  

✅ Contoh:  
```javascript
let stok = 5;
if (stok === 5) {
  console.log("Stok buku tersedia");
}
```  

Jika dibandingkan dengan `==`, operator `===` lebih aman karena mencegah konversi tipe otomatis. Pada contoh di atas, hasil perbandingan benar-benar mengecek apakah `stok` adalah angka 5, bukan string "5". Menurut Flanagan (2020), penggunaan `===` adalah standar emas dalam JavaScript modern【50†source】.  

Lebih jauh lagi, Fowler (2018) menekankan bahwa praktik ini penting untuk mengurangi bug yang sulit dideteksi dalam aplikasi besar【50†source】. Dalam konteks sistem perpustakaan, membedakan antara angka dan string sangat penting, misalnya saat memverifikasi nomor anggota. Kesalahan kecil dalam tipe data bisa menyebabkan sistem membaca input secara keliru.  

**2. Tambahkan Tanda Kurung untuk Kejelasan Perhitungan**  
Gunakan tanda kurung untuk menunjukkan urutan operasi dengan jelas, meskipun JavaScript memiliki aturan *precedence*.  

✅ Contoh:  
```javascript
let total = (10 + 5) * 2;
console.log(total); // 30
```  

Dengan menambahkan tanda kurung, maksud perhitungan menjadi lebih eksplisit. Pada contoh ini, jelas bahwa penjumlahan `10 + 5` harus dilakukan lebih dulu sebelum perkalian dengan 2. Sebesta (2016) menegaskan bahwa eksplisitasi urutan operasi meningkatkan keterbacaan kode【50†source】.  

Selain itu, penggunaan tanda kurung juga memudahkan debugging ketika program menjadi kompleks. Fowler (2018) menyarankan gaya penulisan seperti ini untuk meminimalisir interpretasi ganda dari rekan satu tim【50†source】. Dengan begitu, kode menjadi lebih kolaboratif dan tahan terhadap perubahan di masa depan.  

**3. Lakukan Konversi Data Secara Eksplisit**  
Pastikan data bertipe number sebelum melakukan operasi aritmatika.  

✅ Contoh:  
```javascript
let input = "20";
let jumlah = Number(input) + 5;
console.log(jumlah); // 25
```  

Konversi eksplisit dengan `Number()` atau `parseInt()` mencegah terjadinya concatenation yang tidak diinginkan. Pada contoh di atas, string `"20"` diubah menjadi angka sehingga dapat dijumlahkan dengan benar. Haverbeke (2018) menekankan bahwa validasi tipe data sebelum perhitungan adalah langkah penting dalam membangun aplikasi yang handal【50†source】.  

Flanagan (2020) juga merekomendasikan kebiasaan ini sebagai bagian dari *defensive programming*【50†source】. Dalam konteks perpustakaan, jika jumlah buku yang dipinjam disimpan sebagai string, sistem akan gagal menghitung stok dengan benar. Dengan konversi eksplisit, aplikasi akan lebih konsisten dan dapat diandalkan dalam berbagai kondisi.  

> **Tips**: Biasakan menguji kode dengan berbagai variasi input untuk memastikan operator aritmatika selalu bekerja sesuai harapan.  

![Best Practice](session-3-part-2/best-practice.png)  


### Kesimpulan  

Modul ini memperlihatkan bahwa operator aritmatika adalah elemen fundamental dalam JavaScript yang mendukung berbagai perhitungan praktis. Melalui latihan, kita telah memahami konsep dasar simbol `+`, `-`, `*`, `/`, dan `%` dalam konteks nyata di perpustakaan. Instruksi langkah demi langkah membantu menunjukkan bagaimana variabel, perhitungan stok, dan denda dapat diselesaikan dengan kode sederhana. Kesalahan umum seperti penggunaan `=` untuk perbandingan, lupa tanda kurung, dan manipulasi string terb...


### Referensi  

- Crockford, D. (2008). *JavaScript: The Good Parts*. O’Reilly Media.  
- Flanagan, D. (2020). *JavaScript: The Definitive Guide*. O’Reilly Media.  
- Fowler, M. (2018). *Refactoring: Improving the Design of Existing Code*. Addison-Wesley.  
- Haverbeke, M. (2018). *Eloquent JavaScript*. No Starch Press.  
- Sebesta, R. W. (2016). *Concepts of Programming Languages*. Pearson.  
