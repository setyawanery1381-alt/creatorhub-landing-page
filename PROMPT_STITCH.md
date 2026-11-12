# Prompt Stitch — Digital Product Access Hub & Reseller Vault

Create detailed colored wireframes (structured, layout-focused UI screens) for Digital Product Access Hub & Reseller Vault.
Use a full-color design from the start — apply the color palette, typography, and component styles defined below. Keep the layout structure clear and organized like a wireframe, but render every screen in color.

## Application Context
An all-in-one digital product showcase, direct access vault, and reseller portal built on Google Apps Script and Google Sheets. It allows buyers and resellers to instantly access, view, and download 10+ premium digital assets (worksheet collections, educational games, coding packages, e-books, Canva templates, and mega bundles) with 100% commercial resell rights (PLR/MRR), accompanied by live category filtering, rapid instant search, and WhatsApp support integration.
Has 5 main sections: Public Hub & Showcase, Product Preview & Download Modal, Reseller Commercial License Guide, Admin Content Manager, and Mobile Viewport.

## Design Identity
- Style: Modern Card Grid Hub / Vibrant Digital Asset Vault (Bento & Linktree-inspired high-contrast layout)
- Aesthetic: Clean white rounded cards, vibrant colorful circular icon badges, soft drop shadows, rich gradient backdrop, generous spacing, and gold-accented header framing.
- Color Palette:
  Primary Background: Deep Forest Green to Amber Gold gradient [linear-gradient(145deg, #013827 0%, #064e3b 35%, #3f5509 70%, #9e7d05 100%)] — gives a lush, trustworthy, and high-value commercial appeal
  Surface (Cards): Pure White [#FFFFFF] with soft elevation shadow [box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.25)]
  Header Surface: Semi-transparent Deep Pine [#01291D] with backdrop blur (blur-md) and arched bottom border [#EAB308]
  Accent 1 (Reseller Badge): Bright Orange gradient [#EA580C to #F97316] — highlights 100% Resell Rights guarantee
  Accent 2 (WhatsApp CTA): Vibrant Emerald Green [#10B981 / #059669] — instant support & community connection
  Text Primary (Cards): Dark Slate [#1E293B]
  Text Secondary (Cards): Muted Slate [#64748B]
  Text Headers: Pure White [#FFFFFF] and Light Gold [#FEF08A]
  Card Badge (License Tag): Mint Tint [#ECFDF5] with Forest Green text [#047857] and border [#A7F3D0]
- Typography: Poppins (headings and card titles, 700-800 weight) paired with Inter (search input, metadata, captions, 400-500 weight)
- Icons: Sharp line icons enclosed within solid colored circular containers (Lucide Icons style)
- Visual Language: Inspired by Gumroad, Bento.me, Linktree Pro, and Notion Gallery Views
- Corner Radius: 20px (rounded-2xl) for product cards, 9999px (rounded-full) for badges/pills/action buttons, 36px (rounded-b-[2.25rem]) for the top arched header
- Shadow: Soft atmospheric ambient elevation [0 10px 25px -4px rgba(0,0,0,0.25), 0 4px 6px -2px rgba(0,0,0,0.1)]
- Spacing: 16px base grid; 12px to 16px grid gap between cards
- Typography Scale:
  H1 App Title: 32px / 36px, font-black, tracking-wider, uppercase, text-white
  H2 Tagline: 14px, font-semibold, text-amber-200
  Card Title: 12px / 14px, font-bold, leading-tight, text-slate-800
  Badge & Labels: 10px / 11px, font-bold, uppercase
- Layout & Navigation: Top arched header banner with gold baseline, horizontal quick-category scroll pills, sticky top search bar, 3-column card grid, floating WhatsApp support trigger
- Component Shapes: Buttons [pill / rounded-full], inputs [rounded-xl with semi-transparent black fill], cards [solid white rounded-2xl]
- Micro-interactions: Cards lift upward by 5px with subtle scale (scale-102) on hover; circular icon badges scale by 10% with slight tilt (+5deg); smooth click bounce
- Reference Fidelity: Follows the user reference image faithfully: reproducing the distinctive forest-green-to-warm-gold gradient backdrop, top curved container with gold border, vibrant orange reseller badge ("100% Bisa Dijual Kembali"), and 3-column white card layout with multi-colored circular icon discs.

## Wireframe Pages Required

--- Pages-01: PUBLIC PRODUCT ACCESS HUB (MAIN CATALOG) ---
Layout: Full-height gradient background [linear-gradient(145deg, #013827, #064e3b, #9e7d05)] | Top arched header | Sticky search & category pill bar | 3-column product grid | Floating support button | Minimal footer
- Header Container: Arched bottom border [radius 36px], deep pine surface [#01291D]/80, 2px gold accent border [#EAB308]
  - Title: "DIGITAL PRODUK" in bold white uppercase typography with subtle drop shadow
  - Tagline: "Pelopor Produk Digital No 1" in pale gold [#FEF08A]
  - Floating Badge: Orange pill button [bg #EA580C to #F97316] reading "100% Bisa Dijual Kembali" with shield-check icon
- Search & Filter Section:
  - Search Bar: Full-width rounded-xl glassmorphism input [bg-black/30, border white/20, placeholder emerald-100/60] with search icon on left and clear button on right
  - Category Pills: Horizontal scrollable pill row [Semua (active amber #F59E0B), Mega Bundle, Template Toko, E-Book, Worksheet Anak, Games Edukasi, Aplikasi & Coding, Komunitas]
- Main Grid (3-Columns on Desktop/Tablet, 2-Columns on Mobile):
  - Card 1 [Promo Paket Mega Bundling]: White card, red circular icon [#EF4444] with package icon, bold title, "100% Hak Jual" mint badge
  - Card 2 [Pro Growth Bundle Landing Page]: White card, violet icon [#8B5CF6] with palette icon, bold title, "100% Hak Jual" badge
  - Card 3 [Paket Super Hemat 9 E-Book]: White card, pink icon [#EC4899] with book-open icon, bold title, "100% Hak Jual" badge
  - Card 4 [Paket 3 Coding]: White card, royal blue icon [#3B82F6] with code-2 icon, bold title, "100% Hak Jual" badge
  - Card 5 [Paket 15000++ Worksheet Anak]: White card, teal icon [#14B8A6] with file-spreadsheet icon, bold title, "100% Hak Jual" badge
  - Card 6 [20 Games Edukasi Anak]: White card, orange icon [#F97316] with gamepad-2 icon, bold title, "100% Hak Jual" badge
  - Card 7 [10 Games Edukasi Anak Muslim]: White card, emerald icon [#10B981] with star icon, bold title, "100% Hak Jual" badge
  - Card 8 [39000++ Media Anak Kreatif]: White card, sky blue icon [#0EA5E9] with image icon, bold title, "100% Hak Jual" badge
  - Card 9 [1000++ Worksheet Islami]: White card, green icon [#22C55E] with book-marked icon, bold title, "100% Hak Jual" badge
  - Card 10 [Games Edukasi 8 Seri]: White card, purple icon [#A855F7] with puzzle icon, bold title, "100% Hak Jual" badge
  - Card 11 [WA Grup Komunitas & Reseller]: White card, WhatsApp green icon [#25D366] with message-circle icon, title, "Support Reseller" badge
  - Card 12 [Cover & Banner Promosi]: White card, indigo icon [#6366F1] with layers icon, title, "Bahan Iklan" badge
- Floating Action Button: Fixed bottom-right corner, emerald green pill [#10B981] with pulsing white indicator dot and message icon: "Hubungi Admin"
- Footer: Copyright notice, reseller rights confirmation, dark translucent bar

--- Pages-02: PRODUCT PREVIEW & ACCESS MODAL ---
Layout: Centered modal dialog with backdrop overlay (bg-black/70 with blur-sm)
- Modal Window: White card, rounded-3xl, max-width 480px, padding 24px, relative close button [X] at top-right
- Modal Header:
  - Icon Badge: Centered 64px circular container with product category color and icon
  - Title: Large 20px bold heading (e.g., "Paket 15000++ Worksheet Anak")
  - Badges: Pill row containing "100% Hak Jual (PLR/MRR)" [bg #DCFCE7, text #166534] + "Kategori: Worksheet Anak" [bg #EFF6FF, text #1E40AF]
- Description Block: Soft gray tinted card [#F8FAFC], rounded-xl, padding 16px, listing key features:
  - "Isi 15.000+ file format PDF siap cetak"
  - "Mencakup tracing, mewarnai, berhitung, logika, & kosa kata"
  - "Lisensi komersial: Boleh dijual kembali satuan atau bundling"
- Action Buttons (Full-Width Stack):
  - Primary Action Button: "Buka & Download di Google Drive" [filled emerald #10B981, white text, bold, rounded-xl, 48px height, external link icon]
  - Secondary Action Button: "Salin Link Akses" [outlined gray #E2E8F0, text slate-700, copy icon]
- Notice Footer: "Tips: Simpan link ini di bookmark browser Anda untuk akses berkala."

--- Pages-03: RESELLER COMMERCIAL LICENSE & GUIDELINES ---
Layout: Focused single-column reading container (max-w-xl) on gradient background
- Header: Back navigation button [← Kembali ke Katalog] + Title "Panduan & Lisensi Hak Jual Kembali"
- License Summary Card (White, rounded-2xl, p-6):
  - Green Shield Banner: "Status Lisensi: RESELLER UNLIMITED (PLR / MRR)" [bg #ECFDF5, text #065F46, border #A7F3D0]
  - Permitted Rules (Checkmarks in green):
    - [✓] Boleh menjual kembali produk dengan harga bebas
    - [✓] Boleh dijadikan bonus untuk penawaran produk lain
    - [✓] Boleh di-rebranding dengan nama toko Anda sendiri
    - [✓] Keuntungan penjualan 100% menjadi milik Anda
  - Prohibited Rules (X icons in red):
    - [✕] Dilarang membagikan link akses secara publik gratis tanpa izin
    - [✕] Dilarang menghapus hak cipta pembuat utama
- Marketing Materials Card:
  - Preview grid of 3D Book Mockups & Canva Promotion Templates
  - Button: "Download Banner & Bahan Iklan (Google Drive)" [filled blue #3B82F6, rounded-xl]

--- Pages-04: ADMIN CONTENT & PRODUCT MANAGER ---
Layout: Modern compact management panel with top navigation bar
- Top Navigation: Logo "Digital Produk Admin" [left], Quick Status "12 Produk Aktif" [center], Button "Buka Google Spreadsheet" [green outline, right]
- Quick Actions Bar:
  - Search Input: "Cari data di sheet..."
  - Add New Product Button: "+ Tambah Produk Baru" [filled emerald #10B981, white text]
  - Sync Status: "Status: Terhubung dengan Google Sheets" [green status dot]
- Data Table Card (White, rounded-2xl, shadow-md, overflow-hidden):
  - Table Header: Gray background [#F1F5F9], bold text [Urutan | Judul Produk | Kategori | URL Target | Hak Jual | Status | Aksi]
  - Row 1: "1 | Promo Paket Mega Bundling | Mega Bundle | digitalproduk... | 100% Hak Jual | [Toggle Switch: Aktif] | [Edit Icon] [Trash Icon]"
  - Row 2: "2 | Pro Growth Bundle Landing Page | Template Toko | sangcreator.canva... | 100% Hak Jual | [Toggle Switch: Aktif] | [Edit Icon] [Trash Icon]"
  - Row 3: "3 | Paket Super Hemat 9 E-Book | E-Book | sites.google.com... | 100% Hak Jual | [Toggle Switch: Aktif] | [Edit Icon] [Trash Icon]"
  - Row 4: "4 | Paket 15000++ Worksheet Anak | Worksheet Anak | drive.google.com... | 100% Hak Jual | [Toggle Switch: Aktif] | [Edit Icon] [Trash Icon]"
- Quick Settings Drawer (Right Side / Collapsible):
  - Edit WhatsApp Admin Number (Current: 081331661370)
  - Edit Top Banner Text ("DIGITAL PRODUK")
  - Edit Tagline ("Pelopor Produk Digital No 1")
  - Button "Simpan Pengaturan ke Sheet" [filled amber #F59E0B]

--- Pages-05: MOBILE VIEWPORT BREAKPOINT (SMARTPHONE VIEW) ---
Layout: High-density 2-column card grid optimized for one-hand mobile browsing (375px width preview)
- Top Header: Compact curved container [padding 20px 16px], title 24px bold, tagline 12px, orange badge pill 11px
- Search & Filter: Sticky compact search field + horizontal swiping category chips with snap scrolling
- Product Grid: 2-column layout [gap 10px]
  - Cards: Compact card height (135px), centered 44px circular icon badge, 11px bold product title truncated to 2 lines, micro "100% Hak Jual" mint pill tag
  - Touch Target: Minimum 48px tactile tap area
- Bottom Navigation Bar (Sticky Floating):
  - Quick Button 1: "Semua Produk" [home icon]
  - Quick Button 2: "Lisensi Reseller" [award icon]
  - Quick Button 3: "Chat Admin WA" [message icon with green notification badge]

## Wireframe Style Notes
- FULL COLOR design — do NOT use grayscale or black-and-white wireframe style
- Apply the defined color palette consistently across all pages
- Text placeholders: Use actual representative labels ("Paket 15000++ Worksheet Anak", "Games Edukasi 8 Seri", "Promo Paket Mega Bundling"), not "Lorem Ipsum"
- Buttons: Primary = filled emerald [#10B981] or amber [#F59E0B] with white text; Secondary = outlined with subtle background; Danger = filled red [#EF4444]
- Status badges as colored pills:
  - 100% Hak Jual / Aktif (bg #ECFDF5, text #047857, border #A7F3D0)
  - Support / Komunitas (bg #EFF6FF, text #1D4ED8, border #BFDBFE)
  - Pending / Nonaktif (bg #FEF3C7, text #B45309, border #FDE68A)
- Icon Badges: Render each card's icon inside its exact designated circular hue (Teal, Pink, Royal Blue, Orange, Purple, Emerald, Sky Blue, Red)
- Show mobile breakpoint for the Catalog (Pages-05) as a dedicated smartphone frame alongside the desktop views
- Navigation Flow: Clicking any product card on Pages-01 triggers Pages-02 (Preview Modal) or opens the direct Google Drive/Canva link in a new tab; WhatsApp button opens direct chat with 081331661370.

## Global Design Requirements
- Fully responsive: Desktop (3 columns) and Mobile (2 columns)
- Skeleton loading state: Shimmering translucent pulse rectangles for instant perceived performance
- Empty state: Clean folder-search icon with helpful "Coba kata kunci lain" label
- Micro-animations: 250ms smooth transition for hover lift and active press scale
- Zero latency feel: Client-side cached dataset for instant 0ms search filtering and category switching
- Overall feel: Trustworthy, lively, commercial, clean, and ready-to-sell digital asset powerhouse.

