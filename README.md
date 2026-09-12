# ServisGo - Aplikasi Service Motor Terpadu

![ServisGo](https://img.shields.io/badge/version-1.0.0-blue)
![React](https://img.shields.io/badge/react-18.2.0-green)
![PWA](https://img.shields.io/badge/PWA-Progressive%20Web%20App-orange)
![License](https://img.shields.io/badge/license-MIT-blue)

## 📱 Tentang Aplikasi

**ServisGo** adalah aplikasi mobile service motor yang terpadu, memungkinkan customer untuk memesan servis, montir untuk menerima pekerjaan, dan admin untuk monitoring semua transaksi. Aplikasi ini dibangun dengan React dan dapat diakses via browser serta diinstal sebagai Progressive Web App (PWA).

### ✨ Fitur Utama

#### 👤 Customer
- ✅ Pemesanan service motor online
- ✅ Tracking status servis real-time
- ✅ Riwayat pesanan lengkap
- ✅ Rating dan review untuk montir
- ✅ Berbagai metode pembayaran (Tunai, Transfer, GoPay, OVO, DANA)
- ✅ Notifikasi push untuk update status
- ✅ Dokumentasi foto pekerjaan dari montir

#### 🔧 Montir
- ✅ Menerima pesanan service dari customer
- ✅ Update status pekerjaan
- ✅ Mengajukan biaya tambahan
- ✅ Dokumentasi foto pekerjaan
- ✅ Manajemen online/offline status
- ✅ Rating dan statistik kinerja

#### 📊 Admin
- ✅ Dashboard monitoring real-time
- ✅ Statistik pesanan dan revenue
- ✅ Manajemen data montir
- ✅ Manajemen master layanan
- ✅ Laporan kinerja sistem

---

## 🚀 Quick Start

### Persyaratan Sistem
- Node.js 14+ ([download](https://nodejs.org/))
- npm atau yarn
- Browser modern (Chrome, Firefox, Safari, Edge)

### 1. Clone Repository

```bash
git clone https://github.com/njaenah099-ai/servisgo-app.git
cd servisgo-app
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Jalankan Development Server

```bash
npm start
```

Aplikasi akan terbuka di browser: `http://localhost:3000`

### 4. Build untuk Production

```bash
npm run build
```

File hasil build akan tersimpan di folder `build/`

---

## 📲 Instalasi Sebagai PWA

### Desktop (Chrome/Edge)
1. Buka aplikasi di browser
2. Klik ikon install di address bar (sebelah kanan)
3. Klik "Install ServisGo"
4. Aplikasi akan terbuka sebagai window terpisah

### Mobile (Android)
1. Buka aplikasi di Chrome
2. Tap menu (⋮) → "Install app" atau "Add to Home Screen"
3. Tap "Install"
4. Aplikasi akan muncul di home screen

### Mobile (iPhone/iPad)
1. Buka aplikasi di Safari
2. Tap Share (berbagi)
3. Pilih "Add to Home Screen"
4. Tap "Add"
5. Aplikasi akan muncul di home screen

---

## 🔐 Demo Akun

### Customer
- **Email**: Gunakan email apapun
- **Password**: Apapun
- **Role**: Customer

### Montir
- **Email**: Gunakan email apapun
- **Password**: Apapun
- **Role**: Mechanic

### Admin
- **Email**: `calonbikers85@gmail.com`
- **Password**: `Pekalongan27`
- **Role**: Admin

---

## 🏗️ Struktur Project

```
servisgo-app/
├── public/
│   ├── index.html              # HTML utama
│   ├── manifest.json           # PWA manifest
│   └── serviceWorker.js        # Service worker untuk offline support
├── src/
│   ├── App.jsx                 # Komponen utama aplikasi
│   ├── index.js                # Entry point React
│   └── index.css               # Global styles
├── package.json                # Dependencies
├── README.md                   # Dokumentasi
└── .gitignore                  # Git ignore config
```

---

## 💻 Technology Stack

- **Frontend**: React 18.2.0
- **Styling**: Tailwind CSS
- **PWA**: Service Worker, Web App Manifest
- **Build Tool**: Create React App (CRA)
- **Package Manager**: npm

---

## 🌐 Deployment

### Deploy ke Vercel (Recommended)

```bash
npm install -g vercel
vercel
```

### Deploy ke Netlify

```bash
npm run build
# Drag & drop folder 'build' ke netlify.com
```

### Deploy ke GitHub Pages

1. Update `homepage` di `package.json`:
   ```json
   "homepage": "https://username.github.io/servisgo-app"
   ```

2. Install gh-pages:
   ```bash
   npm install --save-dev gh-pages
   ```

3. Tambahkan scripts di `package.json`:
   ```json
   "predeploy": "npm run build",
   "deploy": "gh-pages -d build"
   ```

4. Deploy:
   ```bash
   npm run deploy
   ```

---

## 🔧 Konfigurasi Build

Untuk production build yang optimal, file `package.json` sudah dikonfigurasi dengan:
- Minifikasi code
- Tree shaking
- Code splitting
- Service Worker caching

---

## 📝 Fitur PWA

✅ **Installable** - Dapat diinstal sebagai aplikasi native-like
✅ **Offline Support** - Berfungsi offline dengan service worker
✅ **Fast Loading** - Caching strategy untuk performa optimal
✅ **Responsive** - Kompatibel dengan semua ukuran layar
✅ **App-like** - Fullscreen mode dan icon di home screen

---

## 🐛 Troubleshooting

### Service Worker tidak terdaftar
- Pastikan aplikasi diakses via HTTPS (kecuali localhost)
- Clear browser cache dan reload
- Check console untuk error messages

### Build gagal
```bash
# Clear node_modules dan install ulang
rm -rf node_modules package-lock.json
npm install
npm run build
```

### Tidak bisa install PWA
- Harus diakses via HTTPS
- Harus memiliki valid manifest.json
- Harus memiliki service worker yang terdaftar

---

## 📞 Support & Kontak

- **Email**: calonbikers85@gmail.com
- **Issues**: [GitHub Issues](https://github.com/njaenah099-ai/servisgo-app/issues)
- **Discussions**: [GitHub Discussions](https://github.com/njaenah099-ai/servisgo-app/discussions)

---

## 📄 License

MIT License - Bebas digunakan untuk keperluan komersial dan personal

---

## 🙏 Kontribusi

Kontribusi sangat diterima! Silakan:
1. Fork repository
2. Buat branch baru (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Buat Pull Request

---

## 🎯 Roadmap

- [ ] Backend API integration
- [ ] Database real-time (Firebase/Supabase)
- [ ] Payment gateway integration (Midtrans/Xendit)
- [ ] Maps integration (Google Maps)
- [ ] SMS/WhatsApp notifications
- [ ] Advanced analytics
- [ ] Multi-bahasa support
- [ ] Dark mode

---

**Terima kasih telah menggunakan ServisGo! 🚗💨**
