---
date: "2025-09-26T09:00:00+07:00"
draft: false
title: "Pahami struktur dasar program JavaScript dengan mudah"
short: "Struktur"
thumb:
    image: "cover.jpg"
    anima: ""
    video: ""
layout: "module"
weight: 1
lister: 5
format:
    media: "article"
    model: "conceptual"
    datum:
        data: "fundamental"
outcome:
    - prop: ""
      name: "Konseptual"
      icon: ""
      desc: "Memahami elemen dasar program seperti statement, ekspresi, variabel, operator, blok kode, dan komentar dalam JavaScript."
    - prop: ""
      name: "Praktik"
      icon: ""
      desc: "Mampu menulis program sederhana e-commerce untuk menghitung total belanja dan diskon menggunakan struktur dasar JavaScript."
require:
    - prop: ""
      name: "Dasar Logika Pemrograman"
      icon: ""
      desc: "Diperlukan pemahaman logika dasar agar mudah mengikuti konsep struktur program JavaScript."
metadata:
    index: false
    thumb: "cover.jpg"
    group: []
    author: ["Al Muhdil Karim"]
description: "Modul ini membahas struktur dasar program JavaScript menggunakan studi kasus e-commerce. Peserta akan belajar statement, ekspresi, variabel, operator, blok kode, dan komentar sebagai fondasi pemrograman modern."
---


## Pendahuluan  

Seorang mahasiswa mencoba menulis program sederhana untuk menghitung diskon belanja online. Ia berharap program itu bisa otomatis mengurangi total harga jika pelanggan membeli lebih dari tiga produk. Namun, kodenya gagal berjalan karena ia tidak memahami struktur dasar JavaScript. Situasi ini menunjukkan betapa pentingnya fondasi sebelum membangun logika yang lebih kompleks.  

Bayangkan sebuah toko online tanpa sistem yang teratur. Jika pesanan tidak dicatat dengan baik, pembeli bisa salah tagih atau tidak mendapatkan diskon yang dijanjikan. JavaScript, seperti kasir digital, mengatur bagaimana setiap instruksi dieksekusi secara runtut. Tanpa struktur yang jelas, alur program akan kacau.  

Struktur dasar program bukan sekadar kumpulan baris kode, tetapi aturan main yang menentukan bagaimana variabel, operator, blok kode, dan komentar bekerja sama. Sama seperti katalog produk yang disusun rapi di e-commerce, kode juga harus tersusun sistematis agar mudah dipahami.  

Dengan memahami struktur dasar ini, pemula dapat melangkah ke konsep lebih lanjut seperti fungsi, perulangan, dan event handling. Pendahuluan ini menjadi jembatan penting menuju pembahasan sistematis mengenai elemen-elemen dasar JavaScript.  

![Pendahuluan](session-1-part-5/intro.png)  

---

## Konsep Dasar  

Struktur program dalam JavaScript dibangun dari **statement** (pernyataan) dan **expression** (ekspresi). *Statement* adalah instruksi lengkap seperti `let total = 0;`, sementara *expression* adalah kombinasi yang menghasilkan nilai, misalnya `harga * jumlah`. Flanagan (2020) menjelaskan bahwa hampir semua alur logika dalam JavaScript berasal dari statement yang berisi satu atau lebih ekspresi.  

Untuk analogi, bayangkan pesanan di e-commerce. Pernyataan “cek jumlah barang dalam keranjang” adalah *statement*, sedangkan perhitungan “harga satuan × jumlah barang” adalah *expression*. Menurut Haverbeke (2018), memahami dua konsep ini penting agar pemula dapat menulis kode yang teratur dan konsisten.  

Struktur dasar lain meliputi **variabel**, **operator**, dan **blok kode**. Variabel menyimpan data seperti harga produk, operator melakukan perhitungan, dan blok kode `{}` mengelompokkan logika. Mozilla Developer Network (2022) menekankan bahwa blok kode digunakan dalam percabangan atau perulangan untuk mengatur eksekusi program.  

Komentar juga bagian penting dari struktur. Sama seperti catatan di invoice belanja, komentar menjelaskan maksud bagian kode tertentu. McConnell (2004) menekankan bahwa komentar adalah sarana dokumentasi yang menjaga keterbacaan jangka panjang.  

Dengan menguasai dasar ini, seorang pemula bisa memahami bahwa JavaScript adalah bahasa yang mengatur logika bisnis, mulai dari harga produk hingga total belanja. Hal ini menjadi pondasi sebelum belajar kontrol alur yang lebih kompleks.  

![Konsep Dasar](session-1-part-5/concept.png)  

---

