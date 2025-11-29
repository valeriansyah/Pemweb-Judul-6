# 🌦️  Weather Dashboard (Tugas Akhir Pemrograman Web)

Proyek ini dibuat untuk memenuhi spesifikasi tugas akhir pada mata kuliah Praktikum Pemrograman Web.

## ✨ Fitur Utama

Aplikasi ini memenuhi semua spesifikasi yang diminta dalam tugas, ditambah beberapa peningkatan desain (Glassmorphism & Dark Mode).

### 1. Current Weather Display

* **Data Real-time:** Menampilkan Suhu, Kelembapan, dan Kecepatan Angin.
* **Kondisi Cuaca:** Deskripsi dan ikon cuaca yang sesuai.
* **Lokasi & Waktu:** Menampilkan nama kota, negara, dan waktu pembaruan data.
* **Update Otomatis:** Data diperbarui secara otomatis setiap **5 menit** (menggunakan `setInterval()` di JavaScript).

### 2. 5-Day Forecast

* Menampilkan prakiraan cuaca harian (Max/Min Suhu, ikon, dan deskripsi) untuk **5 hari ke depan**.

### 3. Search Functionality

* **Pencarian Kota:** Pencarian cuaca berdasarkan nama kota (didukung oleh API OpenWeatherMap).
* **Simpan Favorit:** Fitur untuk menyimpan dan menampilkan daftar kota favorit menggunakan **Local Storage** *browser*.

### 4. Interactive & Usability Features

* **Theme Toggle:** Tombol *toggle* untuk berpindah antara mode **Dark** dan **Light** (dengan efek Glassmorphism).
* **Unit Toggle:** Tombol untuk beralih antara satuan **Celsius (°C)** dan **Fahrenheit (°F)**.
* **Manual Refresh:** Tombol "Refresh" untuk memperbarui data cuaca secara manual kapan saja.
* **Loading Indicators:** Indikator visual saat data sedang dimuat dari API.

---

## 🛠️ Teknologi yang Digunakan

* **Frontend:** HTML5, Tailwind CSS (Single File/CDN), Vanilla JavaScript (ES6+)
* **Styling:** Tailwind CSS (Desain Glassmorphism, Responsive Design)
* **API:** [OpenWeatherMap API](https://openweathermap.org/) (Endpoint `/weather` dan `/forecast`)

---

## 🚀 Cara Menjalankan Proyek

1.  **Clone Repository:**
    ```bash
 
    ```
2.  **Dapatkan API Key:** Pastikan Anda telah memiliki **API Key** dari OpenWeatherMap.
3.  **Konfigurasi API Key:** Buka file `index.html` dan ganti *placeholder* berikut di dalam tag `<script>` dengan API Key Anda yang sebenarnya:
    ```javascript
    ```
4.  **Akses Aplikasi:** Buka file `index.html` langsung di *browser* Anda (`file:///path/to/index.html`).

---

## 💡 Catatan Implementasi

* **Single File:** Seluruh proyek dikemas dalam satu file `index.html` untuk kemudahan pengujian dan pengumpulan (HTML, CSS, dan JS digabung).
* **Unit Conversion:** Satuan suhu (Metric/Imperial) dikelola oleh parameter `&units=` di URL API dan disesuaikan secara dinamis.
* **Forecast Filtering:** Data 5-hari/3-jam dari endpoint `/forecast` difilter di JavaScript untuk menampilkan hanya satu prediksi per hari (biasanya prediksi di sekitar tengah hari).
* **Persistence:** Fitur Favorit Kota menggunakan metode `localStorage` pada *browser* untuk menyimpan data secara persisten.

---

**[M.Valerian Irwansyah]** **[2315061027]** **[Praktikum Pemrograman Web]**
