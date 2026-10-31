# Aplikasi Profil Pengguna

Project ini bikin UI profil simpel pakai Flutter. Kodenya diperbaiki secara bertahap (4 kali commit) agar error-nya hilang, tampilannya rapi, dan komponennya bisa dipakai ulang (reusable).

## Progres Hari Ini: Tahap 1 (Benerin Error Dasar)
Hari ini fokus benerin error syntax biar kodenya bisa di-run:
- **Import Material:** Nambahin `import 'package:flutter/material.dart';` di paling atas biar widget-nya kebaca.
- **Koma Ketinggalan:** Nambahin koma di item ketiga list `experiences` (`'Lead Developer - Aplikasi Sekurindo',`).
- **Benerin Tipe Data:** Ganti angka `42` jadi string `'42'` di widget `StatItem` biar sesuai sama aturan class-nya.
- **Hapus Kurung Lebih:** Ngehapus satu kurung tutup yang kelebihan di bagian bawah `MainApp` biar kodenya nggak berantakan.

## Progres Hari Ini: Tahap 2 (Refactor Reusable Class)
Hari ini fokus merapikan struktur folder dan file biar komponen UI lebih modular (gampang dipakai ulang).
- **Ekstrak Komponen:** Memindahkan class `StatItem` dari `main.dart` ke file khusus di `lib/widgets/stat_item.dart`.
- **Clean Code:** Menambahkan *import* `stat_item.dart` ke dalam `main.dart`. Sekarang kodenya jauh lebih bersih dan kalau nanti butuh widget statistik di halaman lain, tinggal panggil saja.

## Progres Hari Ini: Tahap 3 (Layout & UI Adjustments)
Hari ini berfokus pada perbaikan tata letak (layouting) agar antarmuka aplikasi tidak mengalami *overflow* (bocor) pada layar dengan ukuran berbeda.
- **Fix RenderFlex Overflow:** Menambahkan widget `Expanded` untuk membungkus `ListView.builder`. Ini memperbaiki masalah *unbounded height* yang sering terjadi saat menggabungkan daftar yang bisa di-scroll (`ListView`) di dalam `Column`. Sekarang list pengalaman kerja tampil proporsional dan bisa di-scroll dengan aman.

## Progres Hari Ini: Tahap 4 (Pemisahan Data & Clean Code)
Hari ini adalah tahap akhir penyelesaian tugas. Fokusnya pada struktur data dan kebersihan kode (*clean code*).
- **Separation of Concerns:** Memisahkan data statis (nama pengguna, role, dan daftar pengalaman) dari `main.dart` ke file khusus di `lib/data/user_data.dart`. Ini membuat file utama fokus murni pada UI saja.
- **Code Formatting:** Merapikan indentasi dan format kode menggunakan *auto-formatter* bawaan VS Code agar lebih mudah dibaca dan sesuai standar penulisan Dart.

Tugas perbaikan kode dan refactor selesai! 🚀