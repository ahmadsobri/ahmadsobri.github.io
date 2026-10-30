---
layout: post
title: "AI Writes the Code: What's Left for Engineers?"
date: 2026-10-30 14:00:00 +0700
categories:
  - Software Engineering
tags:
  - AI
  - Software Engineering
  - Future of Work
description: "Exploring how AI is changing software engineering and the evolving role of engineers."
---
# Memahami Masa Depan Software Engineer di Era AI: Apa yang Tersisa Ketika AI Sudah Bisa Menulis Kode?

Pembahasan video: **"AI Writes the Code. So What's Left for Engineers?"** — Laurie Voss, Arize AI

---

## 1. Gambaran besar: Apa sebenarnya pesan utama pembicara?

Ada satu pertanyaan besar yang ingin disampaikan Laurie Voss melalui presentasi ini:

Jika AI sudah mampu menulis kode dengan cepat, lalu apa pekerjaan yang masih harus dilakukan oleh seorang software engineer?

Dahulu, pekerjaan utama seorang software engineer adalah menerjemahkan kebutuhan menjadi kode program. Kita menghabiskan banyak waktu untuk:

- Menulis function dan class.
- Membuat API dan database.
- Memperbaiki bug.
- Membuat unit test.
- Melakukan refactoring.
- Mengembangkan fitur aplikasi.

Namun, dengan hadirnya AI coding agents seperti Claude Code, GitHub Copilot, Cursor, dan berbagai AI agent lainnya, sebagian besar aktivitas tersebut mulai bisa dikerjakan oleh AI.

Menurut Laurie, perubahan ini akan menggeser nilai seorang software engineer.

Dahulu, perusahaan membutuhkan engineer yang jago menulis kode. Ke depannya, perusahaan akan semakin membutuhkan engineer yang mampu:

1. Memahami masalah pengguna.
2. Menentukan solusi yang tepat.
3. Mendefinisikan seperti apa solusi yang berkualitas.
4. Mengarahkan AI untuk membangun solusi tersebut.
5. Memastikan hasil akhirnya benar-benar memberikan manfaat.

Laurie menyebut peran baru ini sebagai **Product Engineer**.

Supaya lebih mudah dipahami, mari kita bahas satu per satu.

---

## 2. Coding menjadi semakin murah karena AI

`01:19 – 03:04`

Laurie menjelaskan bahwa AI coding agents telah membuat aktivitas menulis kode menjadi hampir gratis.

Bukan berarti AI benar-benar tidak membutuhkan biaya. AI tetap membutuhkan biaya penggunaan token, infrastruktur, dan layanan komputasi.

Namun, jika dibandingkan dengan waktu yang dahulu dibutuhkan seorang developer untuk menulis kode secara manual, biaya tersebut menjadi relatif sangat kecil.

### Apa dampaknya?

Sebelum AI berkembang:

Misalnya, seorang developer membutuhkan waktu 5 jam untuk membuat sebuah fitur sederhana.

Setelah menggunakan AI coding agent, pekerjaan menulis kode tersebut mungkin hanya membutuhkan waktu 30 menit.

Artinya, kemampuan menghasilkan kode meningkat secara signifikan.

Namun, ada masalah yang menarik.

Laurie menyebutkan data bahwa developer yang menggunakan autonomous coding agents menghasilkan sekitar 741% lebih banyak kode atau sekitar 8 kali lipat, tetapi kecepatan pengiriman software ke pengguna hanya meningkat sekitar 30%.

**Perbandingan produktivitas berdasarkan data yang disampaikan pembicara**

| Metrik | Peningkatan |
|---|---|
| Jumlah kode yang dihasilkan | **8x** (sekitar 741%) |
| Kecepatan pengiriman software | **+30%** |

*Peningkatan delivery, bukan peningkatan jumlah kode.*

Angka tersebut merupakan data yang dikutip dalam presentasi, bukan hasil pengukuran universal untuk semua perusahaan.

### Mengapa bisa begitu?

Karena menulis kode hanyalah salah satu bagian dari proses pengembangan software.

Setelah kode dibuat, masih ada pekerjaan lain:

- Code review.
- Testing.
- Validasi kebutuhan.
- Security checking.
- Deployment.
- Monitoring.
- Maintenance.

AI mempercepat proses coding, tetapi proses lainnya belum tentu ikut menjadi lebih cepat.

### Analogi sederhana

Bayangkan sebuah restoran.

Sebelumnya, koki membutuhkan waktu 30 menit untuk memasak satu pesanan.

Kemudian restoran membeli mesin otomatis yang mampu memasak 10 pesanan dalam waktu yang sama.

Apakah pelanggan otomatis mendapatkan makanan 10 kali lebih cepat?

Belum tentu.

Karena:

- Pelayan masih harus mencatat pesanan.
- Kasir masih harus memproses pembayaran.
- Makanan masih harus diperiksa kualitasnya.
- Kurir masih harus mengantarkannya.

