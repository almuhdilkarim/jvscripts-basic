---
date: "2025-09-26T00:00:00+07:00"
draft: false
title: "Sejarah Standarisasi ECMAScript: Fondasi Stabilitas JavaScript"
short: "ECMAScript"
thumb:
    image: "cover.jpg"
    anima: ""
    video: ""
layout: "module"
weight: 2
lister: 1
format:
    media: "article"
    model: "history"
    datum:
        data: "Sejarah dan evolusi ECMAScript dari ES1 hingga ES6."
outcome:
    - prop: ""
      name: "Konseptual"
      icon: ""
      desc: "Memahami latar belakang lahirnya ECMAScript, krisis ES4, stabilitas ES5, dan lompatan besar ES6."
require:
    - prop: ""
      name: "Dasar JavaScript"
      icon: ""
      desc: "Pemahaman dasar JavaScript dibutuhkan untuk memahami konteks sejarah ECMAScript."
metadata:
    index: false
    thumb: "cover.jpg"
    group: []
    author: ["Al Muhdil Karim"]
description: "Modul ini membahas sejarah standarisasi ECMAScript dari ES1 hingga ES6, termasuk krisis ES4, stabilitas ES5, dan dampaknya bagi developer modern." 
---

# Session 2 Part 1: Sejarah Standarisasi ECMAScript

## Pendahuluan  

JavaScript lahir pada pertengahan 1990-an sebagai jawaban atas kebutuhan membuat halaman web lebih interaktif dan dinamis. Pada masa itu, browser bersaing ketat, terutama Netscape Navigator dan Internet Explorer, sehingga setiap perusahaan ingin menambahkan fitur sendiri ke dalam bahasa ini. Kondisi tersebut menimbulkan banyak ketidakcocokan, di mana sebuah kode dapat berjalan baik di satu browser namun gagal di browser lain. Fragmentasi ini membuat para pengembang frustasi karena aplikasi web menjadi sulit dipelihara dan dibagikan. Tanpa adanya aturan bersama, JavaScript terancam kehilangan kepercayaan sebagai bahasa standar web. Maka, muncul kebutuhan mendesak untuk menghadirkan sebuah sistem standarisasi. Dari titik inilah awal kisah ECMAScript dimulai.  

Standarisasi bahasa pemrograman bukan hanya soal teknis, melainkan juga tentang menyatukan visi antar pemangku kepentingan. JavaScript, yang awalnya hanya dianggap pelengkap HTML, perlahan berubah menjadi elemen penting bagi ekosistem web global. Perubahan ini memaksa adanya konsensus yang bisa diterima lintas perusahaan teknologi besar. Proses menuju standarisasi penuh tantangan, karena setiap pihak memiliki kepentingan komersial yang berbeda. Namun, tanpa adanya aturan bersama, pertumbuhan JavaScript tidak mungkin berjalan stabil. Inilah alasan mengapa pembentukan ECMAScript menjadi langkah krusial dalam sejarah bahasa ini.  

Bayangkan seorang pengembang pada era 1990-an yang harus menulis dua versi kode hanya untuk memastikan sebuah fitur berjalan di Netscape dan Internet Explorer. Situasi ini menyita waktu, menurunkan produktivitas, dan meningkatkan risiko kesalahan. Standarisasi hadir sebagai solusi yang mampu mengurangi beban tersebut, sekaligus membuka jalan bagi inovasi berikutnya. Dari sinilah ECMAScript muncul sebagai mercusuar yang memberi arah bagi perkembangan JavaScript modern. Dengan latar belakang ini, kita bisa melanjutkan pembahasan pada fase awal lahirnya ECMAScript versi pertama hingga ketiga.  

![ecmascript-history](session-2-part-1/ecmascript-history.png)  

---

## Lahirnya ECMAScript versi awal (ES1–ES3)  

Pada tahun 1996, Netscape menyerahkan JavaScript ke organisasi standarisasi ECMA agar bahasa ini memiliki pedoman resmi. Upaya ini menghasilkan **ECMAScript 1 (ES1)** yang dipublikasikan pada tahun 1997. Versi ini mendefinisikan aturan dasar bahasa seperti tipe data, sintaks dasar, dan operasi kontrol yang sebelumnya hanya ada di implementasi vendor. ES1 berperan penting sebagai titik awal, meskipun masih sederhana dan terbatas dalam fitur. Standarisasi ini memberi keyakinan kepada para pengembang bahwa JavaScript tidak lagi sekadar eksperimen browser, melainkan bagian dari ekosistem web global. Dari sinilah kepercayaan industri mulai terbentuk.  

