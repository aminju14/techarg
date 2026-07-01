# Techarg Synergi Indonesia — Landing Page

Landing page satu halaman untuk **Techarg Synergi Indonesia**, mitra teknologi terpadu di Jakarta yang menyediakan solusi infrastruktur IT: Data Centre, jaringan fiber & wireless, CCTV cerdas, videotron, dan produksi event.

Dibangun sebagai **satu file HTML statis** — tanpa framework, tanpa build step, tanpa dependency. Cukup buka di browser atau host di mana saja.

## ✨ Fitur

- **Single-file & zero-dependency** — hanya `index.html` + `favicon.svg`. Font dimuat dari Google Fonts.
- **Dark / Light theme** — toggle di navbar, preferensi tersimpan di `localStorage`.
- **Bilingual (ID / EN)** — pergantian bahasa runtime lewat sistem i18n sederhana.
- **Fully responsive** — desktop, tablet, dan mobile (termasuk menu hamburger + overlay).
- **Ilustrasi hero isometrik** — SVG infrastruktur (Data Center, Wireless Tower, Fiber, CCTV, Videotron, Cloud) dengan garis koneksi beranimasi, adaptif ke tema.
- **Animasi halus** — aurora background, scroll-reveal, animated stat counter, marquee partner, tombol back-to-top.
- **Logo dua-warna** — wordmark TECH + ARG yang menyesuaikan tema.
- Menghormati `prefers-reduced-motion`.

## 📁 Struktur

```
.
├── index.html      # Landing page (HTML + CSS + JS inline)
├── favicon.svg     # Favicon
├── README.md
└── .gitignore
```

## 🚀 Menjalankan secara lokal

Karena file statis, cukup buka `index.html` di browser. Atau jalankan server lokal (berguna untuk mengakses dari HP di jaringan yang sama):

```bash
# Python 3
python -m http.server 8000

# atau Node
npx serve
```

Lalu buka `http://localhost:8000`. Untuk akses dari HP, ganti `localhost` dengan alamat IP komputer di jaringan WiFi yang sama (mis. `http://192.168.x.x:8000`).

## 🌐 Deploy

File statis, jadi bisa di-host di mana saja:

- **GitHub Pages** — aktifkan di *Settings → Pages*, pilih branch `main` / root. Situs langsung tayang karena file bernama `index.html`.
- **Netlify / Vercel / Cloudflare Pages** — drag-and-drop folder atau hubungkan repo; tidak perlu konfigurasi build.

## 🎨 Kustomisasi

Semua warna dan spacing dikontrol lewat CSS custom properties di `:root` (dan `html[data-theme="dark"]`) pada bagian `<style>` di `index.html`:

- `--accent` — warna brand utama (merah)
- `--maxw` / `--gutter` — lebar maksimum konten & padding horizontal
- Variabel `--iso-*` — palet ilustrasi isometrik hero

Teks bilingual ada di objek kamus `T` (`id` dan `en`) di bagian `<script>`. Untuk mengubah kontak, cari `wa.me`, `info@techarg.id`, dan `+62 857-1952-8523`.

## 📞 Kontak

- **Email:** info@techarg.id
- **WhatsApp:** +62 857-1952-8523
- **Lokasi:** Jakarta, Indonesia

---

© 2025 Techarg Synergi Indonesia. All rights reserved.
