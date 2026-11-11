# Selaras Coffee - One Page Website UMKM

Tugas pembuatan website profil UMKM satu halaman (*One Page Website*) menggunakan kerangka kerja Bootstrap 5 dan CSS kustom dengan tema warna kuning dan hitam.

---

## Ringkasan Pengerjaan

Website UMKM *Selaras Coffee* dirancang dalam bentuk *One Page Website* menggunakan Bootstrap 5 dengan identitas visual bertema kuning dan hitam. Komponen yang diimplementasikan meliputi navbar responsif dengan *hamburger toggle*, hero section informatif, notifikasi promo berbasis alert, tiga kartu produk, modal interaktif, formulir kontak terstruktur, serta footer penutup. Styling eksternal ditambahkan untuk memperkuat branding melalui efek interaksi kartu, aksen garis judul, dan palet warna yang serasi.

Selama proses perancangan, kendala yang dihadapi adalah perbedaan tinggi antar kartu produk saat panjang teks deskripsi tidak sama, serta konflik tampilan warna bawaan Bootstrap yang kurang mencerminkan identitas UMKM kopi. Selain itu, elemen modal sempat tidak terbuka akibat urutan pemanggilan script JS bundle yang belum tepat.

Solusi yang diterapkan adalah menambahkan utility class `h-100` dan `d-flex flex-column` pada kartu agar tingginya proporsional dan tombol aksi tetap sejajar di bagian bawah. Untuk identitas visual, custom CSS eksternal digunakan untuk mendefinisikan warna aksen khusus serta efek *hover*. Masalah interaktivitas modal diselesaikan dengan memastikan script `bootstrap.bundle.min.js` terpanggil sebelum penutup tag `<body>`. Hasil akhir menghasilkan antarmuka yang bersih, fungsional, dan responsif di berbagai resolusi layar.

---

## Checklist Kelengkapan Komponen

| No | Komponen Wajib | Implementasi pada Kode | Keterangan |
|---|---|---|---|
| 1 | Navbar Responsif | `<nav class="navbar navbar-expand-lg ...">` | Collapse ke hamburger menu di mobile |
| 2 | Hero Section | `<header id="hero" class="hero-section ...">` | Headline utama + tombol call-to-action |
| 3 | Minimal 3 Card | 3 kartu menu (`.card-custom`, `.col-md-4`) | Menampilkan menu andalan & harga |
| 4 | Minimal 1 Alert | Alert promo (`.alert-warning alert-dismissible`) | Notifikasi diskon yang bisa ditutup |
| 5 | Minimal 1 Modal | Modal popup (`#modalPromo`) | Detail info promo & kemitraan |
| 6 | Form Kontak | Form input nama, email, dan textarea pesan | Formulir inquiries & pesanan katering |
| 7 | Footer | `<footer>` dengan info hak cipta | Penutup halaman bernuansa gelap |
| 8 | Custom CSS | `css/style.css` | Branding warna kuning-hitam & hover effect |

---

## Struktur Folder Project

```text
pertemuan-09/
│
├── index.html        # File HTML utama (struktur & komponen Bootstrap)
├── README.md         # Dokumentasi ringkasan dan panduan tugas
├── css/
│   └── style.css     # Custom CSS eksternal (warna, hero, efek hover)
├── images/           # Aset gambar pendukung (opsional)
```

---

## Teknologi yang Digunakan

- **HTML5**: Semantik struktur website.
- **Bootstrap 5.3.3**: Framework CSS untuk grid system, layout responsif, dan komponen UI interaktif.
- **Custom CSS3**: Pengaturan palet warna, tipografi, dan transisi visual.

---

## Informasi Mahasiswa

- **Nama:** [Saka laksmana Harimurti]
- **NPM:** [4525210067]