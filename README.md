# TRIFIN: Trivia Finance Challenge

Versi siap GitHub Pages dari `TRIFIN REVISED [USE THIS!!].html`.

## Isi

| Path | Isi |
|---|---|
| `index.html` | Game TRIFIN (World Map + Pos 1–9), sama persis dengan file asli |
| `guru/index.html` | Dashboard & Handbook Guru (decoder nilai) |
| `assets/img/` | 77 gambar (WebP terkompresi) yang sebelumnya tertanam base64 di dalam HTML |
| `.nojekyll` | Supaya GitHub Pages menyajikan file apa adanya |

Bedanya dengan file asli hanya di gambar: dipisah ke `assets/img/` dan dikompres dari PNG ke WebP dengan ukuran piksel yang sama. Seluruh paket jadi sekitar 20 MB (file asli 360 MB), setiap file di bawah 1 MB, halaman terbuka dalam hitungan detik, dan gambar tiap pos baru diunduh saat pos itu dibuka.

## Cara deploy

1. Buat repo baru di GitHub, misalnya `trifin` (Public).
2. **Ekstrak zip dulu.** GitHub Pages tidak bisa membuka file zip. Lalu upload **seluruh isi** folder hasil ekstrak (bukan foldernya) ke root repo. Lewat web: *Add file → Upload files*, seret `index.html`, `README.md`, folder `assets` dan folder `guru` sekaligus, lalu *Commit changes*.
3. *Settings → Pages → Build and deployment*: Source = **Deploy from a branch**, Branch = **main**, folder **/ (root)**, lalu *Save*.
4. Tunggu 1–2 menit. Alamatnya:
   - Game: `https://<username>.github.io/trifin/`
   - Guru: `https://<username>.github.io/trifin/guru/`

## Penting: jangan timpa repo kode akses

QR pos yang sudah dicetak mengarah ke `tugasdipi.github.io/trifin-kode-akses/posN.html`. Jangan upload paket ini ke repo `trifin-kode-akses`, supaya file `pos1.html` … `pos9.html` di sana tetap utuh dan QR tetap berfungsi. Pakai repo terpisah seperti `trifin`.

## Catatan

- Game bisa juga dibuka lokal dengan klik dua kali `index.html`, asalkan folder `assets/` ikut di sebelahnya.
- Font (Google Fonts) dan ikon (Font Awesome) dimuat dari internet, sama seperti file asli.
- Progres pemain tersimpan di `localStorage` browser per alamat situs, jadi progres dari file lokal tidak terbawa ke versi online.
