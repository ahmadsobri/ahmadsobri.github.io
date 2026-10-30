AI Writes the Code. So What's Left for Engineers?
Memahami Masa Depan Software Engineer di Era AI Coding Agents

Pembicara: Laurie Voss
Jabatan: Head of Developer Relations at Arize AI, Co-founder of npm
Topik: Dampak AI Coding Agents terhadap profesi Software Engineer dan masa depan pengembangan perangkat lunak.

1. Pendahuluan

Dalam presentasinya yang berjudul AI Writes the Code. So What's Left for Engineers?, Laurie Voss membahas perubahan besar yang sedang terjadi di dunia software engineering akibat perkembangan AI Coding Agents.

Dahulu, pekerjaan utama seorang software engineer adalah menulis kode, memperbaiki bug, melakukan debugging, dan membangun aplikasi berdasarkan kebutuhan bisnis.

Namun, dengan hadirnya AI Coding Agents seperti GitHub Copilot, Claude Code, Cursor, dan berbagai tools AI lainnya, proses menulis kode menjadi jauh lebih cepat dan murah.

AI sekarang dapat membantu developer untuk:

Membuat kode dari instruksi bahasa manusia.
Membuat struktur project.
Mengimplementasikan fitur baru.
Memperbaiki bug.
Menulis unit test.
Melakukan refactoring.
Membuat dokumentasi.
Membantu melakukan code review.

Hal ini memunculkan sebuah pertanyaan penting:

Jika AI sudah bisa menulis kode, lalu apa yang sebenarnya masih harus dikerjakan oleh seorang software engineer?

Menurut Laurie Voss, pekerjaan software engineer tidak akan sepenuhnya hilang. Namun, peran dan tanggung jawabnya akan berubah.

Developer yang hanya berfokus pada kemampuan menulis kode akan menghadapi tantangan besar. Sebaliknya, developer yang mampu memahami kebutuhan pengguna, menentukan solusi yang tepat, dan memastikan kualitas produk akan semakin dibutuhkan.

Laurie menyebut peran baru tersebut sebagai Product Engineer.

2. Code Menjadi Murah, Tetapi Software Development Tidak Otomatis Menjadi Lebih Cepat
2.1. Apa maksudnya menulis kode menjadi hampir gratis?

Sebelum adanya AI Coding Agents, developer harus menghabiskan banyak waktu untuk menerjemahkan kebutuhan menjadi kode program.

Contohnya, ketika mendapatkan tugas:

"Tambahkan fitur autentikasi pengguna menggunakan email dan password."

Developer harus melakukan beberapa pekerjaan:

Memahami kebutuhan fitur.
Membuat struktur database.
Membuat API login dan register.
Membuat validasi input.
Mengimplementasikan autentikasi.
Menangani error.
Membuat unit test.
Melakukan debugging.

Semua pekerjaan tersebut membutuhkan waktu dan tenaga developer.

Sekarang, dengan AI Coding Agents, developer cukup memberikan instruksi yang jelas.

Contohnya:

text
Buatkan fitur autentikasi menggunakan email dan password.

Kebutuhan:
- User dapat melakukan registrasi.
- User dapat melakukan login.
- Password harus di-hash.
- Gunakan JWT untuk autentikasi.
- Buat middleware untuk memvalidasi token.
- Tambahkan validasi input.
- Buat unit test untuk setiap endpoint.


AI dapat membantu menghasilkan sebagian besar implementasi tersebut dalam waktu yang jauh lebih singkat.

Artinya, biaya dan waktu untuk menghasilkan kode mengalami penurunan yang signifikan.

Namun, ada satu masalah.

Menulis kode menjadi lebih cepat tidak berarti seluruh proses pengembangan software juga menjadi lebih cepat.

2.2. Data peningkatan produktivitas

Dalam presentasinya, Laurie menyebutkan data bahwa developer yang menggunakan autonomous coding agents dapat menghasilkan sekitar:

741% lebih banyak kode.
Sekitar 8 kali lipat jumlah kode dibandingkan sebelumnya.
Namun, peningkatan kecepatan pengiriman software hanya sekitar 30%.

Artinya, walaupun jumlah kode meningkat sangat besar, peningkatan software yang benar-benar berhasil dikirim ke production tidak sebanding.

Mengapa hal tersebut terjadi?

Karena proses lain dalam software development tidak mengalami peningkatan kecepatan yang sama.

Misalnya:

Aktivitas	Sebelum AI	Setelah AI
Menulis kode	Lambat	Sangat cepat
Membuat unit test	Relatif lambat	Lebih cepat
Code review	Membutuhkan waktu	Masih membutuhkan waktu
Testing	Membutuhkan waktu	Lebih cepat dengan otomatisasi
Deployment	Membutuhkan proses	Masih membutuhkan validasi
Security review	Membutuhkan analisis	Masih membutuhkan validasi

Ketika AI menghasilkan kode dalam jumlah besar, manusia tetap harus memastikan bahwa kode tersebut benar, aman, dan sesuai kebutuhan.

Akibatnya, hambatan berpindah dari proses menulis kode ke proses code review.

2.3. Analogi sederhana

Bayangkan sebuah restoran yang memiliki satu koki.

Sebelumnya:

Koki membutuhkan waktu 30 menit untuk memasak satu pesanan.
Pelayan mampu mengantarkan pesanan dalam waktu 5 menit.
Pelanggan harus menunggu proses memasak.

Kemudian restoran menggunakan mesin otomatis yang mampu memasak 10 pesanan sekaligus.

Sekarang, masalahnya bukan lagi proses memasak.

Masalahnya berpindah ke pelayan yang hanya mampu mengantarkan satu pesanan dalam satu waktu.

Walaupun dapur mampu menghasilkan makanan lebih cepat, pelanggan tetap harus menunggu karena proses pengantaran menjadi hambatan.

Inilah yang terjadi ketika AI mampu menghasilkan kode jauh lebih cepat daripada kemampuan manusia untuk memeriksanya.

