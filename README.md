## Preview Website
https://egisatriaa.github.io/FUSEN-Website/ 

---

## Fitur Utama

### 1️⃣ Auto-Swipe Brand Logos
Slider horizontal otomatis yang menampilkan deretan logo brand secara terus-menerus (infinite looping).

Fitur lengkap:

- Auto-scroll halus menggunakan perhitungan frame-based (`requestAnimationFrame`).
- Pause otomatis saat user hover, touch, atau drag.
- Sistem auto-clone agar track logo selalu panjang dan tidak terputus.
- Auto-reset ketika mencapai batas track untuk mencegah lag.
- Ringan, responsif, dan berjalan mulus di semua device.

---


### 2️⃣ Scrollable Categories dengan Button Navigation
Navigasi kategori yang dapat di-scroll secara horizontal menggunakan tombol kiri & kanan.

Kemampuan:

- Tombol geser kiri/kanan dengan perhitungan step otomatis berdasarkan lebar container.
- Scroll halus menggunakan `behavior: "smooth"`.
- Tombol otomatis menghilang jika scroll tidak diperlukan.
- Debugging helper opsional untuk memastikan tombol berfungsi.

---

### 3️⃣ Responsive Layout (TailwindCSS)
Layout sepenuhnya menggunakan TailwindCSS untuk fleksibilitas dan tampilan mobile-first.

Kemampuan:

- Mendukung layout responsif di hampir semua ukuran layar.
- Elemen seperti navbar, kategori, banner, dan section lain menyesuaikan ukuran secara otomatis.
- Utility Tailwind memastikan styling tetap bersih, konsisten, dan mudah di-maintain.

---

### 4️⃣ Modular JavaScript Initialization
Seluruh script dibungkus dalam blok aman:

```js
try {
   // all scripts…
} catch (err) {
   console.error("Script init error:", err);
}
```

### Tujuan:

- Menghindari crash ketika satu fungsi mengalami error.
- Memudahkan proses debugging.
- Tetap aman digunakan dalam bundler, minifier, atau modular environment.

---

### 5️⃣ Event Handling yang Efisien
Setiap fitur ditenagai event listener yang telah dioptimasi untuk performa:

- `mouseenter`, `mouseleave`
- `touchstart`, `touchend`
- `resize`
- `beforeunload`

Hasilnya, animasi dan navigasi tetap berjalan lancar tanpa risiko memory leak.

---

### 6️⃣ Clean Code Architecture
Struktur kode dirancang agar tetap bersih, modular, dan efisien:

- Setiap fitur dipisahkan dalam IIFE (`(function(){…})()`) untuk mencegah polusi global scope.
- Variabel terlindungi dalam block scope sehingga tidak bentrok dengan script lain.
- Rendering & animasi hanya menggunakan API browser yang optimal untuk performa tinggi.

---


### 🛠 Teknologi yang Digunakan

| Teknologi              | Fungsi                                      |
|-----------------------|----------------------------------------------|
| **HTML5**             | Struktur layout utama                        |
| **TailwindCSS**       | Styling & responsive design                  |
| **JavaScript (Vanilla)** | Interaksi & animasi                       |
| **External CSS (animasi.css)** | Efek transisi/animasi tambahan     |
| **Asset gambar/logo** | Digunakan untuk brand carousel & kategori    |

---



