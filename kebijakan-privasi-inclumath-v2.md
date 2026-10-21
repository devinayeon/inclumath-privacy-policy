# Kebijakan Privasi Inclumath

**Terakhir diperbarui:** 21 Oktober 2026  
**Versi:** 2.0  
**Berlaku untuk:** aplikasi Inclumath (`com.inclumath.app`) yang didistribusikan melalui Google Play.

---

## 1. Ringkasan

- Inclumath dapat dimainkan **tanpa akun**. Kami tidak meminta nama, alamat email, nomor telepon, atau kata sandi.
- **Kamera hanya dipakai untuk fitur Augmented Reality (AR).** Gambar kamera diproses di perangkat dan **tidak direkam, tidak disimpan, dan tidak diunggah** oleh kami.
- **Tidak ada iklan** di dalam aplikasi, tidak ada penggunaan **Advertising ID**, dan data pengguna **tidak dijual**.
- Progres permainan dan pengaturan (misalnya status onboarding dan preferensi musik) disimpan **di perangkat**.
- Aplikasi memuat dua komponen pihak ketiga yang mengirim data teknis ke penyedianya:
  - **Vuforia Engine** (PTC Inc.) — validasi lisensi dan statistik teknis.
  - **ARCore / Google Play Services for AR** (Google) — data teknis dan diagnostik saat fitur AR berjalan.
- Pertanyaan dan permintaan terkait privasi: **21adtydwf@gmail.com**.

---

## 2. Siapa yang bertanggung jawab

Penyelenggara aplikasi dan pengendali data adalah:

- **Nama:** Tim Inclumath
- **Alamat:** Indonesia
- **Email privasi:** 21adtydwf@gmail.com

Kami tidak memiliki server aplikasi sendiri dan tidak menyimpan basis data pengguna. Karena itu, sebagian besar data yang dijelaskan di bawah ini berada di perangkat Anda atau diproses langsung oleh penyedia komponen pihak ketiga.

---

## 3. Data yang diproses

### 3.1 Data yang disimpan di perangkat

Aplikasi menyimpan data berikut secara lokal di penyimpanan aplikasi pada perangkat Anda:

| Data | Contoh | Tujuan |
|---|---|---|
| Status onboarding | apakah layar pengenalan sudah diselesaikan | agar pengenalan tidak diulang |
| Preferensi audio | musik aktif/nonaktif, pengaturan suara | mengingat pilihan Anda |
| Progres dan pengaturan permainan | level/aktivitas yang telah diselesaikan, pengaturan tampilan | melanjutkan permainan |

Data ini **tidak dikirim ke kami** dan tidak dapat kami baca. Data lokal dapat ikut serta dalam **Android Auto Backup** apabila fitur pencadangan aktif pada perangkat dan akun Google Anda. Pencadangan tersebut dijalankan oleh sistem Android dan tunduk pada kebijakan Google, bukan pada kendali kami.

### 3.2 Kamera

Aplikasi meminta izin `CAMERA` hanya ketika Anda membuka fitur AR. Saat fitur AR aktif:

- Gambar dari kamera digunakan untuk mengenali penanda (image target) dan menempatkan objek 3D.
- Pemrosesan dilakukan **di perangkat** menggunakan Vuforia Engine dengan basis data target yang tersimpan di dalam aplikasi (*device database*).
- Gambar kamera **tidak direkam, tidak disimpan, dan tidak dikirim** ke kami maupun ke PTC.
- Aplikasi ini **tidak menggunakan Vuforia Cloud Recognition, ARCore Cloud Anchors, atau ARCore Geospatial API**, sehingga tidak ada pengiriman gambar atau lokasi presisi ke server pihak ketiga.

Jika Anda menolak izin kamera, permainan tetap dapat digunakan, tetapi fitur AR tidak akan berfungsi.

### 3.3 Data yang dikirim Vuforia Engine kepada PTC Inc.

Inclumath memuat Vuforia Engine versi 11.4.4. Menurut dokumentasi PTC, aplikasi yang memakai Vuforia Engine mengirim **statistik dasar** dan melakukan **pemeriksaan lisensi** secara daring. Data tersebut meliputi:

