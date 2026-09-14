# IQPOS Web — Static SEO Website

Website statis IQPOS untuk Vercel + custom domain `iqpos.web.id`.

## Struktur
- `index.html` — halaman utama
- `fitur.html` — fitur IQPOS
- `download.html` — halaman download
- `blog/` — artikel SEO
- `assets/css/style.css` — stylesheet
- `assets/js/main.js` — script ringan
- `assets/images/screenshots/` — tempat screenshot aplikasi
- `robots.txt` — aturan crawler
- `sitemap.xml` — sitemap Google
- `vercel.json` — header keamanan dasar

## Download resmi
https://github.com/timestravelers/IqPOS/releases/download/POS/IqPOS_Setup_2.3.0.exe

## Deploy
1. Upload/push folder ini ke repository GitHub baru, misalnya `iqpos-web`.
2. Import repository tersebut ke Vercel.
3. Deploy sebagai static site.
4. Setelah domain `iqpos.web.id` dibeli, tambahkan domain tersebut di Vercel Project > Settings > Domains.
5. Ikuti DNS record yang diberikan Vercel. Vercel mendukung custom domain pada project dan menyediakan konfigurasi DNS dari dashboard.
6. Setelah domain aktif, submit `https://iqpos.web.id/sitemap.xml` di Google Search Console.

## Screenshot
Ganti file berikut dengan screenshot IQPOS Anda:
- `assets/images/screenshots/kasir.jpg`
- `assets/images/screenshots/produk.jpg`
- `assets/images/screenshots/laporan.jpg`

Jika nama file screenshot Anda berbeda, ubah atribut `src` pada `index.html`.

## Catatan
Sitemap sudah menggunakan domain final `https://iqpos.web.id/`. Sebelum domain dibeli, website tetap bisa diuji melalui URL `.vercel.app`.
