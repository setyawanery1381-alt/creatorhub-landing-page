# Ringkasan Desain & Design System Blueprint
## Digital Product Access Hub & Reseller Vault

Dokumen ini merangkum sistem desain terukur hasil bedah gambar referensi (*Vision Fusion*) serta pemetaan halaman untuk Google Stitch AI.

---

### 0. Design System Blueprint (Hasil Bedah Gambar Referensi)

#### 1. Karakter & Gaya Desain (UI Style)
* **Kategori Gaya:** *Vibrant Modern Card Grid Hub* (Kombinasi Bento Grid & Link Hub Modern dengan kontras tinggi).
* **Kesan Umum:** Segar, profesional, prestisius, terorganisir rapi, dan memberikan rasa aman bahwa seluruh produk memiliki izin komersial (*100% Hak Jual*).
* **Target Pengguna:** Pengunjung umum, orang tua murid, guru, pembeli materi digital, serta reseller/pebisnis online.

#### 2. Palet Warna & Token (HEX & Tailwind)
| Token Desain | Kode HEX | Padanan Class Tailwind | Peran & Penggunaan |
| :--- | :--- | :--- | :--- |
| **Primary Background (Gradient Start)** | `#013827` | `from-[#013827]` | Sudut kiri-atas, hijau zamrud pekat / deep pine |
| **Primary Background (Gradient Mid)** | `#064e3b` | `via-emerald-900` | Area tengah layar |
| **Primary Background (Gradient End)** | `#9e7d05` | `to-amber-600` | Sudut kanan-bawah, aksen amber keemasan |
| **Header Surface** | `rgba(1, 41, 29, 0.75)` | `bg-[#01291d]/75` | Latar panel melengkung atas dengan blur |
| **Header Gold Accent Border** | `#EAB308` | `border-amber-500` | Garis batas bawah melengkung pada header |
| **Surface Card** | `#FFFFFF` | `bg-white` | Kartu produk utama |
| **Card Text Primary** | `#1E293B` | `text-slate-800` | Judul produk (sangat kontras dan tebal) |
| **Card Text Secondary** | `#64748B` | `text-slate-500` | Deskripsi atau metadata |
| **Reseller Badge (Gradient)** | `#EA580C` - `#F97316` | `from-orange-600 to-orange-500` | Kapsul status "100% Bisa Dijual Kembali" |
| **License Tag Pill** | `#ECFDF5` / `#047857` | `bg-emerald-50 text-emerald-700` | Label mikro "100% Hak Jual" di tiap kartu |
| **WhatsApp Accent** | `#10B981` / `#059669` | `bg-emerald-500` | Tombol mengambang bantuan cepat |

#### 3. Tipografi & Hierarki
* **Font Family:** `Poppins` (Display/Headings/Card Titles) dan `Inter` (Body/Pencarian/Metadata).
* **H1 (Header Title):** 32px – 38px, `font-black`, uppercase, tracking-wider, warna putih dengan drop-shadow lembut.
* **Tagline:** 12px – 14px, `font-semibold`, warna `#FEF08A` (light gold).
* **Judul Kartu:** 12px – 14px, `font-bold`, leading-tight, warna `#1E293B`.
* **Badge / Label:** 9px – 11px, `font-extrabold`, letter-spacing 0.05em.

#### 4. Struktur Layout & Navigasi
* **Header:** Melengkung di bagian bawah (*curved bottom* `rounded-b-[2.25rem]`), berbatas garis emas 2px.
* **Navigasi & Pencarian:** Bilah pencarian instan transparan (*glassmorphism*) dan chip filter kategori mendatar (*horizontal swipe*).
* **Grid Produk:** 
  - Desktop/Tablet: Grid 3 kolom terpusat (*max-w-2xl* atau *max-w-3xl*, gap 16px).
  - Mobile: Grid 2 kolom rapat (*gap 10px – 12px*), ramah navigasi satu tangan (*thumb-friendly*).
* **Floating Action:** Tombol WhatsApp mengambang di pojok kanan bawah dengan titik indikator berdenyut (*pulsing animation*).

