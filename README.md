# Generator Berita Acara Kebutuhan

Aplikasi SPA (Single Page Application) untuk membuat dokumen "Berita Acara Kebutuhan" secara otomatis dan mengekspornya ke PDF. 100% client-side, tanpa backend.

## Cara Pakai (Lokal)
Cukup buka `index.html` langsung di browser (double click), tidak perlu install apapun.

## Cara Deploy ke GitHub + Vercel/Netlify

1. Buat repository baru di GitHub, upload file `index.html` ini ke root repository.
2. **Vercel**: masuk ke [vercel.com](https://vercel.com) → New Project → Import repository GitHub kamu → biarkan semua setting default (tidak perlu build command) → Deploy.
3. **Netlify**: masuk ke [netlify.com](https://netlify.com) → Add new site → Import from Git → pilih repo → Deploy site (tidak perlu build command, publish directory `/`).
4. Selesai — aplikasi langsung live di URL yang diberikan.

## Fitur
- Form input manual untuk semua field dokumen
- Tabel "Spesifikasi Kebutuhan" dengan baris dinamis (tambah/hapus item)
- Kalkulasi otomatis Total → Grand Total → Perkiraan Total Harga (format Rupiah, real-time)
- Live preview dokumen di sisi kanan, sama persis dengan layout final
- Export ke PDF (A4, pixel-perfect) menggunakan html2pdf.js
- 3 blok tanda tangan tetap: Diajukan oleh, Disetujui oleh, Mengetahui

## Struktur File
Semua kode (HTML, CSS via Tailwind CDN, JavaScript vanilla) ada dalam satu file `index.html` — tidak ada dependency build/npm.