## Ekspresi dan Statement Lebih Dalam  

Ekspresi menghasilkan nilai, misalnya `200000 * 3`, sedangkan statement adalah instruksi lengkap seperti `let totalBelanja = 200000 * 3;`. Flanagan (2020) menyebut ekspresi sebagai unit dasar evaluasi, sementara statement adalah kerangka alur program.  

Sebagai ilustrasi, “jumlah barang × harga produk” adalah ekspresi, sedangkan “Hitung total belanja” adalah statement. Haverbeke (2018) menjelaskan bahwa ekspresi bisa bersarang dalam statement untuk menghasilkan logika yang lebih kaya.  

Contoh lain adalah **ekspresi kondisional**:  

```javascript
let statusDiskon = totalBelanja > 500000 ? "Dapat diskon" : "Tidak ada diskon";
```  

Kode ini mengembalikan nilai berbeda berdasarkan kondisi, seperti sistem promosi di toko online. Mozilla Developer Network (2022) menekankan bahwa ekspresi kondisional membantu menyederhanakan kode yang biasanya ditulis dengan `if-else`.  

Fowler (2018) menambahkan bahwa pemahaman ini membuat kode lebih ringkas dan mudah dipelihara. Ekspresi memperkaya logika, sedangkan statement memastikan alurnya jelas.  

![Ekspresi dan Statement](session-1-part-5/expression-statement.png)  

---

## Variabel dalam Struktur Program  

Variabel adalah tempat penyimpanan data, misalnya jumlah barang, harga produk, atau total belanja. JavaScript menyediakan tiga cara mendeklarasikan variabel: `var`, `let`, dan `const`. Flanagan (2020) menyebut `let` dan `const` lebih aman karena memiliki *block scope*.  

Bayangkan keranjang belanja di e-commerce. Keranjang itu adalah variabel, sedangkan produk di dalamnya adalah nilai. Haverbeke (2018) menjelaskan bahwa variabel adalah label yang mengacu pada data, sehingga memudahkan akses ulang.  

Contoh:  

```javascript
let jumlahBarang = 4;
const hargaProduk = 150000;
```  

`jumlahBarang` bisa berubah jika pembeli menambah produk, sementara `hargaProduk` tetap. Mozilla Developer Network (2022) menekankan bahwa `const` sebaiknya digunakan untuk nilai tetap seperti tarif atau harga dasar.  

Fowler (2018) menekankan pentingnya penamaan variabel yang deskriptif, misalnya `totalBelanja` alih-alih `tb`. McConnell (2004) menambahkan bahwa penamaan yang baik adalah bagian dari desain perangkat lunak yang berkualitas.  

![Variabel](session-1-part-5/variable.png)  

---

## Operator sebagai Bagian dari Struktur Dasar  

Operator memungkinkan manipulasi data. JavaScript memiliki operator aritmatika (`+`, `-`, `*`, `/`), perbandingan (`===`, `!==`), logika (`&&`, `||`), dan penugasan (`=`). Flanagan (2020) menekankan bahwa operator adalah elemen inti yang digunakan hampir di semua program.  

Contoh e-commerce:  

```javascript
let totalBelanja = jumlahBarang * hargaProduk;
if (totalBelanja > 500000 && jumlahBarang > 3) {
    console.log("Anda dapat promo spesial!");
}
```  

Haverbeke (2018) menjelaskan bahwa operator logika seperti `&&` memungkinkan implementasi aturan promosi yang kompleks. Mozilla Developer Network (2022) menambahkan bahwa memahami *precedence* operator mencegah hasil yang salah.  

Kesalahan umum ada pada penggunaan `==` dibandingkan `===`. Fowler (2018) menyarankan selalu menggunakan `===` agar tidak terjadi perbandingan yang ambigu. McConnell (2004) menyebut bug dari operator bisa sulit dideteksi jika programmer tidak disiplin.  

![Operator](session-1-part-5/operator.png)  

---

## Blok Kode dan Struktur Kontrol  

Blok kode `{}` mengelompokkan instruksi. Misalnya:  

```javascript
if (totalBelanja > 500000) {
    let diskon = totalBelanja * 0.1;
    totalBelanja -= diskon;
}
```  

Flanagan (2020) menyebut blok kode sebagai dasar pengendalian alur. Analogi di e-commerce adalah aturan “jika belanja lebih dari Rp500.000, beri diskon 10%”. Haverbeke (2018) menekankan bahwa blok membantu modularitas.  

Mozilla Developer Network (2022) menyebut bahwa struktur `if-else`, `for`, dan `while` selalu bergantung pada blok kode. Fowler (2018) menambahkan bahwa blok yang konsisten membuat debugging lebih mudah.  