3. Code Review Menjadi Bottleneck Baru
3.1. Mengapa code review menjadi masalah?

Code review adalah proses memeriksa kode yang dibuat oleh developer sebelum kode tersebut digabungkan ke dalam branch utama atau dirilis ke production.

Tujuannya adalah memastikan:

Tidak terdapat bug.
Logika program sudah benar.
Kode mudah dipahami.
Tidak menimbulkan masalah pada sistem lain.
Tidak melanggar standar coding.
Tidak menimbulkan celah keamanan.
Implementasi sesuai kebutuhan bisnis.

Ketika AI menghasilkan ribuan baris kode dalam waktu singkat, developer tetap harus melakukan pemeriksaan.

Masalahnya, kemampuan manusia untuk membaca dan memahami kode memiliki batas.

Dalam presentasinya, Laurie mengutip penelitian Cisco yang menyebutkan bahwa kemampuan manusia untuk melakukan code review secara akurat menurun secara signifikan ketika jumlah kode yang diperiksa melebihi sekitar 450 baris per jam.

Bayangkan AI menghasilkan perubahan kode sebanyak 10.000 baris.

Jika seseorang harus memeriksa semuanya dengan kecepatan tersebut, proses review bisa memakan waktu berhari-hari.

Akibatnya, developer sering kali tidak benar-benar memeriksa seluruh kode yang dihasilkan AI.

Hal ini berbahaya karena kode yang terlihat benar belum tentu benar-benar aman dan sesuai kebutuhan.

3.2. Apakah AI bisa menggantikan code reviewer?

Menurut Laurie, AI memang sudah mulai digunakan untuk melakukan code review.

Namun, AI Reviewer masih memiliki keterbatasan.

Dalam presentasinya, ia menjelaskan bahwa beberapa AI Code Reviewer yang diuji mampu menemukan berbagai bug, tetapi masing-masing menemukan masalah yang berbeda.

Artinya, satu AI Reviewer belum tentu mampu menemukan semua kesalahan.

Selain itu, terdapat perbedaan antara:

Kode yang berhasil melewati automated test.
Kode yang benar-benar layak untuk di-merge ke dalam repository.

Keduanya tidak selalu sama.

Contohnya:

Sebuah AI membuat fitur pembayaran.

Semua unit test berhasil dijalankan dan hasilnya PASS.

Namun, ternyata:

Format nominal tidak mengikuti aturan bisnis.
Transaksi bisa diproses dua kali.
Tidak ada mekanisme rollback.
Implementasi tidak mengikuti standar arsitektur project.
Ada potensi kebocoran data pengguna.

Secara teknis, test berhasil.

Namun, secara kualitas software, implementasi tersebut belum tentu layak masuk production.

3.3. Analogi sederhana

Bayangkan seorang siswa mengerjakan ujian matematika.

AI mampu memberikan jawaban dengan cepat.

Kemudian sistem otomatis memeriksa apakah jawaban tersebut sesuai dengan kunci jawaban.

Namun, guru tidak hanya menilai hasil akhir.

Guru juga memperhatikan:

Apakah cara pengerjaannya benar?
Apakah siswa memahami konsepnya?
Apakah ada kesalahan logika?
Apakah metode yang digunakan sesuai?

Begitu juga dengan code review.

Software engineer tidak hanya memastikan kode bisa berjalan, tetapi juga memastikan kode tersebut layak digunakan.

4. Theory of Constraints: Ketika Satu Hambatan Selesai, Hambatan Lain Akan Muncul

Laurie menggunakan konsep dari Eliyahu M. Goldratt yang dikenal sebagai Theory of Constraints.

Konsep ini menjelaskan bahwa setiap sistem memiliki hambatan utama atau bottleneck yang membatasi performa keseluruhan sistem.

Meningkatkan kecepatan bagian lain tidak akan memberikan peningkatan maksimal jika bottleneck utamanya belum diperbaiki.

4.1. Contoh dalam software development

Bayangkan proses pengembangan software memiliki tahapan berikut:

text
Requirement
    |
    v
Coding
    |
    v
Code Review
    |
    v
Testing
    |
    v
Deployment
    |
    v
Production


Sebelum AI hadir, proses coding mungkin menjadi bagian yang paling lama.

Setelah AI hadir, coding menjadi jauh lebih cepat.

Namun, code review masih membutuhkan waktu yang sama.

Akibatnya, antrean kode yang menunggu review semakin panjang.

Jika suatu saat AI sudah mampu melakukan code review dengan sangat baik, bottleneck berikutnya kemungkinan berpindah ke:

Operations.
Deployment.
Infrastructure.
Scalability.
Security.

Artinya, ketika satu hambatan berhasil diatasi, hambatan berikutnya akan menjadi masalah utama.

4.2. Bottleneck yang mungkin terjadi di masa depan
A. Operations

Operations berkaitan dengan bagaimana aplikasi dijalankan dan dipelihara.

Contohnya:

Bagaimana melakukan deployment?
Bagaimana mengatur server?
Bagaimana melakukan monitoring?
Bagaimana menangani server yang mengalami gangguan?
Bagaimana melakukan rollback ketika deployment gagal?
B. Scalability

Scalability adalah kemampuan aplikasi untuk menangani peningkatan jumlah pengguna dan beban sistem.

Contohnya:

Aplikasi awalnya hanya digunakan oleh 100 pengguna.

Kemudian aplikasi berkembang menjadi 1 juta pengguna.

Engineer harus memastikan bahwa sistem tetap stabil dengan melakukan:

Database optimization.
Caching.
Load balancing.
Horizontal scaling.
Queue management.
Infrastructure optimization.
C. Security

Security berkaitan dengan perlindungan sistem dan data pengguna.

Contohnya:

Bagaimana mencegah SQL Injection?
Bagaimana mencegah Cross-Site Scripting?
Bagaimana melindungi data sensitif?
Bagaimana mengelola authentication dan authorization?
Bagaimana memastikan sistem tidak mudah diserang?

