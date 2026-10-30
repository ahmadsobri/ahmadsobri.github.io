Memahami Masa Depan Software Engineer di Era AI: Apa yang Tersisa Ketika AI Sudah Bisa Menulis Kode?

Pembahasan video: AI Writes the Code. So What's Left for Engineers?
Pembicara: Laurie Voss — Head of Developer Relations at Arize AI dan Co-founder npm.

Daftar Isi
Gambaran Besar: Apa Pesan Utama Pembicara?
Coding Menjadi Semakin Murah karena AI
Bottleneck Berpindah dari Coding ke Code Review
Theory of Constraints
Hal yang Sulit Digantikan AI: Memahami Kebutuhan Manusia
Essential Complexity vs Accidental Complexity
Product Engineer: Peran Baru Software Engineer
Masalah Besar: Bagaimana Nasib Junior Developer?
Apakah Orang yang Suka Coding Harus Meninggalkan Programming?
Apa yang Harus Dilakukan Developer Mulai Sekarang?
Roadmap Pengembangan Kemampuan Junior Developer
Studi Kasus: Membangun Aplikasi dengan Pendekatan Product Engineer
Kesimpulan dan Pesan untuk Junior Developer
1. Gambaran Besar: Apa Pesan Utama Pembicara?

Ada satu pertanyaan besar yang ingin disampaikan Laurie Voss melalui presentasinya:

Jika AI sudah mampu menulis kode dengan cepat, lalu apa pekerjaan yang masih harus dilakukan oleh seorang software engineer?

Dahulu, pekerjaan utama seorang software engineer adalah menerjemahkan kebutuhan menjadi kode program. Kita menghabiskan banyak waktu untuk:

Menulis function dan class.
Membuat API dan database.
Memperbaiki bug.
Membuat unit test.
Melakukan refactoring.
Mengembangkan fitur aplikasi.

Namun, dengan hadirnya AI coding agents seperti Claude Code, GitHub Copilot, Cursor, dan berbagai AI agent lainnya, sebagian besar aktivitas tersebut mulai bisa dikerjakan oleh AI.

Menurut Laurie, perubahan ini akan menggeser nilai seorang software engineer.

Dahulu, perusahaan membutuhkan engineer yang jago menulis kode. Ke depannya, perusahaan akan semakin membutuhkan engineer yang mampu:

Memahami masalah pengguna.
Menentukan solusi yang tepat.
Mendefinisikan seperti apa solusi yang berkualitas.
Mengarahkan AI untuk membangun solusi tersebut.
Memastikan hasil akhirnya benar-benar memberikan manfaat.

Laurie menyebut peran baru ini sebagai Product Engineer.

2. Coding Menjadi Semakin Murah karena AI

Timestamp: 01:19 – 03:04

Laurie menjelaskan bahwa AI coding agents telah membuat aktivitas menulis kode menjadi hampir gratis.

Bukan berarti AI benar-benar tidak membutuhkan biaya. AI tetap membutuhkan biaya penggunaan token, infrastruktur, dan layanan komputasi.

Namun, jika dibandingkan dengan waktu yang dahulu dibutuhkan seorang developer untuk menulis kode secara manual, biaya tersebut menjadi relatif sangat kecil.

Apa dampaknya?

Sebelum AI berkembang, misalnya seorang developer membutuhkan waktu 5 jam untuk membuat sebuah fitur sederhana.

Setelah menggunakan AI coding agent, pekerjaan menulis kode tersebut mungkin hanya membutuhkan waktu 30 menit.

Artinya, kemampuan menghasilkan kode meningkat secara signifikan.

Namun, ada masalah yang menarik.

Laurie menyebutkan data bahwa developer yang menggunakan autonomous coding agents menghasilkan sekitar 741% lebih banyak kode atau sekitar 8 kali lipat, tetapi kecepatan pengiriman software ke pengguna hanya meningkat sekitar 30%.

Angka tersebut merupakan data yang dikutip dalam presentasi, bukan hasil pengukuran universal untuk semua perusahaan.

Mengapa bisa begitu?

Karena menulis kode hanyalah salah satu bagian dari proses pengembangan software.

Setelah kode dibuat, masih ada pekerjaan lain:

Code review.
Testing.
Validasi kebutuhan.
Security checking.
Deployment.
Monitoring.
Maintenance.

AI mempercepat proses coding, tetapi proses lainnya belum tentu ikut menjadi lebih cepat.

Analogi sederhana: Restoran

Bayangkan sebuah restoran.

