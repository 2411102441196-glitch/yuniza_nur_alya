
---

## Cara Build / Run

1. Clone / download repository ini.
2. Pastikan semua gambar profil dan feed tersedia di folder `assets/img/`.
3. Buka file `index.html` langsung di browser, atau gunakan server lokal (contoh: VSCode Live Server).
4. Halaman akan otomatis responsif di berbagai ukuran layar (mobile, tablet, desktop).

---

## Dependensi

- **[Bootstrap 5.3.3](https://getbootstrap.com/)**  
  Digunakan untuk grid system, komponen card, navbar, dan tombol.
- **Custom CSS (optional)**  
  Untuk menjaga konsistensi tinggi gambar feed.
- Tidak ada backend atau framework tambahan (pure HTML + CSS + Bootstrap CDN).

---

## Catatan Desain

- **Grid system:**  
  - Mobile ≤576px → 1 kolom (`col-12`)  
  - Tablet ≥768px → 2–3 kolom (`col-sm-6 col-md-4`)  
  - Desktop ≥992px → 4 kolom (`col-lg-3`)  

- **Tombol interaksi:**  
  - Ditempatkan dekat username.  
  - Menggunakan `order-*` agar di mobile berada di bawah username (mudah dijangkau), dan di desktop sejajar ke kanan.  

- **Feed:**  
  - 12 gambar minimal, ditampilkan dalam grid responsif.  
  - Jika jumlah postingan bertambah (misalnya 50), grid tetap rapi.  
  - Disarankan pagination atau infinite scroll untuk performa.  

---

## Preview

Contoh tampilan (mockup):
- **Mobile:** 1 kolom feed
- **Tablet:** 2–3 kolom feed
- **Desktop:** 4 kolom feed

---

## Lisensi
Proyek ini dibuat untuk tujuan pembelajaran dan tidak berafiliasi dengan Instagram.
