# Laporan Kegiatan Kendala Workshop CIS

## 1.1 Pendahuluan

### 1.1.1 Latar Belakang
Kegiatan ini merupakan workshop yang membahas metode pengamanan sistem operasi Linux menggunakan panduan standar global CIS Benchmarks (studi kasus mencakup Arch Linux, Debian, Ubuntu, dan RedHat). Workshop diselenggarakan secara Hybrid untuk menyeimbangkan penyampaian materi langsung di lokasi serta memfasilitasi peserta jarak jauh melalui ruang virtual.

### 1.1.2 Media Virtual / Online
Jitsi Meet (disiarkan langsung melalui YouTube)

### 1.1.3 Sasaran & Jumlah Peserta
- **Peserta Offline (Luring):** 10 orang Mahasiswa
- **Peserta Online (Daring):** Peserta yang bergabung via tautan ruang Jitsi Meet dan penonton live streaming.

---

## 2.1 Evaluasi Pelaksanaan Secara Offline (Luring)

### 2.1.1 Penyampaian Materi
Berjalan dengan sangat interaktif. Narasumber memandu peserta untuk tidak menghafal isi dokumen CIS yang tebal (ribuan halaman), melainkan mengajarkan cara mencari Pola (*Pattern*) dan Objek dari daftar isi agar proses audit keamanan sistem menjadi jauh lebih cepat dan praktis.

### 2.1.2 Sesi Praktik Kelompok
Setelah pemaparan teori, panitia membagi peserta luring menjadi 2 kelompok praktik selama 45 menit untuk mencoba langsung apa yang telah disampaikan oleh pemateri, seperti mencari pattern-nya bagaimana dan object-nya seperti apa.

---

## 2.2 Evaluasi Pelaksanaan Secara Online (Daring via Jitsi)

### 2.2.1 Masalah Koneksi & Kestabilan Platform
Sektor daring menghadapi tantangan teknis yang cukup berat. Akibat beban jaringan atau fluktuasi bandwidth pada platform Jitsi Meet, terjadi beberapa kali kendala putus koneksi secara tiba-tiba (*disconnect/force close*). Hal ini menyebabkan operator atau narasumber terlempar keluar dari ruangan virtual di tengah sesi penjelasan.

### 2.2.2 Dampak Pada Peserta Online
Gangguan tersebut sempat memotong alur presentasi di layar penonton daring dan menyebabkan kualitas audio/video sesekali mengalami delay atau patah-patah, sebelum akhirnya panitia berhasil melakukan stabilitas ulang perangkat broadcast.

---

## Matriks Kendala Hybrid dan Solusi Tepat Guna (Lapangan)

| No | Sektor | Masalah Kendala Nyata di Lapangan | Solusi Instan / Penanganan Panitia |
|----|--------|-----------------------------------|-------------------------------------|
| 1 | Online (Jitsi) | Kamera/Display operator sempat freeze dan narasumber keluar otomatis dari ruang Jitsi | Panitia teknis segera melakukan check screen, membenahi jalur masuk room, dan melakukan re-connect perangkat utama ke Jitsi Meet agar siaran kembali normal |
| 2 | Online (Jitsi) | Kualitas suara narasumber sempat tidak stabil dan putus-putus di sisi audiens daring | Panitia mengondisikan agar penangkapan suara bertumpu pada mikrofon sentral operator |
| 3 | Hybrid Link (Sinkronisasi) | Saat terjadi gangguan Jitsi, peserta online sempat tertinggal progres pengisian catatan/skrip Obsidian yang sedang diketik narasumber | Operator panitia langsung mengambil alih (*take over*) file materi untuk di-*share screen* dari laptop operator yang jaringan internetnya lebih stabil |

---

## 3.1 Evaluasi Umum Pelaksanaan Hybrid

Secara keseluruhan, pelaksanaan workshop CIS Benchmarks berjalan cukup baik dari sisi penyampaian materi dan antusiasme peserta luring. Namun, sektor daring menjadi titik lemah utama akibat ketergantungan pada satu platform (Jitsi Meet) tanpa jalur cadangan (backup), sehingga saat terjadi gangguan koneksi, dampaknya langsung terasa oleh seluruh peserta online tanpa ada solusi mitigasi cepat selain re-connect manual.

Beberapa poin evaluasi utama:

1. **Ketergantungan Infrastruktur Tunggal:** Tidak ada platform cadangan (misalnya Zoom, Google Meet, atau Google Meet, atau line RTMP kedua) saat Jitsi mengalami disconnect.
2. **Perangkat Broadcast Tunggal:** Proses re-connect bergantung pada satu perangkat operator, sehingga saat perangkat tersebut bermasalah, seluruh siaran ikut terhenti.
3. **Sinkronisasi Materi Real-Time:** Peserta daring sempat tertinggal progres catatan/skrip karena proses take-over file hanya dilakukan secara manual saat insiden terjadi.
4. **Belum Ada SOP Tertulis:** Penanganan kendala teknis masih bersifat reaktif dan mengandalkan inisiatif panitia di lapangan, bukan mengikuti prosedur baku yang telah disiapkan sebelumnya.

## 3.2 Saran untuk Workshop Hybrid Selanjutnya

| No | Aspek | Saran Perbaikan |
|----|-------|------------------|
| 1 | Platform & Jaringan | Siapkan koneksi internet cadangan (dedicated line atau tethering modem terpisah) khusus untuk perangkat broadcast, agar tidak bergantung pada satu jaringan yang sama dengan peserta luring. |
| 2 | Redundansi Platform | Sediakan platform virtual cadangan (misalnya Zoom/Google Meet) yang sudah di-setup sebelumnya, sehingga jika Jitsi bermasalah, sesi dapat langsung dipindahkan tanpa banyak jeda. |
| 3 | Perangkat Operator | Gunakan minimal 2 perangkat broadcast (primary & backup) yang sudah login dan siap pakai, agar proses re-connect tidak memakan waktu lama. |
| 4 | SOP Tertulis | Susun SOP tertulis untuk penanganan gangguan teknis (disconnect, audio putus, dsb.) agar respons panitia lebih cepat dan terstandar, tidak lagi bersifat reaktif. |
| 5 | Uji Coba Sebelum Acara (Technical Rehearsal) | Lakukan simulasi/gladi bersih koneksi dan perangkat broadcast H-1 sebelum acara untuk mendeteksi potensi masalah jaringan lebih awal. |
