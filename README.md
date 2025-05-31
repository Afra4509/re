# NutriTrack | Deteksi Dini Stunting 🌱

[![Shiny](https://img.shields.io/badge/Shiny-Dashboard-blue)](https://nutritrack.shinyapps.io/nutritrack/)
[![R](https://img.shields.io/badge/R-4.0%2B-blue)](https://www.r-project.org/)


NutriTrack adalah aplikasi web interaktif berbasis R Shiny yang dirancang untuk memantau pertumbuhan anak dan mencegah stunting di Indonesia. Aplikasi ini menyediakan tools untuk kalkulasi status gizi, rekomendasi nutrisi, dan visualisasi data stunting berdasarkan standar WHO.

## 🚀 Demo Aplikasi

**🌐 Akses Langsung:** [https://nutritrack.shinyapps.io/nutritrack/](https://nutritrack.shinyapps.io/nutritrack/)

## ✨ Fitur Utama

### 1. 📊 Kalkulator Status Gizi
- Analisis status gizi anak berdasarkan standar WHO Growth Standards
- Input data: nama, usia (bulan), jenis kelamin, dan tinggi badan
- Perhitungan Z-Score untuk tinggi badan menurut umur (TB/U)
- Klasifikasi: Normal, Stunting, atau Stunting Berat
- Visualisasi kurva pertumbuhan interaktif

### 2. 🍎 Rekomendasi Gizi
- Panduan gizi berdasarkan kelompok usia:
  - **0-6 bulan**: ASI Eksklusif
  - **6-12 bulan**: ASI + MPASI
  - **1-3 tahun**: Makanan keluarga bervariasi
  - **3-5 tahun**: Pola makan teratur
- Tips responsive feeding dan menu seimbang
- Informasi makanan pencegah stunting

### 3. 🗺️ Data Stunting Indonesia
- Visualisasi prevalensi stunting per provinsi
- Data terbaru tahun 2023 dari Kementerian Kesehatan RI
- Grafik interaktif dan tabel data yang dapat diunduh
- Analisis tren dan rekomendasi kebijakan

### 4. ℹ️ Informasi Edukasi
- Penjelasan tentang stunting dan dampaknya
- Panduan pengukuran yang benar
- Informasi tim pengembang dan teknologi

## 🛠️ Teknologi Yang Digunakan

- **R (4.0+)**: Bahasa pemrograman untuk komputasi statistik
- **Shiny**: Framework untuk aplikasi web interaktif
- **shinydashboard**: Framework dashboard untuk Shiny
- **ggplot2**: Package visualisasi data
- **plotly**: Library grafik interaktif
- **dplyr**: Package manipulasi data
- **shinyWidgets**: Komponen UI tambahan
- **shinycssloaders**: Animasi loading
- **DT**: Tabel data interaktif

## 📋 Prasyarat

Pastikan Anda memiliki:
- R versi 4.0 atau lebih baru
- RStudio (opsional, tapi direkomendasikan)
- Koneksi internet untuk mengunduh packages

## 🔧 Instalasi

### 1. Clone Repository
```bash
git clone https://github.com/njwandyna/nutritrack.git
cd nutritrack
```

### 2. Install Required Packages
```R
# Install required packages
install.packages(c(
  "shiny",
  "ggplot2", 
  "dplyr",
  "shinydashboard",
  "plotly",
  "shinyWidgets",
  "shinycssloaders",
  "DT"
))
```

### 3. Jalankan Aplikasi
```R
# Buka R/RStudio dan jalankan:
shiny::runApp()

# Atau jika menggunakan RStudio, buka file app.R dan klik "Run App"
```

## 📱 Cara Penggunaan

### Kalkulator Status Gizi
1. **Masukkan Data Anak**:
   - Nama anak
   - Usia dalam bulan (contoh: 12 untuk anak 1 tahun)
   - Pilih jenis kelamin
   - Tinggi badan dalam cm

2. **Klik "Analisis Status Gizi"**
   - Aplikasi akan menghitung Z-Score berdasarkan standar WHO
   - Hasil akan menampilkan status gizi dan rekomendasi

3. **Interpretasi Hasil**:
   - **Normal**: Z-Score ≥ -2 (pertumbuhan baik)
   - **Stunting**: -3 ≤ Z-Score < -2 (perlu perhatian)
   - **Stunting Berat**: Z-Score < -3 (perlu penanganan segera)

### Rekomendasi Gizi
- Pilih tab sesuai usia anak
- Ikuti panduan menu dan tips yang diberikan
- Terapkan prinsip responsive feeding

### Data Stunting Indonesia
- Jelajahi data prevalensi per provinsi
- Gunakan filter untuk mengurutkan data
- Unduh data untuk analisis lebih lanjut

## 📊 Sumber Data

- **Standar Pertumbuhan**: [WHO Child Growth Standards](https://www.who.int/tools/child-growth-standards)
- **Data Stunting Indonesia**: [Dashboard Prevalensi Stunting - Kemendagri](https://konvergensi.bangda.kemendagri.go.id/emonev/DashPrev/index/4)
- **Referensi Gizi**: Kementerian Kesehatan Republik Indonesia

## 🏗️ Struktur Project

```
nutritrack/
├── app.R                 # Main application file
├── www/                  # Static assets
│   ├── custom.css       # Custom styling  
│   └── logo_saya.png    # Application logo
├── data/                # Data files (if any)
└── README.md           # This file
```

## 🤝 Kontribusi

Kami menyambut kontribusi dari komunitas! Jika Anda ingin berkontribusi:

1. Fork repository ini
2. Buat branch feature (`git checkout -b feature/AmazingFeature`)
3. Commit perubahan (`git commit -m 'Add some AmazingFeature'`)
4. Push ke branch (`git push origin feature/AmazingFeature`)
5. Buat Pull Request

## 📝 Roadmap

- [ ] Integrasi dengan API data real-time
- [ ] Fitur tracking pertumbuhan berkala
- [ ] Notifikasi dan reminder
- [ ] Export laporan PDF
- [ ] Multi-language support
- [ ] Mobile app version

## 🐛 Melaporkan Bug

Jika Anda menemukan bug atau memiliki saran, silakan buat [issue baru](https://github.com/njwandyna/nutritrack/issues) dengan detail:
- Deskripsi masalah
- Langkah-langkah untuk reproduce
- Screenshot (jika diperlukan)
- Informasi sistem (OS, browser, versi R)

## 📞 Kontak & Support

- **Repository**: [https://github.com/njwandyna/nutritrack](https://github.com/njwandyna/nutritrack)
- **Live Demo**: [https://nutritrack.shinyapps.io/nutritrack/](https://nutritrack.shinyapps.io/nutritrack/)
- **Issues**: [GitHub Issues](https://github.com/njwandyna/nutritrack/issues)


## 🙏 Acknowledgments

- [World Health Organization (WHO)](https://www.who.int/) untuk standar pertumbuhan anak
- [Kementerian Kesehatan RI](https://www.kemkes.go.id/) untuk data stunting Indonesia
- [Kementerian Dalam Negeri RI](https://www.kemendagri.go.id/) untuk dashboard data stunting
- [R Shiny Community](https://shiny.rstudio.com/) untuk dokumentasi dan tutorial

---