| Kategori | Rincian |
|---|---|
| Informasi perangkat | merek, model, firmware, nama dan versi sistem operasi, profil kamera |
| Informasi perangkat lunak | versi Vuforia Engine dan license key |
| Informasi aplikasi | ID paket (`com.inclumath.app`), versi aplikasi, jenis distribusi, ID toko aplikasi |
| Peristiwa penggunaan | waktu sesi, mulai/berhenti/lanjut mesin Vuforia, kamera mulai/berhenti, peristiwa pelacakan dan pengenalan, penggunaan fitur |
| Alamat IP | dipakai untuk menyimpulkan negara atau wilayah; bukan lokasi presisi |
| Identifier teknis | penanda perangkat yang dipakai untuk validasi lisensi dan statistik |

- **Penerima:** PTC Inc., afiliasinya, dan penyedia layanan yang bekerja untuk PTC.
- **Tujuan:** menyediakan dan memvalidasi lisensi, menyusun statistik agregat, serta meningkatkan kualitas SDK.
- **Transfer internasional:** data dapat ditransfer ke dan diproses di Amerika Serikat atau negara lain.
- **Retensi:** mengikuti kebijakan privasi PTC.

Kami tidak menerima laporan individual dari statistik tersebut dan tidak menggunakannya untuk mengidentifikasi pengguna.

### 3.4 Data yang diproses ARCore / Google Play Services for AR

Fitur AR memerlukan **Google Play Services for AR (ARCore)** yang disediakan oleh Google. Menurut dokumentasi Google, ARCore selalu mengumpulkan:

- **User ID** (identifier akun Google apabila Anda masuk ke akun Google di perangkat) **atau Device ID** (apabila Anda tidak masuk);
- **data performa dan diagnostik**, seperti kondisi baterai, waktu pemuatan, latensi, dan frame rate;
- **penggunaan API dan aktivitas aplikasi**, yaitu pemanggilan API ARCore oleh aplikasi.

Data tersebut dikirim ke Google dan diproses menurut **Kebijakan Privasi Google**. Apabila ARCore belum terpasang, Google Play dapat menampilkan proses pemasangan layanan tersebut.

Aplikasi ini **tidak** meminta izin lokasi dan **tidak** memakai Geospatial API atau Cloud Anchors, sehingga ARCore tidak mengumpulkan lokasi presisi atau video melalui aplikasi ini.

### 3.5 Data yang tidak kami kumpulkan

Kami tidak mengumpulkan dan aplikasi tidak meminta:

- nama, alamat email, nomor telepon, atau akun pengguna;
- lokasi presisi melalui GPS. Perkiraan negara atau wilayah hanya disimpulkan oleh PTC dari alamat IP sebagaimana dijelaskan pada bagian 3.3;
- rekaman suara atau mikrofon;
- kontak, kalender, SMS, atau riwayat panggilan;
- foto, video, atau berkas dari galeri dan penyimpanan;
- data kesehatan atau data keuangan;
- **Advertising ID** atau identifier iklan lainnya.

Aplikasi juga tidak memuat SDK iklan, SDK analitik komersial, atau layanan pelaporan kerusakan (crash reporting) pihak ketiga.

---

## 4. Izin Android dan tujuannya

| Izin | Kapan diminta | Tujuan |
|---|---|---|
| `CAMERA` | saat fitur AR dibuka | menampilkan dan melacak penanda AR |
| `INTERNET` | otomatis | validasi lisensi Vuforia dan komunikasi komponen pihak ketiga |
| `ACCESS_NETWORK_STATE` | otomatis | memeriksa ketersediaan koneksi untuk validasi lisensi |
| `HIGH_SAMPLING_RATE_SENSORS` | otomatis | sensor gerak untuk pelacakan AR |

Izin dapat dicabut kapan saja melalui **Pengaturan → Aplikasi → Inclumath → Izin**.

---

## 5. Dasar dan tujuan pemrosesan

| Pemrosesan | Dasar | Tujuan |
|---|---|---|
| Penyimpanan progres dan pengaturan di perangkat | pelaksanaan layanan yang Anda minta | menjalankan fungsi permainan |
| Akses kamera | persetujuan Anda (izin Android) | menjalankan fitur AR |
| Statistik dan validasi lisensi Vuforia | kepentingan yang sah dalam menyediakan dan mengamankan lisensi perangkat lunak; persetujuan apabila diwajibkan hukum | memastikan aplikasi berfungsi sesuai lisensi dan meningkatkan kompatibilitas |
| Diagnostik ARCore | pelaksanaan fungsi AR dan kepentingan sah Google sebagai penyedia layanan | menjalankan dan meningkatkan layanan AR |