Setahun kemudian, **ECMAScript 2 (ES2)** dirilis dengan tujuan memperbaiki kesalahan teknis dan menyesuaikan dokumen dengan standar internasional ISO/IEC. Meski perubahannya terkesan minor, langkah ini memperkuat posisi ECMAScript sebagai standar formal yang diakui secara global. ES2 memastikan kompatibilitas lintas platform semakin konsisten, sehingga developer tidak perlu lagi terlalu khawatir dengan perbedaan implementasi antar browser. Walau tidak membawa fitur baru yang besar, ES2 menunjukkan komitmen jangka panjang terhadap konsistensi JavaScript. Hal ini membuktikan bahwa standarisasi tidak hanya menambahkan fitur, tetapi juga menjaga kestabilan ekosistem.  

Kemudian pada tahun 1999, **ECMAScript 3 (ES3)** dirilis dan menjadi tonggak utama dalam sejarah JavaScript. ES3 memperkenalkan fitur penting seperti regular expression, exception handling, dan perbaikan string manipulation. Inovasi ini menjadikan JavaScript lebih fleksibel dan mampu bersaing dengan bahasa pemrograman lain di ranah web. Banyak konsep modern yang kita gunakan saat ini berakar dari ES3, menjadikannya versi yang paling lama bertahan dan dipakai luas. ES3 juga memicu munculnya framework awal berbasis JavaScript, karena fitur-fiturnya cukup matang untuk membangun aplikasi lebih kompleks. Dari sinilah JavaScript benar-benar melangkah keluar dari bayang-bayang HTML sederhana.  

Namun, meski ES1 hingga ES3 membawa kemajuan, proses adopsinya tetap menghadapi tantangan. Tidak semua vendor browser segera mengikuti spesifikasi terbaru, sehingga masih terjadi fragmentasi di awal 2000-an. Kondisi ini menimbulkan kebutuhan akan koordinasi yang lebih baik antara standar ECMAScript dengan implementasi nyata di browser. Menurut Flanagan (2020), periode ini menjadi pembuktian bahwa standarisasi saja tidak cukup tanpa dukungan ekosistem penuh. Oleh karena itu, ES3 meski sukses, juga membuka babak baru dalam perdebatan tentang arah masa depan JavaScript. Dari titik inilah drama besar tentang krisis ES4 mulai muncul.  

![ecmascript-es1-es3](session-2-part-1/ecmascript-es1-es3.png)  

---

## Krisis ES4 yang gagal disepakati  

Setelah kesuksesan ES3, komunitas JavaScript menantikan lompatan besar berikutnya melalui **ECMAScript 4 (ES4)**. Proposal ES4 ambisius karena membawa fitur yang sangat modern, seperti kelas, modul, generics, hingga strong typing. Tujuan utamanya adalah menjadikan JavaScript setara dengan bahasa pemrograman besar lain seperti Java dan C#. Namun, justru karena ambisinya, ES4 memicu perpecahan besar di antara para anggota TC39. Beberapa pihak merasa perubahan ini terlalu drastis dan berisiko merusak kompat...

Perdebatan memanas karena vendor besar memiliki kepentingan berbeda dalam menentukan arah bahasa. Mozilla, sebagai salah satu penggagas, mendukung penuh rencana ES4 karena percaya bahwa masa depan aplikasi web membutuhkan fitur canggih. Sebaliknya, Microsoft dan beberapa pihak lain menganggap bahwa ES4 terlalu kompleks dan tidak realistis untuk diimplementasikan secara konsisten. Persaingan antar browser di era itu memperkeruh suasana, karena setiap vendor ingin mempertahankan dominasinya. Tanpa adanya k...

Kegagalan menyepakati ES4 menciptakan kebingungan di kalangan pengembang. Banyak yang menunda adopsi teknologi baru karena tidak jelas standar mana yang akan digunakan di masa depan. Di sisi lain, beberapa fitur ES4 mulai diadopsi secara parsial di implementasi tertentu, tetapi tanpa jaminan kompatibilitas. Hal ini membuat ekosistem JavaScript berada di persimpangan yang tidak pasti. Menurut Crockford (2008), krisis ES4 memperlihatkan bahwa terlalu banyak inovasi sekaligus bisa menimbulkan resistensi dan...