Sebelumnya, koki membutuhkan waktu 30 menit untuk memasak satu pesanan.

Kemudian restoran membeli mesin otomatis yang mampu memasak 10 pesanan dalam waktu yang sama.

Apakah pelanggan otomatis mendapatkan makanan 10 kali lebih cepat?

Belum tentu.

Karena:

Pelayan masih harus mencatat pesanan.
Kasir masih harus memproses pembayaran.
Makanan masih harus diperiksa kualitasnya.
Kurir masih harus mengantarkannya.

Mesin memasak bukan lagi masalah. Hambatannya berpindah ke bagian lain.

Inilah fenomena utama yang ingin disampaikan Laurie: ketika coding menjadi lebih cepat, hambatan pengembangan software berpindah ke aktivitas lainnya.

3. Bottleneck Berpindah dari Coding ke Code Review

Timestamp: 03:04 – 08:02

Bottleneck adalah titik yang menghambat keseluruhan proses pekerjaan.

Dalam software development, code review merupakan salah satu bottleneck terbesar ketika AI sudah mampu menghasilkan kode dalam jumlah besar.

Apa itu Code Review?

Code review adalah proses memeriksa kode yang dibuat oleh developer sebelum kode tersebut digabungkan ke codebase utama atau dirilis ke production.

Tujuannya untuk memastikan:

Logika program sudah benar.
Tidak ada bug yang berbahaya.
Kode mudah dipahami.
Tidak merusak fitur lainnya.
Tidak menimbulkan masalah performa.
Sudah mengikuti standar arsitektur dan coding convention.

Misalnya, AI membuat fitur pembayaran.

Kode tersebut terlihat benar dan bahkan berhasil melewati unit test.

Tetapi ternyata AI membuat kesalahan pada proses penghitungan total pembayaran ketika pengguna menggunakan diskon dan pajak secara bersamaan.

Jika tidak diperiksa, kesalahan tersebut bisa menyebabkan kerugian finansial.

Mengapa Code Review Menjadi Masalah?

Bayangkan AI menghasilkan pull request (PR) yang berisi 10.000 baris perubahan kode.

Developer tetap harus memeriksa perubahan tersebut.

Laurie mengutip penelitian Cisco yang menyatakan bahwa kemampuan manusia dalam memahami dan memeriksa kode menurun drastis ketika volume pemeriksaan melewati sekitar 450 baris per jam.

Artinya, semakin banyak kode yang dihasilkan AI, semakin besar pula beban pemeriksaan yang harus ditanggung manusia.

Apakah Code Review Bisa Sepenuhnya Diserahkan kepada AI?

Menurut Laurie, belum sepenuhnya.

AI code reviewer memang dapat menemukan bug, tetapi masing-masing AI reviewer bisa menemukan masalah yang berbeda.

Bahkan, beberapa reviewer AI bisa melewatkan bug yang ditemukan oleh reviewer lainnya.

Mengapa?

Karena memahami apakah kode benar-benar layak digabungkan bukan sekadar memastikan kode berhasil dijalankan.

Seorang senior engineer biasanya juga mempertimbangkan:

Apakah kode sesuai dengan arsitektur aplikasi?
Apakah perubahan ini akan mengganggu sistem lain?
Apakah ada efek samping?
Apakah kode sesuai dengan kebiasaan dan standar tim?
Apakah solusi ini tepat untuk kebutuhan bisnis?

Ada konteks yang tidak selalu tertulis di dalam repository.

Contoh: Fitur Transfer Uang
javascript
app.post("/api/transfer", async (req, res) => {
  const { from, to, amount } = req.body;

  await transferMoney(from, to, amount);

  res.json({ success: true });
});


Secara sintaks, kode tersebut terlihat sederhana.

Namun, senior engineer mungkin langsung mempertanyakan:

Apakah pengguna memiliki hak untuk mengakses rekening from?
Apakah saldo mencukupi?
Bagaimana jika request terkirim dua kali?
Bagaimana jika proses transfer berhasil tetapi penyimpanan transaksi gagal?
Apakah transaksi database menggunakan mekanisme rollback?
Bagaimana jika terjadi request secara bersamaan?

AI bisa menghasilkan kode yang terlihat benar, tetapi belum tentu memahami seluruh konsekuensi dari kode tersebut.

Pelajaran penting: kemampuan menghasilkan kode tidak sama dengan kemampuan menghasilkan software yang benar, aman, dan sesuai kebutuhan.