McConnell (2004) mengingatkan bahwa pemahaman *scope* penting: variabel dalam blok tidak bisa diakses di luar. Ini melindungi kode dari konflik dan menjaga integritas program.  

![Blok Kode](session-1-part-5/block.png)  

---

## Komentar sebagai Panduan Program  

Komentar digunakan untuk menjelaskan logika kode, misalnya:  

```javascript
// Hitung total belanja dengan diskon
let totalBelanja = jumlahBarang * hargaProduk;
```  

Flanagan (2020) menekankan komentar sebagai alat menjaga keterbacaan. Analogi di e-commerce adalah catatan kecil pada invoice agar pembeli paham rincian pesanan. Haverbeke (2018) menambahkan komentar mengurangi waktu debugging.  

Mozilla Developer Network (2022) menyarankan komentar tidak digunakan untuk menutupi kode buruk, melainkan melengkapi kode yang jelas. Fowler (2018) memperingatkan agar komentar diperbarui sesuai perubahan kode. McConnell (2004) menyebut komentar bagian dari desain, bukan sekadar tambahan.  

![Komentar](session-1-part-5/comment.png)  

---

## Clean Code dalam Struktur Dasar  

*Clean code* berarti kode yang rapi, konsisten, dan mudah dipahami. Prinsip ini mencakup indentasi jelas, penamaan variabel deskriptif, dan meminimalkan duplikasi. Flanagan (2020) menekankan bahwa kode yang bersih lebih mudah dipelihara.  

Dalam e-commerce, kode yang rapi seperti katalog produk yang teratur. Haverbeke (2018) menyebut kode adalah bentuk komunikasi antara programmer. Mozilla Developer Network (2022) merekomendasikan penggunaan gaya penulisan yang konsisten.  

Fowler (2018) menambahkan bahwa *refactoring* adalah kunci menjaga *clean code*. McConnell (2004) menegaskan dampak jangka panjangnya: tim lebih cepat beradaptasi dengan kebutuhan baru.  

![Clean Code](session-1-part-5/clean-code.png)  

---

## Studi Kasus E-commerce dalam Struktur Dasar  

Contoh sederhana: menghitung total belanja dengan diskon.  

```javascript
let jumlahBarang = 4;
const hargaProduk = 150000;

let totalBelanja = jumlahBarang * hargaProduk;

if (totalBelanja > 500000) {
    let diskon = totalBelanja * 0.1;
    totalBelanja = totalBelanja - diskon;
    console.log("Total belanja setelah diskon: Rp" + totalBelanja);
} else {
    console.log("Total belanja: Rp" + totalBelanja);
}
```  

Jika pembeli membeli 4 produk, total Rp600.000. Karena melebihi Rp500.000, program memberi diskon 10%, sehingga total akhir Rp540.000. Mozilla Developer Network (2022) menyebut praktik ini melatih penggunaan variabel, operator, blok kode, dan statement dalam satu alur.  

Haverbeke (2018) menekankan pentingnya latihan kecil agar konsep abstrak lebih mudah dipahami. Fowler (2018) menambahkan bahwa studi kasus nyata meningkatkan motivasi belajar. McConnell (2004) menyebut relevansi konteks membuat pemahaman lebih bertahan lama.  

![Studi Kasus E-commerce](session-1-part-5/ecommerce-case.png)  

---

## Kesimpulan  

Struktur dasar JavaScript terdiri dari statement, ekspresi, variabel, operator, blok kode, dan komentar. Semua elemen ini bekerja bersama untuk menyusun alur logika yang rapi dan konsisten. Dalam konteks e-commerce, konsep ini bisa diterapkan untuk menghitung total belanja, menentukan diskon, hingga menampilkan hasil di konsol. Dengan memahami dasar ini, pemula tidak hanya mampu menulis kode yang berjalan, tetapi juga kode yang bersih, mudah dibaca, dan relevan dengan kebutuhan nyata. Struktur dasar ini adalah fondasi yang menopang pembelajaran lebih lanjut seperti fungsi, perulangan, dan event handling.  

---

## Referensi  

- Flanagan, D. (2020). *JavaScript: The Definitive Guide*. O’Reilly.  
- Haverbeke, M. (2018). *Eloquent JavaScript*. No Starch Press.  
- Mozilla Developer Network. (2022). *MDN Web Docs*.  
- Fowler, M. (2018). *Refactoring: Improving the Design of Existing Code*. Addison-Wesley.  
- McConnell, S. (2004). *Code Complete*. Microsoft Press.  
