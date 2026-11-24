<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>AI Logbook - Proyek SakuPintar</title>
  <style>
    /* Pengaturan Dasar Halaman */
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    body {
      background-color: #f1f5f9;
      color: #1e293b;
      padding: 20px;
      line-height: 1.6;
    }

    .container {
      max-width: 900px;
      margin: 0 auto;
      background: #ffffff;
      padding: 30px;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
    }

    /* Header & Tombol Cetak */
    .header-box {
      display: flex;
      justify-content: space-between;
      align-items: center;
      border-bottom: 2px solid #2563eb;
      padding-bottom: 15px;
      margin-bottom: 20px;
      flex-wrap: wrap;
      gap: 10px;
    }

    .header-box h1 {
      color: #1d4ed8;
      font-size: 24px;
    }

    .btn-print {
      background-color: #2563eb;
      color: white;
      border: none;
      padding: 10px 16px;
      border-radius: 8px;
      font-size: 14px;
      font-weight: bold;
      cursor: pointer;
    }

    .btn-print:hover {
      background-color: #1e40af;
    }

    /* Kotak Identitas Proyek */
    .info-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 12px;
      background-color: #eff6ff;
      padding: 16px;
      border-radius: 8px;
      margin-bottom: 25px;
      border-left: 5px solid #2563eb;
      font-size: 14px;
    }

    .info-grid p strong {
      color: #1e3a8a;
    }

    /* Desain Tabel Logbook */
    h2 {
      font-size: 18px;
      margin-bottom: 12px;
      color: #0f172a;
    }

    .table-responsive {
      overflow-x: auto;
      margin-bottom: 25px;
    }

    table {
      width: 100%;
      border-collapse: collapse;
      font-size: 14px;
    }

    th, td {
      border: 1px solid #cbd5e1;
      padding: 12px;
      text-align: left;
      vertical-align: top;
    }

    th {
      background-color: #2563eb;
      color: white;
      font-weight: 600;
    }

    tr:nth-child(even) {
      background-color: #f8fafc;
    }

    .badge {
      display: inline-block;
      padding: 3px 8px;
      border-radius: 4px;
      font-size: 12px;
      font-weight: bold;
      background-color: #dcfce7;
      color: #166534;
      margin-bottom: 4px;
    }

    /* Bagian Kesimpulan */
    .kesimpulan-box {
      background-color: #f8fafc;
      padding: 16px;
      border-radius: 8px;
      border: 1px solid #e2e8f0;
      font-size: 14px;
    }

    .kesimpulan-box ul {
      margin-left: 20px;
      margin-top: 8px;
    }

    .kesimpulan-box li {
      margin-bottom: 6px;
    }

    /* Sembunyikan tombol cetak saat disimpan ke PDF / Print */
    @media print {
      body {
        background: white;
        padding: 0;
      }
      .container {
        box-shadow: none;
        padding: 0;
      }
      .btn-print {
        display: none;
      }
    }
  </style>