Akhirnya, ES4 dibatalkan secara resmi dan menjadi salah satu kegagalan paling terkenal dalam sejarah bahasa pemrograman. Sebagai gantinya, komunitas memutuskan untuk membuat langkah transisi yang lebih aman melalui rilis **ES5**, yang lebih konservatif namun tetap relevan. Walau ES4 tidak pernah terealisasi, ide-idenya tidak hilang begitu saja, melainkan diwariskan ke generasi berikutnya. Banyak fitur modern di ES6 sejatinya adalah hasil revisi dari gagasan ES4 yang dulu ditolak. Dari krisis inilah lahir...

![ecmascript-es4-crisis](session-2-part-1/ecmascript-es4-crisis.png)  

---

## Stabilitas dan popularitas ES5  

Setelah kegagalan ES4, komunitas JavaScript membutuhkan standar yang lebih realistis dan mudah diadopsi. Pada tahun 2009, lahirlah **ECMAScript 5 (ES5)** sebagai hasil kompromi yang mengutamakan stabilitas daripada inovasi radikal. ES5 membawa sejumlah fitur praktis seperti `strict mode`, accessor properties, JSON support, serta perbaikan pada definisi objek. Fokus utama ES5 adalah menjaga kompatibilitas ke belakang sambil menambahkan pondasi bagi masa depan. Pendekatan konservatif ini berhasil membangun...

Keberhasilan ES5 tidak hanya terletak pada fitur barunya, tetapi juga pada tingkat adopsinya yang luas di berbagai browser. Dalam waktu relatif singkat, hampir semua vendor besar mulai mendukung ES5, menciptakan konsistensi yang sebelumnya sulit dicapai. Stabilitas ini memberi rasa aman bagi para pengembang, sehingga mereka berani membangun aplikasi web yang lebih kompleks. ES5 juga menjadi dasar bagi framework modern awal seperti AngularJS dan jQuery, yang memanfaatkan fitur baru untuk memperluas kapabi...

Selain itu, ES5 memperkenalkan konsep **strict mode**, yang memaksa penulisan kode lebih disiplin dan aman. Fitur ini menutup celah-celah lama dalam JavaScript, misalnya mencegah penggunaan variabel tanpa deklarasi. Walaupun pada awalnya beberapa developer merasa strict mode terlalu membatasi, dalam jangka panjang fitur ini meningkatkan kualitas kode. Menurut Flanagan (2020), ES5 membuktikan bahwa penyempurnaan kecil tetapi konsisten dapat memberikan dampak signifikan bagi keberlanjutan bahasa【48†source】...

Popularitas ES5 bertahan cukup lama, bahkan lebih dari satu dekade setelah dirilis, banyak proyek yang masih mengandalkan standar ini. Hal tersebut menunjukkan betapa pentingnya peran ES5 dalam menciptakan ekosistem yang stabil. Framework, library, hingga mesin JavaScript seperti V8, SpiderMonkey, dan Chakra semakin matang berkat dukungan ES5. Dengan fondasi yang kuat ini, komunitas merasa lebih siap menghadapi lompatan besar berikutnya. ES5 bukan hanya standar sementara, tetapi jembatan penting menuju e...

![ecmascript-es5](session-2-part-1/ecmascript-es5.png)  

---

## Lompatan besar ES6 pada tahun 2015  

Setelah bertahun-tahun stagnasi, tahun 2015 menjadi momentum penting bagi JavaScript dengan lahirnya **ECMAScript 6 (ES6)**, juga dikenal sebagai ECMAScript 2015. Rilis ini dianggap sebagai lompatan terbesar sejak kelahiran bahasa JavaScript karena membawa banyak fitur baru. ES6 memperkenalkan `let`, `const`, arrow function, class, module system, dan banyak fitur modern lainnya. Perubahan ini menjadikan JavaScript lebih sejajar dengan bahasa pemrograman tingkat tinggi lainnya. Tidak hanya itu, ES6 juga m...

