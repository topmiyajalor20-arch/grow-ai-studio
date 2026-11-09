# GROW AI STUDIO — Stage 1 (v1.2)

## Isi paket
- `index.html` — dashboard, upload video lokal, preview, rasio, bahasa ID/EN, simpan metadata proyek.
- `manifest.webmanifest` — metadata instalasi PWA.
- `sw.js` — cache dasar agar app shell dapat dibuka kembali setelah pernah dimuat online.

## Deploy melalui GitHub Pages
1. Ekstrak ZIP ini.
2. Upload **tiga file di dalam folder** ke root repository GitHub (bukan folder ZIP-nya).
3. Jika diminta, replace `index.html`, `manifest.webmanifest`, dan `sw.js`.
4. Commit changes.
5. Buka Settings → Pages → Deploy from branch → `main` → `/(root)` → Save.
6. Buka URL GitHub Pages dan refresh.

## Yang sudah bekerja pada Stage 1
- Upload video dari perangkat dan preview.
- Pilihan rasio 9:16, 16:9, 1:1, dan asli mengubah frame preview.
- Bahasa Indonesia / Inggris.
- Simpan nama proyek dan pengaturan ke localStorage browser.
- Responsive untuk iPad, tablet, dan HP.

## Batasan yang disengaja
Tahap 1 belum mengekspor video dan belum menjalankan AI. Tombol export tidak ditampilkan agar tidak mengulang masalah FFmpeg yang macet pada versi lama. Tahap 2 akan menambahkan pipeline pemrosesan video yang diuji terpisah sebelum diaktifkan.

Video tetap berada di perangkat. Daftar proyek menyimpan metadata saja, bukan file video.