#### 5. Bedah Komponen Detail
* **Kartu Produk (*Product Card*):**
  - Bentuk: Persegi panjang vertikal dengan sudut membulat `rounded-2xl` (16px – 20px).
  - Latar: Putih solid `#FFFFFF`, bayangan `shadow-md` hingga `shadow-xl`.
  - Ikon: Berada di bulatan lingkaran tengah atas berdiameter 48px – 52px dengan warna kategori berbeda-beda (Ungu, Toska, Oranye, Pink, Biru, Hijau, Merah).
  - Teks: Judul tebal di bawah ikon, terpotong rapi maksimal 2 baris (*line-clamp-2*).
  - Tag Status: Kapsul hijau muda di dasar kartu bertuliskan *"100% Hak Jual"*.
* **Modal Akses Produk:**
  - Jendela sembulan membulat (*rounded-3xl*) dengan latar belakang gelap blur (*backdrop-blur-sm*).
  - Rincian format berkas, tombol unduh Google Drive hijau besar, dan tombol salin tautan.

#### 6. Detail Visual & Interaksi
* **Mikro-Interaksi:** Kartu terangkat naik 5px saat di-*hover* (`transform: translateY(-5px)`), ikon berputar halus 5 derajat, dan efek tekan membal saat diklik (*active scale 0.96*).
* **Radius Sudut:** 20px untuk kartu, 9999px (pill) untuk seluruh tombol dan badge.
* **Library Ikon:** Lucide Icons (stroke 2.2).

#### 7. Ringkasan Blueprint
> Seluruh halaman mewarisi gaya identik: Latar gradien hijau botol mendalam melandai ke amber emas, kartu putih bersih dengan ikon lingkaran warna-warni, lisensi oranye terang, dan tombol aksi hijau emerald.

---

### 1. Ringkasan Palet Warna Utama

| Token | Warna | Kode HEX | Padanan Tailwind | Alasan & Makna |
| :--- | :--- | :--- | :--- | :--- |
| **Latar Atas** | Deep Forest Green | `#013827` | `bg-[#013827]` | Memberikan kesan mewah, terpercaya, dan teduh |
| **Latar Bawah**| Golden Amber | `#9E7D05` | `bg-amber-600` | Kontras hangat keemasan yang menarik perhatian |
| **Kartu** | Pure White | `#FFFFFF` | `bg-white` | Menjamin keterbacaan teks dan ikon secara maksimal |
| **Lisensi** | Flame Orange | `#EA580C` | `bg-orange-600` | Penegasan kuat bahwa produk 100% bisa dijual kembali |
| **Support** | Emerald Green | `#10B981` | `bg-emerald-500` | Identitas resmi WhatsApp & akses unduh Google Drive |

---

### 2. Daftar Halaman Wireframe Berwarna (Stitch Wireframes)

| ID Halaman | Nama Halaman | Section & Komponen Kunci |
| :--- | :--- | :--- |
| **Pages-01** | **Public Product Access Hub** | Header melengkung bergaris emas, badge oranye, search bar, filter kategori, grid 12 kartu produk real, floating WhatsApp. |
| **Pages-02** | **Product Preview & Access Modal** | Pop-up modal kartu putih, ringkasan fitur, tombol buka Google Drive hijau, tombol salin link. |
| **Pages-03** | **Reseller Commercial License Guide** | Panduan lisensi komersial (PLR/MRR), aturan hak jual kembali, unduh bahan iklan/banner mockup 3D. |
| **Pages-04** | **Admin Content & Product Manager** | Tabel manajemen urutan produk, form edit tautan Google Drive/Canva, tombol sinkronisasi Google Sheets. |
| **Pages-05** | **Mobile Viewport Breakpoint** | Tampilan responsive 2-kolom layar smartphone, touch targets 48px, sticky bottom action bar. |

---

### 3. Tips Penggunaan di Google Stitch

1. Buka file [`PROMPT_STITCH.md`](file:///c:/Users/Saka%20Farma/.gemini/antigravity-ide/scratch/aplikasi%20-landingpage-prodig/PROMPT_STITCH.md) di editor tengah.
2. Tekan **Ctrl + A** lalu **Ctrl + C** (Salin seluruh teks prompt bahasa Inggris).
3. Buka **Google Stitch AI** atau alat prototyping AI Anda, lalu tempel (*paste*) prompt tersebut.
4. Lampirkan juga foto tangkapan layar referensi Anda jika alat tersebut menyediakan fitur upload gambar acuan.
5. Google Stitch akan menghasilkan 5 layar wireframe berwarna penuh (*full-color wireframes*) yang siap dipakai!

