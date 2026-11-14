# NUR Ngaji Manager

App web (PWA) untuk guru mengaji: kehadiran, rekod bacaan Iqra' / Al-Quran, kemajuan murid, laporan ibu bapa (WhatsApp), yuran bulanan dan kalender kelas.

## Ciri
- Kehadiran kelas (Hadir / Tidak hadir / Cuti) dan rekod ngaji (muka surat, Lulus / Separuh / Ulang, catatan guru)
- Kemajuan murid: bar peratus, perjalanan Iqra' 1–6 → Al-Quran, graf, sejarah
- Laporan ibu bapa + butang WhatsApp
- Yuran bulanan: rekod bayaran, resit, peringatan tunggakan, laporan kutipan
- Kalender kelas: batal kelas, kelas ganti, cuti beberapa hari
- Boleh dipasang di telefon dan digunakan tanpa internet

## Data
Semua data disimpan **dalam pelayar peranti itu sahaja** (localStorage). Tiada pelayan, tiada akaun.

- Data **tidak** selari antara telefon dan laptop. Guna satu peranti utama.
- Buat sandaran setiap minggu: **Tetapan → Muat turun fail sandaran**. Simpan fail `.json` di Google Drive atau WhatsApp sendiri.
- Untuk pindah peranti: muat turun sandaran di peranti lama → **Pulihkan dari fail** di peranti baru.
- Jangan kosongkan data pelayar (Clear browsing data / site data) untuk laman ini tanpa sandaran.

## Deploy (GitHub Pages)
1. Push semua fail ke repo GitHub.
2. Settings → Pages → Source: *Deploy from a branch* → `main` / `(root)`.
3. Buka `https://<username>.github.io/<repo>/`.

## Kemas kini app
Selepas mengubah `index.html`, naikkan `VERSION` dalam `sw.js` (contoh `nur-ngaji-v1.0.1`) supaya telefon mengambil versi baru.

## Fail
```
index.html              App (HTML + CSS + JS dalam satu fail)
manifest.webmanifest    Maklumat PWA (nama, ikon, warna)
sw.js                   Service worker (offline)
icons/                  Ikon app
```
