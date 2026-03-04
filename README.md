# SLIDE SHOW · MULTI FOLDER MEDIA PLAYER

Aplikasi slideshow berbasis web yang dapat menampilkan gambar dan video dari berbagai sumber (Folder Lokal, Google Drive, HFS) dengan animasi PowerPoint 2007, teks berjalan, dan efek background. Cocok untuk presentasi di TV, monitor, atau proyektor.

---

## 📋 **DAFTAR ISI**
- [Fitur Utama](#fitur-utama)
- [Persyaratan Sistem](#persyaratan-sistem)
- [Cara Instalasi](#cara-instalasi)
- [Cara Penggunaan](#cara-penggunaan)
- [Konfigurasi](#konfigurasi)
- [Anti 404 Protection](#anti-404-protection)
- [Remote Control untuk TV](#remote-control-untuk-tv)
- [Membuat APK Android TV](#membuat-apk-android-tv)
- [Troubleshooting](#troubleshooting)
- [Lisensi](#lisensi)
- [Kontak](#kontak)

---

## ✨ **FITUR UTAMA**

| Fitur | Keterangan |
|-------|------------|
| 🖼️ **Multi-source Media** | Load dari Folder Lokal, Google Drive, HFS |
| 🎞️ **50+ Animasi PowerPoint** | Entrance, Emphasis, Exit, Motion Paths |
| 🌧️ **Efek Background** | Hujan, Salju, Hati Neon, Campuran |
| 📝 **Running Text** | Teks berjalan dengan kustomisasi lengkap |
| 🎵 **Audio MP3** | Playlist dengan kontrol prev/next |
| 📅 **Tanggal & Waktu** | Tampilan real-time |
| 📱 **PWA Support** | Dapat diinstall sebagai aplikasi |
| 🔄 **Auto Update** | Deteksi perubahan file di Google Drive |
| 🚫 **Anti 404** | Proteksi terhadap file tidak ditemukan |
| 🖥️ **TV Support** | Bisa pakai remote dengan Android wrapper |

---

## 💻 **PERSYARATAN SISTEM**

### **Untuk Menjalankan di Browser:**
- Browser: Chrome 80+, Firefox 75+, Edge 80+
- RAM: Minimal 2GB (4GB recommended)
- Koneksi Internet: Untuk akses Google Drive / HFS

### **Untuk Menjalankan di TV:**
- Android TV (Sony, Sharp, Xiaomi, TCL) atau
- Smart TV dengan browser + mouse USB
- Port USB untuk mouse/keyboard

---

## 📦 **CARA INSTALASI**

### **Opsi 1: Jalankan Langsung dari File**
1. Download semua file:
   - index.html
   - manifest.json
   - sw.js
   - icon-192.png
2. Buka file index.html dengan Chrome

### **Opsi 2: Hosting dengan HTTP Server**
```bash
python -m http.server 8080
```
Buka browser: http://localhost:8080

---

## 🎮 **CARA PENGGUNAAN**

### **Tombol Kontrol:**
- ⏪ Previous Slide
- ⏯️ Play/Pause
- ⏩ Next Slide
- 🔇/🔊 Music
- 📁 Pilih Folder Lokal
- 🌐 Load dari HFS
- 🖵 Fullscreen
- 🛠️ Settings

### **Shortcut Keyboard:**
- → (Panah Kanan) : Next Slide
- ← (Panah Kiri)  : Previous Slide
- Spasi           : Play/Pause
- F11             : Fullscreen

---

## ⚙️ **KONFIGURASI**

### **Google Drive Setup:**
```javascript
const CONFIG = {
  APPS_SCRIPT_URL: 'https://script.google.com/macros/s/.../exec',
  GOOGLE_DRIVE_FOLDER_ID: '1I5wVeLcrSS2sjlaRLCftwd9JPfbNri0l'
};
```

### **HFS Setup:**
1. Download HFS dari: http://rejetto.com/hfs/
2. Jalankan HFS di laptop
3. Drag folder media ke HFS
4. Catat IP laptop (ipconfig di CMD)
5. Masukkan IP di settings panel

---

## 🛡️ **ANTI 404 PROTECTION**

| Komponen | Proteksi |
|----------|----------|
| **Gambar** | Tampil placeholder "Error" |
| **Video** | Auto skip ke slide berikutnya |
| **Audio** | Auto skip ke lagu berikutnya |
| **Google Drive** | Tampil pesan error |
| **HFS** | Tampil pesan error |
| **Splash Screen** | Langsung ke main app jika tidak ada |

---

## 📺 **REMOTE CONTROL UNTUK TV**

### **Opsi 1: Pakai Mouse USB (Termudah)**
- Beli mouse wireless (Rp 50-100rb)
- Colok receiver ke port USB TV
- Mouse langsung berfungsi

### **Opsi 2: Buat APK Android TV**
1. Kumpulkan semua file jadi ZIP
2. Buka: https://www.web2apk.com
3. Upload ZIP, buat APK
4. Install APK ke TV via USB

---

## 📱 **MEMBUAT APK ANDROID TV**

### **Langkah-langkah:**
1. Kumpulkan semua file aplikasi dalam 1 folder
2. Seleksi semua file → Klik kanan → Send to → Compressed folder
3. Hasil: slideshow.zip
4. Buka https://www.web2apk.com
5. Upload file ZIP
6. Isi App Name: Slideshow TV
7. Klik "Create APK" (pilih yang gratis)
8. Download APK
9. Install ke TV via USB

---

## 🔧 **TROUBLESHOOTING**

| Masalah | Solusi |
|---------|--------|
| **Gambar tidak muncul** | Cek koneksi internet, refresh |
| **Video tidak jalan** | Pastikan format MP4 H.264 |
| **Audio tidak bunyi** | Klik tombol play manual |
| **Google Drive error** | Cek folder ID |
| **HFS tidak terhubung** | Cek IP dan port |
| **Remote TV tidak bisa klik** | Gunakan mouse USB |

---

## 📋 **STRUKTUR FILE**

```
project/
├── index.html              # File utama
├── splash.html             # (Opsional) Halaman splash
├── manifest.json           # PWA manifest
├── sw.js                   # Service Worker
├── icon-192.png            # Icon 192x192
├── icon-512.png            # Icon besar (opsional)
└── README.md               # Dokumentasi ini
```

---

## 📝 **LISENSI**

© 2026 Koramil 1609-05/Sukasada
Dibuat oleh: Serka I Nyoman Arta

Aplikasi ini gratis untuk digunakan.

---

## 📞 **KONTAK**

| | |
|---|---|
| **Pengembang** | Serka I Nyoman Arta |
| **Unit** | Koramil 1609-05/Sukasada |
| **Lokasi** | Buleleng, Bali |

---

## 🙏 **TERIMA KASIH**

Terima kasih telah menggunakan aplikasi ini. Semoga bermanfaat!

**Selamat mencoba!** 🎉
