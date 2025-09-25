---
date: "2025-09-26T10:00:00+07:00"
draft: false
title: "Siapkan lingkungan coding dengan instalasi JavaScript pertama"
short: "Instalasi"
thumb:
    image: "cover.png"
    anima: ""
    video: ""
layout: ""
weight: 1
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
      desc: "Mengetahui peran lingkungan coding dalam pengembangan JavaScript."
    - prop: ""
      name: "Praktik"
      icon: ""
      desc: "Mampu menginstal Node.js, VSCode, dan menjalankan kode JavaScript pertama."
require:
    - prop: "Software"
      name: "Node.js & VSCode"
      icon: "download"
      desc: "Dibutuhkan untuk menulis dan menjalankan program JavaScript."
metadata:
    index: false
    thumb: "cover.png"
    group: []
    author: ["Al Muhdil Karim"]
description: "Modul ini membimbing peserta menyiapkan environment coding JavaScript dengan menginstal Node.js, VSCode, dan membuat program pertama."
---


## Pendahuluan

Belajar pemrograman JavaScript tidak hanya soal menulis kode, tetapi juga menyiapkan lingkungan kerja yang tepat. Tanpa adanya persiapan ini, seorang pemula akan mudah kebingungan ketika kode yang ditulis tidak bisa dijalankan. Bayangkan seorang pelajar yang menuliskan perintah sederhana `console.log("Hello World")` di editor teks biasa, tetapi tidak tahu bagaimana mengeksekusinya. Situasi ini dapat membuat semangat belajar menurun karena kesalahan bukan pada logika program, melainkan pada lingkungan yang belum siap. Oleh karena itu, mengenali kebutuhan instalasi adalah langkah penting sebelum melangkah ke praktik yang lebih kompleks. Modul ini akan membawa peserta untuk memahami mengapa instalasi Node.js dan Visual Studio Code menjadi fondasi awal yang tidak boleh dilewatkan.

Lingkungan coding adalah tempat di mana kode dibuat, dijalankan, dan diuji secara berulang. Dalam konteks JavaScript, Node.js berfungsi sebagai mesin eksekusi di luar browser, sehingga memberikan fleksibilitas lebih bagi pengembang. Visual Studio Code hadir sebagai editor yang ringan namun kaya fitur, yang memudahkan pemula maupun profesional dalam menulis baris-baris program. Kasus nyata di lapangan menunjukkan bahwa mereka yang memiliki lingkungan coding yang benar sejak awal, cenderung lebih cepat menguasai konsep pemrograman dasar. Dengan memahami cara instalasi yang sistematis, peserta akan lebih percaya diri ketika menulis kode pertamanya. Bagian pendahuluan ini menjadi jembatan menuju pembahasan konsep dasar yang akan memperjelas peran setiap komponen instalasi.

![instalasi-awal](session-1-part-3/instalasi-awal.png)

---

## Konsep Dasar

Lingkungan pemrograman adalah kombinasi perangkat lunak dan alat bantu yang memungkinkan seorang pengembang menulis, menjalankan, dan menguji kode. Dalam konteks JavaScript, terdapat dua komponen utama yang sangat penting, yaitu Node.js dan Visual Studio Code. Node.js adalah sebuah *runtime environment* yang dibangun di atas mesin V8 milik Google Chrome, yang memungkinkan JavaScript dijalankan di luar browser. Hal ini berarti kode JavaScript dapat digunakan tidak hanya untuk interaktivitas halaman web, tetapi juga untuk membangun aplikasi server. Visual Studio Code atau VSCode, di sisi lain, merupakan editor kode sumber yang dilengkapi dengan banyak fitur pendukung seperti ekstensi, debugging, dan integrasi Git. Dengan menggabungkan keduanya, pembelajar memiliki pondasi kuat untuk memulai perjalanan mereka di dunia pemrograman modern (Flanagan, 2020).

Jika dianalogikan, Node.js adalah mesin kendaraan yang membuat roda bisa bergerak, sedangkan VSCode adalah dashboard yang memudahkan pengemudi mengendalikan laju. Seorang pemula yang hanya menggunakan browser untuk menjalankan JavaScript akan terbatas pada eksperimen kecil di konsol. Sebaliknya, dengan instalasi Node.js, mereka bisa mengeksekusi file `.js` secara langsung dan mengembangkan program lebih serius. VSCode kemudian memberikan pengalaman menulis kode yang rapi dan terorganisir, berbeda jauh dibandingkan menggunakan *text editor* sederhana. Konsep ini menjelaskan bahwa menyiapkan lingkungan coding bukanlah pilihan, melainkan kebutuhan agar pembelajaran bisa berlanjut ke tahap berikutnya. Memahami dasar ini akan membantu peserta menyadari hubungan erat antara alat eksekusi program dan editor yang digunakan.

