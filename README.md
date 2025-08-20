# WiFi Password Generator 📶

Aplikasi web sederhana untuk menghasilkan password default WiFi **khusus router FiberHome** menggunakan metode konversi SSID dengan mapping karakter khusus.

## 🚀 Demo
[Live Demo](https://wi-fi-password-generator.vercel.app/)

## ✨ Fitur
- **Khusus FiberHome Router** - Dirancang khusus untuk router merek FiberHome
- **Konversi SSID otomatis** - Ekstrak dan konversi bagian penting dari nama WiFi
- **Copy to clipboard** - Salin password hasil generate dengan satu klik
- **Responsive design** - Tampilan optimal di desktop dan mobile
- **Real-time conversion** - Generate password secara instan
- **Clean UI** - Interface minimalis dan user-friendly

## 🔧 Cara Penggunaan

1. Masukkan nama SSID WiFi FiberHome (contoh: `fh_b91f20_5G`)
2. Klik tombol **"Generate Password"**
3. Password akan muncul dengan format `wlan + konversi`
4. Klik **"Copy"** untuk menyalin password

### Contoh SSID FiberHome:
- **Input:** `fh_b91f20_5G`
- **Ekstrak:** `b91f20`
- **Konversi:** `b→4, 9→6, 1→e, f→0, 2→d, 0→f`
- **Output:** `wlan46e0df`

> **📌 Catatan:** Tool ini hanya bekerja untuk router FiberHome dengan format SSID: `fh_[hex]_[band]`

## 🔐 Metode Konversi

### Mapping Karakter:
- **Huruf ke angka:** `a=5, b=4, c=3, d=2, e=1, f=0`
- **Angka ke huruf:** `0=f, 1=e, 2=d, 3=c, 4=b, 5=a`
- **Angka ke angka:** `6=9, 7=8, 8=7, 9=6`

### Algoritma:
1. Ekstrak bagian hexadecimal dari SSID (biasanya setelah underscore)
2. Konversi setiap karakter menggunakan mapping di atas
3. Tambahkan prefix "wlan" di depan hasil konversi

## 🛠️ Teknologi
- **HTML5** - Struktur aplikasi
- **CSS3** - Styling dengan gradient dan glassmorphism effect
- **Vanilla JavaScript** - Logic konversi dan interaksi UI
- **No dependencies** - Tidak memerlukan library eksternal

## 🚀 Instalasi & Deployment

### Local Development:
1. Clone repository:
   ```bash
   git clone https://github.com/yourusername/wifi-password-generator.git
   cd wifi-password-generator
   ```

2. Buka `index.html` di browser atau gunakan live server

## ⚠️ Disclaimer

**Tool ini hanya untuk tujuan edukasi dan testing keamanan jaringan sendiri.**

- **Khusus router FiberHome** - Hanya berfungsi untuk router merek FiberHome
- Pastikan Anda memiliki izin sebelum mencoba mengakses jaringan WiFi
- Penulis tidak bertanggung jawab atas penyalahgunaan tool ini
- Gunakan secara etis dan sesuai dengan hukum yang berlaku
- Tool ini tidak menjamin 100% berhasil karena beberapa router mungkin menggunakan password custom

## 🤝 Kontribusi

Kontribusi sangat diterima! Silakan:

1. Fork repository ini
2. Buat branch fitur baru (`git checkout -b feature/AmazingFeature`)
3. Commit perubahan (`git commit -m 'Add some AmazingFeature'`)
4. Push ke branch (`git push origin feature/AmazingFeature`)
5. Buat Pull Request

## 📧 Kontak

Jika ada pertanyaan atau saran, silakan buat issue di repository ini.

---

⭐ **Jika project ini membantu, berikan star ya!** ⭐