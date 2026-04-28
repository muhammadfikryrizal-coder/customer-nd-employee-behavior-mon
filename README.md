# Vision Link AI

Vision Link AI adalah dashboard manajemen cerdas berbasis AI untuk industri food and beverage (F&B), khususnya operasional kedai kopi. Proyek ini membantu pemilik bisnis memantau produktivitas staf secara real-time sekaligus meningkatkan loyalitas pelanggan dengan pengalaman yang lebih personal.

## Topik

Digital & Creative Economy

## Ringkasan Eksekutif

Industri F&B menghadapi dua tantangan utama:
- Konsistensi produktivitas staf sering menurun karena distraksi (misalnya penggunaan ponsel berlebih) yang tidak selalu terpantau manajer secara langsung.
- Customer lifetime value belum optimal karena pelanggan tidak selalu mendapatkan apresiasi personal yang mendorong kunjungan ulang.

Vision Link AI menjawab tantangan tersebut dengan mengintegrasikan Computer Vision dan AI Agent untuk:
- Memantau perilaku karyawan secara otomatis.
- Memberikan intervensi cepat melalui chatbot.
- Mengenali pelanggan dan mengotomatisasi loyalty flow.

## Problem Statement

Bagaimana mengintegrasikan Computer Vision dan AI Agent untuk memantau produktivitas karyawan secara otomatis sekaligus menciptakan sistem loyalitas pelanggan yang proaktif dan terpersonalisasi?

## Solusi

Vision Link AI bertindak sebagai "mata digital" untuk pemilik bisnis:
- Menggunakan Azure AI Vision untuk menganalisis aktivitas staf dan pelanggan.
- Menggunakan Azure OpenAI untuk menghasilkan pesan teguran/promo yang natural.
- Menghubungkan pengenalan pelanggan dengan sistem poin loyalitas dan strategi upselling via WhatsApp.

## Fitur Utama

- **AI Employee Monitoring**: Deteksi otomatis perilaku karyawan (fokus bekerja vs distraksi/bermain HP) beserta sistem skor performa.
- **Automated Discipline Chatbot**: Pengiriman peringatan SOP otomatis ke WhatsApp ketika pelanggaran berulang terdeteksi.
- **VIP Customer Recognition**: Pengenalan wajah pelanggan di kasir untuk sapaan personal dan pencatatan poin otomatis.
- **Smart Upselling & Retention**: Pengiriman voucher/promo via WhatsApp berdasarkan konteks perilaku pelanggan (contoh: duduk >90 menit).

## Teknologi Microsoft Azure

- **Azure AI Vision (Spatial Analysis)**: Pelacakan pergerakan dan aktivitas di area operasional.
- **Azure OpenAI Service**: Penyusunan pesan otomatis untuk teguran staf dan promosi pelanggan.
- **Azure SQL Database**: Penyimpanan data label wajah, riwayat poin pelanggan, dan skor performa staf.
- **Azure App Service**: Hosting aplikasi web manajemen kedai.

## Alur Penggunaan Produk

1. **Setup & Onboarding**
   - Pemilik kedai mendaftarkan data wajah karyawan.
   - CCTV diintegrasikan dengan Azure AI Vision.
   - Pelanggan melakukan registrasi wajah dengan persetujuan eksplisit.

2. **Operasional Staf**
   - Kamera memantau area kerja secara real-time.
   - Poin performa bertambah saat perilaku kerja sesuai SOP.
   - Jika distraksi terdeteksi berulang, sistem mengirim peringatan WhatsApp otomatis.

3. **Pelayanan Pelanggan**
   - Sistem mengenali pelanggan saat datang.
   - Nama pelanggan ditampilkan untuk mendukung sapaan personal.
   - Poin loyalitas otomatis diperbarui setelah transaksi.

4. **Automated Retention**
   - Saat pola tertentu terdeteksi (misalnya durasi duduk lama), sistem memicu promo WhatsApp untuk mendorong pembelian tambahan.

## Cara Menjalankan Project Ini

Project ini berupa antarmuka web statis:

1. Buka file `index.html` langsung di browser.
2. Atau jalankan lewat local server sederhana (direkomendasikan agar perilaku aset/tautan lebih konsisten):
   - VS Code Live Server, atau
   - `python -m http.server` lalu akses `http://localhost:8000`.

## Inovasi Manajerial

Sistem menyediakan data objektif untuk mendukung keputusan manajerial seperti evaluasi performa dan penentuan bonus berbasis poin.

## Privasi & Etika

- Pengawasan karyawan dilakukan pada area publik operasional.
- Data wajah pelanggan diproses hanya setelah consent eksplisit.
- Implementasi disarankan mengikuti regulasi perlindungan data yang berlaku.
