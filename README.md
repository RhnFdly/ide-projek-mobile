Kebab House App
🎯 Fitur Utama
Halaman Produk (Menu):
Menampilkan daftar kebab dan side dishes yang tersedia dengan gambar, deskripsi, dan harga.
Filter/pencarian berdasarkan kategori (misalnya, Beef Kebab, Chicken Kebab, Sides).

Detail Produk:
Tampilan detail produk.
Pilihan kustomisasi (misalnya, tingkat kepedasan, tambahan sayuran/keju, ukuran porsi).
Tombol "Tambah ke Keranjang."

Keranjang Belanja (Cart):
Melihat item yang sudah ditambahkan.
Mengubah kuantitas atau menghapus item.
Menampilkan subtotal.
Checkout & Pembayaran:
Memasukkan alamat pengiriman atau memilih opsi pickup.
Memilih metode pembayaran (tunai/COD, transfer bank, atau dompet digital).
Konfirmasi pesanan.

Pelacakan Pesanan:
Melihat status pesanan saat ini (misalnya, Dipesan, Diproses, Dalam Pengiriman, Selesai).

Autentikasi Pengguna:
Login/Register menggunakan email atau akun sosial.
Profil pengguna (riwayat pesanan, alamat tersimpan).


# 🥙 Kebab House App

Aplikasi pemesanan makanan mobile (fokus pada kebab) yang dibuat menggunakan Flutter untuk pengalaman pemesanan yang cepat dan mulus.

## 📖 Daftar Isi

* [Fitur](#-fitur)
* [Teknologi](#-teknologi)
* [Instalasi](#-instalasi)
* [Struktur Proyek](#-struktur-proyek)
* [Kontributor](#-kontributor)
* [Lisensi](#-lisensi)

## ✨ Fitur

* **Tampilan Menu Interaktif:** Daftar produk dengan kategori dan pencarian.
* **Kustomisasi Pesanan:** Pilihan untuk mengubah bahan/opsi produk.
* **Alur Keranjang & Checkout:** Pengelolaan keranjang yang intuitif.
* **Opsi Pengiriman:** Pilihan *Delivery* atau *Takeaway/Pickup*.
* **Pelacakan Real-time:** Status pesanan yang diperbarui secara langsung.
* **Autentikasi Pengguna:** Login/Register.

## 🛠️ Teknologi

Aplikasi ini dibangun menggunakan:

* **Frontend:** [Flutter](https://flutter.dev/) (dengan Dart)
* **State Management:** [Provider](https://pub.dev/packages/provider) / [Bloc](https://pub.dev/packages/flutter_bloc) (Pilih salah satu)
* **Database/Backend:** [Firebase Firestore](https://firebase.google.com/docs/firestore) untuk data produk dan pesanan, [Firebase Authentication](https://firebase.google.com/docs/auth) untuk otentikasi.
* **Asset Management:** [Cached Network Image](https://pub.dev/packages/cached_network_image)
* **Dependencies Lainnya (Contoh):**
    * `http` (untuk API non-Firebase, jika ada)
    * `Maps_flutter` (untuk pemilihan lokasi pengiriman)

## 📂 Struktur Proyek

Struktur folder utama aplikasi (lib) diorganisasi sebagai berikut:

lib/ ├── core/ │ ├── constants/ # Konstanta aplikasi (warna, string, asset paths) │ ├── services/ # Layer interaksi dengan API/Firebase (misalnya: AuthService, OrderService) │ └── utils/ # Fungsi utilitas ├── data/ │ └── models/ # Model data (misalnya: Product, User, Order) ├── presentation/ │ ├── providers/ # File State Management (Provider/Blocs/Cubits) │ ├── screens/ # Folder untuk setiap halaman utama │ │ ├── auth/ │ │ ├── menu/ │ │ └── cart/ │ └── widgets/ # Komponen UI yang dapat digunakan kembali └── main.dart