4. Theory of Constraints: Ketika Satu Masalah Selesai, Masalah Lain Muncul

Timestamp: 08:02 – 09:00

Laurie memperkenalkan konsep Theory of Constraints dari Eliyahu M. Goldratt, yang dijelaskan dalam bukunya berjudul The Goal.

Inti teorinya adalah:

Setiap sistem memiliki bottleneck utama. Meningkatkan kecepatan bagian lain tidak akan meningkatkan performa keseluruhan secara signifikan jika bottleneck utamanya belum diselesaikan.

Ketika bottleneck berhasil diperbaiki, biasanya hambatan akan berpindah ke bagian lainnya.

Contoh dalam Software Development
Tahap 1 — Coding

AI mampu menghasilkan kode dengan sangat cepat.

Tahap 2 — Code Review

Manusia kesulitan memeriksa kode yang dihasilkan AI dalam jumlah besar.

Tahap 3 — Operations

Bagaimana cara deployment, scaling, dan mengelola sistem?

Tahap 4 — Security

Bagaimana memastikan aplikasi aman, data terlindungi, dan sistem tidak disalahgunakan?

Tahap 5 — Product Understanding

Menentukan apa yang sebenarnya dibutuhkan pengguna dan seperti apa solusi yang tepat.

Laurie memperkirakan bahwa code review, operations, dan security secara bertahap akan semakin bisa diotomatisasi oleh AI.

Namun, ia berpendapat bahwa memahami kebutuhan manusia dan menentukan definisi kualitas akan menjadi hambatan yang jauh lebih sulit untuk diotomatisasi.

Perlu dicatat bahwa ini adalah prediksi Laurie, bukan kepastian bahwa semua pekerjaan tersebut akan sepenuhnya digantikan AI.

5. Hal yang Sulit Digantikan AI: Memahami Kebutuhan Manusia

Timestamp: 11:21 – 13:45

Inilah salah satu bagian paling penting dalam presentasi.

Menurut Laurie, AI bisa membantu membuat software, tetapi belum tentu mengetahui software seperti apa yang sebenarnya dibutuhkan seseorang.

Mengapa?

Karena kebutuhan pengguna sering kali tidak bisa dijelaskan hanya melalui instruksi teknis.

Contoh: Aplikasi Pencatatan Pesanan

Bayangkan seorang pemilik toko berkata:

"Saya ingin aplikasi untuk mencatat pesanan pelanggan."

Instruksi tersebut terdengar sederhana.

Seorang developer mungkin langsung berpikir untuk membuat:

Form input pesanan.
Database pesanan.
Halaman daftar pesanan.
Fitur update status pesanan.
Fitur pencarian pesanan.

AI bisa membuat semua fitur tersebut.

Tetapi apakah aplikasi itu sudah sesuai kebutuhan pemilik toko?

Belum tentu.

Mari kita lihat tiga jenis bisnis yang berbeda.

A. Bisnis Bakery

Pemilik toko membutuhkan pencatatan pesanan kue berdasarkan:

Tanggal pengambilan.
Jenis kue.
Ukuran.
Permintaan khusus pelanggan.
B. Toko Spare Part

Pemilik toko membutuhkan pencatatan pesanan berdasarkan:

Nomor part.
Kompatibilitas kendaraan.
Jumlah stok.
Supplier.
C. Perusahaan Manufaktur

Perusahaan membutuhkan pencatatan pesanan berdasarkan:

Spesifikasi produk.
Kapasitas produksi.
Bahan baku.
Jadwal pengiriman.

Ketiganya sama-sama membutuhkan sistem pencatatan pesanan.

Tetapi kebutuhan bisnis, aturan operasional, dan definisi keberhasilannya sangat berbeda.

Inilah mengapa developer tidak boleh hanya menerima requirement lalu langsung coding.

Developer perlu menggali informasi lebih dalam.

Apa yang Harus Dilakukan Developer?

Misalnya, ketika bertemu dengan pemilik bakery, jangan hanya bertanya:

"Fitur apa yang Anda inginkan?"

Cobalah bertanya:

Bagaimana proses pemesanan kue saat ini?
Apa masalah terbesar yang sering terjadi?
Bagaimana cara mencatat pesanan custom?
Bagaimana jika pelanggan mengubah tanggal pengambilan?
Bagaimana cara mengetahui kapasitas produksi harian?
Informasi apa yang paling penting bagi karyawan toko?

Dari jawaban tersebut, developer dapat memahami masalah sebenarnya.

