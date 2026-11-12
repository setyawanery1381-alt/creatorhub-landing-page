# Product Requirements Document (PRD)
## Digital Product Access Hub & Reseller Vault

---

### 1. Judul dan Ringkasan Eksekutif
* **Nama Proyek:** Digital Product Access Hub & Reseller Vault (*Web App Portofolio & Direktori Akses Produk Digital*)
* **Versi:** 1.0.0
* **Platform:** Google Apps Script (GAS) Web App + Google Sheets
* **Status Lisensi:** **100% Hak Jual Kembali (PLR / MRR)**
* **Ringkasan:**  
  Aplikasi web satu halaman (*All-in-One Access Hub*) yang berfungsi sebagai etalase dan pintu akses terpusat bagi seluruh paket produk digital (15.000+ Worksheet Anak, 20 Games Edukasi, Paket Coding, E-Book, Template Canva, hingga Mega Bundling). Siapa pun yang membeli paket dapat langsung membuka dan mengunduh seluruh materi tanpa alur pembayaran manual, serta memiliki izin penuh untuk menjual kembali produk-produk tersebut (*Resell Rights*).

---

### 2. Daftar 10 Produk Digital & Tautan Akses

Seluruh produk di bawah ini sudah terintegrasi ke dalam sistem dan memiliki **100% Hak Jual Kembali**:

| No | Nama Produk Digital | Kategori | Jenis Akses / URL Target | Hak Lisensi |
| :-: | :--- | :--- | :--- | :---: |
| 1 | **Promo Paket Mega Bundling** | Mega Bundle | `https://www.digitalprodukno1seindonesia.my.id/` | 100% Hak Jual |
| 2 | **Pro Growth Bundle Landing Page** | Template Toko | `https://sangcreator.my.canva.site/c3wht4nzam1rpg0r` | 100% Hak Jual |
| 3 | **Paket Super Hemat 9 E-Book** | E-Book | `https://sites.google.com/view/paket-ebook-sangcreator/halaman-muka` | 100% Hak Jual |
| 4 | **Paket 3 Coding** | Aplikasi & Coding | `https://sites.google.com/view/codinglevel1-3sangcreator/halaman-muka` | 100% Hak Jual |
| 5 | **Paket 15000++ Worksheet Anak** | Worksheet Anak | `https://drive.google.com/drive/folders/1BNRtr4nRGlQxtGUMX4YrWA5rFZ2TrEL2` | 100% Hak Jual |
| 6 | **20 Games Edukasi Anak** | Games Edukasi | `https://sites.google.com/view/game-edukasi-2` | 100% Hak Jual |
| 7 | **10 Games Edukasi Anak Muslim** | Games Edukasi | `https://sites.google.com/view/gameedukasianakmuslim` | 100% Hak Jual |
| 8 | **39000++ Media Anak Kreatif** | Media Kreatif | `https://drive.google.com/drive/folders/1xsQ7LMcDhzeIsjdnAJ3XbKW8IO72G8ue?usp=drive_link` | 100% Hak Jual |
| 9 | **1000++ Worksheet Islami** | Worksheet Anak | `https://drive.google.com/drive/folders/1B9k8lSlHZXhrmegfGKj8arpWZxiZ4sPN?usp=sharing` | 100% Hak Jual |
| 10 | **Games Edukasi 8 Seri** | Games Edukasi | `https://sites.google.com/view/landingpagesangcreator/halaman-muka` | 100% Hak Jual |
| 11 | **WA Grup Komunitas & Reseller** | Komunitas | `https://wa.me/6281331661370` | Support Reseller |
| 12 | **Cover & Banner Promosi (Bahan Iklan)**| Aset Promosi | `https://drive.google.com` | Siap Pakai |

---

### 3. Arsitektur Data Google Sheets

Data produk dikelola dinamis di Google Sheets:

**Sheet 1: `Katalog_Produk`**
* Kolom: `ID_Produk` | `Urutan` | `Judul` | `Kategori` | `Icon_Type` | `Warna_Icon` | `URL_Tujuan` | `Deskripsi_Singkat` | `Status_Aktif`

**Sheet 2: `Pengaturan_Web`**
* Kolom: `Parameter` | `Nilai` | `Keterangan`
* Parameter: `Judul_Header`, `Sub_Header`, `Badge_Header`, `Nomor_WA_Admin`, `Pesan_WA`.

---

### 4. Rancangan Tampilan UI/UX
* **Latar Belakang:** Gradien hijau zamrud gelap melandai ke kuning keemasan (`linear-gradient(145deg, #013827, #064e3b, #3f5509, #9e7d05)`).
* **Header:** Melengkung di bawah dengan list aksen emas tipis, judul bold "DIGITAL PRODUK", slogan "Pelopor Produk Digital No 1", dan kapsul oranye "100% Bisa Dijual Kembali".
* **Kartu Produk:** Kartu putih membulat dengan ikon lingkaran warna-warni, judul produk, dan badge hijau "100% Hak Jual".
* **Fitur Tambahan:** Filter kategori instan, pencarian cepat, tombol WhatsApp floating untuk konsultasi.

---

### 5. Cara Pasang di Google Apps Script

1. Buat Google Spreadsheet baru di Google Drive (misal beri nama: `Database Produk Digital`).
2. Klik menu **Extensions** (Ekstensi) > **Apps Script**.
3. Buat file `Code.gs` dan salin kode dari [`Code.gs`](file:///c:/Users/Saka%20Farma/.gemini/antigravity-ide\scratch\aplikasi%20-landingpage-prodig\Code.gs).
4. Buat file HTML bernama `Index.html` dan salin kode dari [`Index.html`](file:///c:/Users/Saka%20Farma/.gemini/antigravity-ide\scratch\aplikasi%20-landingpage-prodig\Index.html).
5. Pada menu drop-down fungsi di atas, pilih **`setupDatabase`** lalu klik tombol **Run** (Jalankan) dan izinkan hak akses (*Review Permissions*).
6. Buka kembali Google Sheet Anda; sheet `Katalog_Produk` dan `Pengaturan_Web` otomatis terisi dengan 10 produk di atas!
7. Di Apps Script, klik tombol biru **Deploy** > **New deployment**:
   - Pilih jenis: **Web app**
   - Description: `Versi 1.0 Real`
   - Execute as: `Me`
   - Who has access: `Anyone`
8. Klik **Deploy** dan salin URL Web App yang dihasilkan. Web siap disebarkan ke pembeli atau disematkan di domain kustom!

---

🎨 **Langkah Berikutnya: Menentukan Tampilan**
1. Sudah punya referensi? Unggah tangkapan layar, warna, dan gaya antarmuka yang Anda inginkan.
2. Belum punya referensi?
   - Salin seluruh teks PRD Final di atas.
   - Buka Google Stitch dan tempel teksnya.
   - Unduh pratinjau desain yang dihasilkan.
   - Unggah gambarnya ke percakapan ini supaya bisa diterapkan ke kode HTML dan CSS.
