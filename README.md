# Kreasi AI Studio

Website statis (HTML/CSS/JavaScript) dengan 8 modul produksi konten berbasis Gemini API:
Pabrik Konten, Character Generator, Video Generator (Veo), Prompt Library, Character Clone, Image Generator, UGC Konten, dan Influencer Maker.

## Menjalankan
Buka `index.html` atau jalankan server lokal:
```bash
python3 -m http.server 8080
```
Lalu buka `http://localhost:8080`.

## Deploy GitHub Pages
1. Unggah seluruh file ke repository GitHub.
2. Settings → Pages → Deploy from branch → `main` / root.
3. Buka URL Pages, klik ikon pengaturan, masukkan Gemini API key.

## Keamanan
API key disimpan hanya di `localStorage` browser dan tidak ada key di source code. Untuk penggunaan publik/komersial, disarankan memakai backend proxy agar key dan kuota lebih aman. Batasi API key ke Gemini API dan tetapkan kuota di Google Cloud.

## Catatan API
- Model teks default: `gemini-2.5-flash`
- Model gambar default: `gemini-2.5-flash-image`
- Model video default: `veo-3.1-generate-preview`

Ketersediaan model bergantung pada akun, wilayah, billing, dan perubahan API Google. Nama model dapat diganti melalui Pengaturan.