Intinya: pengguna sering menyampaikan solusi yang mereka bayangkan, sedangkan tugas engineer adalah menemukan masalah yang sebenarnya perlu diselesaikan.

6. Essential Complexity vs Accidental Complexity

Timestamp: 13:45 – 16:34

Laurie mengutip pemikiran Fred Brooks, penulis buku The Mythical Man-Month.

Brooks membagi kompleksitas software menjadi dua jenis.

A. Accidental Complexity

Kompleksitas yang muncul karena keterbatasan tools, bahasa pemrograman, atau cara kita mengimplementasikan sesuatu.

Contohnya:

Mengingat sintaks JavaScript.
Menulis boilerplate code.
Membuat konfigurasi proyek.
Menulis kode CRUD.
Mengatur struktur folder.
Menghubungkan library.
Menulis kode repetitif.

Hal-hal tersebut relatif mudah dibantu atau diotomatisasi oleh AI.

Contoh:

Dahulu developer perlu menulis kode API secara manual.

Sekarang kita bisa meminta AI:

text
Buatkan REST API untuk manajemen produk
menggunakan Express.js dan PostgreSQL.

Buat endpoint:
- GET /products
- GET /products/:id
- POST /products
- PUT /products/:id
- DELETE /products/:id

Sertakan validasi input dan error handling.


AI bisa membantu menghasilkan sebagian besar implementasinya.

B. Essential Complexity

Kompleksitas yang memang berasal dari masalah yang ingin diselesaikan.

Contohnya:

Bagaimana menentukan harga produk?
Bagaimana menangani refund?
Bagaimana menghitung biaya pengiriman?
Bagaimana mengelola stok barang?
Bagaimana menghindari transaksi ganda?
Bagaimana menentukan hak akses pengguna?
Bagaimana sistem harus bekerja ketika terjadi kegagalan?

Ini lebih sulit karena membutuhkan pemahaman terhadap konteks bisnis dan konsekuensi keputusan.

Perbandingan
Accidental Complexity	Essential Complexity
Bagaimana menulis kode?	Apa yang harus dibuat?
Bagaimana membuat API?	API harus menyelesaikan masalah apa?
Bagaimana membuat database?	Data apa yang perlu disimpan?
Bagaimana membuat validasi?	Aturan bisnis apa yang harus divalidasi?
Bagaimana memperbaiki syntax error?	Apakah solusi yang dibuat sudah benar?
Analogi: Membangun Rumah

Bayangkan Anda diminta membangun sebuah rumah.

Accidental complexity adalah bagaimana menggunakan palu, memasang bata, mengukur kayu, dan mencampur semen.

Essential complexity adalah menentukan:

Rumah tersebut untuk siapa?
Berapa jumlah penghuninya?
Berapa jumlah kamar yang diperlukan?
Apakah harus tahan banjir?
Bagaimana sirkulasi udara?
Bagaimana desainnya agar nyaman?

AI dapat membantu proses pembangunan rumah menjadi lebih cepat.

Namun, jika desain rumahnya salah sejak awal, pembangunan yang cepat justru akan menghasilkan rumah yang salah dengan lebih cepat.

Kesimpulannya, AI sangat membantu mengurangi kesulitan teknis dalam coding, tetapi menentukan solusi yang tepat tetap membutuhkan pemahaman masalah yang mendalam.

7. Product Engineer: Peran Baru Seorang Software Engineer

Timestamp: 16:34 – 19:45

Inilah konsep utama yang diperkenalkan Laurie.

Ia menyebut peran baru tersebut sebagai Product Engineer.

Product Engineer adalah engineer yang tidak hanya bertanggung jawab menulis kode, tetapi juga memahami pengguna, menemukan masalah, menentukan solusi, dan memastikan software yang dibuat memberikan nilai nyata.

Dengan kata lain:

Product Engineer adalah seseorang yang menggabungkan kemampuan software engineering dengan pemahaman produk dan bisnis.

Perbedaan Software Engineer Tradisional dan Product Engineer
Software Engineer Tradisional	Product Engineer
Menerima task dari PM	Ikut menemukan kebutuhan pengguna
Fokus implementasi	Fokus hasil dan dampak
Menerjemahkan requirement ke kode	Mengubah masalah menjadi spesifikasi
Menyelesaikan tiket	Menyelesaikan masalah pengguna
Banyak menulis kode manual	Mengarahkan AI untuk membangun solusi
Mengukur jumlah pekerjaan selesai	Mengukur keberhasilan produk