Kami tidak memproses data untuk iklan, pemasaran ulang, pembuatan profil perilaku, atau pengambilan keputusan otomatis yang berdampak hukum bagi Anda.

---

## 6. Pembagian data dan transfer internasional

Kami **tidak menjual** data pengguna dan **tidak membagikannya untuk iklan**. Data hanya sampai kepada pihak ketiga dalam keadaan berikut:

1. **PTC Inc.** — statistik dan validasi lisensi Vuforia sebagaimana dijelaskan pada bagian 3.3.
2. **Google** — data ARCore sebagaimana dijelaskan pada bagian 3.4, dan pencadangan Android apabila Anda mengaktifkannya.
3. **Kewajiban hukum** — apabila diwajibkan oleh peraturan perundang-undangan atau perintah yang berwenang.

Karena PTC dan Google beroperasi secara global, data dapat diproses di luar Indonesia, termasuk di Amerika Serikat. Kami tidak mengendalikan lokasi pemrosesan tersebut; rinciannya diatur dalam kebijakan privasi masing-masing penyedia (bagian 15).

---

## 7. Penyimpanan dan penghapusan

**Data di perangkat** disimpan sampai Anda menghapusnya. Anda dapat menghapus seluruh data lokal dengan:

- **Pengaturan Android → Aplikasi → Inclumath → Penyimpanan → Hapus data**, atau
- **menghapus aplikasi (uninstall)**.

Setelah itu, progres dan pengaturan tidak dapat dipulihkan. Menonaktifkan musik atau menyelesaikan onboarding tidak menghapus data lain.

**Data yang telah dikirim ke PTC atau Google** tidak berada dalam kendali kami dan tidak dapat kami hapus. Untuk menggunakan hak Anda atas data tersebut, hubungi PTC atau Google melalui kanal yang tercantum pada kebijakan privasi mereka. Kami akan membantu mengarahkan permintaan Anda sejauh yang kami mampu.

**Data di sisi kami:** tidak ada, karena kami tidak mengoperasikan server aplikasi maupun basis data pengguna.

---

## 8. Keamanan

- Komunikasi dengan layanan Vuforia dan Google menggunakan **HTTPS/TLS**.
- Data lokal berada dalam **sandbox aplikasi Android** dan hanya dapat diakses oleh aplikasi ini, kecuali pada perangkat yang telah dimodifikasi (misalnya di-root).
- Kami tidak menyimpan data pengguna di server, sehingga tidak ada basis data pusat yang dapat bocor dari pihak kami.
- Keamanan data di perangkat tetap bergantung pada kunci layar, pembaruan sistem, dan praktik keamanan Anda.
- Aplikasi ini **belum** menjalani audit keamanan independen.

Tidak ada sistem yang sepenuhnya aman. Jika Anda menemukan masalah keamanan, hubungi kami melalui 21adtydwf@gmail.com.

---

## 9. Hak Anda

Sesuai Undang-Undang Nomor 27 Tahun 2022 tentang Pelindungan Data Pribadi dan ketentuan lain yang berlaku, Anda berhak untuk:

- mengetahui dan memperoleh informasi tentang pemrosesan data pribadi Anda;
- memperoleh akses dan salinan data yang kami kendalikan;
- meminta pembetulan atau pembaruan data yang tidak akurat;
- meminta penghapusan data;
- menarik kembali persetujuan yang telah diberikan;
- mengajukan keberatan atas pemrosesan tertentu;
- mengajukan keluhan kepada lembaga pengawas pelindungan data pribadi.

Karena kami tidak menyimpan data pribadi di server, permintaan yang menyangkut data lokal dapat Anda lakukan sendiri melalui langkah pada bagian 7. Untuk permintaan lain, kirim email ke 21adtydwf@gmail.com dengan subjek **“Permintaan Privasi Inclumath”**. Kami akan menanggapi dalam waktu yang wajar sesuai ketentuan yang berlaku. Kami mungkin meminta informasi tambahan secukupnya untuk memverifikasi permintaan, tanpa meminta data yang tidak relevan.

---

## 10. Audiens dan privasi anak

