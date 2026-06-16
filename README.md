# Rekty POS - Aplikasi Kasir Flutter

Aplikasi Point of Sale (POS) sederhana yang dibangun dengan Flutter + Isar Database.

## Fitur
- 📦 Manajemen Produk (CRUD, stok, kategori)
- 🛒 Kasir / Transaksi dengan keranjang belanja
- 💳 Berbagai metode pembayaran (Tunai, Transfer, QRIS)
- 📊 Laporan penjualan harian / mingguan / bulanan
- 🗄️ Database lokal offline dengan Isar

## Struktur Project
```
lib/
├── main.dart
├── database/
│   └── isar_service.dart
├── models/
│   ├── product.dart
│   ├── transaction.dart
│   └── customer.dart
├── screens/
│   ├── dashboard_screen.dart
│   ├── product_screen.dart
│   ├── transaction_screen.dart
│   └── report_screen.dart
└── widgets/
    ├── summary_card.dart
    ├── product_card.dart
    └── cart_item_tile.dart
```

## Cara Menjalankan

1. Install Flutter SDK (https://flutter.dev)
2. Clone atau ekstrak project ini
3. Jalankan perintah berikut:
```bash
flutter pub get
flutter pub run build_runner build
flutter run
```

## Dependencies
- `isar` + `isar_flutter_libs` — database lokal cepat
- `path_provider` — lokasi penyimpanan
- `intl` — format tanggal & mata uang

## Catatan
File `*.g.dart` (generated) perlu dibuat dengan:
```bash
flutter pub run build_runner build --delete-conflicting-outputs
```