Menurut Laurie, AI pada akhirnya berpotensi membantu mengotomatisasi sebagian besar pekerjaan tersebut.

Namun, prosesnya membutuhkan waktu dan tidak terjadi secara instan.

5. Hal yang Sulit Digantikan AI: Memahami Apa yang Sebenarnya Dibutuhkan Manusia

Inilah salah satu gagasan paling penting dari presentasi Laurie Voss.

Menurutnya, bagian yang paling sulit diotomatisasi bukanlah menulis kode.

Bagian yang sulit adalah memahami apa yang sebenarnya dibutuhkan oleh manusia dan menentukan seperti apa solusi yang benar-benar baik.

5.1. Requirement tidak selalu menggambarkan kebutuhan sebenarnya

Misalnya, seorang pemilik bisnis mengatakan:

"Saya membutuhkan aplikasi untuk mengelola pesanan pelanggan."

Sekilas, requirement tersebut terdengar sederhana.

Developer mungkin langsung berpikir untuk membuat:

CRUD pesanan.
Halaman daftar pesanan.
Form tambah pesanan.
Form edit pesanan.
Status pesanan.
Laporan transaksi.

Namun, apakah semua itu sudah cukup?

Belum tentu.

Developer harus memahami konteks bisnisnya terlebih dahulu.

Contohnya:

Kasus A: Bisnis toko roti

Pemilik toko roti membutuhkan sistem untuk:

Mencatat pesanan pelanggan.
Menentukan jadwal pengambilan.
Mengelola stok bahan baku.
Menentukan jumlah produksi harian.
Mengelola pesanan dalam jumlah besar.
Kasus B: Bisnis toko sparepart kendaraan

Pemilik bisnis membutuhkan sistem untuk:

Mencatat pesanan pelanggan.
Memeriksa ketersediaan sparepart.
Mengelola berbagai jenis dan merek produk.
Memeriksa kompatibilitas sparepart dengan kendaraan.
Mengelola pemasok.

Kedua bisnis sama-sama membutuhkan aplikasi pengelolaan pesanan.

Namun, kebutuhan sebenarnya sangat berbeda.

Jika developer hanya menerima requirement secara mentah tanpa memahami proses bisnis, aplikasi yang dibuat mungkin bisa berjalan tetapi tidak benar-benar menyelesaikan masalah pengguna.

5.2. Mengapa AI kesulitan memahami kebutuhan tersebut?

AI dapat mempelajari banyak pola dari data yang tersedia.

Namun, ada informasi yang tidak tersedia dalam dokumentasi, database, atau kode program.

Informasi tersebut berada di dalam pikiran pengguna.

Misalnya:

Mengapa proses bisnis dilakukan dengan cara tertentu?
Mengapa pelanggan lebih menyukai metode pembayaran tertentu?
Mengapa perusahaan memiliki aturan khusus?
Apa masalah yang paling sering dihadapi karyawan?
Apa yang sebenarnya dianggap penting oleh pengguna?

Untuk mendapatkan informasi tersebut, engineer perlu berkomunikasi langsung dengan pengguna.

Caranya melalui:

Interview.
Observasi.
Diskusi.
User research.
Analisis proses bisnis.
Evaluasi feedback pengguna.

AI dapat membantu menganalisis hasil wawancara, tetapi manusia tetap harus mampu menggali informasi yang tepat.

5.3. Analogi sederhana

Bayangkan seseorang meminta seorang arsitek untuk membangun rumah.

Pemilik rumah hanya mengatakan:

"Saya ingin rumah yang nyaman."

Apakah arsitek bisa langsung membangun rumah?

Tentu tidak.

Arsitek perlu bertanya:

Berapa jumlah anggota keluarga?
Apakah membutuhkan ruang kerja?
Apakah ada anak kecil?
Apakah membutuhkan garasi?
Apakah lebih suka rumah terbuka atau tertutup?
Berapa anggaran pembangunan?

Setelah memahami kebutuhan tersebut, arsitek dapat membuat rancangan yang tepat.

Software engineer juga memiliki tanggung jawab yang sama.

Developer bukan hanya pembuat kode, tetapi juga penerjemah kebutuhan manusia menjadi solusi teknologi.

6. Essential Complexity vs Accidental Complexity

Laurie mengutip pemikiran Fred Brooks, penulis buku The Mythical Man-Month.

Brooks membagi kompleksitas software menjadi dua jenis.

6.1. Accidental Complexity

Accidental Complexity adalah kesulitan yang muncul akibat penggunaan tools, bahasa pemrograman, framework, atau proses teknis.

Contohnya:

Menulis syntax JavaScript.
Mengatur konfigurasi framework.
Membuat struktur folder.
Menulis boilerplate code.
Mengatur konfigurasi API.
Membuat konfigurasi database.
Menulis kode repetitif.

Kesulitan seperti ini semakin mudah dikurangi dengan bantuan AI.

Misalnya, dahulu developer harus menulis kode berikut secara manual:

javascript
function add(a, b) {
    return a + b;
}


Sekarang developer cukup meminta AI untuk membuat fungsi tersebut.

Bahkan, AI dapat membuat implementasi yang jauh lebih kompleks.

6.2. Essential Complexity

Essential Complexity adalah kompleksitas yang berasal dari masalah sebenarnya yang ingin diselesaikan.

Contohnya:

Menentukan bagaimana sistem pembayaran bekerja.
Menentukan aturan bisnis.
Menentukan bagaimana stok barang dikelola.
Menentukan alur persetujuan transaksi.
Menentukan bagaimana sistem menangani transaksi bersamaan.
Menentukan bagaimana pengalaman pengguna seharusnya berjalan.

Hal-hal tersebut tidak bisa diselesaikan hanya dengan mengetahui syntax atau framework.

Developer harus memahami masalah dan konteksnya.

