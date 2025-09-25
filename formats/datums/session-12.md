## Pertemuan 12: Error Handling

---

### Modul 1 : Sejarah Penanganan Error / history

1. Pendahuluan : Mengapa error handling menjadi kebutuhan.
2. Penanganan error di bahasa Assembly (kode status).
3. Exception di Java dan C++.
4. Mekanisme error di Python.
5. Error handling awal di JavaScript (try-catch).
6. Evolusi error object (`Error`, `TypeError`, dll.).
7. Promise & penanganan error async.
8. Error handling modern dengan Async/Await.
9. Pentingnya error handling untuk keamanan aplikasi.

* **Kesimpulan**: Error handling berevolusi dari kode status sederhana hingga mekanisme exception modern yang lebih robust.
* **Referensi**:

  * Sebesta, R. W. (2016). *Concepts of Programming Languages*. Pearson.
  * Flanagan, D. (2020). *JavaScript: The Definitive Guide*. O’Reilly.
  * Mozilla Developer Network. (2022). *MDN Web Docs*.
  * Haverbeke, M. (2018). *Eloquent JavaScript*. No Starch Press.
  * Fowler, M. (2018). *Refactoring*.

---

### Modul 2 : Konsep Try-Catch / concept

1. Pendahuluan : Penanganan error secara struktural.
2. Sintaks dasar try-catch-finally.
3. Studi kasus perpustakaan: validasi input nomor anggota.
4. Studi kasus e-commerce: validasi kuantitas produk.
5. Studi kasus kesehatan: validasi format data pasien.
6. Peran blok finally.
7. Best practice: tangani error spesifik.
8. Hindari try-catch berlebihan.
9. Error sebagai bagian normal program.

* **Kesimpulan**: Try-catch memberikan kontrol lebih baik saat terjadi error, tanpa menghentikan aplikasi.
* **Referensi**:

  * Flanagan, D. (2020). *JavaScript: The Definitive Guide*.
  * Mozilla Developer Network. (2022). *MDN Web Docs*.
  * Haverbeke, M. (2018). *Eloquent JavaScript*.
  * Freeman, E. (2014). *Head First JavaScript Programming*.
  * Crockford, D. (2008). *JavaScript: The Good Parts*.

---

### Modul 3 : Praktik Try-Catch / practical

1. Pendahuluan : Latihan penanganan error langsung.
2. Konsep try-catch sederhana.
3. Studi kasus transportasi: cek input nomor tiket.
4. Studi kasus sosial media: cek panjang username.
5. Studi kasus perbankan: cek validasi saldo.
6. Kesalahan umum: catch tanpa pesan error.
7. Best practice: log error dengan jelas.
8. Debugging error di console.
9. Mini aplikasi validasi input sederhana.

* **Kesimpulan**: Praktik try-catch melatih kesiapan menghadapi error nyata dalam program.
* **Referensi**:

  * Mozilla Developer Network. (2022). *MDN Web Docs*.
  * Flanagan, D. (2020). *JavaScript: The Definitive Guide*.
  * Haverbeke, M. (2018). *Eloquent JavaScript*.
  * Fowler, M. (2018). *Refactoring*.
  * Freeman, E. (2014). *Head First JavaScript Programming*.

---

### Modul 4 : Konsep Debugging / concept

1. Pendahuluan : Debugging sebagai seni menemukan kesalahan.
2. Definisi bug dalam sejarah komputer.
3. Tools debugging di browser (Chrome DevTools).
4. Studi kasus perpustakaan: error data buku.
5. Studi kasus e-commerce: error hitung diskon.
6. Studi kasus sosial media: error tampil komentar.
7. Breakpoint untuk analisis alur kode.
8. Watch expression untuk monitor variabel.
9. Pentingnya skill debugging bagi developer.

* **Kesimpulan**: Debugging adalah keterampilan penting untuk meningkatkan kualitas kode dan aplikasi.
* **Referensi**:

  * Fowler, M. (2018). *Refactoring*. Addison-Wesley.
  * Mozilla Developer Network. (2022). *MDN Web Docs*.
  * Flanagan, D. (2020). *JavaScript: The Definitive Guide*.
  * Haverbeke, M. (2018). *Eloquent JavaScript*.
  * Freeman, E. (2014). *Head First JavaScript Programming*.

---

### Modul 5 : Praktik Debugging / practical

1. Pendahuluan : Latihan menggunakan debugging tools.
2. Konsep debugging dengan `console.log`.
3. Studi kasus kesehatan: cek input data pasien.
4. Studi kasus transportasi: cek hitung ongkos tiket.
5. Studi kasus perpustakaan: cek validasi jumlah buku.
6. Kesalahan umum: lupa hapus console log.
7. Best practice: gunakan tools DevTools.
8. Debugging dengan breakpoint.
9. Mini aplikasi debugging kalkulator sederhana.

* **Kesimpulan**: Praktik debugging mengajarkan cara sistematis menemukan dan memperbaiki error.
* **Referensi**:

  * Mozilla Developer Network. (2022). *MDN Web Docs*.
  * Flanagan, D. (2020). *JavaScript: The Definitive Guide*.
  * Haverbeke, M. (2018). *Eloquent JavaScript*.
  * Fowler, M. (2018). *Refactoring*.
  * Freeman, E. (2014). *Head First JavaScript Programming*.