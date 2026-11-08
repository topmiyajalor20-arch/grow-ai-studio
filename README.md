# GROW AI STUDIO — versi 1.0

Aplikasi web editor video dasar yang responsif untuk iPad/HP.

## Fitur versi 1
- Pilih video dari perangkat dan pratinjau.
- Atur titik mulai dan selesai.
- Ubah rasio ke 9:16, 16:9, atau 1:1.
- Export MP4 menggunakan FFmpeg.wasm di browser.
- Bahasa Indonesia / Inggris.
- Tidak membutuhkan akun dan tidak mengunggah video ke server aplikasi.

## Batasan penting
Versi ini **belum memiliki generasi video AI** atau editing berbasis prompt. Proses export dilakukan di browser dan dapat berat pada iPad/HP. Gunakan klip pendek terlebih dahulu. Mesin FFmpeg diunduh dari CDN pada export pertama sehingga internet diperlukan. Ketersediaan CDN dan kompatibilitas browser dapat berubah.

## Cara pasang gratis lewat GitHub Pages
1. Buka https://github.com/ di Safari/Chrome dan buat akun gratis jika belum punya.
2. Buat repository baru bernama `grow-ai-studio`.
3. Pilih **Public**, lalu buat repository.
4. Pilih **Add file → Upload files**.
5. Upload `index.html`, `manifest.webmanifest`, dan `sw.js` dari folder ini. (Boleh upload file satu per satu dari aplikasi Files.)
6. Tekan **Commit changes**.
7. Buka **Settings → Pages**.
8. Pada **Build and deployment**, pilih **Deploy from a branch**.
9. Pilih branch `main`, folder `/ (root)`, lalu **Save**.
10. Tunggu proses publikasi, lalu buka alamat `https://USERNAME.github.io/grow-ai-studio/`.
11. Di iPad/iPhone: buka link di Safari → tombol Share → **Add to Home Screen**. Di Android: menu browser → **Add to Home screen**.

## Cara menggunakan
1. Buka aplikasi.
2. Tekan **Pilih video dari perangkat**.
3. Atur waktu mulai dan selesai dalam detik.
4. Pilih rasio output dan kualitas.
5. Tekan **Export MP4**. Pada pemakaian pertama, izinkan browser mengunduh mesin FFmpeg dari CDN.
6. Tunggu proses selesai, lalu simpan file hasil.

## Catatan privasi
File video diproses secara lokal di browser; aplikasi ini tidak memiliki fungsi upload video ke server. GitHub Pages hanya meng-host file aplikasi statis. Jangan mengunggah video pribadi ke repositori GitHub.
