# 💰 SakuPintar — AI Logbook Pengembangan Proyek

![Status](https://shields.io)
![Tech](https://shields.io)
![Offline](https://shields.io)

> **Tema Pelatihan:** Solusi Digital untuk Kehidupan Sehari-hari Berbantuan Kecerdasan Artifisial  
> **Nama Siswa:** `[SILVIYA RIZKI N ANGGRAINI DAN LAEDYSKA TAHTA LAKSANA ZAMRUD]`  
> **Kelas / Sekolah:** XI SMA/SMK - `[SMKN 2 BLITAR]`  


---

### 📓 Catatan Kolaborasi dengan AI

| Tahap Pengerjaan | Tujuan | Prompt yang Diberikan ke AI | Ringkasan Hasil / Output AI | Evaluasi & Tindakan Siswa |
| :--- | :--- | :--- | :--- | :--- |
| **1. Ideasi & Konsep** | Mencari ide website bermanfaat bagi pelajar usia 17 tahun yang bisa diinstal di HP dan jalan *offline*. | *"Berikan ide website berbasis PWA offline untuk kehidupan sehari-hari siswa SMA usia 17 tahun yang baru belajar HTML, CSS, JS, lengkap dengan struktur file dan fitur."* | AI menyarankan aplikasi **SakuPintar** untuk mencatat pemasukan/pengeluaran harian dengan penasihat keuangan AI *offline* dan struktur 5 file utama. | **Disetujui.** Ide sesuai dengan kebutuhan sehari-hari pelajar untuk mencegah boros uang jajan tanpa butuh kuota internet. |
| **2. Perancangan Tampilan (`index.html` & `style.css`)** | Membuat kerangka halaman dan desain antarmuka (*UI*) yang pas di layar HP. | *"Buatkan kode index.html dan style.css untuk aplikasi 'SakuPintar' desain ramah layar HP, berisi kartu saldo, form input, kotak saran AI, dan riwayat."* | AI membuat kerangka HTML dan CSS responsif (lebar maksimal 420px) dengan indikator 3 warna saldo (hijau aman, kuning waspada, merah kritis). | **Berhasil.** Tampilan diuji menggunakan mode layar HP di browser dan sudah terlihat rapi serta mudah dibaca. |
| **3. Logika & Otak AI (`app.js`)** | Membuat fitur hitung saldo otomatis, penyimpanan data *offline*, dan analisis AI. | *"Buatkan kode app.js agar form bisa menghitung saldo, menyimpannya di LocalStorage, dan memiliki fungsi AI sederhana untuk memberi saran keuangan."* | AI menghasilkan kode `LocalStorage` agar data tersimpan permanen di memori HP, serta logika *Rule-Based AI* yang memberi nasihat berdasarkan persentase pengeluaran. | **Dimodifikasi.** Menambahkan tombol **"Reset"** agar data uji coba mudah dihapus saat aplikasi didemonstrasikan. |
| **4. Mode Offline & Instalasi (`manifest.json` & `sw.js`)** | Mengubah website menjadi aplikasi HP (PWA) yang bisa dibuka saat mode pesawat. | *"Buatkan kode manifest.json dan sw.js agar proyek SakuPintar bisa diinstal di HP dan jalan offline saat di-deploy di GitHub Pages."* | AI membuat konfigurasi identitas aplikasi (`manifest.json`) dan skrip penyimpan *cache* file (`sw.js`), serta kode pendaftaran di `index.html`. | **Selesai.** Menyiapkan gambar ikon (`icon.png`), mengunggah semua file ke GitHub Pages, dan menguji instalasi di HP. |
