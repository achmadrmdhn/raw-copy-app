# RAW Copy App

**RAW Copy App** adalah aplikasi web ringan untuk **menemukan, menyalin, atau memindahkan file RAW** dari folder lokal berdasarkan **nama file** atau **3–4 digit terakhir**. Cocok untuk alur kerja fotografi (wedding, wisuda dan event), maupun pengelolaan file lainnya.

> **Alur singkat:** Pilih Folder → Masukkan Daftar File → Salin/Pindah → Selesai.

---

## Daftar Isi

- [RAW Copy App](#raw-copy-app)
  - [Daftar Isi](#daftar-isi)
  - [Link Aplikasi](#link-aplikasi)
  - [Ringkasan](#ringkasan)
  - [Fitur Utama](#fitur-utama)
  - [Untuk Siapa?](#untuk-siapa)
  - [Cara Kerja (Singkat)](#cara-kerja-singkat)
  - [Cara Menggunakan](#cara-menggunakan)
  - [Format Input Nama File](#format-input-nama-file)
  - [Ekstensi RAW yang Didukung](#ekstensi-raw-yang-didukung)
  - [Kompatibilitas Browser](#kompatibilitas-browser)
  - [Keamanan \& Privasi](#keamanan--privasi)
  - [Profil Pembuat](#profil-pembuat)

---

## Link Aplikasi

- **Production URL:** <https://raw-copy-app.vercel.app/>
---

## Ringkasan

Aplikasi memanfaatkan **File System Access API** sehingga dapat membaca/menulis langsung ke **folder lokal** Anda **tanpa unggah** ke server. Pengguna memilih folder sumber & tujuan, memasukkan daftar nama atau digit akhir file, lalu menjalankan **Salin** atau **Pindah** dengan progress dan hasil yang jelas.

---

## Fitur Utama

- **Pilih Folder Sumber & Tujuan** (lokal; tanpa upload).
- **Mode Rekursif** (opsional) untuk memindai subfolder.
- **Filter Ekstensi RAW** (Sony/Canon/Nikon, dst) + opsi **Custom…**.
- Input fleksibel: **nama file** (dengan/tanpa ekstensi) atau **3–4 digit terakhir**.
- **Salin** atau **Pindah**.
- **Progress bar**, status real-time, daftar **Berhasil/Gagal**, dengan alert.
- **UI modern** (Tailwind), responsif, **light/dark mode** (ungu sebagai brand).

---

## Untuk Siapa?

- **Fotografer** (wedding, wisuda, event, komersial).
- **Editor/Studio** yang memilah file dari banyak sesi.
- **Siapa pun** yang ingin mengelola file berdasarkan pola nama/angka secara cepat.

---

## Cara Kerja (Singkat)

1. Browser meminta Anda **memilih folder** (akses terbatas via File System Access API).
2. Aplikasi memindai isi folder (dan subfolder jika **Rekursif** aktif).
3. Aplikasi mencocokkan input Anda (nama/3–4 digit akhir) dengan file yang ditemukan.
4. File yang cocok **disalin** atau **dipindahkan** ke folder tujuan.

> Semua proses berlangsung **lokal** di perangkat Anda.

---

## Cara Menggunakan

1. **Buka aplikasi**.
2. **Folder Sumber** → pilih folder berisi file RAW.
3. **Folder Tujuan** → pilih folder penyimpanan hasil.
4. (Opsional) Aktifkan **Rekursif** jika sumber punya subfolder.
5. Pilih **Ekstensi RAW** yang relevan, atau gunakan **Custom…**.
6. Tempel daftar **nama file** atau **3–4 digit terakhir** (satu baris per entri).
7. Klik **Mulai Salin** atau **Mulai Pindah**.
8. Pantau **progress** dan cek daftar **Berhasil/Gagal**. Aplikasi akan menampilkan **alert** saat selesai.

> Tombol **Bersihkan** mengosongkan input & hasil.

---

## Format Input Nama File

- **Satu entri per baris**.
- Contoh valid:
  - Nama tanpa ekstensi: `DSC0217`
  - Nama lengkap: `DSC0217.ARW`
  - 3–4 digit terakhir: `2153` atau `0217`
- **Penomoran/bullet di awal baris diabaikan otomatis**, mis.:
  - `1. 2153` → `2153`
  - `2) DSC0217` → `DSC0217`
  - `- IMG_4521` → `IMG_4521`

> Pencocokan digit akhir mencari angka pada **bagian akhir nama file** (mis. `DSC0217.ARW` cocok dengan `217` atau `0217`).

---

## Ekstensi RAW yang Didukung

**Umum:** `.ARW`, `.CR2`, `.CR3`, `.NEF`, `.RAF`, `.RW2`, `.ORF`, `.PEF`, `.DNG`  
**Custom…:** masukkan ekstensi lain secara manual (mis. `.SR2`)

---

## Kompatibilitas Browser

- **Direkomendasikan:** Browser berbasis **Chromium** (Chrome, Edge, Brave, Opera).
- **Terbatas/eksperimental:** Firefox & Safari (dukungan File System Access API belum setara).
- **Wajib HTTPS** untuk produksi (mis. **Vercel** sudah HTTPS by default).

---

## Keamanan & Privasi

- Akses file **hanya** pada folder yang Anda pilih (scoped).
- Izin dapat **ditolak** atau **dicabut** kapan saja.
- Proses berjalan **lokal**; aplikasi **tidak mengunggah** file.
- Gunakan pada perangkat & jaringan tepercaya.

---

## Profil Pembuat

**Nama:** Achmad Rifa'i Ramadhan

- 📸 **Instagram:** <https://www.instagram.com/rifairmdhnn_/>  
- 💼 **LinkedIn:** <https://www.linkedin.com/in/achmadrifairamadhan/>  
- 💻 **GitHub:** <https://github.com/achmadrmdhn/>  

> Ingin kolaborasi atau ada masukan? Silakan hubungi saya.
