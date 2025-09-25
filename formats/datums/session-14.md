## Pertemuan 14: Storage & API

---

### Modul 1 : Sejarah Web Storage / history

1. Pendahuluan : Kebutuhan menyimpan data di sisi client.
2. Era awal: cookie sebagai penyimpanan data user.
3. Keterbatasan cookie (ukuran, keamanan).
4. Munculnya Web Storage API (HTML5).
5. LocalStorage dan SessionStorage.
6. IndexedDB sebagai solusi database di browser.
7. Evolusi API untuk penyimpanan offline.
8. Integrasi dengan Progressive Web Apps (PWA).
9. Dampak web storage pada UX modern.

* **Kesimpulan**: Web storage menggantikan cookie dengan cara lebih aman, cepat, dan efisien untuk menyimpan data lokal.
* **Referensi**:

  * W3C. (2010). *Web Storage Specification*.
  * Flanagan, D. (2020). *JavaScript: The Definitive Guide*. O’Reilly.
  * Haverbeke, M. (2018). *Eloquent JavaScript*. No Starch Press.
  * Mozilla Developer Network. (2022). *MDN Web Docs*.
  * Freeman, E. (2014). *Head First JavaScript Programming*.

---

### Modul 2 : Konsep LocalStorage / concept

1. Pendahuluan : LocalStorage sebagai penyimpanan key-value.
2. Definisi dan sifat persistent storage.
3. Sintaks dasar `setItem`, `getItem`, `removeItem`.
4. Studi kasus perpustakaan: simpan preferensi tampilan katalog.
5. Studi kasus e-commerce: simpan keranjang belanja.
6. Studi kasus sosial media: simpan draft postingan.
7. Limitasi kapasitas LocalStorage.
8. Perbedaan dengan SessionStorage.
9. Pentingnya clear data untuk keamanan.

* **Kesimpulan**: LocalStorage menyederhanakan penyimpanan data user tanpa database server.
* **Referensi**:

  * Mozilla Developer Network. (2022). *MDN Web Docs*.
  * Flanagan, D. (2020). *JavaScript: The Definitive Guide*.
  * Haverbeke, M. (2018). *Eloquent JavaScript*.
  * W3C. (2010). *Web Storage Specification*.
  * Fowler, M. (2018). *Refactoring*.

---

### Modul 3 : Praktik LocalStorage / practical

1. Pendahuluan : Latihan menggunakan LocalStorage.
2. Konsep penyimpanan key-value.
3. Studi kasus: simpan daftar buku favorit.
4. Studi kasus: simpan data checkout belanja.
5. Studi kasus: simpan preferensi tema aplikasi.
6. Kesalahan umum: menyimpan object langsung tanpa JSON.
7. Best practice: gunakan `JSON.stringify()` dan `JSON.parse()`.
8. Debugging data di Application tab browser.
9. Mini aplikasi catatan sederhana.

* **Kesimpulan**: Praktik LocalStorage memperlihatkan kemudahan menyimpan data tanpa backend.
* **Referensi**:

  * Mozilla Developer Network. (2022). *MDN Web Docs*.
  * Flanagan, D. (2020). *JavaScript: The Definitive Guide*.
  * Haverbeke, M. (2018). *Eloquent JavaScript*.
  * Freeman, E. (2014). *Head First JavaScript Programming*.
  * Crockford, D. (2008). *JavaScript: The Good Parts*.

---

### Modul 4 : Konsep Fetch API / concept

1. Pendahuluan : Kebutuhan komunikasi client-server.
2. Definisi Fetch API sebagai pengganti XMLHttpRequest.
3. Sintaks dasar `fetch()`.
4. Studi kasus perpustakaan: ambil katalog buku dari server.
5. Studi kasus kesehatan: ambil jadwal vaksinasi.
6. Studi kasus transportasi: ambil jadwal kereta.
7. Promise dan chaining pada fetch.
8. Error handling dengan `catch`.
9. Perbandingan dengan AJAX lama.

* **Kesimpulan**: Fetch API menyederhanakan pengambilan data eksternal dengan pendekatan modern berbasis Promise.
* **Referensi**:

  * Mozilla Developer Network. (2022). *MDN Web Docs*.
  * Flanagan, D. (2020). *JavaScript: The Definitive Guide*.
  * Haverbeke, M. (2018). *Eloquent JavaScript*.
  * Tilkov, S., & Vinoski, S. (2010). *IEEE Internet Computing*.
  * Resig, J., & Bibeault, B. (2013). *Secrets of the JavaScript Ninja*.

---

### Modul 5 : Praktik Fetch API / practical

1. Pendahuluan : Latihan ambil data dengan Fetch API.
2. Konsep dasar penggunaan `fetch()`.
3. Studi kasus: ambil data buku dari API.
4. Studi kasus: ambil data produk e-commerce.
5. Studi kasus: ambil data cuaca (transportasi).
6. Kesalahan umum: lupa `await` atau `then`.
7. Best practice: gunakan async-await dengan try-catch.
8. Debugging response dengan console.
9. Mini aplikasi pencarian data API publik.

* **Kesimpulan**: Praktik Fetch API memberi pengalaman nyata menghubungkan aplikasi dengan server eksternal.
* **Referensi**:

  * Mozilla Developer Network. (2022). *MDN Web Docs*.
  * Flanagan, D. (2020). *JavaScript: The Definitive Guide*.
  * Haverbeke, M. (2018). *Eloquent JavaScript*.
  * Fowler, M. (2018). *Refactoring*.
  * Freeman, E. (2014). *Head First JavaScript Programming*.