![konsep-lingkungan](session-1-part-3/konsep-lingkungan.png)

---

## Panduan Langkah per Langkah

Tujuan dari panduan ini adalah memastikan setiap peserta dapat menyiapkan lingkungan coding JavaScript yang siap digunakan. Dengan mengikuti instruksi, peserta akan berhasil menginstal Node.js, memasang Visual Studio Code, dan menjalankan program pertama mereka. Langkah-langkah ini dibuat sederhana agar pemula dapat mengikuti dengan mudah. Namun, penjelasan teknis tetap diberikan agar setiap perintah dipahami dengan jelas. Proses instalasi berbeda di Windows, Linux, dan macOS, sehingga penyesuaian perlu dilakukan sesuai sistem operasi masing-masing. Dengan menyelesaikan panduan ini, peserta memiliki pondasi kokoh untuk modul-modul berikutnya. Panduan ini disusun berdasarkan dokumentasi resmi Node.js dan VSCode (Mozilla Developer Network, 2022).

![panduan](session-1-part-3/panduan.png)

---

### Langkah 1: Mengunduh dan Menginstal Node.js

![download-node](session-1-part-3/download-node.png)

**Windows:** Jalankan installer `.msi` lalu ikuti wizard instalasi.  
**Linux (Ubuntu):**

```bash
sudo apt install nodejs npm
```

**macOS (Homebrew):**

```bash
brew install node
```

Setelah instalasi selesai, lakukan verifikasi dengan:

```bash
node -v
npm -v
```

Perintah `node -v` memastikan Node.js sudah terpasang, sedangkan `npm -v` mengecek package manager. Jika keduanya menampilkan angka versi, berarti instalasi berhasil. Di Linux, kadang `npm` perlu diinstal terpisah menggunakan `sudo apt install npm`. Perbedaan kecil antar sistem operasi ini menunjukkan pentingnya memahami konteks teknis sebelum memulai coding. Dengan Node.js, peserta dapat menjalankan file `.js` langsung dari terminal tanpa bergantung pada browser.

![install-node](session-1-part-3/install-node.png)

---

### Langkah 2: Menginstal Visual Studio Code

![download-vscode](session-1-part-3/download-vscode.png)

**Windows:** Jalankan installer `.exe` dan ikuti proses instalasi.  
**Linux (Ubuntu):**

```bash
sudo snap install code --classic
```

**macOS:** Unduh file `.dmg` dan seret aplikasi ke folder `Applications`.

Setelah instalasi, jalankan VSCode untuk melihat antarmuka editor. Tambahkan ekstensi seperti *JavaScript (ES6) Code Snippets* atau *Prettier* untuk mendukung proses belajar.

Visual Studio Code menyediakan fitur seperti syntax highlighting, debugging, dan integrasi Git yang sangat membantu. Dengan menggunakan editor ini, proses menulis program menjadi lebih rapi dan profesional. VSCode bukan hanya alat penunjang, tetapi bagian dari ekosistem modern JavaScript. Dengan menguasai editor sejak awal, peserta dapat fokus pada logika program tanpa terganggu keterbatasan alat tulis kode.

![install-vscode](session-1-part-3/install-vscode.png)

---

### Langkah 3: Menjalankan Program JavaScript Pertama

![buat-file](session-1-part-3/buat-file.png)

Buat folder proyek baru, kemudian tambahkan file bernama `app.js`:

```javascript
// app.js
console.log("Hello, JavaScript World!");
```

Jalankan program dengan perintah berikut di terminal:

```bash
node app.js
```

Jika berhasil, terminal akan menampilkan teks *Hello, JavaScript World!* di layar. Output sederhana ini menjadi bukti bahwa lingkungan coding sudah siap digunakan. Walaupun sederhana, momen ini penting untuk meningkatkan rasa percaya diri peserta. Dengan langkah ini, peserta sudah memiliki editor untuk menulis kode, runtime untuk menjalankannya, dan keterampilan dasar yang diperlukan. Tahap ini adalah batu loncatan menuju praktik JavaScript yang lebih kompleks. Program kecil ini juga memperkenalkan pola kerja: menulis kode, menyimpan file, dan menjalankannya di terminal. Dengan membiasakan alur ini sejak awal, peserta akan lebih mudah memahami konsep-konsep berikutnya.