Salah satu dampak paling terasa dari ES6 adalah meningkatnya produktivitas developer. Fitur seperti arrow function dan template literal menyederhanakan sintaks yang sebelumnya panjang. Module system membuat pemisahan kode lebih terstruktur dan mudah dikelola. Class memberikan sintaks yang lebih familiar bagi developer dari bahasa lain, meskipun di baliknya tetap berbasis prototipe. Semua inovasi ini mempermudah adopsi JavaScript oleh pengembang baru maupun berpengalaman. Tidak mengherankan bila ES6 menja...

Selain fitur, ES6 juga memperkenalkan pendekatan baru dalam siklus rilis standar ECMAScript. Mulai dari ES6, TC39 memutuskan untuk merilis pembaruan tahunan agar evolusi bahasa lebih terukur. Langkah ini mencegah terulangnya krisis seperti ES4 yang terlalu ambisius. Menurut Haverbeke (2018), strategi ini berhasil menyeimbangkan kebutuhan inovasi dengan stabilitas bahasa【48†source】. Dengan demikian, ES6 tidak hanya penting karena fiturnya, tetapi juga karena menetapkan pola pengembangan yang lebih berkela...

Adopsi ES6 berjalan relatif cepat, terutama karena browser modern segera mengintegrasikan dukungannya. Selain itu, transpiler seperti **Babel** membantu developer menggunakan fitur ES6 bahkan di lingkungan yang belum mendukung penuh. Hal ini mempercepat penyebaran standar baru dan memperkuat posisinya sebagai fondasi utama JavaScript modern. Banyak framework besar seperti React, Angular, dan Vue segera memanfaatkan ES6 sebagai basis pengembangan. ES6 bukan hanya rilis biasa, tetapi simbol kebangkitan Jav...

![ecmascript-es6](session-2-part-1/ecmascript-es6.png)  

---

## Pembaruan tahunan melalui TC39  

Setelah keberhasilan ES6, komite teknis **TC39** yang bertanggung jawab atas ECMAScript mengubah strategi rilis. Sebelumnya, setiap versi ECMAScript membutuhkan waktu bertahun-tahun untuk disepakati, sehingga perkembangan bahasa terasa lambat. Sejak 2015, TC39 memutuskan untuk merilis standar baru setiap tahun, dimulai dengan **ES2016 (ES7)**. Pendekatan ini membuat pengembangan JavaScript lebih terprediksi dan transparan. Dengan siklus tahunan, fitur dapat diperkenalkan secara bertahap tanpa menimbulkan...

Proses di TC39 didasarkan pada sistem proposal yang harus melalui beberapa tahap, mulai dari *stage 0* hingga *stage 4*. Setiap tahap menunjukkan tingkat kesiapan fitur sebelum menjadi bagian resmi dari standar. Misalnya, fitur `async/await` yang sangat populer, awalnya melalui tahap proposal sebelum resmi masuk ke ES2017. Model ini memberi kesempatan bagi komunitas untuk memberi masukan sebelum fitur dirilis. Dengan demikian, pengembangan ECMAScript menjadi lebih inklusif dan kolaboratif. Hal ini juga m...

Selain memberikan struktur, pembaruan tahunan juga meningkatkan kecepatan adopsi inovasi. Developer tidak lagi harus menunggu bertahun-tahun untuk fitur baru, karena setiap tahun selalu ada tambahan kecil namun signifikan. Menurut Osmani (2012), model iteratif ini jauh lebih sehat dibandingkan pendekatan lama yang penuh risiko kegagalan besar seperti ES4【48†source】. Dengan rilis tahunan, JavaScript bisa tetap kompetitif dibandingkan bahasa pemrograman lain. Ini juga membuat framework dan library lebih mu...

Keberadaan TC39 sebagai garda depan evolusi JavaScript juga memperlihatkan pentingnya tata kelola yang kuat dalam bahasa pemrograman. Komite ini terdiri dari perwakilan perusahaan besar seperti Google, Microsoft, Mozilla, dan Apple. Kolaborasi antar pesaing besar dalam forum yang sama menjadi bukti bahwa masa depan JavaScript adalah kepentingan bersama. Dari sinilah JavaScript berhasil mempertahankan posisinya sebagai bahasa paling dominan di web. Dengan model rilis tahunan, pengembang dapat merencanakan...

![ecmascript-tc39](session-2-part-1/ecmascript-tc39.png)  

---

## Fitur modern: let, const, arrow function  