6.3. Perbandingan
Aspek	Accidental Complexity	Essential Complexity
Sumber masalah	Tools dan implementasi teknis	Masalah bisnis dan kebutuhan pengguna
Contoh	Syntax, boilerplate, konfigurasi	Business logic, workflow, aturan bisnis
Bantuan AI	Sangat besar	Membantu, tetapi membutuhkan konteks
Fokus developer	Implementasi teknis	Pemahaman masalah dan solusi
Nilai jangka panjang	Semakin mudah diotomatisasi	Tetap membutuhkan penilaian dan pemahaman mendalam
6.4. Kesimpulan konsep

AI semakin mampu menyelesaikan masalah teknis dalam penulisan kode.

Namun, AI tidak otomatis mengetahui apakah solusi yang dibuat benar-benar menyelesaikan masalah pengguna.

Karena itu, nilai seorang engineer akan semakin bergeser dari kemampuan menulis kode menuju kemampuan memahami masalah yang kompleks.

7. Specification Menjadi Sangat Penting

Laurie juga menyampaikan pemikiran bahwa kode merupakan representasi dari specification atau spesifikasi kebutuhan.

Dengan kata lain:

Kode adalah hasil penerjemahan dari spesifikasi.

Jika spesifikasinya salah, kode yang dihasilkan juga berpotensi salah.

Bahkan, AI bisa menghasilkan implementasi yang sangat rapi dan terlihat profesional, tetapi tetap tidak berguna jika requirement yang diberikan tidak tepat.

7.1. Contoh specification yang buruk
text
Buatkan fitur pembayaran untuk aplikasi e-commerce.


Instruksi tersebut terlalu umum.

AI harus menebak banyak hal, seperti:

Metode pembayaran yang digunakan.
Apakah pembayaran harus langsung diproses?
Bagaimana menangani pembayaran gagal?
Bagaimana menangani transaksi duplikat?
Apakah pembayaran dapat dikembalikan?
Bagaimana status transaksi disimpan?
Bagaimana sistem melakukan verifikasi pembayaran?

Akibatnya, hasil implementasi mungkin tidak sesuai kebutuhan.

7.2. Contoh specification yang lebih baik
text
Buatkan fitur pembayaran untuk aplikasi e-commerce.

Business Requirements:

1. User dapat melakukan checkout.
2. Sistem harus membuat transaksi dengan status PENDING.
3. Sistem harus mengirimkan permintaan pembayaran ke payment gateway.
4. Sistem harus menerima webhook dari payment gateway.
5. Status transaksi berubah menjadi PAID ketika pembayaran berhasil.
6. Status transaksi berubah menjadi FAILED ketika pembayaran gagal.
7. Sistem tidak boleh memproses pembayaran yang sama lebih dari satu kali.
8. Semua perubahan status transaksi harus tercatat.

Technical Requirements:

1. Gunakan REST API.
2. Gunakan PostgreSQL.
3. Terapkan idempotency untuk mencegah transaksi duplikat.
4. Validasi signature webhook.
5. Tambahkan unit test dan integration test.

Acceptance Criteria:

1. Transaksi berhasil ketika pembayaran dikonfirmasi.
2. Transaksi gagal ketika pembayaran ditolak.
3. Webhook yang dikirim berulang tidak menghasilkan transaksi ganda.
4. Transaksi yang belum dibayar tidak boleh berstatus PAID.


Dengan specification yang lebih jelas, AI dapat menghasilkan implementasi yang lebih sesuai.

7.3. Analogi sederhana

Bayangkan Anda meminta seorang kontraktor membangun rumah.

Instruksi pertama:

"Buatkan rumah yang bagus."

Instruksi kedua:

"Buatkan rumah dua lantai dengan tiga kamar tidur, dua kamar mandi, satu ruang keluarga, garasi untuk dua mobil, ventilasi yang baik, dan anggaran maksimal 500 juta."

Instruksi kedua memberikan informasi yang jauh lebih jelas.

Hasil pekerjaan pun memiliki kemungkinan lebih besar untuk sesuai harapan.

Begitu juga dengan AI Coding Agents.

Semakin baik specification yang diberikan, semakin besar peluang AI menghasilkan solusi yang benar.

8. Munculnya Peran Baru: Product Engineer

Setelah menjelaskan perubahan tersebut, Laurie memperkenalkan sebuah peran yang disebut Product Engineer.

Product Engineer adalah engineer yang tidak hanya bertugas menulis kode, tetapi juga memahami pengguna, menemukan masalah, menentukan solusi, dan memastikan software yang dibuat benar-benar memberikan nilai.

8.1. Perbedaan Programmer dan Product Engineer
Programmer Tradisional	Product Engineer
Fokus pada penulisan kode	Fokus pada penyelesaian masalah
Mengerjakan task yang diberikan	Ikut menentukan task yang perlu dibuat
Mengikuti specification	Membantu menyusun specification
Berorientasi pada implementasi	Berorientasi pada hasil produk
Mengukur jumlah kode	Mengukur dampak terhadap pengguna
Mengandalkan kemampuan coding	Menggabungkan technical skill dan product thinking
Menggunakan tools untuk menulis kode	Menggunakan AI untuk mempercepat implementasi

Perlu dipahami bahwa Product Engineer bukan berarti tidak perlu memiliki kemampuan programming.

Justru kemampuan teknis tetap penting.

Namun, kemampuan tersebut digunakan sebagai alat untuk menghasilkan solusi, bukan menjadi satu-satunya fokus pekerjaan.

8.2. Tanggung jawab Product Engineer

Seorang Product Engineer idealnya mampu:

Memahami kebutuhan pengguna.
Melakukan diskusi dengan stakeholder.
Mengidentifikasi masalah bisnis.
Menentukan prioritas fitur.
Membuat specification.
Menentukan acceptance criteria.
Menggunakan AI Coding Agents untuk implementasi.
Melakukan evaluasi hasil AI.
Memastikan kualitas software.
Mengukur dampak produk terhadap pengguna.
8.3. Contoh penerapan