Mesin memasak bukan lagi masalah. Hambatannya berpindah ke bagian lain.

**Inilah fenomena utama yang ingin disampaikan Laurie: ketika coding menjadi lebih cepat, hambatan pengembangan software berpindah ke aktivitas lainnya.**

---

## 3. Bottleneck berpindah dari coding ke code review

`03:04 – 08:02`

Bottleneck adalah titik yang menghambat keseluruhan proses pekerjaan.

Dalam software development, code review merupakan salah satu bottleneck terbesar ketika AI sudah mampu menghasilkan kode dalam jumlah besar.

### Apa itu code review?

Code review adalah proses memeriksa kode yang dibuat oleh developer sebelum kode tersebut digabungkan ke codebase utama atau dirilis ke production.

Tujuannya untuk memastikan:

- Logika program sudah benar.
- Tidak ada bug yang berbahaya.
- Kode mudah dipahami.
- Tidak merusak fitur lainnya.
- Tidak menimbulkan masalah performa.
- Sudah mengikuti standar arsitektur dan coding convention.

### Contoh

Misalnya, AI membuat fitur pembayaran.

Kode tersebut terlihat benar dan bahkan berhasil melewati unit test.

Tetapi ternyata AI membuat kesalahan pada proses penghitungan total pembayaran ketika pengguna menggunakan diskon dan pajak secara bersamaan.

Jika tidak diperiksa, kesalahan tersebut bisa menyebabkan kerugian finansial.

### Mengapa code review menjadi masalah?

Bayangkan AI menghasilkan pull request (PR) yang berisi 10.000 baris perubahan kode.

Developer tetap harus memeriksa perubahan tersebut.

Laurie mengutip penelitian Cisco yang menyatakan bahwa kemampuan manusia dalam memahami dan memeriksa kode menurun drastis ketika volume pemeriksaan melewati sekitar 450 baris per jam.

Artinya, semakin banyak kode yang dihasilkan AI, semakin besar beban pemeriksaan yang harus ditanggung manusia.

### Apakah code review bisa sepenuhnya diserahkan kepada AI?

Menurut Laurie, belum sepenuhnya.

AI code reviewer memang dapat menemukan bug, tetapi masing-masing AI reviewer bisa menemukan masalah yang berbeda.

Bahkan, beberapa reviewer AI bisa melewatkan bug yang ditemukan oleh reviewer lainnya.

### Mengapa?

Karena memahami apakah kode benar-benar layak digabungkan bukan sekadar memastikan kode berhasil dijalankan.

Seorang senior engineer biasanya juga mempertimbangkan:

- Apakah kode sesuai dengan arsitektur aplikasi?
- Apakah perubahan ini akan mengganggu sistem lain?
- Apakah ada efek samping?
- Apakah kode sesuai dengan kebiasaan dan standar tim?
- Apakah solusi ini tepat untuk kebutuhan bisnis?
- Ada konteks yang tidak selalu tertulis di dalam repository.

### Contoh nyata

Misalnya, AI membuat endpoint:

```javascript
app.post("/api/transfer", async (req, res) => {
  const { from, to, amount } = req.body;

  await transferMoney(from, to, amount);

  res.json({ success: true });
});
```

Secara sintaks, kode tersebut terlihat sederhana.

Namun, senior engineer mungkin langsung mempertanyakan:

- Apakah pengguna memiliki hak untuk mengakses rekening `from`?
- Apakah saldo mencukupi?
- Bagaimana jika request terkirim dua kali?
- Bagaimana jika proses transfer berhasil tetapi penyimpanan transaksi gagal?
- Apakah transaksi database menggunakan mekanisme rollback?
- Bagaimana jika terjadi request secara bersamaan?

AI bisa menghasilkan kode yang terlihat benar, tetapi belum tentu memahami seluruh konsekuensi dari kode tersebut.

---

## 4. Theory of Constraints: Ketika satu masalah selesai, masalah lain muncul

`08:02 – 09:00`

