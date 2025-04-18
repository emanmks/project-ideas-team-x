# Ide - ide project akhir untuk siswa

## Daftar Isi
1. [CDC Alumni Photobook](#cdc-alumni-photobook)
2. [SiapJemput](#siapjemput)
3. [KamuTidakSendiri](#kamu-tidak-sendiri)
4. [SantunDigital](#santun-digital)
5. [TemanDuduk](#teman-duduk)
6. [CariMUA](#cari-mua)
7. [MenuBot](#menubot)

---

## CDC Alumni Photobook

### Ikhtisar Proyek
CDC Alumni Photobook adalah platform digital untuk menampilkan dan mengelola data alumni untuk kelas CDC tahun 2024 & 2025. Sistem ini memungkinkan pendamping kelas untuk memasukkan dan mengelola data siswa, sementara juga menyediakan antarmuka publik untuk menjelajahi informasi alumni dengan kemampuan pemfilteran.

### Peran Pengguna
1. **Pendamping Kelas** - Personel berwenang yang mengelola data kelas dan entri siswa
2. **Pengguna Publik** - Siapa saja yang ingin menjelajahi informasi alumni

### Persyaratan Fungsional

#### Fitur Pendamping Kelas
1. **Sistem Autentikasi**
   - Form login aman dengan username/password
   - Manajemen sesi
   - Fungsionalitas pemulihan kata sandi

2. **Manajemen Kelas**
   - Lihat daftar semua kelas
   - Filter kelas berdasarkan tahun (2024/2025)
   - Akses detail kelas

3. **Manajemen Siswa**
   - Lihat siswa di setiap kelas
   - Tambahkan siswa baru ke kelas
   - Unggah foto siswa (format yang didukung: JPG, PNG)
   - Edit informasi siswa yang sudah ada

4. **Bidang Data Siswa**
   - Nama lengkap
   - Kelas
   - Sekolah asal
   - Kota asal
   - Foto
   - Catatan tambahan (opsional)

#### Fitur Pengguna Publik
1. **Direktori Alumni**
   - Jelajahi daftar lengkap alumni
   - Lihat profil siswa dengan foto
   - Filter alumni berdasarkan:
     - Kelas
     - Sekolah asal
     - Kota asal
   - Fungsi pencarian berdasarkan nama siswa
   - Opsi pengurutan (alfabetis, berdasarkan kelas, dll.)

### Persyaratan Teknis
1. **Desain Responsif**
   - Antarmuka yang ramah untuk perangkat mobile
   - Kompatibilitas tablet dan desktop

2. **Database**
   - Penyimpanan autentikasi pengguna
   - Catatan kelas
   - Catatan siswa dengan penyimpanan foto

3. **Keamanan**
   - Kredensial pengguna terenkripsi
   - Akses admin yang aman
   - Validasi data

4. **Kinerja**
   - Pemuatan gambar yang cepat
   - Sistem pemfilteran yang efisien
   - Optimasi pencarian

---

## SiapJemput

### Ikhtisar Proyek
SiapJemput adalah sistem manajemen penjemputan siswa real-time untuk sekolah. Sistem ini memungkinkan petugas gerbang untuk memberi tahu ruang kelas ketika orang tua/wali siswa tiba untuk penjemputan, membantu guru dan siswa mengetahui kapan saatnya meninggalkan kelas.

### Peran Pengguna
1. **Petugas Gerbang** - Staf yang ditempatkan di pintu masuk sekolah yang mencatat status penjemputan siswa
2. **Tampilan Kelas** - Layar di ruang kelas yang menampilkan informasi penjemputan

### Persyaratan Fungsional

#### Fitur Petugas Gerbang
1. **Pencarian Siswa**
   - Cari siswa berdasarkan nama
   - Filter berdasarkan kelas
   - Akses cepat ke siswa yang baru-baru ini dilihat

2. **Manajemen Status Penjemputan**
   - Tandai status siswa sebagai:
     - Belum dijemput (default)
     - Penjemput menunggu di gerbang
     - Siswa telah dijemput dan pergi
   - Kirim notifikasi real-time ke ruang kelas
   - Tambahkan catatan untuk situasi khusus

3. **Dasbor**
   - Ringkasan penjemputan yang tertunda
   - Statistik penjemputan yang selesai
   - Riwayat pencarian

#### Fitur Tampilan Kelas
1. **Tampilan Daftar Siswa**
   - Tampilkan semua siswa di kelas
   - Indikator visual yang jelas untuk status penjemputan:
     - Belum dijemput
     - Penjemput menunggu di gerbang
     - Siswa telah dijemput dan pergi
   - Pembaruan real-time
   - Peringatan suara opsional untuk perubahan status

2. **Manajemen Tampilan**
   - Fungsi penyegaran otomatis
   - Mode siang/malam untuk visibilitas
   - Pengaturan tampilan yang dapat disesuaikan

### Persyaratan Teknis
1. **Komunikasi Real-time**
   - WebSocket atau teknologi serupa untuk pembaruan instan
   - Mekanisme fallback untuk masalah konektivitas

2. **Antarmuka Pengguna**
   - Tampilan kontras tinggi untuk visibilitas di kelas
   - Antarmuka yang ramah sentuh untuk petugas gerbang
   - Warna status mengikuti pedoman aksesibilitas

3. **Integrasi Sistem**
   - Integrasi dengan database siswa sekolah
   - Integrasi opsional dengan sistem notifikasi sekolah

4. **Keamanan**
   - Kontrol akses berbasis peran
   - Log audit untuk semua perubahan status
   - Kepatuhan privasi data

---

## Kamu Tidak Sendiri

### Ikhtisar Proyek
KamuTidakSendiri adalah aplikasi peringatan darurat yang memungkinkan pengguna untuk dengan cepat memberi sinyal untuk bantuan selama keadaan darurat seperti bencana alam, kecelakaan, atau insiden kejahatan. Aplikasi ini menghubungkan korban dengan tim penyelamat dan menyediakan pelacakan lokasi dan alat komunikasi.

### Peran Pengguna
1. **Korban/Pengguna** - Orang dalam kesulitan yang membutuhkan bantuan darurat
2. **Tim Penyelamat** - Responden darurat yang menerima dan menanggapi peringatan

### Persyaratan Fungsional

#### Fitur Korban/Pengguna
1. **Sistem Peringatan Darurat**
   - Tombol darurat sekali tekan
   - Jenis keadaan darurat yang dikategorikan:
     - Bencana alam
     - Kecelakaan
     - Kejahatan
     - Keadaan darurat medis
   - Berbagi lokasi dengan koordinat GPS
   - Fungsionalitas offline untuk area dengan konektivitas terbatas

2. **Alat Komunikasi**
   - Pesan SOS berbasis teks
   - Pesan darurat yang telah ditentukan untuk pengiriman cepat
   - Catatan suara untuk situasi di mana mengetik sulit
   - Unggah foto/video bukti bila sesuai

3. **Informasi Keselamatan**
   - Pedoman darurat berdasarkan situasi
   - Zona aman terdekat
   - Informasi kontak untuk otoritas lokal

#### Fitur Tim Penyelamat
1. **Manajemen Peringatan**
   - Notifikasi keadaan darurat secara real-time
   - Antarmuka peta yang menampilkan lokasi korban
   - Sistem prioritas untuk situasi kritis
   - Penugasan kasus dan pelacakan status

2. **Koordinasi Respons**
   - Saluran komunikasi dengan korban
   - Koordinasi anggota tim
   - Alat alokasi sumber daya
   - Berbagi ETA dengan korban

3. **Dokumentasi Kasus**
   - Pencatatan insiden
   - Pembaruan status
   - Pencatatan penyelesaian
   - Analitik dan pelaporan

### Persyaratan Teknis
1. **Layanan Lokasi**
   - Integrasi GPS presisi tinggi
   - Berbagi lokasi bahkan dengan sinyal minimal
   - Visualisasi peta

2. **Backend Komunikasi**
   - Notifikasi push
   - Pesan dengan bandwidth rendah
   - Enkripsi untuk komunikasi sensitif

3. **Kehandalan**
   - Fungsionalitas offline
   - Optimasi baterai
   - Metode komunikasi cadangan

4. **Keamanan & Privasi**
   - Enkripsi end-to-end
   - Minimalisasi data
   - Kontrol persetujuan pengguna
   - Kepatuhan dengan undang-undang privasi regional

---

## Santun Digital

### Ikhtisar Proyek
SantunDigital adalah alat moderasi konten yang menganalisis teks untuk menentukan apakah itu pantas untuk publikasi online. Layanan ini membantu pengguna menjaga wacana yang sopan dengan menandai konten yang berpotensi menyinggung, membahayakan, atau tidak pantas sebelum diposting.

### Peran Pengguna
1. **Pengguna Akhir** - Orang yang ingin memeriksa kesesuaian konten
2. **Administrator** - Mengelola sistem dan standar moderasi

### Persyaratan Fungsional

#### Fitur Pengguna Akhir
1. **Analisis Konten**
   - Kolom input teks untuk konten yang akan dianalisis
   - Penilaian kesesuaian instan
   - Sorotan frasa/kata yang bermasalah
   - Penjelasan mengapa konten mungkin tidak pantas

2. **Sistem Saran**
   - Saran kata alternatif
   - Penyesuaian nada
   - Umpan balik konstruktif

3. **Alat Pengguna**
   - Riwayat pemeriksaan sebelumnya (opsional)
   - Kamus kustom untuk standar pribadi
   - Ekstensi browser untuk integrasi yang mulus

#### Fitur Administrator
1. **Manajemen Standar Moderasi**
   - Set aturan yang dapat disesuaikan
   - Pedoman khusus kategori
   - Pengaturan konteks budaya

2. **Pemantauan Sistem**
   - Statistik penggunaan
   - Pelaporan positif/negatif palsu
   - Metrik kinerja

### Persyaratan Teknis
1. **Pemrosesan Bahasa Alami**
   - Analisis sentimen
   - Pemahaman konteks
   - Dukungan multi-bahasa

2. **Pembelajaran Mesin**
   - Peningkatan berkelanjutan dari umpan balik
   - Adaptasi terhadap penggunaan bahasa yang berkembang
   - Pelatihan khusus domain

3. **Integrasi API**
   - REST API untuk integrasi pihak ketiga
   - Kemampuan pemrosesan batch
   - Persyaratan respons real-time

4. **Privasi & Etika**
   - Tidak ada penyimpanan permanen konten pengguna
   - Metode pemrosesan yang transparan
   - Strategi mitigasi bias

---

## Teman Duduk

### Ikhtisar Proyek
TemanDuduk adalah layanan pencocokan pendamping untuk transportasi umum yang membantu pelancong menemukan teman duduk yang cocok untuk perjalanan yang lebih menyenangkan. Sistem ini mencocokkan penumpang berdasarkan preferensi, minat, dan kebiasaan perjalanan.

### Peran Pengguna
1. **Penumpang** - Orang yang mencari teman perjalanan yang kompatibel
2. **Administrator Layanan** - Mengelola platform dan menyelesaikan masalah

### Persyaratan Fungsional

#### Fitur Penumpang
1. **Pembuatan Profil**
   - Preferensi pribadi:
     - Tingkat percakapan (cerewet, pendiam, dll.)
     - Minat bersama
     - Preferensi rentang usia
     - Preferensi jenis kelamin (opsional)
   - Kebiasaan perjalanan:
     - Tidur selama perjalanan
     - Bekerja/belajar selama perjalanan
     - Preferensi hiburan

2. **Perencanaan Perjalanan**
   - Masukkan detail perjalanan
   - Lihat teman potensial yang kompatibel
   - Kirim/terima permintaan duduk
   - Konfirmasi pengaturan

3. **Keamanan & Komunikasi**
   - Pesan dalam aplikasi sebelum perjalanan
   - Sistem verifikasi
   - Umpan balik dan penilaian setelah perjalanan
   - Laporkan perilaku tidak pantas

#### Fitur Administrator
1. **Manajemen Pengguna**
   - Proses verifikasi
   - Kemampuan penangguhan/larangan
   - Penyelesaian sengketa

2. **Pemantauan Sistem**
   - Statistik penggunaan
   - Metrik tingkat keberhasilan
   - Pelacakan masalah

### Persyaratan Teknis
1. **Algoritma Pencocokan**
   - Penilaian kompatibilitas berbasis preferensi
   - Pembelajaran mesin untuk pencocokan yang lebih baik seiring waktu
   - Batasan geografis

2. **Antarmuka Pengguna**
   - Desain sederhana, intuitif
   - Presentasi faktor kompatibilitas yang jelas
   - Penerimaan/penolakan saran yang mudah

3. **Privasi & Keamanan**
   - Pembagian informasi pribadi yang terbatas
   - Mekanisme persetujuan yang jelas
   - Kepatuhan perlindungan data

4. **Kemungkinan Integrasi**
   - Sistem pemesanan transportasi umum
   - Aplikasi perencanaan perjalanan
   - Layanan verifikasi identitas

---

## Cari MUA

### Ikhtisar Proyek
CariMUA adalah platform yang menghubungkan klien dengan penata rias (MUA) berdasarkan preferensi gaya, anggaran, dan ketersediaan. Layanan ini bertujuan untuk membantu pengguna menemukan MUA yang sempurna untuk kebutuhan spesifik dan preferensi estetika mereka.

### Peran Pengguna
1. **Klien** - Orang yang mencari jasa makeup
2. **Penata Rias (MUA)** - Profesional yang menawarkan jasa makeup
3. **Administrator Platform** - Mengelola sistem dan akun pengguna

### Persyaratan Fungsional

#### Fitur Klien
1. **Penemuan MUA**
   - Cari berdasarkan lokasi, rentang harga, ketersediaan
   - Filter berdasarkan gaya/spesialisasi makeup:
     - Natural
     - Glamour
     - Editorial
     - Pengantin
     - Efek khusus
   - Jelajahi portofolio dan galeri sebelum/sesudah

2. **Manajemen Pemesanan**
   - Periksa ketersediaan MUA
   - Minta janji temu
   - Kelola pemesanan yang ada
   - Pemrosesan pembayaran

3. **Sistem Ulasan**
   - Nilai pengalaman masa lalu
   - Tinggalkan umpan balik terperinci
   - Lihat ulasan klien lain

#### Fitur Penata Rias
1. **Manajemen Profil**
   - Pembuatan dan pengelolaan portofolio
   - Daftar layanan dengan harga
   - Kalender ketersediaan
   - Tag spesialisasi dan indikator gaya

2. **Administrasi Pemesanan**
   - Terima/tolak permintaan pemesanan
   - Kelola jadwal
   - Alat komunikasi klien
   - Pelacakan pembayaran

3. **Dasbor Analitik**
   - Statistik pemesanan
   - Pelacakan pendapatan
   - Wawasan demografis klien
   - Metrik kinerja

#### Fitur Administrator
1. **Manajemen Platform**
   - Verifikasi pengguna
   - Moderasi konten
   - Penyelesaian sengketa
   - Manajemen biaya

### Persyaratan Teknis
1. **Pencarian dan Pencocokan**
   - Sistem pemfilteran lanjutan
   - Algoritma pengenalan gaya
   - Layanan geolokasi

2. **Manajemen Media**
   - Hosting gambar berkualitas tinggi
   - Organisasi portofolio
   - Alat perbandingan sebelum/sesudah

3. **Sistem Komunikasi**
   - Pesan dalam aplikasi
   - Sistem notifikasi
   - Pengingat janji temu

4. **Pemrosesan Pembayaran**
   - Penanganan transaksi yang aman
   - Berbagai metode pembayaran
   - Sistem deposit pemesanan
   - Pemrosesan pengembalian dana

---

## MenuBot

### Ikhtisar Proyek
MenuBot adalah sistem rekomendasi menu otomatis untuk kafe atau kedai kopi yang membantu pengunjung menemukan menu berdasarkan suasana hati mereka. Sistem ini menggunakan kamera untuk mendeteksi ekspresi wajah pelanggan dan memberikan rekomendasi menu yang sesuai dengan suasana hati yang terdeteksi.

### Peran Pengguna
1. **Pengunjung Kafe** - Pelanggan yang mencari rekomendasi menu
2. **Staf Kafe** - Mengelola item menu dan konfigurasi sistem
3. **Administrator Sistem** - Mengawasi fungsionalitas platform

### Persyaratan Fungsional

#### Fitur Pengunjung
1. **Deteksi Suasana Hati**
   - Analisis ekspresi wajah melalui kamera
   - Identifikasi suasana hati dasar:
     - Senang
     - Sedih
     - Lelah
     - Stres
     - Bersemangat
     - Netral
   - Konfirmasi hasil deteksi (opsional)

2. **Sistem Rekomendasi**
   - Saran menu yang dipersonalisasi berdasarkan suasana hati
   - Rekomendasi khusus berdasarkan waktu hari
   - Opsi untuk mempertimbangkan preferensi tambahan:
     - Preferensi rasa (manis, pahit, asam)
     - Level kafein
     - Jenis makanan ringan
   - Penjelasan mengapa menu tersebut direkomendasikan

3. **Mekanisme Umpan Balik**
   - Nilai kepuasan terhadap rekomendasi
   - Berikan umpan balik spesifik
   - Tingkatkan rekomendasi masa depan

#### Fitur Staf Kafe
1. **Manajemen Menu**
   - Tambah/edit/hapus item menu
   - Perbarui ketersediaan
   - Sorotan item khusus
   - Penandaan kategori suasana hati untuk menu

2. **Dasbor Analitik**
   - Wawasan menu populer berdasarkan suasana hati
   - Tren preferensi pelanggan
   - Efektivitas rekomendasi
   - Bantuan perencanaan inventaris

#### Fitur Administrator
1. **Manajemen Sistem**
   - Penyesuaian algoritma
   - Pengaturan kamera dan pengenalan wajah
   - Dukungan integrasi
   - Pemantauan kinerja

### Persyaratan Teknis
1. **Mesin Rekomendasi**
   - Pembelajaran mesin untuk pencocokan suasana hati dengan menu
   - Penyaringan kolaboratif
   - Saran sadar konteks (waktu, cuaca)

2. **Kemampuan Integrasi**
   - Kompatibilitas dengan sistem POS
   - Platform menu digital
   - Sistem pemesanan online

3. **Computer Vision**
   - Pengenalan ekspresi wajah real-time
   - Privasi dan keamanan data wajah
   - Bekerja dalam berbagai kondisi pencahayaan

4. **Antarmuka Pengguna**
   - Desain ramah perangkat mobile
   - Kepatuhan aksesibilitas
   - Dukungan multi-bahasa
   - Visualisasi menu interaktif

5. **Manajemen Data**
   - Penyimpanan preferensi pelanggan yang aman
   - Analitik penggunaan anonim
   - Kepatuhan GDPR/privasi
   - Protokol pembersihan data reguler