Perintah `console.log()` berfungsi untuk menampilkan teks ke layar sehingga kita dapat memverifikasi bahwa kode dijalankan sesuai harapan. Fungsi ini adalah salah satu alat debugging paling dasar yang digunakan bahkan oleh programmer berpengalaman. Jika output tidak muncul, biasanya penyebabnya adalah kesalahan dalam penamaan file, lokasi folder, atau kesalahan instalasi Node.js. Oleh karena itu, penting bagi peserta untuk mengecek kembali perintah yang diketik serta jalur direktori tempat file disimpan. Dengan memahami fungsi `console.log`, peserta akan lebih siap untuk memantau alur eksekusi kode di modul-modul mendatang. Praktik sederhana ini juga memperlihatkan hubungan langsung antara instruksi yang ditulis dan hasil yang ditampilkan. Dengan demikian, peserta dapat merasakan kontrol penuh atas kode yang mereka buat.

![hello-world](session-1-part-3/hello-world.png)

---

## Kesalahan Umum

![error-umum](session-1-part-3/error-umum.png)

Dalam proses instalasi JavaScript, banyak pemula yang melakukan kesalahan kecil namun berdampak besar. Kesalahan tersebut biasanya terjadi karena terburu-buru atau tidak membaca instruksi dengan seksama. Beberapa masalah yang sering muncul meliputi salah menuliskan perintah, tidak menambahkan Node.js ke environment path, atau mencoba menjalankan kode di lokasi folder yang salah. Situasi ini sering membuat pembelajar merasa bingung karena output tidak sesuai harapan. Oleh karena itu, memahami kesalahan umum berikut akan membantu peserta lebih cepat mengatasi hambatan awal dalam belajar.

### Kesalahan 1: Lupa Menambahkan Node.js ke Environment Path

![path-error](session-1-part-3/path-error.png)

```bash
node -v
# 'node' is not recognized as an internal or external command
```

```bash
node -v
# v20.10.0
```

Kesalahan ini sering muncul di Windows ketika installer Node.js tidak otomatis menambahkan path ke sistem. Akibatnya, perintah `node` tidak dikenali oleh terminal. Solusinya adalah menambahkan folder instalasi Node.js ke variabel **PATH** secara manual melalui pengaturan sistem. Di Linux dan macOS, masalah ini lebih jarang karena package manager biasanya menambahkan path secara otomatis. Dengan memastikan path sudah benar, peserta dapat menjalankan Node.js dari direktori mana pun di komputer mereka. Hal ini juga menjadi langkah penting untuk menghindari frustrasi di tahap awal belajar (Flanagan, 2020; Mozilla Developer Network, 2022).

### Kesalahan 2: Salah Menyimpan atau Menjalankan File JavaScript

![file-error](session-1-part-3/file-error.png)

```bash
node app.js
# Error: Cannot find module '/user/downloads/app.js'
```

```bash
cd Documents/project
node app.js
# Hello, JavaScript World!
```

Kesalahan ini biasanya terjadi karena file `app.js` tidak disimpan di folder yang sama dengan tempat terminal aktif. Akibatnya, Node.js tidak dapat menemukan file yang dimaksud dan menampilkan pesan error. Untuk menghindarinya, peserta harus memastikan direktori kerja di terminal sama dengan lokasi file. Perintah `cd` digunakan untuk berpindah ke folder yang sesuai sebelum menjalankan file. Dengan memahami hubungan antara direktori kerja dan file, peserta akan lebih mudah mengelola proyek-proyek yang lebih besar. Hal ini memperlihatkan pentingnya keterampilan dasar manajemen file dalam pemrograman (Haverbeke, 2018; Fowler, 2018).

### Kesalahan 3: Mengetik Kode dengan Sintaks yang Salah

![syntax-error](session-1-part-3/syntax-error.png)

```javascript
console.log("Hello, JavaScript World!);
```

```javascript
console.log("Hello, JavaScript World!");
```

Kesalahan sintaks seperti lupa menutup tanda kutip sering terjadi pada pemula. JavaScript akan langsung menampilkan error ketika mencoba mengeksekusi baris kode ini. Meski terlihat sederhana, kesalahan seperti ini bisa memakan waktu lama untuk ditemukan jika tidak terbiasa membaca pesan error. Oleh karena itu, penting bagi peserta untuk selalu memperhatikan detail kecil seperti tanda kutip dan titik koma. Editor seperti VSCode biasanya memberikan peringatan otomatis dengan tanda merah pada baris yang salah. Dengan memanfaatkan fitur ini, peserta bisa belajar memperbaiki kesalahan sintaks lebih cepat. Kesadaran terhadap detail ini akan sangat membantu dalam menulis program yang lebih kompleks di masa depan (Crockford, 2008; Freeman, 2014).

---

## Best Practice

![best-practice](session-1-part-3/best-practice.png)