</head>
<body>

  <div class="container">
    <!-- Judul & Tombol Simpan PDF -->
    <div class="header-box">
      <div>
        <h1>📓 AI Logbook Pengembangan Proyek</h1>
        <p style="color: #64748b; font-size: 14px;">Dokumentasi Kolaborasi Siswa & Kecerdasan Artifisial</p>
      </div>
      <button class="btn-print" onclick="window.print()">🖨️ Cetak / Simpan PDF</button>
    </div>

    <!-- Identitas Proyek (Bisa diedit sesuai nama siswa) -->
    <div class="info-grid">
      <div>
        <p><strong>Tema Pelatihan:</strong> Solusi Digital Sehari-hari Berbantuan AI</p>
        <p><strong>Nama Aplikasi:</strong> SakuPintar (Asisten Uang Saku)</p>
        <p><strong>Teknologi:</strong> HTML, CSS, JS, LocalStorage, PWA</p>
      </div>
      <div>
        <p><strong>Nama Siswa:</strong> [SILVIYA RIZKI N ANGGRAINI DAN LAEDYSKA TAHTA LAKSANA ZAMRUD]</p>
        <p><strong>Kelas / Sekolah:</strong> XI SMA/SMK - [SMKN 2 BLITAR]</p>
        <p><strong>Link Aplikasi:</strong> <a href="./index.html" target="_blank">Buka Aplikasi SakuPintar</a></p>
      </div>
    </div>

    <!-- Tabel Catatan Logbook -->
    <h2>Catatan Proses Pengembangan (Prompting & Evaluasi)</h2>
    <div class="table-responsive">
      <table>
        <thead>
          <tr>
            <th style="width: 15%;">Tahap</th>
            <th style="width: 25%;">Prompt ke AI</th>
            <th style="width: 30%;">Ringkasan Output AI</th>
            <th style="width: 30%;">Evaluasi & Tindakan Siswa</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td><strong>1. Ideasi & Konsep</strong></td>
            <td><em>"Berikan ide website PWA offline untuk kehidupan sehari-hari siswa SMA usia 17 tahun yang baru belajar HTML, CSS, JS, lengkap dengan struktur file dan fitur."</em></td>
            <td>AI mengusulkan aplikasi <strong>SakuPintar</strong> untuk mencatat uang saku harian dengan fitur penasihat keuangan AI offline serta struktur 5 file utama.</td>
            <td><span class="badge">Disetujui</span><br>Ide sangat relevan untuk mengatasi masalah boros uang jajan pelajar tanpa bergantung pada kuota internet.</td>
          </tr>
          <tr>
            <td><strong>2. Desain Tampilan (UI)</strong></td>
            <td><em>"Buatkan kode index.html dan style.css untuk aplikasi 'SakuPintar' desain ramah layar HP, berisi kartu saldo, form input, kotak saran AI, dan riwayat."</em></td>
            <td>AI menghasilkan kerangka HTML dan CSS responsif (lebar maksimal 420px) lengkap dengan indikator warna saldo (hijau, kuning, merah).</td>
            <td><span class="badge">Berhasil</span><br>Kode diuji di browser dengan mode tampilan HP. Tampilan rapi, warna disesuaikan agar nyaman dibaca.</td>
          </tr>
          <tr>
            <td><strong>3. Logika & Otak AI</strong></td>
            <td><em>"Buatkan kode app.js agar form bisa menghitung saldo, menyimpannya di LocalStorage, dan memiliki fungsi AI sederhana untuk memberi saran keuangan."</em></td>
            <td>AI membuat skrip penyimpanan data permanen di memori HP (<code>LocalStorage</code>) serta logika <em>Rule-Based AI</em> berdasarkan rasio pengeluaran.</td>
            <td><span class="badge">Dimodifikasi</span><br>Menambahkan fitur tombol "Reset" agar data uji coba mudah dihapus saat melakukan demonstrasi aplikasi.</td>
          </tr>
          <tr>
            <td><strong>4. Mode Offline (PWA)</strong></td>
            <td><em>"Buatkan kode manifest.json dan sw.js agar proyek SakuPintar bisa diinstal di HP dan jalan offline saat di-deploy di GitHub Pages."</em></td>
            <td>AI memberikan konfigurasi identitas aplikasi (<code>manifest.json</code>) dan mekanisme <em>caching</em> file aset (<code>sw.js</code>).</td>
            <td><span class="badge">Selesai</span><br>Menambahkan file gambar <code>icon.png</code>, mendaftarkan Service Worker di HTML, dan menguji aplikasi dalam mode pesawat.</td>
          </tr>
        </tbody>
      </table>
    </div>

    <!-- Kesimpulan Refleksi Siswa -->
    <div class="kesimpulan-box">
      <strong>Kesimpulan & Refleksi Pembelajaran:</strong>
      <ul>
        <li><strong>Peran AI:</strong> Mempercepat penulisan struktur kode dasar HTML, CSS, JavaScript, serta membantu memberikan solusi teknis untuk fitur penyimpanan offline (PWA).</li>
        <li><strong>Peran Siswa:</strong> Menentukan kebutuhan pengguna, memecah perintah (<em>prompting</em>) secara bertahap agar kode mudah dipahami, menguji fungsionalitas, dan melakukan penyesuaian akhir.</li>
      </ul>
    </div>
  </div>

</body>
</html>
