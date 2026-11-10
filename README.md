# DOUCE-WEB
Douce  Douce is a website for a handmade fashion accessories brand. The name "Douce" is French for "soft" or "gentle", reflecting a delicate, minimalist, and elegant style.

DOUCE STORE - Web Store Handcrafted Accessories

Douce Store adalah web store berbasis PHP + MySQL untuk menjual
produk aksesori handmade buatan tangan (clay charm, lighter case,
polaroid charm, dll). Terdapat dua peran pengguna:
  - Admin  : Mengelola katalog produk (tambah, edit, ubah status)
  - Customer: Melihat katalog, dan login akun

CARA MENJALANKAN APLIKASI

LANGKAH 1 - Pastikan XAMPP sudah terinstal

LANGKAH 2 - Jalankan XAMPP
1. Klik tombol [Start] Apache 
2. Klik tombol [Start] MySQL    

LANGKAH 3 - Salin folder project ke htdocs
Salin seluruh folder DOUCE ke:

  C:\xampp\htdocs\douce\

LANGKAH 4 - Import database ke phpMyAdmin
1. Buka browser, ketik: http://localhost/phpmyadmin
2. Klik buat database baru douce_db
3. setelah itu impport fil app.sql
4. Pastikan muncul pesan "Import has been successfully finished"

LANGKAH 5 - Buka aplikasi di browser

  http://localhost/douce/index.php     --> Halaman utama toko
  http://localhost/douce/login.php     --> Login akun
  http://localhost/douce/registrasi.php --> Daftar akun baru
  http://localhost/douce/admin.php     --> Dashboard Admin (login dulu)


AKUN UJI (DEMO ACCOUNT)

AKUN ADMIN:
  Email    : admin@douce.com
  Password : admin123
  Akses    : Bisa login dan masuk ke halaman Admin Panel untuk tambah/edit/hapus produk dan ubah status stok

AKUN CUSTOMER:
  Email    : usesr@gmail.com
  Password : user123
  Akses    : Login dan lihat katalog produk

Atau bisa daftar akun customer baru melalui:
  http://localhost/douce/registrasi.php


STRUKTUR FILE
  index.php         --> Halaman utama + katalog produk (dinamis)
  login.php         --> Login akun (admin & customer)
  logout.php        --> Proses keluar dari akun
  registrasi.php    --> Daftar akun customer baru
  detail.php        --> Halaman detail produk
  admin.php         --> Dashboard admin (kelola produk)
  admin_actions.php --> Proses tambah/edit/hapus produk
  koneksi.php       --> Koneksi ke database MySQL
  sesi.php          --> Manajemen sesi, e(), flash(), wajibLogin(), wajibPeran()
  validasi.php      --> Helper validasi input (panjang, email, pilihan, dll)
  style.css         --> Gaya tampilan Douce
  script.js         --> Interaksi halaman (navbar, toast, dll)
  app.sql           --> Struktur tabel + data awal
  Asset/            --> Gambar produk, logo, icon
