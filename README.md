# HIMPRENEUR BINUS — Website Profile

## Cara Penggunaan

1. Buka `index.html` di browser manapun — tidak perlu server.
2. Untuk hosting online, upload file `index.html` ke GitHub Pages, Netlify, atau hosting manapun.

## Menambahkan Logo

Simpan file logo dengan nama `logo.png` di folder yang sama dengan `index.html`.
- Disarankan format PNG transparan
- Ukuran minimal: 200×200px

## Menambahkan Foto

Cari komentar `<!-- PHOTO PLACEHOLDER -->` di dalam `index.html` untuk menemukan semua lokasi foto:

| Lokasi | Keterangan |
|--------|------------|
| Hero Section | Logo HIMPRENEUR (gunakan `logo.png`) |
| Profile Section | Foto kepengurusan (rasio 4:5) |
| Program Card 1–3 | Foto kegiatan angkatan (rasio 16:10) |
| Gallery Section | 5 foto dokumentasi kegiatan |
| Contact Section | Foto contact person (opsional) |

Cara mengganti placeholder dengan foto asli:
```html
<!-- Ganti ini: -->
<div class="profile-photo-placeholder"> ... </div>

<!-- Dengan ini: -->
<img src="nama-foto.jpg" alt="Deskripsi foto" style="width:100%;border-radius:4px">
```

## Mengisi Kontak

Cari teks `(isi nomor resmi)` dan `(isi handle)` di dalam `index.html` dan ganti dengan data yang benar.

## Ganti Tema Warna

Klik ikon 🎨 di pojok kanan bawah untuk memilih tema:
- **Navy + Gold** (default) — Deep navy dengan aksen emas
- **Maroon + Gold** — Merah marun dengan aksen emas  
- **Light / White** — Tema terang dominan putih

## Menambahkan Program Kerja

Duplikat salah satu `.program-card` dan isi dengan informasi proker baru.

## Dibuat oleh
Mohammad Kautsar Lutfie · Ubay Manarul Hidayat · Cedric Aryasatya M. W. A.
