# 🎓 Oneformatic

<div align="center">

  ![Oneformatic Banner](https://img.shields.io/badge/Status-Production-success?style=for-the-badge)
  ![Oneformatic Data](https://img.shields.io/badge/Data-Supabase-green?style=for-the-badge)
  ![Oneformatic Framework](https://img.shields.io/badge/Framework-Next.js_14-black?style=for-the-badge)

  **Platform Manajemen Kelas Digital Terintegrasi untuk Siswa SMK**
  
  [Lihat Demo](https://oneformatic.vercel.app/) · [Laporkan Bug](#) · [Request Fitur](#)
</div>

---

## 📖 Tentang Project

**Oneformatic** adalah aplikasi manajemen kelas "All-in-One" yang dirancang khusus untuk memenuhi kebutuhan administrasi dan sosial siswa kelas **X TKJ 1**. Platform ini menjembatani kebutuhan akademik yang kaku dengan interaksi sosial siswa yang dinamis, menciptakan ekosistem digital yang tidak hanya fungsional tapi juga menyenangkan.

Dibangun dengan teknologi web modern, Oneformatic menawarkan pengalaman pengguna yang cepat, responsif, dan real-time.

---

## ⚡ Tech Stack

Project ini dibangun menggunakan teknologi mutakhir untuk performa maksimal:

| Kategori | Teknologi | Deskripsi |
| :--- | :--- | :--- |
| **Framework** | ![Next JS](https://img.shields.io/badge/Next-black?style=flat-square&logo=next.js&logoColor=white) | App Router, Server Components |
| **Language** | ![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white) | Standar ketat untuk kode yang aman |
| **Styling** | ![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white) | Utility-first CSS framework |
| **UI Library** | ![Radix UI](https://img.shields.io/badge/Radix_UI-161618?style=flat-square&logo=radix-ui&logoColor=white) | Headless UI components (via Shadcn/UI) |
| **Database** | ![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white) | PostgreSQL, Auth, Realtime, Storage |
| **Animation** | ![Framer Motion](https://img.shields.io/badge/Framer_Motion-black?style=flat-square&logo=framer&logoColor=white) | Smooth layout transitions |

---

## ✨ Fitur Unggulan

Oneformatic membagi fiturnya menjadi dua pilar utama:

### 🛠️ Produktivitas & Akademik
> *Membantu siswa tetap terorganisir dan disiplin sesuai standar sekolah.*

- 📅 **Jadwal Pelajaran Interaktif**: Tampilan jadwal yang responsif dengan detail guru, jam, dan ruang.
- 🧹 **Monitoring Piket**: Daftat petugas piket harian yang selalu terupdate.
- 📝 **Tugas & PR Tracker**: List tugas dengan status pengerjaan (Pending/Selesai).
- 📊 **Monitoring Absensi**: Integrasi data absensi siswa dengan rekap otomatis.
- 👥 **Direktori Siswa**: Profil lengkap seluruh siswa dengan fitur pencarian cepat.
- 📋 **Jurnal Kelas**: Catatan harian aktivitas kelas.

### 🎉 Life & Social (New Features!)
> *Membangun kebersamaan dan keseruan antar warga kelas.*

- **💰 Transparansi Kas**: Dashboard keuangan kelas yang transparan (Debit/Kredit).
- **💬 Class Wall**: "Sosmed" mini kelas untuk berbagi pesan dan pengumuman santai.
- **🏆 Leaderboard**: Ranking seru-seruan (Ter-rajin, Ter-lucu, dll) based on voting.
- **📝 Quote of the Day**: Widget kata bijak harian dari siswa (dengan sistem approval Admin).
- **🎵 Class Playlist**: Playlist kolaboratif! Tambahkan lagu favorit dari YouTube/Spotify.
- **👻 Anonymous Confession**: Kirim pesan rahasia/curhat tanpa nama (Aman & Filtered).

---

## 🚀 Update Log (18 Januari 2026)

Fokus utama update ini adalah optimalisasi manajemen pengguna dan perbaikan sistem inti.

### 🌟 New Features
1.  **Bulk User Generation (Mass Account Creation)**
    *   **Masalah**: Membuat akun satu per satu untuk 36 siswa sangat memakan waktu.
    *   **Solusi One-Click**: Admin cukup menekan satu tombol "Generate Akun Siswa" di dashboard.
    *   **Algoritma Cerdas**: Sistem otomatis mendeteksi siswa yang belum punya akun, lalu membuatkannya kredensial (Email: `{absen}@tkj.pal`, Pass: `{absen}123`).
    *   **Auto-Link Profile**: Akun yang dibuat langsung terhubung dengan data profil dan biodata siswa.
    
2.  **Sistem Absensi v2 (Refined)**
    *   **Flow Absensi Modern**:
        *   **Buka Sesi**: Pengurus/Guru membuka sesi absensi harian (07:00 - 15:00).
        *   **Self Check-in**: Siswa melakukan absen mandiri via dashboard masing-masing.
        *   **Monitor Real-time**: Admin memantau siapa yang sudah/belum absen secara live.
        *   **Tutup Sesi**: Tombol "Tutup Sesi" baru untuk mengakhiri absensi hari itu tanpa menghapus data sejarah.
    *   **Fitur Keamanan & Integritas**:
        *   **Role-Based Access**: Hanya siswa terdaftar yang bisa absen. Tamu/Guest blocked.
        *   **Duplicate Prevention**: Mencegah double-input untuk satu hari yang sama.
        *   **Data Consistency**: Perbaikan relasi database (FK Constraints) agar data tetap aman meski ada perubahan struktur.

3.  **User Interface & Navigation (Revamped)**
    *   **Logical Grouping**: Menu navigasi tidak lagi berantakan, tapi dikelompokkan:
        *   **Utama**: Dashboard & Profil.
        *   **Akademik**: Mapel, Materi, Tugas, Forum, Prestasi.
        *   **Kelas**: Piket, Event, Kas, Absensi.
        *   **Tools**: Cheat Sheet & Network Utilities.
    *   **Clear Terminology**: Perubahan nama fitur agar lebih mudah dimengerti (Contoh: "Materi" -> "Bank Materi").

4.  **Security & Profile**
    *   **Change Password**: Siswa kini bisa mengubah password default mereka via halaman Profil.

---

## 🚀 Update Log (16 Januari 2026)

Pembaruan masif dilakukan untuk meningkatkan interaktivitas dan manajemen data.

### 🌟 Major Updates
1.  **Ekosistem Dashboard Admin Baru**
    *   Navigasi sidebar khusus admin untuk kelola **Kas**, **Quotes**, **Confession**, dan **Leaderboard**.
    *   Sistem **Approval Queue** untuk Quotes & Confession (Mencegah spam/konten tidak layak).
    
2.  **Playlist Next-Gen**
    *   **Smart Thumbnail**: Otomatis mengambil cover art dari link YouTube/Video.
    *   **Platform Detection**: Mendeteksi dan menampilkan logo platform (Spotify/YouTube/SoundCloud).

3.  **Sistem Leaderboard**
    *   Admin dapat membuat kategori ranking custom dengan selector Emoji 🏆.
    *   Sistem voting real-time oleh siswa.

### 🔧 Improvements & Fixes
*   **Data Integrity**: Merubah istilah **"NIS"** menjadi **"Nomor Absen"** di seluruh sistem agar sesuai konteks kelas.
*   **Smart Sorting**: Semua list siswa kini diurutkan berdasarkan **Nomor Absen** (1-36) secara otomatis.
*   **Realtime Engine**: Perbaikan bug pada submission Quotes/Confession agar data muncul instan tanpa refresh page.
*   **Logic Fix**: Dashboard Count kini pintar membedakan "Mapel Akademik" vs "Kegiatan Non-Akademik" (seperti Upacara/Istirahat).

---

<div align="center">
  <p>Dibuat dengan ❤️ untuk Kelas X TKJ 1</p>
  <p>&copy; 2026 Oneformatic Team</p>
</div>
