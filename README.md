# ELDEN Hospital Expo - landing page

Halaman statis satu file. Tidak ada build step, framework, atau dependensi selain Google Fonts.

## Isi folder
- `index.html`: seluruh halaman (HTML, CSS, dan sedikit JavaScript untuk hitung mundur)
- `logo.png`: logo ELDEN di header

## Cara tayang
Cocok untuk hosting statis gratis yang boleh dipakai komersial, misalnya Cloudflare Pages atau Netlify.
- Push folder ini ke repo GitHub, lalu sambungkan repo ke hosting. Build command dikosongkan, output directory `/` (root).
- Atau upload folder ini langsung lewat dashboard hosting, tanpa GitHub.
- Jangan pakai Vercel paket Hobby. Paket itu hanya untuk penggunaan non-komersial.

## Yang biasa diubah
1. **Tanggal tutup:** cari `DEADLINE` di script paling bawah `index.html`. Saat ini 15 Oktober 2026, 23.59 WIB. Tulisan "Sisa ... hari" dihitung otomatis dari tanggal ini. Teks "Tutup 15 Okt ..." di pita atas, section kuota, dan bagian bawah halaman ditulis manual, jadi ubah juga.
2. **Nomor WhatsApp dan pesan otomatis:** cari `wa.me` di `index.html`. Ada beberapa tombol dengan link yang sama, ganti semuanya. Pesannya berisi `[nama klinik]` yang diisi calon klien sebelum mengirim.
3. **Warna:** `--brand` (biru ELDEN, #0155FF) dan `--deep` (biru tua) di blok `<style>` paling atas.

## Catatan
- Halaman ini tidak mengumpulkan data apa pun. Semua tombol langsung membuka WhatsApp.
- Setelah 8 slot penuh atau tanggal lewat, tulisan hitung mundur berubah jadi "Penawaran ditutup". Tombol WhatsApp tetap aktif, jadi nonaktifkan atau ganti halamannya secara manual kalau perlu.
