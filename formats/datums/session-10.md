## Pertemuan 10: Event Handling

---

### Modul 1 : Sejarah Event Driven Programming / history

1. Pendahuluan : Mengapa paradigma event-driven lahir.
2. Awal event handling di GUI (Smalltalk).
3. Event loop di C dan X Window System.
4. Perkembangan event di Visual Basic.
5. JavaScript dan DOM Level 2 Events.
6. Asynchronous event dengan AJAX.
7. Event loop dalam Node.js.
8. Framework modern (React, Vue) dan synthetic events.
9. Dampak event-driven pada UX modern.

* **Kesimpulan**: Event-driven programming menjadikan software lebih interaktif dengan merespons input user secara real-time.
* **Referensi**:

  * Sebesta, R. W. (2016). *Concepts of Programming Languages*. Pearson.
  * Flanagan, D. (2020). *JavaScript: The Definitive Guide*. O’Reilly.
  * Resig, J., & Bibeault, B. (2013). *Secrets of the JavaScript Ninja*. Manning.
  * Haverbeke, M. (2018). *Eloquent JavaScript*. No Starch Press.
  * Mozilla Developer Network. (2022). *MDN Web Docs*.

---

### Modul 2 : Konsep Event JavaScript / concept

1. Pendahuluan : Definisi event dalam konteks DOM.
2. Jenis event: mouse, keyboard, form, window.
3. Event bubbling dan capturing.
4. Studi kasus e-commerce: klik tombol checkout.
5. Studi kasus perpustakaan: submit form anggota.
6. Studi kasus transportasi: pilih jadwal tiket.
7. Pentingnya event listener.
8. Prevent default pada event.
9. Delegasi event untuk efisiensi.

* **Kesimpulan**: Event adalah sinyal interaksi user, inti dari web dinamis.
* **Referensi**:

  * Flanagan, D. (2020). *JavaScript: The Definitive Guide*.
  * Mozilla Developer Network. (2022). *MDN Web Docs*.
  * Haverbeke, M. (2018). *Eloquent JavaScript*.
  * Freeman, E. (2014). *Head First JavaScript Programming*.
  * Crockford, D. (2008). *JavaScript: The Good Parts*.

---

### Modul 3 : Praktik Event Klik / practical

1. Pendahuluan : Klik adalah event paling umum di web.
2. Konsep dasar `addEventListener("click")`.
3. Studi kasus perpustakaan: tombol pinjam buku.
4. Studi kasus e-commerce: tombol tambah ke keranjang.
5. Studi kasus sosial media: tombol like.
6. Kesalahan umum: event listener ganda.
7. Best practice: gunakan fungsi terpisah untuk handler.
8. Debugging dengan console log.
9. Mini aplikasi tombol interaktif.

* **Kesimpulan**: Event klik memperlihatkan bagaimana interaksi sederhana bisa mengubah UI.
* **Referensi**:

  * Mozilla Developer Network. (2022). *MDN Web Docs*.
  * Flanagan, D. (2020). *JavaScript: The Definitive Guide*.
  * Haverbeke, M. (2018). *Eloquent JavaScript*.
  * Fowler, M. (2018). *Refactoring*.
  * Freeman, E. (2014). *Head First JavaScript Programming*.

---

### Modul 4 : Praktik Event Keyboard / practical

1. Pendahuluan : Keyboard input untuk navigasi dan form.
2. Konsep event `keydown`, `keyup`, `keypress`.
3. Studi kasus perpustakaan: cari buku dengan mengetik judul.
4. Studi kasus sosial media: deteksi shortcut pesan.
5. Studi kasus transportasi: input kode tiket.
6. Kesalahan umum: tidak membedakan keyCode dan value.
7. Best practice: gunakan `event.key`.
8. Debugging input dengan console.
9. Mini aplikasi pencarian instan.

* **Kesimpulan**: Event keyboard meningkatkan aksesibilitas dan kecepatan interaksi user.
* **Referensi**:

  * Mozilla Developer Network. (2022). *MDN Web Docs*.
  * Flanagan, D. (2020). *JavaScript: The Definitive Guide*.
  * Haverbeke, M. (2018). *Eloquent JavaScript*.
  * Freeman, E. (2014). *Head First JavaScript Programming*.
  * Fowler, M. (2018). *Refactoring*.

---

### Modul 5 : Praktik Event Form / practical

1. Pendahuluan : Form sebagai sarana input utama user.
2. Konsep event `submit` dan `change`.
3. Studi kasus perpustakaan: form pendaftaran anggota.
4. Studi kasus e-commerce: form checkout belanja.
5. Studi kasus kesehatan: form registrasi pasien.
6. Kesalahan umum: form reload karena tidak prevent default.
7. Best practice: gunakan validasi sebelum submit.
8. Debugging data input dengan console.
9. Mini aplikasi form login sederhana.

* **Kesimpulan**: Event form sangat penting untuk interaksi data antara user dan aplikasi.
* **Referensi**:

  * Mozilla Developer Network. (2022). *MDN Web Docs*.
  * Flanagan, D. (2020). *JavaScript: The Definitive Guide*.
  * Haverbeke, M. (2018). *Eloquent JavaScript*.
  * Freeman, E. (2014). *Head First JavaScript Programming*.
  * Crockford, D. (2008). *JavaScript: The Good Parts*.