Laurie memperkenalkan konsep **Theory of Constraints** dari Eliyahu M. Goldratt, yang dijelaskan dalam bukunya berjudul [*The Goal*](https://www.goodreads.com/book/show/113934.The_Goal).

Inti teorinya adalah:

**Setiap sistem memiliki bottleneck utama. Meningkatkan kecepatan bagian lain tidak akan meningkatkan performa keseluruhan secara signifikan jika bottleneck utamanya belum diselesaikan.**

Ketika bottleneck berhasil diperbaiki, biasanya hambatan akan berpindah ke bagian lainnya.

### Contoh dalam software development

**Perpindahan bottleneck dalam proses software development**

1. **Tahap 1 — Coding**
   *Semakin mudah diotomatisasi*

   AI mampu menghasilkan kode dengan sangat cepat.

2. **Tahap 2 — Code Review**
   *Bottleneck saat ini*

   Manusia kesulitan memeriksa kode yang dihasilkan AI dalam jumlah besar.

3. **Tahap 3 — Operations**
   *Bottleneck berikutnya*

   Bagaimana cara deployment, scaling, dan mengelola sistem?

4. **Tahap 4 — Security**
   *Bottleneck selanjutnya*

   Bagaimana memastikan aplikasi aman, data terlindungi, dan sistem tidak disalahgunakan?

5. **Tahap 5 — Product Understanding**
   *Peran manusia yang diprediksi tetap penting*

   Menentukan apa yang sebenarnya dibutuhkan pengguna dan seperti apa solusi yang tepat.

Laurie memperkirakan bahwa code review, operations, dan security secara bertahap akan semakin bisa diotomatisasi oleh AI.

Namun, ia berpendapat bahwa memahami kebutuhan manusia dan menentukan definisi kualitas akan menjadi hambatan yang jauh lebih sulit untuk diotomatisasi.

Perlu dicatat bahwa ini adalah prediksi Laurie, bukan kepastian bahwa semua pekerjaan tersebut akan sepenuhnya digantikan AI.

---

## 5. Hal yang sulit digantikan AI: Memahami kebutuhan manusia

`11:21 – 13:45`

Inilah salah satu bagian paling penting dalam presentasi.

Menurut Laurie, AI bisa membantu membuat software, tetapi belum tentu mengetahui software seperti apa yang sebenarnya dibutuhkan seseorang.

### Mengapa?

Karena kebutuhan pengguna sering kali tidak bisa dijelaskan hanya melalui instruksi teknis.

### Contoh: Aplikasi pencatatan pesanan

Bayangkan seorang pemilik toko berkata:

> "Saya ingin aplikasi untuk mencatat pesanan pelanggan."

Instruksi tersebut terdengar sederhana.

Seorang developer mungkin langsung berpikir untuk membuat:

- Form input pesanan.
- Database pesanan.
- Halaman daftar pesanan.
- Fitur update status pesanan.
- Fitur pencarian pesanan.

AI bisa membuat semua fitur tersebut.

Tetapi apakah aplikasi itu sudah sesuai kebutuhan pemilik toko?

Belum tentu.

Mari kita lihat tiga jenis bisnis yang berbeda.

**Bisnis bakery**

Pemilik toko membutuhkan pencatatan pesanan kue berdasarkan tanggal pengambilan, jenis kue, ukuran, dan permintaan khusus pelanggan.

**Toko spare part**

Pemilik toko membutuhkan pencatatan pesanan berdasarkan nomor part, kompatibilitas kendaraan, jumlah stok, dan supplier.

**Perusahaan manufaktur**

Perusahaan membutuhkan pencatatan pesanan berdasarkan spesifikasi produk, kapasitas produksi, bahan baku, dan jadwal pengiriman.

Ketiganya sama-sama membutuhkan sistem pencatatan pesanan.

Tetapi kebutuhan bisnis, aturan operasional, dan definisi keberhasilannya sangat berbeda.

Inilah mengapa developer tidak boleh hanya menerima requirement lalu langsung coding.

Developer perlu menggali informasi lebih dalam.

### Apa yang harus dilakukan developer?

Misalnya, ketika bertemu dengan pemilik bakery, jangan hanya bertanya:

> "Fitur apa yang Anda inginkan?"

Cobalah bertanya:

- Bagaimana proses pemesanan kue saat ini?
- Apa masalah terbesar yang sering terjadi?
- Bagaimana cara mencatat pesanan custom?
- Bagaimana jika pelanggan mengubah tanggal pengambilan?
- Bagaimana cara mengetahui kapasitas produksi harian?
- Informasi apa yang paling penting bagi karyawan toko?

Dari jawaban tersebut, developer dapat memahami masalah sebenarnya.

**Intinya: pengguna sering menyampaikan solusi yang mereka bayangkan, sedangkan tugas engineer adalah menemukan masalah yang sebenarnya perlu diselesaikan.**

---

## 6. Essential Complexity vs Accidental Complexity

`13:45 – 16:34`

Laurie mengutip pemikiran Fred Brooks, penulis buku *The Mythical Man-Month*.

Brooks membagi kompleksitas software menjadi dua jenis.

### A. Accidental Complexity

Kompleksitas yang muncul karena keterbatasan tools, bahasa pemrograman, atau cara kita mengimplementasikan sesuatu.

Contohnya:

- Mengingat sintaks JavaScript.
- Menulis boilerplate code.
- Membuat konfigurasi proyek.
- Menulis kode CRUD.
- Mengatur struktur folder.
- Menghubungkan library.
- Menulis kode repetitif.

Hal-hal tersebut relatif mudah dibantu atau diotomatisasi oleh AI.

Contoh:

Dahulu developer perlu menulis kode API secara manual.

Sekarang kita bisa meminta AI:

```text
Buatkan REST API untuk manajemen produk
menggunakan Express.js dan PostgreSQL.

Buat endpoint:
- GET /products
- GET /products/:id
- POST /products
- PUT /products/:id
- DELETE /products/:id

Sertakan validasi input dan error handling.
```

AI bisa membantu menghasilkan sebagian besar implementasinya.

### B. Essential Complexity

Kompleksitas yang memang berasal dari masalah yang ingin diselesaikan.

Contohnya:

- Bagaimana menentukan harga produk?
- Bagaimana menangani refund?
- Bagaimana menghitung biaya pengiriman?
- Bagaimana mengelola stok barang?
- Bagaimana menghindari transaksi ganda?
- Bagaimana menentukan hak akses pengguna?
- Bagaimana sistem harus bekerja ketika terjadi kegagalan?

Ini lebih sulit karena membutuhkan pemahaman terhadap konteks bisnis dan konsekuensi keputusan.

### Perbandingan sederhana

| Accidental Complexity | Essential Complexity |
|---|---|
| Bagaimana menulis kode? | Apa yang harus dibuat? |
| Bagaimana membuat API? | API harus menyelesaikan masalah apa? |
| Bagaimana membuat database? | Data apa yang perlu disimpan? |
| Bagaimana membuat validasi? | Aturan bisnis apa yang harus divalidasi? |
| Bagaimana memperbaiki syntax error? | Apakah solusi yang dibuat sudah benar? |

### Analogi

Bayangkan Anda diminta membangun sebuah rumah.

**Accidental complexity** adalah bagaimana menggunakan palu, memasang bata, mengukur kayu, dan mencampur semen.

**Essential complexity** adalah menentukan:

- Rumah tersebut untuk siapa?
- Berapa jumlah penghuninya?
- Berapa jumlah kamar yang diperlukan?
- Apakah harus tahan banjir?
- Bagaimana sirkulasi udara?
- Bagaimana desainnya agar nyaman?

AI dapat membantu proses pembangunan rumah menjadi lebih cepat.

Namun, jika desain rumahnya salah sejak awal, pembangunan yang cepat justru akan menghasilkan rumah yang salah dengan lebih cepat.

**Kesimpulannya, AI sangat membantu mengurangi kesulitan teknis dalam coding, tetapi menentukan solusi yang tepat tetap membutuhkan pemahaman masalah yang mendalam.**

---

## 7. Product Engineer: Peran baru seorang software engineer

`16:34 – 19:45`

Inilah konsep utama yang diperkenalkan Laurie.

Ia menyebut peran baru tersebut sebagai **Product Engineer**.

Product Engineer adalah engineer yang tidak hanya bertanggung jawab menulis kode, tetapi juga memahami pengguna, menemukan masalah, menentukan solusi, dan memastikan software yang dibuat memberikan nilai nyata.

Dengan kata lain:

**Product Engineer adalah seseorang yang menggabungkan kemampuan software engineering dengan pemahaman produk dan bisnis.**

### Perbedaan Software Engineer tradisional dan Product Engineer

| Software Engineer tradisional | Product Engineer |
|---|---|
| Menerima task dari PM | Ikut menemukan kebutuhan pengguna |
| Fokus implementasi | Fokus hasil dan dampak |
| Menerjemahkan requirement ke kode | Mengubah masalah menjadi spesifikasi |
| Menyelesaikan tiket | Menyelesaikan masalah pengguna |
| Banyak menulis kode manual | Mengarahkan AI untuk membangun solusi |
| Mengukur jumlah pekerjaan selesai | Mengukur keberhasilan produk |

Perlu dipahami bahwa ini merupakan perbandingan model kerja yang disederhanakan, bukan berarti software engineer tradisional tidak pernah memahami produk.

### Contoh kasus nyata

Misalnya, Anda bekerja di perusahaan e-commerce.

Product Manager memberikan tiket:

```text
Task:
Implementasikan fitur voucher diskon.

Requirement:
- User bisa memasukkan kode voucher.
- Sistem menghitung diskon.
- Diskon ditampilkan pada checkout.
```

Seorang developer yang hanya berorientasi pada implementasi mungkin langsung meminta AI membuat fitur tersebut.

Sementara Product Engineer akan menggali lebih dalam:

- Apakah voucher berlaku untuk semua produk?
- Apakah ada minimum pembelian?
- Apakah voucher bisa digunakan bersamaan?
- Apakah voucher memiliki batas penggunaan?
- Bagaimana jika voucher kedaluwarsa ketika pengguna checkout?
- Bagaimana jika dua pengguna menggunakan kuota terakhir secara bersamaan?
- Apakah voucher bisa digunakan untuk produk yang sedang diskon?

Setelah memahami aturan tersebut, Product Engineer menyusun spesifikasi yang jelas.

Kemudian AI digunakan untuk membantu:

- Mendesain database.
- Membuat API.
- Membuat business logic.
- Menulis unit test.
- Membuat integration test.
- Menyusun dokumentasi.

Engineer tetap bertanggung jawab terhadap keputusan dan hasil akhirnya.

### Alur kerja Product Engineer

1. **Memahami pengguna**
   Mengidentifikasi masalah dan kebutuhan sebenarnya.

   ↓

2. **Membuat spesifikasi (spec)**
   Menentukan fitur, aturan bisnis, batasan, dan kriteria keberhasilan.

   ↓

3. **AI Coding Agent**
   Membantu menulis kode, test, dokumentasi, dan implementasi.

   ↓

4. **Validasi dan evaluasi**
   Memastikan implementasi sesuai kebutuhan dan aman.

   ↓

5. **Release ke production**
   Meluncurkan produk dan memantau dampaknya kepada pengguna.

Ada satu kalimat penting dari Laurie:

> Engineer yang memahami pengguna, bisa mengambil keputusan tentang apa yang harus dibangun, dan langsung membangunnya akan mampu bekerja dengan sangat cepat.

---

## 8. Masalah besar: Bagaimana nasib Junior Developer?

`19:45 – 22:57`

Menurut saya, ini adalah bagian yang paling perlu diperhatikan oleh developer junior.

Laurie mengangkat sebuah masalah yang cukup serius: bagaimana perusahaan akan melatih junior developer jika pekerjaan yang dahulu diberikan kepada junior sekarang bisa dikerjakan AI?

### Bagaimana sistem pembelajaran junior developer sebelumnya?

Biasanya, perjalanan seorang junior developer seperti ini:

1. Senior memberikan task yang spesifik.
2. Junior mengerjakan task tersebut.
3. Junior membuat pull request.
4. Senior melakukan code review.
5. Senior memberikan masukan dan koreksi.
6. Junior memperbaiki kesalahan dan belajar dari pengalaman.

Misalnya, senior memberikan task:

```text
Buat REST API untuk CRUD data customer
menggunakan Express.js.

Gunakan PostgreSQL.
Tambahkan validasi input.
Buat unit test.
```

Junior mengerjakan task tersebut dan belajar dari kesalahan.

Namun, sekarang AI bisa mengerjakan task yang sama dalam waktu singkat.

Artinya, perusahaan mulai mempertanyakan:

> "Kalau AI bisa mengerjakan pekerjaan junior, untuk apa kita merekrut banyak junior developer?"

Inilah yang disebut Laurie sebagai **masalah junior developer**.

### Dampaknya terhadap industri

Dalam presentasinya, Laurie menunjukkan data statistik ketenagakerjaan Amerika Serikat sejak Januari 2023.

Ia menyampaikan bahwa:

- Lapangan pekerjaan untuk engineer usia 22–25 tahun mengalami penurunan.
- Pekerjaan untuk engineer usia 41–49 tahun justru meningkat.
- Senior engineer tetap memiliki nilai yang tinggi.
- Junior developer semakin kesulitan mendapatkan pekerjaan.

Perlu dicatat, data tersebut menggambarkan kondisi pasar tenaga kerja yang dibahas dalam presentasi, bukan gambaran pasti seluruh negara atau semua perusahaan.

### Mengapa ini menjadi masalah besar?

Karena senior engineer tidak muncul begitu saja.

Senior engineer berasal dari junior developer yang mendapatkan kesempatan untuk belajar, melakukan kesalahan, memperbaiki kode, dan memahami sistem secara bertahap.

Jika perusahaan berhenti merekrut junior, siapa yang akan menjadi senior engineer lima atau sepuluh tahun mendatang?

Inilah masalah regenerasi talenta yang disoroti Laurie.

### Bagaimana seharusnya junior developer belajar?

Menurut arah pemikiran Laurie, junior developer perlu mulai dilatih bukan hanya untuk menulis kode, tetapi juga untuk memahami masalah dan kebutuhan pengguna.

Misalnya, daripada hanya diberikan task:

```text
Buat halaman dashboard menggunakan React.
```

Junior bisa diberikan tugas yang lebih komprehensif:

```text
Pelajari proses bisnis toko terlebih dahulu.

Cari tahu masalah yang dialami pemilik toko
ketika mengelola stok barang.

Identifikasi kebutuhan pengguna.

Buat spesifikasi solusi.

Gunakan AI untuk membantu implementasi.

Validasi apakah solusi tersebut benar-benar
menyelesaikan masalah pengguna.
```

Dengan cara tersebut, junior belajar berpikir seperti seorang engineer yang memahami produk, bukan sekadar seseorang yang bisa menggunakan framework.

---

## 9. Apakah orang yang suka coding harus meninggalkan dunia programming?

`22:57 – 25:11`

Laurie menyadari bahwa banyak orang masuk ke dunia software engineering karena memang menyukai aktivitas programming.

Mereka menikmati:

- Menulis kode.
- Memecahkan bug yang sulit.
- Membuat algoritma.
- Mendesain arsitektur.
- Membuat abstraksi yang elegan.
- Mengoptimalkan performa aplikasi.

Namun, jika AI semakin banyak mengambil alih aktivitas coding, pekerjaan engineer mungkin akan lebih banyak melibatkan komunikasi, analisis, dan pengambilan keputusan.

Tidak semua programmer akan menyukai perubahan ini.

Laurie memberikan analogi yang menarik:

**Programmer akan tetap melakukan programming seperti penyanyi tetap bernyanyi dan tukang kayu tetap membuat furnitur, meskipun industri musik dan furnitur sudah memiliki mesin produksi.**

Artinya, programming sebagai sebuah keterampilan dan aktivitas kreatif tidak akan hilang.

Orang tetap bisa menikmati coding, membuat proyek pribadi, bereksperimen dengan teknologi, dan mengembangkan open-source software.

Namun, aktivitas menulis kode secara manual mungkin tidak lagi menjadi alasan utama perusahaan membayar seorang engineer dengan kompensasi tinggi.

Perusahaan akan lebih menghargai kemampuan engineer dalam menghasilkan solusi yang benar-benar dibutuhkan.

---

## 10. Apa yang harus dilakukan developer mulai sekarang?

`25:11 – 27:01`

Pada bagian terakhir, Laurie memberikan beberapa arahan praktis.

Mari kita terjemahkan menjadi tindakan yang relevan untuk software engineer, khususnya junior developer.

### A. Mulai terbiasa bekerja dengan AI coding agents

Jangan menganggap AI hanya sebagai alat untuk bertanya tentang syntax.

Mulailah memanfaatkan AI untuk membantu seluruh proses development.

Contoh tools yang bisa dipelajari:

- [Claude Code](https://claude.com/claude-code) — membantu memahami repository, menulis kode, dan menjalankan pekerjaan coding.
- [Cursor](https://cursor.com) — membantu pengembangan software dengan AI di dalam editor.
- [GitHub Copilot](https://github.com/features/copilot) — membantu coding dan code review.
- [OpenAI Codex](https://openai.com/codex) — membantu mengerjakan tugas pengembangan software.

Jangan hanya belajar bagaimana memberikan prompt agar AI menghasilkan kode.

Belajarlah bagaimana memberikan konteks, membagi pekerjaan, memeriksa hasil, dan mengevaluasi implementasi AI.

### B. Fokus pada kode yang memiliki risiko tinggi

Laurie menyarankan agar engineer lebih selektif dalam melakukan code review manual.

Prioritaskan kode yang memiliki dampak besar apabila terjadi kesalahan.

Contohnya:

- Authentication dan authorization.
- Payment dan financial transactions.
- Database migration.
- Security configuration.
- Data privacy.
- Core business logic.
- Infrastruktur production.

Sementara pekerjaan yang lebih mudah diverifikasi dapat dibantu oleh automated reviewer dan automated tests.

Tetapi ingat, otomatisasi bukan berarti tidak perlu pengawasan.

### C. Buat standar kualitas yang jelas

Jangan hanya memberikan instruksi kepada AI seperti:

> "Buatkan kode yang bagus."

Instruksi tersebut terlalu abstrak.

Tuliskan standar kualitas yang dapat diperiksa.

Contoh:

```text
Coding standards:

1. Gunakan TypeScript.
2. Terapkan separation of concerns.
3. Semua endpoint wajib melakukan input validation.
4. Jangan menyimpan password dalam bentuk plain text.
5. Semua database operation harus menangani error.
6. Buat unit test untuk business logic.
7. Gunakan transaction untuk proses finansial.
8. Pastikan tidak ada data sensitif di dalam log.
```

Dengan aturan yang jelas, AI memiliki pedoman untuk menghasilkan kode yang sesuai standar tim.

Laurie menyebut pentingnya mengubah pengetahuan dan penilaian senior engineer menjadi specification, rules, dan evaluation criteria yang dapat dipahami mesin.

### D. Belajar membuat specification yang baik

Ini merupakan salah satu keterampilan yang paling penting untuk masa depan.

Sebelum meminta AI membuat fitur, Anda harus mampu menjelaskan:

- Apa masalahnya?
- Siapa penggunanya?
- Mengapa masalah tersebut harus diselesaikan?
- Bagaimana solusi yang diharapkan?
- Apa saja business rules?
- Apa saja kondisi yang mungkin terjadi?
- Bagaimana cara menguji keberhasilannya?

Contoh specification sederhana:

**Contoh: Spesifikasi fitur pemesanan produk**

**Problem**
Pelanggan kesulitan mengetahui status pesanan setelah melakukan pembelian.

**Goal**
Pelanggan dapat memantau status pesanan secara mandiri.

**Functional requirements**

- Pelanggan dapat melihat daftar pesanan.
- Pelanggan dapat melihat detail pesanan.
- Status pesanan diperbarui ketika admin mengubah status.
- Pelanggan hanya dapat melihat pesanannya sendiri.

**Business rules**

- Status pesanan: pending, paid, processing, shipped, completed, cancelled.
- Pesanan yang sudah completed tidak dapat dibatalkan.
- Perubahan status harus tercatat dalam riwayat.

**Acceptance criteria**

- Pengguna hanya dapat mengakses pesanan miliknya.
- Perubahan status tercermin pada halaman detail.
- Riwayat perubahan status tersimpan dengan benar.
- Sistem menolak transisi status yang tidak valid.

Perhatikan bahwa specification tersebut menjelaskan apa yang harus dilakukan sistem, bukan sekadar bagaimana menulis kodenya.

AI dapat membantu menerjemahkan specification menjadi implementasi.

### E. Ukur hasil, bukan jumlah kode

Laurie memberikan penekanan yang sangat penting:

**741% lebih banyak kode bukanlah tujuan utama.**

Tujuan utama software development adalah menghasilkan software yang bermanfaat dan benar-benar digunakan.

Contoh metrik yang lebih relevan:

| Metrik | Apa yang diukur? |
|---|---|
| Feature delivery time | Seberapa cepat fitur dirilis |
| Defect rate | Seberapa sering bug muncul |
| Production incidents | Seberapa sering sistem mengalami gangguan |
| Test effectiveness | Seberapa baik pengujian menemukan masalah |
| User satisfaction | Seberapa puas pengguna |
| Feature adoption | Seberapa banyak pengguna menggunakan fitur |
| Business impact | Seberapa besar dampak fitur terhadap bisnis |

Contohnya, membuat 100 fitur bukan berarti perusahaan lebih produktif daripada membuat 10 fitur.

Jika 10 fitur tersebut menyelesaikan masalah pelanggan, sedangkan 100 fitur lainnya tidak digunakan, maka 10 fitur tersebut bisa jadi jauh lebih bernilai.

---

# 11. Bagaimana menerapkan pemikiran ini sebagai Junior Developer?

Sekarang kita terjemahkan semua pembahasan tadi menjadi roadmap belajar yang lebih praktis.

Menurut saya, junior developer tidak perlu meninggalkan fundamental programming.

Justru fundamental tersebut tetap menjadi modal untuk memahami, mengarahkan, dan mengevaluasi hasil pekerjaan AI.

Namun, cara belajar perlu diperluas.

## Roadmap pengembangan kemampuan Junior Developer

Urutan pembelajaran yang bisa digunakan sebagai panduan pribadi.

1. **Tahap 1 — Kuasai fundamental programming**

   Pelajari:

   - JavaScript/TypeScript atau bahasa utama Anda.
   - Data structures dan algorithms.
   - OOP dan clean code.
   - Database dan SQL.
   - HTTP, REST API, dan networking.
   - Git dan software development workflow.

   *Tetap wajib*

2. **Tahap 2 — Pahami software engineering**

   Pelajari:

   - System design.
   - Software architecture.
   - Design patterns.
   - Testing.
   - Debugging.
   - Security.
   - Deployment dan monitoring.

   Tujuannya agar Anda memahami kualitas sistem, bukan hanya sintaks.

3. **Tahap 3 — Kuasai AI-assisted development**

   Pelajari:

   - Menggunakan AI coding agents.
   - Memberikan konteks repository.
   - Membuat task breakdown.
   - Membuat specification untuk AI.
   - Memeriksa hasil kode AI.
   - Mengotomatisasi testing dan validation.

4. **Tahap 4 — Belajar memahami kebutuhan bisnis**

   - Identifikasi masalah.
   - Wawancara calon pengguna.
   - Buat requirement.
   - Buat specification.
   - Tentukan arsitektur.
   - Gunakan AI untuk implementasi.
   - Lakukan testing.
   - Deploy.
   - Evaluasi berdasarkan feedback pengguna.

5. **Tahap 5 — Berlatih menjadi Product Engineer**

   Biasakan mengerjakan satu proyek dari awal sampai akhir:

   - Identifikasi masalah.
   - Wawancara calon pengguna.
   - Buat requirement.
   - Buat specification.
   - Tentukan arsitektur.
   - Gunakan AI untuk implementasi.
   - Lakukan testing.
   - Deploy.
   - Evaluasi berdasarkan feedback pengguna.

   Cobalah membuat aplikasi berdasarkan masalah nyata.

   Contoh:

   - Aplikasi manajemen stok toko.
   - Sistem booking salon.
   - Aplikasi pemesanan makanan.
   - Sistem manajemen keuangan UMKM.

   Jangan langsung coding. Cari tahu terlebih dahulu bagaimana pengguna bekerja.

---

## 12. Contoh penerapan: Membangun aplikasi menggunakan pendekatan Product Engineer

Supaya lebih konkret, mari gunakan studi kasus sederhana.

Anda ingin membuat aplikasi manajemen stok untuk toko kelontong.

**Pendekatan developer yang hanya fokus coding:**

1. Membuat project React.
2. Membuat database.
3. Membuat CRUD produk.
4. Membuat halaman dashboard.
5. Membuat fitur laporan.

Hasilnya mungkin aplikasi yang secara teknis berjalan dengan baik.

Tetapi belum tentu menyelesaikan masalah pemilik toko.

**Pendekatan Product Engineer:**

1. Berbicara dengan pemilik toko.
2. Mengetahui bahwa stok sering tidak cocok dengan barang fisik.
3. Menemukan bahwa karyawan lupa mencatat barang masuk dan keluar.
4. Mengetahui bahwa pemilik ingin mendapatkan notifikasi ketika stok menipis.
5. Menentukan kebutuhan sistem berdasarkan proses bisnis tersebut.
6. Membuat specification.
7. Menggunakan AI untuk membantu membuat implementasi.
8. Menguji sistem bersama pemilik toko.
9. Mengumpulkan feedback dan melakukan perbaikan.

Perhatikan perbedaannya.

Pendekatan pertama berorientasi pada pembuatan aplikasi.

Pendekatan kedua berorientasi pada penyelesaian masalah.

Inilah pergeseran pola pikir yang ingin disampaikan Laurie Voss.

---

# 13. Kesimpulan: Masa depan software engineer bukan sekadar tentang siapa yang paling jago coding

Menurut saya, inti presentasi Laurie Voss dapat dirangkum dalam lima poin utama.

1. **AI mengubah nilai aktivitas coding.**
   Menulis kode menjadi semakin murah dan cepat. Kemampuan coding tetap penting, tetapi tidak lagi menjadi satu-satunya keunggulan seorang engineer.

2. **Bottleneck akan terus berpindah.**
   Ketika coding semakin mudah, hambatan berpindah ke code review, operations, security, dan akhirnya pemahaman terhadap kebutuhan pengguna.

3. **Memahami masalah menjadi kemampuan yang sangat berharga.**
   Developer yang mampu memahami kebutuhan pengguna, aturan bisnis, dan konteks sistem akan memiliki keunggulan dalam mengarahkan AI.

4. **Peran Product Engineer akan semakin penting.**
   Engineer tidak hanya bertugas menerjemahkan tiket menjadi kode, tetapi juga menemukan masalah, menentukan solusi, membuat specification, mengarahkan AI, dan memastikan hasilnya memberikan nilai.

5. **Junior developer harus memiliki cara belajar yang lebih luas.**
   Jangan hanya belajar framework dan syntax. Pelajari fundamental programming, software engineering, AI tools, komunikasi, analisis kebutuhan, dan pemahaman bisnis.

> **Pesan terpenting dari video ini**
>
> # Don't just learn how to write code. Learn how to solve problems.
>
> Masa depan software engineering bukan hanya tentang kemampuan menghasilkan kode sebanyak-banyaknya, tetapi tentang kemampuan menentukan kode seperti apa yang perlu dibuat, mengapa kode tersebut harus dibuat, dan bagaimana memastikan kode itu benar-benar menyelesaikan masalah.

---

## Penutup: Saran saya untuk Junior Developer

Ada satu hal yang ingin saya tekankan.

**Jangan salah memahami pesan video ini sebagai tanda bahwa belajar programming sudah tidak penting.**

Justru sebaliknya.

Untuk bisa menjadi Product Engineer yang baik, Anda harus memahami programming dan software engineering secara mendalam.

Bagaimana Anda bisa menilai kode yang dibuat AI jika Anda tidak memahami kode tersebut?

Bagaimana Anda bisa menentukan arsitektur yang tepat jika Anda tidak memahami konsekuensi teknisnya?

Bagaimana Anda bisa memastikan sistem aman jika Anda tidak memahami security?

AI bukan alasan untuk berhenti belajar fundamental.

AI adalah alasan untuk meningkatkan level kemampuan Anda.

Mulailah mengubah pola pikir:

- Dari sekadar menyelesaikan task menjadi menyelesaikan masalah.
- Dari sekadar menulis kode menjadi memahami alasan di balik kode.
- Dari sekadar menggunakan AI menjadi mampu mengarahkan dan mengevaluasi AI.
- Dari sekadar membuat fitur menjadi membangun produk yang memberikan manfaat.
- Dari sekadar berpikir sebagai programmer menjadi berpikir sebagai engineer yang memahami produk.

**Pada akhirnya, developer yang paling bernilai bukan selalu orang yang paling cepat mengetik kode, melainkan orang yang paling mampu menentukan apa yang seharusnya dibangun dan memastikan hasilnya benar-benar berguna.**
