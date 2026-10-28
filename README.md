# Aplikasi Profil Pengguna

Project ini bikin UI profil simpel pakai Flutter. Kodenya lagi di-fix pelan-pelan biar error-nya hilang, tampilannya rapi, dan komponennya bisa dipakai ulang (reusable).

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
