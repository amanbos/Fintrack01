# 💰 FinTrack — Keuangan Pribadi

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Android-3DDC84?style=for-the-badge&logo=android&logoColor=white"/>
  <img src="https://img.shields.io/badge/Min%20SDK-21%20(Android%205.0)-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Language-Java-orange?style=for-the-badge&logo=java"/>
</p>

<p align="center">
  Aplikasi pencatat keuangan pribadi berbasis Android — gratis, offline, dan simpel.
</p>

---

## 📲 Download APK

> **Download langsung tanpa perlu build sendiri:**

➡️ Pergi ke tab **[Releases](../../releases/latest)** → download `app-debug.apk`

Atau dari tab **[Actions](../../actions)** → pilih build terbaru → download artifact `FinTrack-debug-apk`

---

## ✨ Fitur Aplikasi

| Fitur | Keterangan |
|-------|-----------|
| 📊 Dashboard | Ringkasan saldo, pemasukan & pengeluaran bulan ini |
| 💳 Multi Rekening | Kelola beberapa akun (tunai, bank, e-wallet) |
| 📝 Transaksi | Catat pemasukan, pengeluaran, dan transfer |
| 🎯 Anggaran | Atur batas pengeluaran per kategori |
| 🏆 Tujuan Tabungan | Pantau progress target keuangan |
| 📈 Grafik | Visualisasi keuangan bulanan |
| 📤 Export CSV | Export data ke file CSV |
| 🌙 Dark Mode | Tampilan gelap elegan |
| 📱 Offline | Semua data tersimpan di HP, tidak butuh internet |

---

## 🚀 Cara Build Sendiri

### Prasyarat
- [Android Studio](https://developer.android.com/studio) (versi terbaru)
- JDK 17+

### Langkah-langkah

```bash
# 1. Clone repository ini
git clone https://github.com/USERNAME/FinTrack.git

# 2. Masuk ke folder project
cd FinTrack

# 3. Build APK via command line
./gradlew assembleDebug

# 4. APK siap di:
# app/build/outputs/apk/debug/app-debug.apk
```

Atau buka di **Android Studio** → **Build → Build APK(s)**

---

## 🤖 Build Otomatis (GitHub Actions)

Setiap kali ada **push ke branch `main`**, GitHub akan otomatis:

1. ✅ Build APK debug
2. ✅ Upload APK ke **Releases** dengan tag versi baru
3. ✅ APK bisa langsung didownload dari halaman Releases

Lihat workflow di: [`.github/workflows/build-apk.yml`](.github/workflows/build-apk.yml)

---

## 📁 Struktur Project

```
FinTrack/
├── .github/
│   └── workflows/
│       └── build-apk.yml       ← GitHub Actions (build otomatis)
├── app/
│   └── src/main/
│       ├── AndroidManifest.xml
│       ├── assets/
│       │   └── index.html      ← Aplikasi HTML/CSS/JS
│       ├── java/com/fintrack/app/
│       │   └── MainActivity.java
│       └── res/
│           ├── layout/
│           ├── values/
│           └── mipmap-*/       ← Icon launcher
├── gradle/wrapper/
├── build.gradle
├── settings.gradle
└── gradlew
```

---

## 🛠️ Tech Stack

- **Frontend**: HTML5, CSS3, JavaScript (Vanilla)
- **Charting**: Chart.js 4.4
- **Storage**: localStorage (WebView)
- **Android**: WebView wrapper (Java)
- **Build**: Gradle 8.4

---

## 📋 Spesifikasi

| Item | Nilai |
|------|-------|
| Package | `com.fintrack.app` |
| Min Android | 5.0 (API 21) |
| Target Android | 14 (API 34) |
| Orientasi | Portrait |
| Ukuran APK | ~3-5 MB |

---

<p align="center">Dibuat dengan ❤️ menggunakan HTML + Android WebView</p>
