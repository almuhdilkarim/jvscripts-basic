## Pertemuan 13: Modularisasi JavaScript

---

### Modul 1 : Sejarah Modularisasi / history

1. Pendahuluan : Kebutuhan pemisahan kode dalam proyek besar.
2. Awal modularisasi dengan file terpisah.
3. CommonJS dan Node.js.
4. AMD (Asynchronous Module Definition).
5. ES6 Modules sebagai standar resmi.
6. Perbandingan import/export dengan require.
7. Modularisasi di browser modern.
8. Framework modern dan modul (React, Vue).
9. Dampak modularisasi pada maintainability software.

* **Kesimpulan**: Modularisasi lahir dari kebutuhan menjaga keteraturan kode, kini menjadi standar di JavaScript modern.
* **Referensi**:

  * Flanagan, D. (2020). *JavaScript: The Definitive Guide*. O’Reilly.
  * Tilkov, S., & Vinoski, S. (2010). *IEEE Internet Computing*.
  * Haverbeke, M. (2018). *Eloquent JavaScript*. No Starch Press.
  * Mozilla Developer Network. (2022). *MDN Web Docs*.
  * Freeman, E. (2014). *Head First JavaScript Programming*.

---

### Modul 2 : Konsep Export & Import / concept

1. Pendahuluan : Dasar komunikasi antar file.
2. Definisi export dalam modul.
3. Named export vs default export.
4. Studi kasus perpustakaan: ekspor fungsi hitung denda.
5. Studi kasus e-commerce: ekspor fungsi hitung diskon.
6. Studi kasus kesehatan: ekspor fungsi hitung BMI.
7. Import modul dalam file lain.
8. Manfaat pemisahan file.
9. Risiko circular dependency.

* **Kesimpulan**: Export & import memudahkan reuse kode, tetapi harus terstruktur agar tidak menimbulkan konflik.
* **Referensi**:

  * Flanagan, D. (2020). *JavaScript: The Definitive Guide*.
  * Mozilla Developer Network. (2022). *MDN Web Docs*.
  * Haverbeke, M. (2018). *Eloquent JavaScript*.
  * Crockford, D. (2008). *JavaScript: The Good Parts*.
  * Fowler, M. (2018). *Refactoring*.

---

### Modul 3 : Praktik Export & Import / practical

1. Pendahuluan : Latihan membuat file modular.
2. Konsep pemisahan kode.
3. Studi kasus: file modul daftar buku perpustakaan.
4. Studi kasus: file modul transaksi bank.
5. Studi kasus: file modul data produk e-commerce.
6. Kesalahan umum: salah penulisan path file.
7. Best practice: gunakan struktur folder rapi.
8. Debugging dengan log modul terimport.
9. Mini aplikasi modul kalkulasi sederhana.

* **Kesimpulan**: Praktik export & import memperlihatkan manfaat nyata modularisasi.
* **Referensi**:

  * Mozilla Developer Network. (2022). *MDN Web Docs*.
  * Flanagan, D. (2020). *JavaScript: The Definitive Guide*.
  * Haverbeke, M. (2018). *Eloquent JavaScript*.
  * Freeman, E. (2014). *Head First JavaScript Programming*.
  * Fowler, M. (2018). *Refactoring*.

---

### Modul 4 : Konsep Scope Modul / concept

1. Pendahuluan : Scope variabel dalam modul.
2. Perbedaan scope global vs lokal modul.
3. Variabel modul tidak bocor ke global.
4. Studi kasus sosial media: modul user profile.
5. Studi kasus transportasi: modul jadwal tiket.
6. Pentingnya namespace unik.
7. Perbandingan dengan IIFE sebelum ES6.
8. Modular scope meningkatkan keamanan kode.
9. Hubungan modular scope dengan encapsulation.

* **Kesimpulan**: Scope modul melindungi variabel agar tidak konflik, mendukung clean code.
* **Referensi**:

  * Flanagan, D. (2020). *JavaScript: The Definitive Guide*.
  * Mozilla Developer Network. (2022). *MDN Web Docs*.
  * Haverbeke, M. (2018). *Eloquent JavaScript*.
  * Sebesta, R. W. (2016). *Concepts of Programming Languages*.
  * Crockford, D. (2008). *JavaScript: The Good Parts*.

---

### Modul 5 : Praktik Struktur Modul / practical

1. Pendahuluan : Membuat proyek kecil modular.
2. Konsep struktur folder.
3. Studi kasus: proyek perpustakaan mini (modul buku, anggota).
4. Studi kasus: proyek e-commerce mini (modul produk, keranjang).
5. Studi kasus: proyek kesehatan mini (modul pasien, jadwal).
6. Kesalahan umum: import file ganda.
7. Best practice: gunakan index.js untuk agregasi modul.
8. Debugging struktur modul.
9. Mini aplikasi modular sederhana.

* **Kesimpulan**: Struktur modul membuat proyek lebih scalable dan mudah dirawat.
* **Referensi**:

  * Mozilla Developer Network. (2022). *MDN Web Docs*.
  * Flanagan, D. (2020). *JavaScript: The Definitive Guide*.
  * Haverbeke, M. (2018). *Eloquent JavaScript*.
  * Freeman, E. (2014). *Head First JavaScript Programming*.
  * Fowler, M. (2018). *Refactoring*.