Salah satu daya tarik utama ES6 adalah hadirnya **let** dan **const** sebagai alternatif deklarasi variabel. Sebelum ES6, JavaScript hanya memiliki `var` yang sering menimbulkan kebingungan karena sifat *function scope* dan hoisting. Dengan adanya `let`, variabel kini memiliki *block scope*, sehingga lebih mudah diprediksi. Sementara itu, `const` memungkinkan deklarasi nilai yang tidak bisa diubah, sehingga meningkatkan keamanan data dalam program. Kedua fitur ini membawa JavaScript lebih dekat dengan pr...

Selain variabel, ES6 memperkenalkan **arrow function** dengan sintaks lebih ringkas. Fungsi yang sebelumnya memerlukan kata kunci `function` kini dapat ditulis hanya dengan tanda panah `=>`. Arrow function sangat populer karena tidak memiliki `this` sendiri, melainkan mewarisi dari konteks luar. Hal ini menyederhanakan banyak kasus penggunaan, terutama pada callback dan event handler. Menurut Flanagan (2020), fitur ini adalah salah satu inovasi yang paling meningkatkan keterbacaan kode【48†source】. Dengan...

Kombinasi `let`, `const`, dan arrow function membuat JavaScript lebih kompetitif di mata pengembang dari bahasa lain. Banyak developer yang sebelumnya terbiasa dengan Java atau C# merasa lebih nyaman ketika menemukan sintaks yang mirip. Fitur ini juga membantu mengurangi bug yang biasanya disebabkan oleh variabel global atau kesalahan penanganan `this`. Dengan adanya pembaruan tersebut, ekosistem framework dan library segera menyesuaikan diri. React, misalnya, sangat memanfaatkan arrow function dalam pen...

Penerimaan terhadap fitur modern ini sangat positif dan cepat diadopsi di seluruh dunia. Dukungan transpiler seperti **Babel** membantu developer menggunakan fitur ES6 meskipun browser belum mendukung penuh. Hal ini mempercepat transisi dan membuat pengembang tidak perlu menunggu implementasi resmi di semua platform. Dengan cara ini, fitur modern menjadi standar de facto bahkan sebelum semua browser mengadopsinya. Haverbeke (2018) menyebutkan bahwa kehadiran fitur ES6 mempercepat transformasi JavaScript ...

![ecmascript-modern-features](session-2-part-1/ecmascript-modern-features.png)  

---

## Implementasi lintas browser  

Salah satu tantangan terbesar dalam sejarah JavaScript adalah memastikan fitur baru dapat berjalan konsisten di berbagai browser. Setelah ES6 diperkenalkan, browser modern seperti Chrome, Firefox, Safari, dan Edge berlomba untuk mengimplementasikan standar tersebut. Namun, adopsi penuh tidak terjadi secara instan karena setiap vendor memiliki prioritas yang berbeda. Beberapa fitur segera didukung, sementara yang lain membutuhkan waktu bertahun-tahun untuk stabil. Hal ini sempat menciptakan situasi di ma...

Implementasi lintas browser menjadi bukti pentingnya koordinasi antara **TC39** dengan vendor. Setiap fitur yang masuk ke tahap akhir standar diuji dalam berbagai mesin JavaScript, seperti V8 milik Google atau SpiderMonkey milik Mozilla. Dengan cara ini, kemungkinan fragmentasi dapat ditekan seminimal mungkin. Namun, perbedaan versi browser yang masih digunakan oleh sebagian besar pengguna tetap menjadi kendala. Misalnya, beberapa perusahaan masih bergantung pada Internet Explorer lama, yang tidak menduk...

Polyfill sendiri menjadi alat penting yang memungkinkan fitur baru berjalan di lingkungan lama. Misalnya, method `Array.from()` atau `Object.assign()` dapat digunakan melalui polyfill sebelum browser resmi mendukungnya. Hal ini membantu developer menjaga pengalaman pengguna tetap konsisten di berbagai perangkat. Menurut Mozilla Developer Network (2022), penggunaan polyfill menjadi strategi umum dalam transisi menuju standar baru【48†source】. Dengan demikian, meskipun browser belum seragam, developer tetap...