Inclumath adalah game edukasi matematika yang **ditujukan untuk remaja usia 13–17 tahun**, termasuk remaja berkebutuhan khusus. Aplikasi ini **tidak ditujukan untuk anak di bawah 13 tahun**.

Aplikasi ini:

- tidak menampilkan iklan dan tidak memakai Advertising ID;
- tidak meminta akun, nama, email, atau nomor telepon;
- tidak mengakses lokasi, mikrofon, kontak, atau galeri;
- tidak membuat profil perilaku untuk iklan;
- memproses gambar kamera hanya di perangkat.

Karena sebagian pengguna berusia di bawah 18 tahun, kami menyarankan orang tua, wali, atau pendamping untuk:

- meninjau kebijakan ini bersama pengguna;
- mengatur izin kamera melalui pengaturan Android;
- mendampingi penggunaan fitur AR.

Kami tidak dengan sengaja mengumpulkan data pribadi anak di bawah 13 tahun. Apabila Anda mengetahui bahwa seorang anak di bawah 13 tahun menggunakan aplikasi ini, hubungi 21adtydwf@gmail.com agar kami dapat membantu menjelaskan pengaturan privasi dan langkah penghapusan data lokal.

Untuk pengguna di bawah 18 tahun, persetujuan atas pemrosesan yang dijelaskan pada bagian 3.3 dan 3.4 diberikan oleh orang tua atau wali.

---

## 11. Keselamatan penggunaan AR

Fitur AR menampilkan objek maya di atas gambar nyata melalui kamera.

- Jangan menggunakan fitur AR saat **mengemudi, mengendarai kendaraan, menyeberang jalan, atau melakukan aktivitas lain yang membutuhkan perhatian penuh**.
- Perhatikan lingkungan sekitar dan jangan berjalan sambil menatap layar.
- Awasi anak-anak saat menggunakan fitur AR dan pastikan ruang di sekitarnya aman.
- Hentikan penggunaan apabila Anda merasa pusing, mual, atau tidak nyaman.

---

## 12. Persetujuan atas statistik Vuforia

Dengan menggunakan fitur AR pada Inclumath, Anda menyetujui bahwa **PTC Inc., afiliasinya, dan penyedia layanannya** mengumpulkan, menyimpan, menggunakan, dan mentransfer **Statistik** sebagaimana dijelaskan pada bagian 3.3, termasuk transfer ke Amerika Serikat dan negara lain, untuk tujuan menyediakan dan memvalidasi lisensi, menyusun statistik agregat, dan meningkatkan SDK.

Persetujuan ini merupakan bagian dari syarat penggunaan fitur AR. Apabila Anda tidak menyetujuinya, jangan gunakan fitur AR; bagian permainan lain tetap dapat dimainkan. Untuk pengguna yang belum dewasa, persetujuan diberikan oleh orang tua atau wali.

---

## 13. Perubahan kebijakan

Kebijakan ini dapat diperbarui apabila fitur, komponen pihak ketiga, atau praktik pengelolaan data berubah. Versi terbaru selalu tersedia di halaman ini beserta tanggal pembaruannya. Perubahan material akan diumumkan melalui halaman aplikasi di Google Play atau pemberitahuan di dalam aplikasi sebelum berlaku.

---

## 14. Kontak

**Tim Inclumath**
Email: 21adtydwf@gmail.com
Alamat: Indonesia

Untuk pertanyaan tentang kebijakan ini atau permintaan terkait data pribadi, sertakan nama aplikasi (**Inclumath**) dan jelaskan permintaan Anda secara singkat.

---

## 15. Layanan pihak ketiga

Kebijakan pihak ketiga berikut berlaku atas pemrosesan yang mereka lakukan:

| Penyedia | Peran | Kebijakan |
|---|---|---|
| PTC Inc. (Vuforia Engine) | validasi lisensi dan statistik SDK | https://www.ptc.com/en/documents/policies/privacy |
| PTC Inc. (Vuforia Statistics) | penjelasan statistik Vuforia | https://developer.vuforia.com/legal/statistics |
| Google (ARCore / Play Services for AR) | pelacakan AR dan diagnostik | https://policies.google.com/privacy |
| Google (Android Auto Backup) | pencadangan data perangkat | https://policies.google.com/privacy |

Kami tidak bertanggung jawab atas isi atau praktik privasi situs dan layanan pihak ketiga tersebut.