Misalnya, sebuah perusahaan ingin membuat aplikasi manajemen inventaris.

Developer dengan pendekatan tradisional mungkin langsung menerima task:

text
Buat CRUD barang.


Kemudian developer mulai membuat:

Endpoint GET.
Endpoint POST.
Endpoint PUT.
Endpoint DELETE.
Database table.
Frontend form.

Namun, seorang Product Engineer akan bertanya lebih dahulu:

Siapa yang menggunakan aplikasi ini?
Apakah barang memiliki banyak lokasi penyimpanan?
Apakah stok harus diperbarui secara real-time?
Bagaimana jika dua karyawan mengambil barang secara bersamaan?
Apakah perusahaan membutuhkan stock opname?
Bagaimana proses barang masuk dan keluar?
Bagaimana menangani stok yang rusak?
Informasi apa yang dibutuhkan oleh manajer?

Setelah mendapatkan jawaban, Product Engineer menyusun specification dan menggunakan AI untuk membantu mengimplementasikannya.

Hasilnya bukan hanya aplikasi CRUD, tetapi sistem yang benar-benar sesuai dengan proses bisnis perusahaan.

9. Tantangan Besar: Masa Depan Junior Developer

Salah satu bagian yang cukup mengkhawatirkan dari presentasi Laurie adalah dampak AI terhadap junior developer.

9.1. Bagaimana junior developer biasanya belajar?

Secara tradisional, perusahaan memberikan task sederhana kepada junior developer.

Contohnya:

Membuat endpoint CRUD.
Membuat form login.
Memperbaiki bug sederhana.
Membuat unit test.
Menambahkan validasi.
Melakukan refactoring kecil.

Kemudian senior developer akan melakukan code review dan memberikan feedback.

Melalui proses tersebut, junior developer belajar:

Struktur project.
Clean code.
Software architecture.
Debugging.
Testing.
Best practices.
Cara berpikir seorang engineer.

Dengan kata lain, pekerjaan sederhana merupakan sarana pembelajaran untuk menjadi senior engineer.

9.2. Mengapa pola tersebut mulai berubah?

Sekarang AI dapat mengerjakan sebagian besar task sederhana tersebut.

Ketika senior developer membutuhkan implementasi CRUD, mereka bisa langsung meminta AI untuk membuatnya.

Akibatnya, perusahaan mungkin merasa tidak perlu lagi merekrut banyak junior developer untuk mengerjakan pekerjaan dasar.

Inilah yang disebut sebagai masalah junior developer.

Laurie juga menunjukkan data ketenagakerjaan dalam presentasinya yang menggambarkan penurunan pekerjaan engineer berusia 22–25 tahun, sementara kelompok usia 41–49 tahun mengalami peningkatan.

Data tersebut digunakan untuk menunjukkan bahwa dampak perubahan ini sudah mulai terlihat di pasar tenaga kerja.

9.3. Mengapa hal ini berbahaya?

Jika perusahaan hanya merekrut senior engineer dan berhenti memberikan kesempatan kepada junior developer, maka akan muncul masalah jangka panjang.

Pertanyaannya:

Dari mana senior engineer generasi berikutnya akan berasal?

Senior engineer tidak muncul secara otomatis.

Mereka berasal dari junior developer yang mendapatkan kesempatan untuk belajar dan berkembang.

Jika jalur pembelajaran tersebut hilang, industri software engineering berpotensi mengalami kekurangan engineer berpengalaman di masa depan.

9.4. Analogi sederhana

Bayangkan sebuah perusahaan konstruksi.

Dahulu, seorang pekerja baru belajar dengan membantu pekerjaan sederhana:

Mengukur material.
Membantu pemasangan.
Menyiapkan peralatan.
Mengikuti instruksi senior.

Setelah bertahun-tahun, pekerja tersebut mampu menjadi mandor atau engineer berpengalaman.

Namun, jika semua pekerjaan dasar digantikan mesin dan perusahaan tidak menyediakan cara baru untuk melatih pekerja pemula, maka perusahaan akan kesulitan mendapatkan tenaga ahli di masa depan.

Hal yang sama dapat terjadi di dunia software engineering.

9.5. Bagaimana cara mengatasi masalah ini?

Menurut Laurie, perusahaan perlu mengubah cara melatih junior developer.

Junior developer tidak cukup hanya dilatih untuk menulis kode.

Mereka juga perlu dilatih untuk:

Berkomunikasi dengan pengguna.
Memahami proses bisnis.
Mengidentifikasi masalah.
Menyusun requirement.
Membuat specification.
Menentukan acceptance criteria.
Menggunakan AI secara efektif.
Mengevaluasi kualitas hasil AI.

Artinya, jalur pengembangan karier harus mulai diarahkan menuju kemampuan Product Engineering.

10. Apakah Kemampuan Programming Akan Hilang?

Tidak.

Laurie menjelaskan bahwa masih akan ada orang yang menulis kode karena mereka memang menyukai aktivitas tersebut.

Ada developer yang menikmati:

Menyelesaikan algoritma yang sulit.
Membuat abstraksi yang elegan.
Memperbaiki bug yang kompleks.
Merancang arsitektur.
Mengoptimalkan performa.
Menulis kode yang bersih.

Aktivitas tersebut tetap memiliki nilai dan tidak akan hilang begitu saja.

Namun, Laurie berpendapat bahwa menulis kode secara manual kemungkinan tidak lagi menjadi pekerjaan utama yang paling dihargai oleh perusahaan.

Ia menggunakan analogi woodworking atau pertukangan.

Ketika industri manufaktur furniture berkembang, pekerjaan membuat furniture secara manual tidak menghilang.

Orang masih membuat furniture dengan tangan karena menyukai proses dan keahliannya.

Namun, produksi massal lebih banyak menggunakan mesin.

Begitu juga dengan programming.

Orang tetap bisa menulis kode secara manual karena menyukai prosesnya, tetapi pekerjaan profesional di industri akan semakin banyak melibatkan AI.

