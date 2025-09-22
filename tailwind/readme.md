
---

## Cara Run

1. Download / clone project ini.
2. Simpan gambar profil dan feed minimal 12 file di `assets/img/`.
3. Buka `index.html` di browser.
4. Tailwind sudah terhubung via CDN, jadi tidak perlu build tambahan.

---

## Desain Grid & Responsivitas

### Feed (Grid)
- **Mobile (default → `grid-cols-1`)**  
  1 kolom penuh → foto besar, mudah dilihat di layar kecil.
- **Tablet (`sm:grid-cols-2 md:grid-cols-3`)**  
  2–3 kolom → layar lebih besar, grid lebih efisien.
- **Desktop (`lg:grid-cols-4`)**  
  4 kolom → layout padat tapi tetap proporsional.
- **Gap (`gap-2`)**  
  Cukup kecil agar tampilan mirip feed Instagram: rapat tapi tetap ada jarak visual.

### Tombol Follow / Message
- Menggunakan `order-2 md:order-1` →  
  - Mobile: tombol di bawah username (mudah dijangkau jempol).  
  - Desktop: tombol sejajar username (tampilan profesional).  
- Ukuran tombol (`text-sm md:text-base`, `px-3 md:px-4`) berubah sesuai breakpoint agar tetap nyaman digunakan.

### Layout Mobile-first
- Default menggunakan **utility mobile**, lalu ditingkatkan dengan `sm:`, `md:`, `lg:`.  
- Contoh: `flex-col md:flex-row` → stack vertikal di mobile, horizontal di desktop.  
- Semua responsivitas diatur tanpa media query manual.

---

## Pertanyaan Reflektif

### 1. Kenapa memilih konfigurasi grid-cols & gap per breakpoint?
- Mobile 1 kolom → fokus ke kenyamanan pengguna layar kecil.  
- Tablet 2–3 kolom → memanfaatkan ruang ekstra, tidak terlalu rapat.  
- Desktop 4 kolom → tampilan mirip Instagram asli, rapi, padat.  
- Gap kecil (`gap-2`) → menjaga estetika grid tetap rapat.

### 2. Bagaimana utility responsive Tailwind membantu di mobile?
- `order-*` memastikan tombol selalu dekat dengan username.  
- `flex-col md:flex-row` menjaga struktur nyaman dibaca di layar kecil.  
- Ukuran teks/tombol otomatis menyesuaikan (`text-sm md:text-base`).  
Semua dilakukan tanpa menulis CSS custom.

### 3. Trade-off: banyak utility classes vs custom CSS
- **Utility-first (Tailwind murni)**  
  -  Pro: cepat, konsisten, fleksibel, mobile-first.  
  -  Kontra: HTML panjang, bisa sulit dibaca pemula.  
- **Custom component CSS**  
  -  Pro: HTML lebih ringkas, mudah reuse.  
  -  Kontra: rawan inkonsistensi, perlu maintain CSS tambahan.  

**Kesimpulan:**  
Utility classes cocok untuk prototyping cepat dan project kecil–menengah.  
Custom CSS lebih baik untuk project besar yang butuh HTML bersih dan banyak reuse komponen.

---

## Lisensi
Proyek ini dibuat untuk pembelajaran. Tidak berafiliasi dengan Instagram.
