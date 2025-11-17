# Dashboard Prakiraan Cuaca Jombang - BMKG

Dashboard web interaktif untuk menampilkan prakiraan cuaca wilayah Jombang menggunakan API terbuka dari BMKG (Badan Meteorologi, Klimatologi, dan Geofisika).

## 📋 Fitur

- ✅ Menampilkan cuaca real-time dari API BMKG
- ✅ Prakiraan cuaca 3 hari ke depan (per 3 jam)
- ✅ Pemilihan 21 kecamatan di wilayah Jombang
- ✅ Informasi detail: suhu, kelembapan, kecepatan angin, arah angin, jarak pandang, tutupan awan
- ✅ Tampilan responsif (mobile-friendly)
- ✅ Caching data untuk performa lebih baik
- ✅ Menyimpan pilihan wilayah terakhir

## 🚀 Cara Menggunakan

### Metode 1: Langsung Buka File HTML

1. Buka file `index.html` di browser (Chrome, Firefox, Edge, dll)
2. Pilih kecamatan/wilayah Jombang dari dropdown
3. Klik tombol "Muat Data Cuaca"
4. Data cuaca akan ditampilkan secara otomatis

### Metode 2: Menggunakan Local Server (Direkomendasikan)

Jika menggunakan Visual Studio Code:

1. Install extension "Live Server"
2. Klik kanan pada `index.html`
3. Pilih "Open with Live Server"
4. Browser akan otomatis terbuka

Atau menggunakan Python:

```bash
# Python 3
python -m http.server 8000

# Akses di browser: http://localhost:8000
```

## 📁 Struktur File

```
random-forest-weather/
├── index.html      # File HTML utama
├── style.css       # Styling dan desain
├── script.js       # Logika JavaScript dan API
└── README.md       # Dokumentasi ini
```

## 🔧 Teknologi yang Digunakan

- **HTML5** - Struktur halaman web
- **CSS3** - Styling dengan gradient modern dan responsive design
- **JavaScript (Vanilla)** - Fetch API untuk mengambil data dari BMKG
- **BMKG API** - Sumber data cuaca resmi

## 📡 API BMKG

API yang digunakan:
```
https://api.bmkg.go.id/publik/prakiraan-cuaca?adm4={kode_wilayah}
```

### Kode Wilayah Jombang yang Tersedia:

- 35.17.01.1001 - Denanyar
- 35.17.02.1001 - Mojoagung
- 35.17.03.1001 - Sumobito
- 35.17.04.1001 - Jogoroto
- 35.17.05.1001 - Peterongan
- 35.17.06.1001 - Jombang Kota
- 35.17.07.1001 - Megaluh
- 35.17.08.1001 - Tembelang
- 35.17.09.1001 - Kesamben
- 35.17.10.1001 - Kudu
- 35.17.11.1001 - Ngusikan
- 35.17.12.1001 - Ploso
- 35.17.13.1001 - Kabuh
- 35.17.14.1001 - Bandar Kedung Mulyo
- 35.17.15.1001 - Perak
- 35.17.16.1001 - Gudo
- 35.17.17.1001 - Ngoro
- 35.17.18.1001 - Mojowarno
- 35.17.19.1001 - Bareng
- 35.17.20.1001 - Wonosalam
- 35.17.21.1001 - Diwek

## 📊 Data yang Ditampilkan

### Cuaca Saat Ini:
- Suhu udara (°C)
- Kondisi cuaca dengan icon
- Kelembapan udara (%)
- Kecepatan angin (km/jam)
- Arah angin
- Jarak pandang
- Tutupan awan (%)

### Prakiraan 3 Hari:
- 8 prakiraan per hari (setiap 3 jam)
- Informasi lengkap untuk setiap periode waktu
- Visualisasi dengan card yang interaktif

## ⚠️ Catatan Penting

1. **Koneksi Internet**: Diperlukan koneksi internet untuk mengakses API BMKG
2. **CORS**: Jika mengalami masalah CORS, gunakan local server (Live Server atau Python HTTP server)
3. **Rate Limit**: API BMKG memiliki batas 60 permintaan per menit per IP
4. **Sumber Data**: Wajib mencantumkan BMKG sebagai sumber data sesuai ketentuan

## 🎨 Kustomisasi

### Mengubah Warna Tema:
Edit file `style.css` pada bagian gradient:

```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

### Menambah Wilayah Lain:
Tambahkan option baru di `index.html`:

```html
<option value="KODE_WILAYAH">Nama Wilayah</option>
```

## 📝 Lisensi

Program ini menggunakan data dari BMKG yang bersifat terbuka. Wajib mencantumkan:

**"Sumber Data: BMKG (Badan Meteorologi, Klimatologi, dan Geofisika)"**

## 🔗 Referensi

- [BMKG Data Terbuka](https://data.bmkg.go.id/prakiraan-cuaca)
- [GitHub BMKG Data Cuaca](https://github.com/infoBMKG/data-cuaca)

## 👨‍💻 Pengembangan

Dikembangkan untuk keperluan monitoring cuaca wilayah Jombang, Jawa Timur.

---

**Selamat menggunakan Dashboard Prakiraan Cuaca Jombang! 🌤️**