Programming mungkin berubah dari aktivitas utama menjadi salah satu kemampuan yang digunakan untuk mengarahkan dan mengevaluasi hasil AI.

11. Apa yang Harus Dilakukan Developer Mulai Sekarang?

Bagian ini merupakan salah satu bagian paling praktis dari presentasi Laurie.

Ia memberikan beberapa arahan mengenai bagaimana engineer sebaiknya beradaptasi dengan perubahan tersebut.

11.1. Mulai terbiasa bekerja dengan AI Coding Agents

Jangan menganggap AI hanya sebagai alat untuk bertanya atau mencari contoh kode.

Mulailah menggunakannya sebagai bagian dari workflow development.

Contoh tools yang dapat dipelajari:

GitHub Copilot.
Cursor.
Claude Code.
OpenAI Codex.
Windsurf.

Pelajari bagaimana memberikan instruksi, memberikan konteks repository, menjalankan test, dan mengevaluasi hasil implementasi.

Tujuannya bukan sekadar menghasilkan kode sebanyak mungkin.

Tujuannya adalah menyelesaikan pekerjaan dengan lebih efektif.

11.2. Fokus pada kode yang memiliki dampak besar jika terjadi kesalahan

Laurie menyarankan agar developer memberikan perhatian lebih besar pada kode yang memiliki high blast radius.

High blast radius adalah bagian sistem yang apabila mengalami kesalahan dapat menyebabkan dampak besar terhadap keseluruhan aplikasi atau bisnis.

Contohnya:

Authentication.
Authorization.
Payment processing.
Database transaction.
Data migration.
Infrastructure configuration.
Security-sensitive logic.

Bagian tersebut membutuhkan pengawasan dan evaluasi lebih ketat.

Sementara itu, pekerjaan yang relatif sederhana dan mudah diverifikasi dapat lebih banyak didelegasikan kepada AI.

11.3. Otomatiskan proses verifikasi

Daripada memeriksa semua kode secara manual, engineer perlu membangun sistem otomatis untuk memeriksa kualitas hasil pekerjaan AI.

Contohnya:

Unit testing.
Integration testing.
End-to-end testing.
Static code analysis.
Linting.
Type checking.
Security scanning.
Performance testing.

Contoh sederhana:

text
AI Agent
   |
   v
Generate Code
   |
   v
Run Unit Tests
   |
   v
Run Integration Tests
   |
   v
Run Security Scan
   |
   v
Check Code Quality
   |
   v
Human Review
   |
   v
Deploy


Dengan cara ini, developer tidak harus memeriksa setiap detail kode dari awal.

Namun, hasil pemeriksaan otomatis tetap perlu dievaluasi, terutama untuk bagian yang memiliki risiko tinggi.

11.4. Tingkatkan kemampuan membuat specification

Ini adalah salah satu kemampuan yang paling penting untuk dikembangkan.

Belajarlah membuat requirement yang jelas dan terukur.

Specification yang baik setidaknya menjelaskan:

Problem Statement.
User Requirements.
Business Rules.
Functional Requirements.
Non-Functional Requirements.
Technical Constraints.
Acceptance Criteria.
Edge Cases.

Contoh:

Jangan hanya mengatakan:

text
Buatkan fitur login.


Tetapi jelaskan:

text
Problem:
Pengguna membutuhkan mekanisme autentikasi untuk mengakses aplikasi.

Functional Requirements:
- User dapat login menggunakan email dan password.
- User mendapatkan access token setelah berhasil login.
- User mendapatkan pesan error ketika kredensial salah.

Security Requirements:
- Password harus disimpan menggunakan hashing.
- Token harus memiliki masa berlaku.
- Endpoint yang membutuhkan autentikasi harus memvalidasi token.

Acceptance Criteria:
- Login berhasil dengan kredensial yang benar.
- Login gagal dengan kredensial yang salah.
- User yang tidak terautentikasi tidak dapat mengakses endpoint private.
- Password tidak pernah dikembalikan melalui API response.


Semakin baik specification, semakin kecil kemungkinan AI menghasilkan implementasi yang salah arah.

11.5. Pelajari business domain

Jangan hanya memahami teknologi.

Mulailah memahami bisnis tempat software tersebut digunakan.

Contohnya:

Jika bekerja di perusahaan e-commerce, pelajari:

Order management.
Payment processing.
Inventory management.
Shipping.
Refund.
Customer experience.

Jika bekerja di perusahaan fintech, pelajari:

Financial transactions.
Reconciliation.
Fraud detection.
Risk management.
Compliance.

Jika bekerja di perusahaan logistik, pelajari:

Shipment tracking.
Warehouse management.
Delivery scheduling.
Fleet management.

Semakin memahami domain bisnis, semakin baik kemampuan developer dalam membuat solusi yang tepat.

11.6. Tingkatkan kemampuan komunikasi

Seorang Product Engineer harus mampu berdiskusi dengan orang yang tidak memiliki latar belakang teknis.

Misalnya:

Product Manager.
Business Analyst.
Customer.
Stakeholder.
Operations Team.
Marketing Team.

Developer perlu mampu mengubah kebutuhan yang tidak jelas menjadi requirement yang dapat diimplementasikan.

Kemampuan bertanya menjadi sangat penting.

Contohnya:

Ketika pengguna mengatakan:

"Sistem ini lambat."

Jangan langsung melakukan optimasi database.

Tanyakan terlebih dahulu:

Bagian mana yang terasa lambat?
Sejak kapan masalah terjadi?
Apakah semua pengguna mengalami masalah?
Apakah terjadi pada jam tertentu?
Berapa lama waktu respons yang diharapkan?

Dengan demikian, developer dapat menemukan akar masalah sebelum menentukan solusi.

11.7. Ukur hasil, bukan jumlah kode

Laurie menekankan bahwa menghasilkan 741% lebih banyak kode bukanlah tujuan utama.

