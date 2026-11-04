# Wira Bahasa: Misi Kontra

Game web Bahasa Melayu untuk murid Tahun 1–6.

## Muat naik ke GitHub Pages

1. Pastikan nama fail ialah `index.html` (huruf kecil semua) dan berada di root repo. Padam `Index.html` yang lama.
2. Muat naik `index.html`, `README.md`, `spritecook-assets.json` dan folder `assets/`.
3. Pergi ke **Settings → Pages**, pilih **Deploy from a branch**, branch `main`, folder `/ (root)`, kemudian tekan **Save**.
4. Selepas beberapa minit, buka `https://cikguhisyam91.github.io/wirabahasa/`.

## Guna Git

Git perlu dipasang dahulu.

```bash
git init
git add .
git commit -m "Naik taraf grafik Wira Bahasa"
git branch -M main
git remote add origin https://github.com/CikguHisyam91/wirabahasa.git
git pull origin main --allow-unrelated-histories
git push -u origin main
```

## Aset yang dijana

Jika sesuatu fail tiada atau gagal dimuatkan, game menggunakan lukisan Canvas asal.

Model: GPT-Image-2 kualiti rendah, 2 kredit setiap gambar. **Jumlah: 20 gambar, 40 kredit SpriteCook.** Saiz semua aset di bawah 1 MB.

| Fail | Isi | Gambar | Kredit |
|---|---|---|---|
| `assets/sprites/wira.png` | Diam/lari/tembak, lompat, tembak atas, tembak menyerong | 4 | 8 |
| `assets/sprites/askar.png` | Askar | 1 | 2 |
| `assets/sprites/dron.png` | Dron | 1 | 2 |
| `assets/sprites/menara.png`, `menara_laras.png` | Tapak dan laras menara meriam | 2 | 4 |
| `assets/sprites/bos1.png` hingga `bos5.png` | Raja Salah Eja, Gergasi Tatabahasa, Robot Kata Rojak, Naga Peribahasa, Maharaja Buta Huruf | 5 | 10 |
| `assets/sprites/letupan.png` | Letupan 8 frame | 1 | 2 |
| `assets/bg/tema1.png` hingga `tema5.png` | Hutan Belantara, Gua Kristal, Bandar Neon, Gunung Berapi, Kubu Langit | 5 | 10 |
| `assets/ui/nyawa.png` | Ikon nyawa | 1 | 2 |

## Belum dibuat (kredit habis)

Bahagian ini masih menggunakan lukisan Canvas atau CSS asal:

- Animasi berbilang frame untuk watak dan bos. Lari, jalan dan serang kini menggunakan gerakan ringkas daripada kod.
- Latar parallax 3 lapisan. Setiap tema kini satu gambar yang bergerak perlahan.
- Tileset platform dan tanah.
- Kesan peluru.
- Kit UI: butang, panel kuiz dan bar HP bos. Hanya ikon nyawa yang siap.
