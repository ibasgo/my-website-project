# Website Ibasgo (Quarto)

Proyek website personal siap render. Struktur mengikuti prototype referensi.

## Cara menjalankan

1. Pasang Quarto dari https://quarto.org/docs/get-started/
2. Buka folder ini di terminal
3. Pratinjau langsung:

```
quarto preview
```

4. Render seluruh situs:

```
quarto render
```

Hasil ada di folder `_site`.

## Struktur file

- `_quarto.yml` — konfigurasi utama: navbar, tema, footer
- `styles.scss` — warna, font, dan komponen (hero, kartu, chip)
- `index.qmd` — beranda dan tentang, berisi kurva epidemi
- `portofolio.qmd` — daftar proyek otomatis dari folder `proyek/`
- `proyek/` — satu file `.qmd` per proyek, plus gambar thumbnail
- `publikasi.qmd` — daftar publikasi otomatis dari `referensi.bib`
- `referensi.bib` — sumber data publikasi, tambah entri baru di sini
- `blog.qmd` — daftar tulisan otomatis dari folder `posts/`
- `posts/` — satu folder per tulisan
- `cv.qmd` — CV dan kontak

## Cara menambah konten

Proyek baru: buat file `.qmd` baru di `proyek/`, isi frontmatter title, description, date, categories, image.

Publikasi baru: tambah entri di `referensi.bib`.

Tulisan blog baru: buat folder baru di `posts/`, isi `index.qmd`.

## Ganti warna dan font

Ubah nilai di bagian atas `styles.scss`. Warna utama: `$teal`, `$signal`, `$ink`, `$paper`.

## Ganti foto profil

Taruh foto Anda, lalu tambahkan di `index.qmd` bagian hero jika ingin foto seperti website lama Anda.