Perlu dipahami bahwa ini merupakan perbandingan model kerja yang disederhanakan, bukan berarti software engineer tradisional tidak pernah memahami produk.

Contoh Kasus: Fitur Voucher E-Commerce

Misalnya, Anda bekerja di perusahaan e-commerce.

Product Manager memberikan tiket:

text
Task:
Implementasikan fitur voucher diskon.

Requirement:
- User bisa memasukkan kode voucher.
- Sistem menghitung diskon.
- Diskon ditampilkan pada checkout.


Seorang developer yang hanya berorientasi pada implementasi mungkin langsung meminta AI membuat fitur tersebut.

Sementara Product Engineer akan menggali lebih dalam:

Apakah voucher berlaku untuk semua produk?
Apakah ada minimum pembelian?
Apakah voucher bisa digunakan bersamaan?
Apakah voucher memiliki batas penggunaan?
Bagaimana jika voucher kedaluwarsa ketika pengguna checkout?
Bagaimana jika dua pengguna menggunakan kuota terakhir secara bersamaan?
Apakah voucher bisa digunakan untuk produk yang sedang diskon?

Setelah memahami aturan tersebut, Product Engineer menyusun spesifikasi yang jelas.

Kemudian AI digunakan untuk membantu:

Mendesain database.
Membuat API.
Membuat business logic.
Menulis unit test.
Membuat integration test.
Menyusun dokumentasi.

Engineer tetap bertanggung jawab terhadap keputusan dan hasil akhirnya.

Alur Kerja Product Engineer
Memahami pengguna — Mengidentifikasi masalah dan kebutuhan sebenarnya.
Membuat specification — Menentukan fitur, aturan bisnis, batasan, dan kriteria keberhasilan.
Menggunakan AI coding agent — Membantu menulis kode, test, dokumentasi, dan implementasi.
Validasi dan evaluasi — Memastikan implementasi sesuai kebutuhan dan aman.
Release ke production — Meluncurkan produk dan memantau dampaknya kepada pengguna.

Ada satu kalimat penting dari Laurie:

Engineer yang memahami pengguna, bisa mengambil keputusan tentang apa yang harus dibangun, dan langsung membangunnya akan mampu bekerja dengan sangat cepat.

8. Masalah Besar: Bagaimana Nasib Junior Developer?

Timestamp: 19:45 – 22:57

Menurut saya, ini adalah bagian yang paling perlu diperhatikan oleh developer junior.

Laurie mengangkat sebuah masalah yang cukup serius: bagaimana perusahaan akan melatih junior developer jika pekerjaan yang dahulu diberikan kepada junior sekarang bisa dikerjakan AI?

Bagaimana Sistem Pembelajaran Junior Developer Sebelumnya?

Biasanya, perjalanan seorang junior developer seperti ini:

Senior memberikan task yang spesifik.
Junior mengerjakan task tersebut.
Junior membuat pull request.
Senior melakukan code review.
Senior memberikan masukan dan koreksi.
Junior memperbaiki kesalahan dan belajar dari pengalaman.

Misalnya, senior memberikan task:

text
Buat REST API untuk CRUD data customer
menggunakan Express.js.

Gunakan PostgreSQL.
Tambahkan validasi input.
Buat unit test.


Junior mengerjakan task tersebut dan belajar dari kesalahan.

Namun, sekarang AI bisa mengerjakan task yang sama dalam waktu singkat.

Artinya, perusahaan mulai mempertanyakan:

"Kalau AI bisa mengerjakan pekerjaan junior, untuk apa kita merekrut banyak junior developer?"

Inilah yang disebut Laurie sebagai masalah junior developer.

Dampaknya terhadap Industri

Dalam presentasinya, Laurie menunjukkan data statistik ketenagakerjaan Amerika Serikat sejak Januari 2023.

Ia menyampaikan bahwa:

Lapangan pekerjaan untuk engineer usia 22–25 tahun mengalami penurunan.
Pekerjaan untuk engineer usia 41–49 tahun justru meningkat.
Senior engineer tetap memiliki nilai yang tinggi.
Junior developer semakin kesulitan mendapatkan pekerjaan.

Perlu dicatat, data tersebut menggambarkan kondisi pasar tenaga kerja yang dibahas dalam presentasi, bukan gambaran pasti seluruh negara atau semua perusahaan.

Mengapa Ini Menjadi Masalah Besar?

Karena senior engineer tidak muncul begitu saja.

Senior engineer berasal dari junior developer yang mendapatkan kesempatan untuk belajar, melakukan kesalahan, memperbaiki kode, dan memahami sistem secara bertahap.

