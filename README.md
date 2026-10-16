# Google Office App 🚀

Aplikasi Flutter untuk menampilkan daftar kantor Google di seluruh dunia beserta informasi detailnya. Proyek ini dibangun sebagai **Proyek Akhir (Submission)** untuk kelas Flutter Pemula.

---

## Features ✨
- **Responsive Layout:** Tampilan otomatis berubah menjadi **GridView** di layar lebar (>700px) seperti Desktop/Web, dan menjadi **ListView** di layar HP (≤700px).
- **Search System:** Fitur pencarian dinamis berdasarkan nama atau alamat kantor menggunakan `setState`.
- **Advanced Navigation:** Perpindah halaman menggunakan pengiriman data `googleOfficeId` melalui *initializer list* disertai animasi transisi slide dari bawah ke atas.

---

## Panduan Menjalankan Aplikasi 🛠️

Ikuti langkah-langkah di bawah ini untuk menjalankan proyek ini di komputer lokal Anda menggunakan **VS Code**.

### 1. Prasyarat (Prerequisites)
Pastikan Anda sudah memasang komponen berikut di komputer Anda:
- [Flutter SDK](https://flutter.dev) (Versi terbaru direkomendasikan)
- [Visual Studio Code](https://visualstudio.com)
- Ekstensi **Flutter** dan **Dart** di VS Code
- Android Emulator, iOS Simulator, atau Google Chrome yang siap digunakan

### 2. Persiapan Proyek (Setup)
1. Clone repositori ini atau unduh berkas ZIP-nya:
   ```bash
   git clone https://github.com/putraharifin/google_office_app.git 
   ```
2. Buka folder proyek menggunakan **VS Code**.
3. Buka **Terminal** di VS Code, lalu unduh semua *dependencies* / *packages* yang diperlukan dengan mengetik perintah:
   ```bash
   flutter pub get
   ```

### 3. Menjalankan Aplikasi (Run App)
1. Hubungkan HP fisik Anda atau nyalakan **Emulator Android / iOS Simulator**.
2. Perhatikan pojok kanan bawah VS Code, pastikan perangkat target Anda sudah terpilih (misalnya: `Pixel 9 Pro` atau `iPhone Simulator`). Jika belum sesuai, klik area tersebut dan pilih perangkat yang aktif.
3. Buka berkas `lib/main.dart`.
4. Tekan tombol **F5** pada *keyboard* Anda (atau klik menu **Run > Start Debugging** di bagian atas VS Code).
5. Tunggu proses kompilasi (*Gradle task* atau *Xcode build*) selesai. Aplikasi akan otomatis terbuka di perangkat Anda.

---

## Mengatasi Masalah Gambar Tidak Muncul (Khusus macOS Desktop) 🖥️
Jika Anda menjalankan aplikasi ini sebagai aplikasi **macOS Desktop** dan gambar internet tidak muncul, pastikan izin jaringan sudah diaktifkan di berkas konfigurasi macOS:
1. Buka berkas `macos/Runner/DebugProfile.entitlements` dan `macos/Runner/Release.entitlements`.
2. Pastikan atau tambahkan baris berikut di dalam tag `<dict>`:
   ```xml
   <key>com.apple.security.network.client</key>
   <true/>
   ```
3. Hentikan aplikasi, lalu jalankan ulang (`F5`).