Yang lebih penting adalah berapa banyak software yang benar-benar berhasil dikirim dan memberikan manfaat.

Beberapa metrik yang dapat digunakan:

Metrik	Tujuan
Deployment Frequency	Mengukur seberapa sering software dirilis
Lead Time for Changes	Mengukur waktu dari perubahan kode hingga dirilis
Change Failure Rate	Mengukur persentase perubahan yang menyebabkan kegagalan
Mean Time to Recovery (MTTR)	Mengukur waktu pemulihan setelah terjadi masalah
Test Pass Rate	Mengukur keberhasilan automated test
Review Feedback Resolution	Mengukur seberapa banyak feedback review yang ditindaklanjuti
User Satisfaction	Mengukur kepuasan pengguna
Business Impact	Mengukur dampak software terhadap bisnis

Fokuslah pada nilai yang dihasilkan software, bukan sekadar jumlah baris kode yang dibuat.

12. Roadmap Pengembangan Kemampuan untuk Junior Developer

Berdasarkan gagasan Laurie Voss, berikut roadmap praktis yang dapat digunakan oleh junior developer untuk mempersiapkan diri menghadapi era AI.

Tahap 1: Fundamental Software Engineering

Jangan meninggalkan fundamental programming hanya karena AI bisa menulis kode.

Pelajari:

Data Structures and Algorithms.
Object-Oriented Programming.
Functional Programming.
Database Design.
REST API.
Authentication and Authorization.
Software Architecture.
Clean Code.
Design Patterns.
Git dan Version Control.
Testing.
Debugging.

Mengapa masih penting?

Karena Anda tidak mungkin mengevaluasi kode AI dengan baik jika tidak memahami bagaimana software bekerja.

Tahap 2: AI-Assisted Development

Pelajari cara menggunakan AI untuk mempercepat pekerjaan development.

Latih kemampuan:

Prompt Engineering.
Context Engineering.
AI Coding Agents.
Repository Understanding.
Automated Testing.
Code Review dengan AI.
Debugging menggunakan AI.
Refactoring dengan AI.
Documentation Generation.

Jangan hanya meminta AI menghasilkan kode.

Pelajari juga cara memberikan konteks dan memverifikasi hasilnya.

Tahap 3: Problem Solving dan Product Thinking

Mulailah belajar memahami masalah dari sudut pandang pengguna.

Pelajari:

Problem Identification.
Requirement Gathering.
User Interview.
User Journey.
Business Process Analysis.
Product Discovery.
Feature Prioritization.
Acceptance Criteria.
Specification Writing.

Latih diri untuk memahami mengapa sebuah fitur dibutuhkan sebelum memikirkan bagaimana cara membuatnya.

Tahap 4: Production Engineering

Pelajari bagaimana aplikasi berjalan di lingkungan production.

Materi yang perlu dipelajari:

Docker.
CI/CD.
Cloud Infrastructure.
Monitoring.
Logging.
Observability.
Performance Optimization.
Scalability.
Security.
Incident Management.

Developer harus memahami bahwa software development tidak berhenti ketika kode selesai dibuat.

Software harus bisa dijalankan, dipelihara, dan memberikan layanan secara konsisten.

Tahap 5: Product Engineer Mindset

Gabungkan semua kemampuan sebelumnya.

Mulailah membangun project dengan pendekatan berikut:

Temukan masalah nyata.
Lakukan observasi terhadap calon pengguna.
Identifikasi kebutuhan.
Buat specification.
Tentukan acceptance criteria.
Rancang solusi.
Gunakan AI untuk membantu implementasi.
Lakukan testing.
Deploy ke production.
Kumpulkan feedback pengguna.
Evaluasi hasil.
Lakukan perbaikan.

Dengan pendekatan ini, Anda tidak hanya berlatih menjadi programmer, tetapi juga mengembangkan kemampuan sebagai Product Engineer.

13. Contoh Studi Kasus: Membangun Aplikasi Manajemen Inventaris

Untuk memahami seluruh konsep di atas, mari gunakan contoh sederhana.

Misalnya, Anda mendapatkan proyek untuk membangun aplikasi manajemen inventaris sebuah perusahaan distribusi barang.

13.1. Pendekatan developer tradisional

Developer menerima task:

text
Buat aplikasi inventory management.


Kemudian langsung membuat:

Database barang.
CRUD barang.
CRUD kategori.
CRUD supplier.
Halaman stok.
API inventory.

Developer fokus pada penyelesaian task teknis.

Masalahnya, belum tentu aplikasi tersebut sesuai dengan kebutuhan perusahaan.

13.2. Pendekatan Product Engineer

Product Engineer memulai dengan memahami masalah bisnis.

Ia bertanya kepada pengguna:

Bagaimana proses barang masuk?
Bagaimana proses barang keluar?
Apakah perusahaan memiliki beberapa gudang?
Bagaimana proses pemindahan barang?
Bagaimana jika stok fisik berbeda dengan stok sistem?
Siapa yang boleh mengubah stok?
Apakah perusahaan membutuhkan laporan stok harian?
Bagaimana perusahaan mengetahui barang yang hampir habis?

Setelah mendapatkan informasi, Product Engineer membuat specification.

Contoh:

text
Project:
Inventory Management System

Problem Statement:
Perusahaan mengalami kesulitan dalam memantau
stok barang di beberapa gudang.

Business Requirements:
1. Sistem dapat mencatat barang masuk.
2. Sistem dapat mencatat barang keluar.
3. Sistem mendukung banyak gudang.
4. Sistem dapat mencatat perpindahan barang.
5. Sistem dapat menampilkan stok secara real-time.
6. Sistem mencatat histori perubahan stok.

Business Rules:
1. Barang keluar tidak boleh melebihi stok tersedia.
2. Setiap transaksi stok harus memiliki histori.
3. Perpindahan barang harus memiliki gudang asal
   dan gudang tujuan.
4. Hanya user dengan permission tertentu yang
   dapat melakukan penyesuaian stok.

