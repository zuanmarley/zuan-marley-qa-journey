# 🛡️ Quality Assurance (QA): Penjamin Kualitas Software

Quality Assurance (QA) adalah peran krusial dalam siklus pengembangan perangkat lunak yang berfokus pada **pencegahan** masalah dan **penjaminan kualitas** produk akhir.

---

## 🎯 Apa Itu QA?

QA adalah **Penjaga Kualitas** yang bertujuan untuk memastikan bahwa software berjalan dengan **benar** dan bekerja **sempurna** sebelum dipublikasikan (`publish`).

## 👨‍💻 Peran & Tanggung Jawab QA

### 1. Peran Utama QA dalam Software:

* **Menjamin Kualitas Produk:** Memastikan software stabil dan berfungsi optimal.
* **Menjamin Kenyamanan User:** Memberikan *User Experience* (UX) yang baik.
* **Memastikan Kesesuaian Spesifikasi:** Memastikan produk sesuai dengan semua persyaratan teknis dan fungsional.
* **Mengurangi Risiko Kegagalan:** Mendeteksi dan mencegah kesalahan sejak dini.

### 2. Tugas Utama QA:

1.  **Perencanaan Pengujian:** Membuat **Test Scenario** dan **Test Case** berdasarkan kebutuhan.
2.  **Melakukan Testing:** Menjalankan berbagai jenis pengujian (*Functional, Performance, Manual & Automation*).
3.  **Membuat Dokumentasi:** Menyusun laporan hasil pengujian dan laporan *bug*.
4.  **Validasi Perubahan:** Memastikan pembaruan (*update*) tidak merusak fitur yang sudah ada.
5.  **Memberikan Feedback:** Berkolaborasi dengan developer untuk perbaikan berkelanjutan.

---

## 🔄 SDLC & STLC: Siklus Pengembangan & Pengujian

Dua konsep siklus ini mendasari semua proses rekayasa perangkat lunak:

### 1. SDLC (Software Development Life Cycle)

| Konsep | Penjelasan |
| :--- | :--- |
| **Definisi** | Serangkaian tahapan sistematis yang diikuti **seluruh tim** untuk merancang, membuat, dan memelihara sebuah software. |
| **Sederhana** | SDLC adalah **ROADMAP** proyek yang memandu proses pembuatan software dari ide hingga pemeliharaan. |

### 2. STLC (Software Testing Life Cycle)

| Konsep | Penjelasan |
| :--- | :--- |
| **Definisi** | Serangkaian tahapan sistematis yang diikuti **tim QA** untuk menguji software secara efektif dan efisien. |
| **Fokus** | Memastikan software sudah **sesuai spesifikasi** dan **bebas dari bug**. |

---

## 💡 Mengapa QA Sangat Penting? (Business Value)

Peran QA memberikan nilai strategis yang berdampak langsung pada keberhasilan bisnis:

| Faktor Penting | Penjelasan Dampak |
| :--- | :--- |
| **Menghemat Biaya** | Mencegah *bug* pada tahap awal jauh lebih cepat dan efisien. Memperbaiki *bug* setelah peluncuran bisa **10 hingga 100x lebih mahal**. |
| **Meningkatkan Loyalitas User** | Menjamin *User Experience* yang baik, memastikan software **bebas *crash*** dan **stabil**. |
| **Menjaga Reputasi & Keamanan** | Mencegah peluncuran *software* dengan *bug* fatal dan melakukan **Security Testing** untuk data user. |
| **Memastikan Kepatuhan** | Memastikan software sesuai dengan fungsionalitas dan mematuhi **regulasi standar** industri yang ketat. |

---

# 🔬 Level & Jenis Pengujian (*Testing*)

Aktivitas pengujian dibagi berdasarkan level dan jenisnya untuk memastikan cakupan kualitas yang komprehensif.

## A. Testing Levels (Tingkatan Pengujian)

| Level | Fokus Pengujian | Pelaku Utama |
| :--- | :--- | :--- |
| **Unit Testing** | Menguji kode yang paling kecil (satuan/fungsi), memastikan kode bekerja seharusnya. | Developer |
| **Integration Testing** | Menguji bagaimana dua atau lebih modul kode saling "nyambung" dan bekerja sama dengan baik. | Developer & QA |
| **System Testing** | Menguji **keseluruhan aplikasi** (*end-to-end*) sebagai satu kesatuan terhadap semua persyaratan. | QA |
| **UAT (User Acceptance Testing)** | Tes terakhir di mana **calon *user*** atau *stakeholder* menguji aplikasi untuk memastikan aplikasi **benar-benar bisa digunakan** untuk menyelesaikan masalah bisnis. | Stakeholder/User didampingi QA |

## B. Testing Types (Jenis Pengujian)

### Functional Testing (Menguji Fungsionalitas)

| Jenis Tes | Tujuan / Fokus |
| :--- | :--- |
| **Smoke/Sanity Testing** | Memastikan fitur-fitur utama aplikasi masih berjalan dengan baik setelah ada perubahan kode baru (Jika gagal, tes lanjut tidak perlu dilakukan). |
| **Regression Testing** | Menguji ulang fitur-fitur yang sudah diuji sebelumnya untuk memastikan perubahan atau penambahan fitur baru **tidak merusak** fungsi lama. |

### Non-Functional Testing (Menguji Aspek Non-Fungsional)

| Jenis Tes | Tujuan / Fokus |
| :--- | :--- |
| **Performance Testing** | Menguji kecepatan, stabilitas, dan respons aplikasi saat digunakan oleh banyak *user*. |
| **Load Testing** | Menguji performa sistem di bawah beban (jumlah pengguna) yang diperkirakan atau maksimal. |
| **Stress Testing** | Menguji sistem di bawah beban **sangat tinggi** (melebihi batas normal) untuk melihat titik rusak/ *crash* sistem. |
| **Security Testing** | Menguji kerentanan sistem terhadap serangan dari luar (misalnya *hacking* atau pencurian data). |
| **Usability Testing** | Menguji apakah aplikasi sudah **user friendly** (mudah digunakan). |
| **Compatibility Testing** | Menguji apakah aplikasi berjalan baik di berbagai lingkungan (misalnya di browser Chrome, Firefox, atau OS Android vs iOS). |