Pada akhirnya, implementasi lintas browser adalah kunci keberhasilan ECMAScript. Tanpa dukungan penuh dari vendor, standar hanyalah dokumen tanpa kekuatan praktis. ES6 membuktikan bahwa kolaborasi erat antara komite standar, vendor, dan komunitas developer bisa menghasilkan transisi yang relatif mulus. Kini, mayoritas browser modern telah mengadopsi hampir seluruh fitur ES6 dan seterusnya. Keberhasilan ini menghapus trauma fragmentasi era awal JavaScript. Dari sinilah JavaScript benar-benar meneguhkan dir...

![ecmascript-browser-support](session-2-part-1/ecmascript-browser-support.png)  

---

## Dampak bagi developer JavaScript modern  

Transformasi ECMAScript dari ES1 hingga ES6 telah mengubah cara developer bekerja secara fundamental. Jika sebelumnya JavaScript sering dipandang sebelah mata, kini bahasa ini menjadi inti dari hampir semua aplikasi web. Kehadiran fitur modern membuat penulisan kode lebih singkat, jelas, dan aman. Developer tidak lagi terjebak dengan praktik lama yang rawan bug seperti penggunaan `var` sembarangan. Sebaliknya, mereka didorong untuk menggunakan `let`, `const`, serta memanfaatkan arrow function. Perub...

Dampak lain yang signifikan adalah munculnya ekosistem framework dan library modern yang sepenuhnya bergantung pada standar ECMAScript. React, Angular, dan Vue adalah contoh nyata bagaimana JavaScript modern digunakan untuk membangun aplikasi berskala besar. Framework ini tidak akan bisa berkembang pesat tanpa adanya dukungan fitur seperti class, module, dan template literal. Menurut Haverbeke (2018), kemajuan JavaScript modern telah membuatnya sejajar dengan bahasa pemrograman lain di ranah enterprise【4...

Bagi developer individu, perubahan ECMAScript membawa peluang sekaligus tantangan. Mereka harus terus belajar dan beradaptasi dengan fitur baru yang hadir hampir setiap tahun. Namun, dengan rilis tahunan yang lebih terukur, proses pembelajaran menjadi lebih mudah dibandingkan perubahan drastis seperti rencana ES4. Komunitas juga menyediakan banyak dokumentasi, kursus, dan sumber belajar gratis. Hal ini membuat JavaScript menjadi salah satu bahasa yang paling ramah untuk pemula sekaligus kuat untuk profes...

Secara keseluruhan, evolusi ECMAScript meningkatkan kualitas hidup developer di seluruh dunia. Kini mereka memiliki bahasa yang stabil, kaya fitur, dan didukung penuh oleh semua browser modern. Kepercayaan ini mendorong inovasi berkelanjutan, baik di level individu maupun industri. Menurut Flanagan (2020), dampak utama ES6 adalah membuka jalan bagi JavaScript untuk menjadi bahasa “general purpose” yang tidak hanya terbatas pada web【48†source】. Dengan kata lain, perjalanan dari ES1 hingga ES6 tidak hanya te...

![ecmascript-developer-impact](session-2-part-1/ecmascript-developer-impact.png)  

---

## Kesimpulan  

Perjalanan standarisasi ECMAScript menunjukkan bagaimana JavaScript berevolusi dari bahasa sederhana menjadi pilar utama ekosistem web modern. Dimulai dari ES1 hingga ES3, bahasa ini membangun fondasi dasar yang kokoh untuk kompatibilitas lintas browser. Krisis ES4 menjadi pelajaran berharga bahwa inovasi harus diimbangi dengan kompromi dan realisme. ES5 kemudian hadir sebagai standar stabil yang berhasil mengembalikan kepercayaan komunitas pengembang. Lompatan besar ES6 pada 2015 memperkenalkan fitur ...

---

## Referensi  

- Crockford, D. (2008). *JavaScript: The Good Parts*. O’Reilly Media.  
- ECMA International. (2015). *ECMAScript Language Specification*. Retrieved from https://262.ecma-international.org/  
- Flanagan, D. (2020). *JavaScript: The Definitive Guide* (7th ed.). O’Reilly Media.  
- Haverbeke, M. (2018). *Eloquent JavaScript* (3rd ed.). No Starch Press.  
- Osmani, A. (2012). *Learning JavaScript Design Patterns*. O’Reilly Media.  
- Mozilla Developer Network. (2022). *MDN Web Docs – JavaScript Guide*. Retrieved from https://developer.mozilla.org/  