Acceptance Criteria:
1. Stok bertambah ketika barang masuk berhasil.
2. Stok berkurang ketika barang keluar berhasil.
3. Stok gudang asal berkurang ketika transfer berhasil.
4. Stok gudang tujuan bertambah ketika transfer berhasil.
5. Sistem menolak transaksi yang menyebabkan stok negatif.


Kemudian Product Engineer menggunakan AI Coding Agent untuk membantu:

Membuat database schema.
Membuat backend API.
Membuat frontend.
Membuat unit test.
Membuat integration test.
Membuat dokumentasi.
Melakukan refactoring.

Setelah itu, Product Engineer memeriksa hasil implementasi dan memastikan sistem memenuhi kebutuhan bisnis.

13.3. Perbedaan hasil
Aspek	Developer Tradisional	Product Engineer
Awal pekerjaan	Menerima task	Memahami masalah
Requirement	Mengikuti instruksi	Menggali kebutuhan
Implementasi	Menulis kode manual	Menggunakan AI dan kemampuan teknis
Evaluasi	Memastikan fitur berjalan	Memastikan masalah terselesaikan
Hasil	Aplikasi sesuai task	Aplikasi sesuai kebutuhan bisnis

Perbedaan utamanya bukan terletak pada siapa yang menulis kode.

Perbedaannya terletak pada siapa yang memahami masalah dan memastikan solusi yang dibuat benar-benar tepat.

14. Kesimpulan

Berdasarkan presentasi Laurie Voss, kita dapat mengambil beberapa kesimpulan penting.

14.1. AI mengubah cara software dikembangkan

AI Coding Agents membuat proses penulisan kode menjadi jauh lebih cepat dan murah.

Namun, hal tersebut tidak otomatis membuat seluruh proses software development menjadi lebih cepat.

Bottleneck hanya berpindah dari coding ke code review, kemudian berpotensi berpindah lagi ke operations, security, dan aspek lainnya.

14.2. Kemampuan coding saja tidak lagi cukup

Kemampuan programming tetap penting, tetapi tidak cukup untuk menjadi pembeda utama seorang engineer.

Developer perlu memahami bagaimana software digunakan, masalah apa yang ingin diselesaikan, dan bagaimana menentukan solusi yang tepat.

14.3. Specification menjadi salah satu kemampuan paling berharga

AI sangat bergantung pada konteks dan instruksi yang diberikan.

Jika requirement tidak jelas, AI bisa menghasilkan kode yang secara teknis terlihat benar tetapi tidak sesuai kebutuhan.

Karena itu, kemampuan requirement gathering, problem analysis, dan specification writing akan semakin penting.

14.4. Product Engineer menjadi peran yang semakin relevan

Product Engineer adalah engineer yang mampu menggabungkan:

Technical Skills.
Problem Solving.
Product Thinking.
Business Understanding.
Communication.
AI-Assisted Development.

Peran ini tidak hanya berfokus pada bagaimana membuat software, tetapi juga mengapa software tersebut harus dibuat dan apakah software tersebut benar-benar memberikan manfaat.

14.5. Junior Developer harus mengubah cara belajar

Junior developer tidak boleh hanya mengandalkan kemampuan membuat CRUD, mengikuti tutorial, atau menghafal syntax.

Fundamental programming tetap harus dikuasai, tetapi perlu dilengkapi dengan kemampuan:

Menggunakan AI.
Memahami kebutuhan pengguna.
Menganalisis masalah.
Menulis specification.
Melakukan testing.
Memahami sistem production.
Berkomunikasi dengan stakeholder.

Junior developer perlu belajar menjadi engineer yang mampu menyelesaikan masalah secara menyeluruh.

15. Pesan Penting untuk Junior Developer

Jika Anda saat ini sedang belajar menjadi software engineer, jangan langsung merasa bahwa masa depan programming sudah berakhir karena AI.

Justru, ini adalah kesempatan untuk mengembangkan kemampuan yang lebih luas.

Jangan hanya belajar bagaimana menulis kode.

Belajarlah bagaimana memahami masalah, menentukan solusi, dan memastikan solusi tersebut memberikan nilai.

Mulailah mengubah pola pikir dari:

text
"Saya harus bisa membuat fitur ini menggunakan kode."


Menjadi:

text
"Saya harus memahami masalah yang ingin diselesaikan,
menentukan solusi yang tepat, kemudian menggunakan
teknologi dan AI untuk mewujudkan solusi tersebut."


Ingat bahwa AI bisa membantu Anda menulis ribuan baris kode dalam waktu singkat.

Namun, menghasilkan ribuan baris kode bukan berarti Anda telah menyelesaikan masalah.

Nilai seorang software engineer bukan hanya terletak pada seberapa banyak kode yang dapat ditulis, tetapi pada seberapa baik masalah manusia dapat diselesaikan melalui software yang dibuatnya.

Pada akhirnya, pesan utama Laurie Voss dapat dirangkum dalam satu kalimat:

The rise of the Product Engineer is about what's left when the models do the building.

Artinya:

Ketika AI sudah mampu membangun software, peran engineer yang paling bernilai adalah memahami apa yang perlu dibangun, menentukan seperti apa solusi yang baik, dan memastikan software tersebut benar-benar bermanfaat bagi manusia.

Referensi Konsep

Beberapa konsep dan tokoh yang disebutkan dalam presentasi:

Theory of Constraints — Eliyahu M. Goldratt. Konsep mengenai bottleneck dalam suatu sistem.
The Mythical Man-Month — Fred Brooks. Membahas kompleksitas dalam pengembangan software.
Essential Complexity vs Accidental Complexity — Konsep dari Fred Brooks mengenai dua jenis kompleksitas software.
Product Engineer — Peran engineer yang menggabungkan pemahaman produk, kebutuhan pengguna, dan kemampuan teknis.
AI Coding Agents — Sistem AI yang dapat membantu atau menjalankan berbagai tahapan pengembangan software secara otomatis.
