# SIPITUNG 2026 — Paket Countdown dan Quick Count

Paket kerja bersih yang diambil dari repository sumber.

## Halaman yang dipertahankan
- `index.html`: Countdown Pilkades, dengan logo SIPITUNG dan logo desa.
- `dashboard.html`: Dashboard Quick Count SIPITUNG.

## Integrasi data
Dashboard tetap menggunakan Google Sheets ID dan nama sheet dari sumber asli. Pembacaan `dashboard_desa`, `calon`, `pra_tps`, dan `hasil`, termasuk perakitan rekap dusun, dipertahankan. Apps Script eksternal tidak diubah.

## Catatan
- Jangan mengganti Spreadsheet ID, nama sheet, atau struktur kolom tanpa pengujian dan persetujuan.
- Jalankan melalui GitHub Pages atau server lokal (bukan `file://`) agar `fetch` Google Sheets bekerja.
- Halaman input petugas tidak dibuat/diubah dalam paket pemilahan ini.


## Formulir petugas TPS
- `entry.html` adalah formulir input petugas yang dibuka melalui GitHub Pages.
- URL Web App Apps Script sudah dipasang pada konfigurasi `API_URL` di `entry.html`.
- Token TPS dibaca dari fragment URL (`#token=...`) dan diverifikasi oleh Apps Script.
- Jangan mengubah struktur sheet atau Apps Script tanpa pengujian.
