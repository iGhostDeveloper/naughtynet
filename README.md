# NaughtyNet - Fake Adult Prelander Site

Proyek ini adalah implementasi dari dokumentasi NaughtyNet untuk membuat prelander site dengan monetisasi CPA dan push notification menggunakan Astro.

## Fitur

- ✅ Fake video player dengan animasi loading
- ✅ Timer countdown untuk menciptakan urgensi
- ✅ Sistem redirect ke CPA offers
- ✅ Cloaking untuk bot search engine
- ✅ Design responsif dan mobile-friendly
- ✅ Push notification integration (placeholder)
- ✅ Dark theme dengan gradient background

## Struktur Proyek

```
naughtynet/
├── src/
│   └── pages/
│       ├── index.astro     # Halaman utama dengan fake video player
│       └── safe.astro      # Halaman aman untuk bot crawler
├── public/
│   └── favicon.svg         # Icon website
├── package.json            # Dependencies dan scripts
├── astro.config.mjs        # Konfigurasi Astro
└── README.md              # Dokumentasi proyek
```

## Instalasi dan Menjalankan

1. Install dependencies:
```bash
npm install
```

2. Jalankan development server:
```bash
npm run dev
```

3. Build untuk production:
```bash
npm run build
```

4. Preview build:
```bash
npm run preview
```

## Konfigurasi CPA Links

Edit array `cpaLinks` di file `src/pages/index.astro` untuk mengganti placeholder links dengan CPA offers yang sebenarnya:

```javascript
const cpaLinks = [
    'https://your-cpa-offer-1.com',
    'https://your-cpa-offer-2.com',
    'https://your-cpa-offer-3.com'
];
```

## Deployment

Proyek ini dapat di-deploy ke:
- Cloudflare Pages
- Vercel
- Netlify
- GitHub Pages

Untuk Cloudflare Pages:
1. Push ke GitHub repository
2. Connect repository ke Cloudflare Pages
3. Set build command: `npm run build`
4. Set output directory: `dist`

## Fitur Keamanan

- **Bot Cloaking**: Otomatis redirect bot search engine ke halaman `/safe`
- **User Agent Detection**: Mendeteksi dan memfilter traffic bot
- **Safe Content**: Halaman safe tidak mengandung konten eksplisit

## Catatan Penting

⚠️ **Disclaimer**: Proyek ini dibuat untuk tujuan edukasi. Pastikan mematuhi:
- Terms of Service platform hosting
- Kebijakan CPA networks
- Regulasi lokal yang berlaku

## Customization

### Mengubah Timer
Edit variabel `timeLeft` di script untuk mengatur durasi countdown:
```javascript
let timeLeft = 89; // dalam detik (1:29)
```

### Mengubah Warna Theme
Edit CSS variables di bagian `:root` untuk mengubah color scheme.

### Menambah Halaman
Buat file `.astro` baru di folder `src/pages/` untuk menambah halaman.

## Browser Support

- Chrome/Chromium ✅
- Firefox ✅
- Safari ✅
- Edge ✅
- Mobile browsers ✅

## Performance

- Lightweight (< 50KB total)
- Fast loading time
- Mobile optimized
- SEO friendly (safe page)