Menyiapkan lingkungan pemrograman bukan hanya soal instalasi, tetapi juga memastikan setiap komponen digunakan dengan cara terbaik. Praktik terbaik ini membantu menghindari kesalahan yang sama di masa depan dan memberikan dasar yang kuat untuk menulis kode JavaScript secara konsisten. Dengan mengikuti best practice, peserta dapat membangun kebiasaan baik sejak awal. Hal ini sangat penting karena pola kerja yang benar akan memudahkan pembelajaran di tahap selanjutnya. Berikut adalah beberapa praktik terbaik yang sebaiknya diterapkan dalam proses instalasi dan penggunaan lingkungan coding JavaScript.

### Best Practice 1: Gunakan Versi LTS Node.js

![node-lts](session-1-part-3/node-lts.png)

```bash
node -v
# v20.10.0 (LTS)
```

Menggunakan versi **LTS (Long Term Support)** sangat dianjurkan bagi pemula karena lebih stabil dan mendapatkan dukungan keamanan lebih lama. Versi Current mungkin menawarkan fitur terbaru, tetapi berisiko mengalami bug atau perubahan mendadak. Dengan memilih LTS, peserta bisa fokus pada pembelajaran tanpa khawatir tentang kompatibilitas. Praktik ini juga memudahkan dalam mengikuti tutorial atau dokumentasi, karena mayoritas menggunakan versi LTS. Selain itu, perusahaan besar umumnya juga menggunakan LTS untuk aplikasi produksi. Dengan cara ini, peserta tidak hanya belajar tetapi juga mengikuti standar industri (Flanagan, 2020).

### Best Practice 2: Buat Folder Khusus untuk Proyek

![project-folder](session-1-part-3/project-folder.png)

```bash
mkdir belajar-js
cd belajar-js
```

Membuat folder khusus untuk setiap proyek membantu menjaga keteraturan kode. Jika semua file JavaScript diletakkan sembarangan, besar kemungkinan terjadi kebingungan dalam manajemen file. Dengan struktur folder yang jelas, peserta dapat memisahkan proyek satu dengan lainnya. Hal ini juga melatih kebiasaan dokumentasi dan keteraturan sejak dini. Pada tahap lanjutan, manajemen folder yang baik akan mempermudah penggunaan version control seperti Git. Dengan demikian, peserta akan lebih disiplin dalam mengorganisir kode mereka (Haverbeke, 2018).

### Best Practice 3: Manfaatkan Ekstensi VSCode

![vscode-extensions](session-1-part-3/vscode-extensions.png)

**Ekstensi Rekomendasi:**  
- Prettier – Code formatter  
- ESLint – Linter untuk kualitas kode

Ekstensi di VSCode memberikan nilai tambah besar dalam menulis kode yang rapi dan konsisten. Prettier, misalnya, secara otomatis memformat kode sehingga lebih mudah dibaca. ESLint membantu menemukan kesalahan kecil atau pola buruk sebelum dijalankan. Dengan memanfaatkan ekstensi ini, peserta bisa belajar menulis kode seperti seorang profesional sejak awal. Ekstensi juga dapat disesuaikan sesuai kebutuhan proyek. Dengan cara ini, lingkungan coding menjadi lebih adaptif terhadap berbagai skenario pembelajaran (Mozilla Developer Network, 2022).

---

## Kesimpulan

![kesimpulan](session-1-part-3/kesimpulan.png)

Instalasi lingkungan JavaScript merupakan langkah awal yang sangat menentukan keberhasilan proses belajar pemrograman. Pendahuluan telah menjelaskan mengapa Node.js dan Visual Studio Code menjadi fondasi penting sebelum menulis kode. Konsep dasar memperlihatkan bagaimana runtime dan editor saling melengkapi dalam mendukung proses belajar. Panduan langkah per langkah kemudian memberikan instruksi praktis untuk memastikan peserta dapat menginstal Node.js, memasang VSCode, dan menjalankan program pertama mereka. Bagian kesalahan umum mengingatkan peserta agar berhati-hati terhadap kendala seperti path yang salah, direktori kerja yang keliru, atau sintaks kode yang tidak lengkap. Sementara itu, best practice menunjukkan cara terbaik dalam memilih versi LTS, membuat folder proyek, dan memanfaatkan ekstensi VSCode. Dengan mengikuti keseluruhan modul ini, peserta akan memiliki pondasi yang kuat untuk melanjutkan perjalanan mereka dalam mempelajari JavaScript.

---

## Referensi

- Flanagan, D. (2020). *JavaScript: The Definitive Guide* (7th ed.). O’Reilly Media.  
- Fowler, M. (2018). *Refactoring: Improving the Design of Existing Code*. Addison-Wesley.  
- Freeman, E., & Robson, E. (2014). *Head First JavaScript Programming*. O’Reilly Media.  
- Haverbeke, M. (2018). *Eloquent JavaScript* (3rd ed.). No Starch Press.  
- Mozilla Developer Network. (2022). *MDN Web Docs – JavaScript Guide*. Retrieved from https://developer.mozilla.org