Jika perusahaan berhenti merekrut junior, siapa yang akan menjadi senior engineer lima atau sepuluh tahun mendatang?

Inilah masalah regenerasi talenta yang disoroti Laurie.

Bagaimana Seharusnya Junior Developer Belajar?

Menurut arah pemikiran Laurie, junior developer perlu mulai dilatih bukan hanya untuk menulis kode, tetapi juga untuk memahami masalah dan kebutuhan pengguna.

Misalnya, daripada hanya diberikan task:

text
Buat halaman dashboard menggunakan React.


Junior bisa diberikan tugas yang lebih komprehensif:

text
Pelajari proses bisnis toko terlebih dahulu.

Cari tahu masalah yang dialami pemilik toko
ketika mengelola stok barang.

Identifikasi kebutuhan pengguna.

Buat spesifikasi solusi.

Gunakan AI untuk membantu implementasi.

Validasi apakah solusi tersebut benar-benar
menyelesaikan masalah pengguna.


Dengan cara tersebut, junior belajar berpikir seperti seorang engineer yang memahami produk, bukan sekadar seseorang yang bisa menggunakan framework.

9. Apakah Orang yang Suka Coding Harus Meninggalkan Dunia Programming?

Timestamp: 22:57 – 25:11

Laurie menyadari bahwa banyak orang masuk ke dunia software engineering karena memang menyukai aktivitas programming.

Mereka menikmati:

Menulis kode.
Memecahkan bug yang sulit.
Membuat algoritma.
Mendesain arsitektur.
Membuat abstraksi yang elegan.
Mengoptimalkan performa aplikasi.

Namun, jika AI semakin banyak mengambil alih aktivitas coding, pekerjaan engineer mungkin akan lebih banyak melibatkan komunikasi, analisis, dan pengambilan keputusan.

Tidak semua programmer akan menyukai perubahan ini.

Laurie memberikan analogi yang menarik:

Programmer akan tetap melakukan programming seperti penyanyi tetap bernyanyi dan tukang kayu tetap membuat furnitur, meskipun industri musik dan furnitur sudah memiliki mesin produksi.

Artinya, programming sebagai sebuah keterampilan dan aktivitas kreatif tidak akan hilang.

Orang tetap bisa menikmati coding, membuat proyek pribadi, bereksperimen dengan teknologi, dan mengembangkan open-source software.

Namun, aktivitas menulis kode secara manual mungkin tidak lagi menjadi alasan utama perusahaan membayar seorang engineer dengan kompensasi tinggi.

Perusahaan akan lebih menghargai kemampuan engineer dalam menghasilkan solusi yang benar-benar dibutuhkan.

10. Apa yang Harus Dilakukan Developer Mulai Sekarang?

Timestamp: 25:11 – 27:01

Pada bagian terakhir, Laurie memberikan beberapa arahan praktis.

Mari kita terjemahkan menjadi tindakan yang relevan untuk software engineer, khususnya junior developer.

A. Mulai Terbiasa Bekerja dengan AI Coding Agents

Jangan menganggap AI hanya sebagai alat untuk bertanya tentang syntax.

Mulailah memanfaatkan AI untuk membantu seluruh proses development.

Contoh tools yang bisa dipelajari:

Claude Code — membantu memahami repository, menulis kode, dan menjalankan pekerjaan coding.
Cursor — membantu pengembangan software dengan AI di dalam editor.
GitHub Copilot — membantu coding dan code review.
OpenAI Codex — membantu mengerjakan tugas pengembangan software.

Jangan hanya belajar bagaimana memberikan prompt agar AI menghasilkan kode.

Belajarlah bagaimana memberikan konteks, membagi pekerjaan, memeriksa hasil, dan mengevaluasi implementasi AI.

B. Fokus pada Kode yang Memiliki Risiko Tinggi

Laurie menyarankan agar engineer lebih selektif dalam melakukan code review manual.

Prioritaskan kode yang memiliki dampak besar apabila terjadi kesalahan.

Contohnya:

Authentication dan authorization.
Payment dan financial transactions.
Database migration.
Security configuration.
Data privacy.
Core business logic.
Infrastruktur production.

Sementara pekerjaan yang lebih mudah diverifikasi dapat dibantu oleh automated reviewer dan automated tests.

Tetapi ingat, otomatisasi bukan berarti tidak perlu pengawasan.

C. Buat Standar Kualitas yang Jelas

J
