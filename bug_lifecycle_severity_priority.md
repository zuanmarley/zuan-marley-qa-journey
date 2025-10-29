## I. 🔄 Siklus Hidup Bug (Bug Lifecycle Diagram)

Siklus ini menjelaskan perjalanan suatu bug dari saat ditemukan hingga diverifikasi dan ditutup.

| Tahap (Status) | Pihak yang Bertanggung Jawab | Deskripsi Tindakan |
| :--- | :--- | :--- |
| **1. NEW (Baru)** | QA Tester | Bug pertama kali ditemukan dan dilaporkan ke dalam sistem (misalnya Jira). |
| **2. ASSIGNED (Ditugaskan)** | Project Manager / Tech Lead | Bug ditugaskan kepada Developer spesifik yang relevan. |
| **3. OPEN (Terbuka)** | Developer | Developer sedang menganalisis dan mulai proses perbaikan (*fixing*). |
| **4. FIXED (Selesai)** | Developer | Developer telah menerapkan perbaikan kode (*patch*) dan siap dikirim ke QA. |
| **5. PENDING RETEST** | QA Tester | Bug berada dalam antrian untuk diuji ulang (verifikasi perbaikan). |
| **6. RETEST (Tes Ulang)** | QA Tester | QA menguji kembali bug dengan langkah-langkah yang sama. |
| **7. VERIFIED / CLOSED** | QA Tester | Jika bug sudah hilang, QA mengubah status menjadi Verified dan Closed. |
| **Jalur Lain** | | Status lain: **REOPEN** (jika perbaikan gagal), **DEFERRED** (ditunda ke rilis berikutnya), **DUPLICATE** (sudah pernah dilaporkan). |

---

## II. ⚡ Severity vs Priority

Dua metrik kunci untuk menentukan pentingnya sebuah bug.

### A. 💥 Severity (Tingkat Keparahan)

**Definisi:** Mengukur **dampak teknis** atau **tingkat kerusakan** yang diakibatkan oleh bug pada sistem.

| Tingkat | Dampak Teknis | Contoh Sederhana |
| :--- | :--- | :--- |
| **1. CRITICAL** | Fungsi utama aplikasi **lumpuh total** (*crash*) atau data vital hilang. | "Aplikasi mati total saat *checkout*." |
| **2. MAJOR** | Fungsi penting (vital) tidak bisa digunakan, tetapi bagian lain masih bekerja. | "Tombol pembayaran rusak, tapi halaman *login* normal." |
| **3. MEDIUM** | Fungsi berjalan, tetapi ada *bug* yang mengganggu atau menyebabkan inkonsistensi. | "Tampilan tabel di halaman admin berantakan." |
| **4. MINOR** | Masalah kosmetik (tampilan), *typo*, atau masalah kecil di area yang jarang diakses. | "*Typo* di *placeholder* kolom pencarian." |

***

### B. ✅ Priority (Prioritas)

**Definisi:** Mengukur **tingkat urgensi** dari sudut pandang bisnis atau waktu rilis. Menentukan **seberapa cepat** bug harus diperbaiki.

| Tingkat | Urgensi | Siapa yang Menentukan |
| :--- | :--- | :--- |
| **P1 - IMMEDIATE** | **Harus segera diperbaiki.** Mendatangkan kerugian bisnis/reputasi besar. | PM / PO |
| **P2 - HIGH** | Harus diperbaiki **sebelum rilis berikutnya** atau siklus *sprint* berikutnya. | PM / PO |
| **P3 - MEDIUM** | Perbaikan bisa dijadwalkan dan dilakukan jika ada waktu luang. | PM / PO |
| **P4 - LOW** | Perbaikan bisa ditunda jauh atau dikerjakan belakangan. | PM / PO |

***

## III. 💡 Contoh Kasus Penerbangan (Severity vs Priority)

| Skenario Bug | Severity | Priority | Alasan Kunci |
| :--- | :--- | :--- | :--- |
| **Crash Pembayaran** | **Critical** (Fungsi inti mati) | **P1 - Immediate** (Kerugian uang langsung) | **S TINGGI, P TINGGI.** Harus diperbaiki detik itu juga. |
| **Typos di Judul Email Resmi** | **Minor** (Hanya tampilan) | **P2 - High** (Dampak citra merek) | **S RENDAH, P TINGGI.** Masalah kecil tapi terlihat oleh banyak pelanggan. |
| **Tombol *Refund* Lama Rusak** | **Major** (Fungsi *refund* gagal) | **P4 - Low** (Fitur jarang diakses) | **S TINGGI, P RENDAH.** Dampak teknis tinggi, tapi urgensi bisnis rendah. |
