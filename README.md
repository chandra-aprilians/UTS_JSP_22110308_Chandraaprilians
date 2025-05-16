 SISTEM PEMESANAN TIKET BIOSKOP (JSP TANPA DATABASE)
Deskripsi Proyek

Aplikasi ini merupakan sistem pemesanan tiket bioskop berbasis web yang dibangun menggunakan teknologi **Java Server Pages (JSP)**. Aplikasi ini **tidak menggunakan database**, melainkan menyimpan data secara langsung di session. Tujuan dari aplikasi ini adalah untuk memberikan simulasi proses login, pemilihan film, pemesanan tiket, dan pencetakan struk.
Fitur Aplikasi

1. Login User
   * Autentikasi sederhana menggunakan username dan password yang sudah ditentukan.
2. Daftar Film Indonesia
   * Tersedia daftar film dengan detail seperti judul, genre, durasi, harga tiket, dan jam tayang.
3. Pemesanan Tiket
   * Pengguna dapat memilih film, jam tayang, dan jumlah tiket.
4. Struk Pemesanan
   * Setelah pemesanan, aplikasi akan menampilkan struk dengan rincian lengkap.
5. **Tampilan Menarik**
   * Desain menggunakan gaya **Neumorphism** langsung di dalam file JSP (tanpa CSS terpisah).
Struktur Folder dan File
TiketBioskopJSP/
│
├── login.jsp          (Halaman login)
  ├── prosesLogin.jsp    (Proses login)
├── index.jsp          (Halaman daftar film dan form pemesanan)
├── pesan.jsp          (Proses pemesanan tiket)
├── struk.jsp          (Halaman struk pesanan)
├── logout.jsp         (Logout dan hapus sesi)
└── WEB-INF/
    └── web.xml        (Konfigurasi Tomcat)

Data Login (Default)

* **Username**: admin
* **Password**: admin

 Cara Menjalankan Proyek

1. Pastikan **XAMPP** sudah terinstall dan aktifkan **Apache dan Tomcat**.
2. Simpan folder `TiketBioskopJSP` ke direktori berikut:
   `C:\xampp\tomcat\webapps\`
3. Jalankan Apache dan Tomcat dari XAMPP Control Panel.
4. Buka browser dan akses:

   ```
   http://localhost:8080/TiketBioskopJSP/login.jsp
   ```
5. Login menggunakan akun default, pilih film, pesan tiket, dan lihat struk.

---

### Catatan

* Semua logika pemrosesan dilakukan di dalam file JSP.
* Data film didefinisikan langsung di `index.jsp`, bukan dari database.
* File `Film.java` **tidak digunakan**, karena objek `Film` langsung dideklarasikan dalam halaman JSP.
* Desain menggunakan **inline CSS**, sehingga tidak perlu folder CSS terpisah.

---

### Informasi Tambahan

Proyek ini dibuat untuk memenuhi tugas **UAS Pemrograman Java Lanjut**.
Silakan disesuaikan dengan kebutuhan Anda untuk presentasi atau laporan akhir.
