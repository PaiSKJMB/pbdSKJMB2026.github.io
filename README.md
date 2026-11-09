# Dashboard Pencapaian PBD Pendidikan Islam & Pelajaran Jawi
SK Jalan Matang Buluh, 2026. Laman statik (HTML, CSS, JavaScript). Tiada langkah binaan.

## Struktur
- `index.html` – kerangka halaman
- `css/style.css` – gaya dan tema terang/gelap
- `js/app.js` – penapis, KPI, carta (Chart.js), jadual, senarai murid, rumusan
- `js/data.js` – data murid (dijana)
- `assets/logo.png` – logo sekolah
- `tools/build_data.py` – jana semula `js/data.js` daripada CSV/XLSX

## Jalankan setempat
Buka `index.html` dalam pelayar, atau: `python -m http.server 8000` kemudian buka http://localhost:8000
(Perlu internet untuk memuat Chart.js dan fon.)

## Kemas kini data
    pip install openpyxl
    python tools/build_data.py islam.csv jawi.xlsx js/data.js

## Deploy ke Netlify
Seret seluruh folder ini ke Netlify Drop (app.netlify.com/drop), atau sambungkan repositori GitHub
dengan Publish directory `.` dan Build command kosong.

## Perhatian
`js/data.js` mengandungi nama murid. Jangan jadikan repositori atau laman ini awam tanpa kebenaran sekolah.
