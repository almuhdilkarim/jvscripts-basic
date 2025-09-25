## Pertemuan 11: Asynchronous JavaScript

---

### Modul 1 : Sejarah AJAX / history

1. Pendahuluan : Kebutuhan web interaktif tanpa reload.
2. Awal XMLHttpRequest di Internet Explorer.
3. Popularitas AJAX di tahun 2005 (Google Maps & Gmail).
4. Peran JSON dalam pertukaran data ringan.
5. Evolusi ke Fetch API.
6. Node.js dan event loop asynchronous.
7. Promise sebagai solusi callback hell.
8. Async/Await untuk kode yang lebih bersih.
9. Dampak asynchronous pada aplikasi real-time.

* **Kesimpulan**: AJAX membuka jalan web interaktif, dilanjutkan Promise dan Async/Await yang membuat JavaScript semakin kuat.
* **Referensi**:

  * Garrett, J. J. (2005). Ajax: A New Approach to Web Applications. *Adaptive Path*.
  * Flanagan, D. (2020). *JavaScript: The Definitive Guide*. O’Reilly.
  * Haverbeke, M. (2018). *Eloquent JavaScript*. No Starch Press.
  * Mozilla Developer Network. (2022). *MDN Web Docs*.
  * Tilkov, S., & Vinoski, S. (2010). Node.js: Using JavaScript to Build High-Performance Network Programs. *IEEE Internet Computing*.

---

### Modul 2 : Konsep Asynchronous & Callback / concept

1. Pendahuluan : JavaScript menggunakan single-threaded model.
2. Definisi asynchronous dan event loop.
3. Callback function sebagai dasar async.
4. Studi kasus perpustakaan: cek ketersediaan buku dari server.
5. Studi kasus e-commerce: validasi stok produk real-time.
6. Callback hell sebagai masalah umum.
7. Pentingnya error-first callback.
8. Perbandingan sync vs async.
9. Relevansi asynchronous di aplikasi modern.

* **Kesimpulan**: Callback adalah fondasi asynchronous, meski sering membuat kode sulit dibaca.
* **Referensi**:

  * Flanagan, D. (2020). *JavaScript: The Definitive Guide*.
  * Mozilla Developer Network. (2022). *MDN Web Docs*.
  * Haverbeke, M. (2018). *Eloquent JavaScript*.
  * Freeman, E. (2014). *Head First JavaScript Programming*.
  * Tilkov, S., & Vinoski, S. (2010). *IEEE Internet Computing*.

---

### Modul 3 : Praktik Callback / practical

1. Pendahuluan : Implementasi fungsi callback.
2. Konsep callback dengan parameter fungsi.
3. Studi kasus sosial media: load komentar setelah postingan.
4. Studi kasus transportasi: cek jadwal bus dari API.
5. Studi kasus perbankan: validasi transaksi.
6. Kesalahan umum: nested callback (callback hell).
7. Best practice: pecah callback ke fungsi terpisah.
8. Debugging alur eksekusi dengan console.
9. Mini aplikasi simulasi delay loading data.

* **Kesimpulan**: Callback memungkinkan asynchronous berjalan, tetapi perlu dikelola agar kode tetap terbaca.
* **Referensi**:

  * Mozilla Developer Network. (2022). *MDN Web Docs*.
  * Flanagan, D. (2020). *JavaScript: The Definitive Guide*.
  * Haverbeke, M. (2018). *Eloquent JavaScript*.
  * Fowler, M. (2018). *Refactoring*.
  * Freeman, E. (2014). *Head First JavaScript Programming*.

---

### Modul 4 : Konsep Promise / concept

1. Pendahuluan : Promise sebagai solusi callback hell.
2. Definisi Promise (pending, fulfilled, rejected).
3. Sintaks dasar `new Promise()`.
4. Studi kasus perpustakaan: peminjaman buku dengan delay.
5. Studi kasus e-commerce: cek status pembayaran.
6. Method `then`, `catch`, `finally`.
7. Chaining Promise.
8. Error handling yang lebih jelas.
9. Peran Promise di Fetch API.

* **Kesimpulan**: Promise menyederhanakan asynchronous dengan struktur yang lebih rapi daripada callback.
* **Referensi**:

  * Flanagan, D. (2020). *JavaScript: The Definitive Guide*.
  * Mozilla Developer Network. (2022). *MDN Web Docs*.
  * Haverbeke, M. (2018). *Eloquent JavaScript*.
  * Crockford, D. (2008). *JavaScript: The Good Parts*.
  * Tilkov, S., & Vinoski, S. (2010). *IEEE Internet Computing*.

---

### Modul 5 : Praktik Async Await / practical

1. Pendahuluan : Async/Await membuat async mirip sync.
2. Konsep `async function` dan `await`.
3. Studi kasus perpustakaan: ambil data katalog buku dari API.
4. Studi kasus kesehatan: ambil jadwal dokter online.
5. Studi kasus sosial media: ambil postingan terbaru.
6. Kesalahan umum: lupa pakai `await`.
7. Best practice: selalu gunakan `try...catch`.
8. Debugging dengan log step by step.
9. Mini aplikasi fetch data sederhana.

* **Kesimpulan**: Async/Await menjadikan asynchronous lebih mudah dibaca dan dikelola.
* **Referensi**:

  * Mozilla Developer Network. (2022). *MDN Web Docs*.
  * Flanagan, D. (2020). *JavaScript: The Definitive Guide*.
  * Haverbeke, M. (2018). *Eloquent JavaScript*.
  * Fowler, M. (2018). *Refactoring*.
  * Freeman, E. (2014). *Head First JavaScript Programming*.