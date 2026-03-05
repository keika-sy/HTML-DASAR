# HTML DASAR
```html
<!DOCTYPE html>
<!-- 
  DEKLARASI DOCTYPE
  - Menyatakan bahwa dokumen ini menggunakan HTML5
  - Wajib ada di baris pertama sebelum tag <html>
  - Memastikan browser merender halaman dalam mode standar
-->
<html lang="id">
<!-- 
  TAG <html>
  - Elemen root yang membungkus seluruh konten halaman
  - Atribut lang="id" menyatakan bahasa utama adalah Bahasa Indonesia
  - Penting untuk aksesibilitas dan SEO
-->
<head>
    <!-- 
        BAGIAN <head>
        - Berisi metadata dan informasi tentang dokumen
        - Tidak ditampilkan langsung di halaman web
        - Berisi konfigurasi, resource eksternal, dan informasi penting lainnya
    -->
    
    <meta charset="UTF-8">
    <!-- 
        META CHARSET
        - Menentukan encoding karakter dokumen
        - UTF-8 mendukung semua karakter Unicode termasuk huruf Indonesia
        - Mencegah masalah tampilan karakter khusus
    -->
    
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!-- 
        META VIEWPORT
        - Mengontrol tampilan pada perangkat mobile
        - width=device-width: lebar sesuai lebar perangkat
        - initial-scale=1.0: zoom awal 100%
        - Penting untuk desain responsif
    -->
    
    <title>Contoh HTML Dasar</title>
    <!-- 
        TAG <title>
        - Menentukan judul halaman yang muncul di tab browser
        - Ditampilkan di hasil pencarian mesin pencari
        - Penting untuk SEO dan identifikasi halaman
    -->
    
    <meta name="description" content="Halaman contoh HTML dengan penjelasan lengkap">
    <!-- 
        META DESCRIPTION
        - Deskripsi singkat tentang konten halaman
        - Muncul di hasil pencarian Google
        - Maksimal 160 karakter untuk hasil terbaik
    -->
</head>

<body>
    <!-- 
        BAGIAN <body>
        - Berisi semua konten yang akan ditampilkan di browser
        - Teks, gambar, link, video, dan elemen interaktif lainnya
        - Hanya ada satu elemen <body> dalam satu halaman
    -->
    
    <!-- ==================== HEADER ==================== -->
    <header>
        <!-- 
            TAG <header>
            - Bagian atas halaman yang biasanya berisi logo dan navigasi
            - Bisa digunakan di awal halaman atau dalam elemen lain (article, section)
            - Membantu struktur semantik dokumen
        -->
        <h1>Selamat Datang di HTML Dasar</h1>
        <!-- 
            TAG <h1>
            - Heading level 1, judul utama halaman
            - Hanya boleh ada satu <h1> per halaman untuk SEO yang baik
            - Ukuran font terbesar secara default
        -->
        
        <nav>
            <!-- 
                TAG <nav>
                - Bagian navigasi utama halaman
                - Berisi link ke halaman lain atau bagian dalam halaman
                - Membantu screen reader mengidentifikasi menu navigasi
            -->
            <ul>
                <!-- 
                    TAG <ul>
                    - Unordered List: daftar tak berurutan (bullet points)
                    - Setiap item di dalamnya menggunakan <li>
                -->
                <li><a href="#pengenalan">Pengenalan</a></li>
                <!-- 
                    TAG <li>
                    - List Item: item dalam daftar
                    - Bisa berisi teks, link, atau elemen lain
                -->
                <li><a href="#struktur">Struktur</a></li>
                <li><a href="#konten">Konten</a></li>
            </ul>
        </nav>
    </header>

    <!-- ==================== KONTEN UTAMA ==================== -->
    <main>
        <!-- 
            TAG <main>
            - Konten utama halaman yang unik (tidak berulang di halaman lain)
            - Tidak boleh ada lebih dari satu <main> per halaman
            - Tidak boleh berada dalam <article>, <aside>, <footer>, <header>, atau <nav>
        -->
        
        <section id="pengenalan">
            <!-- 
                TAG <section>
                - Mengelompokkan konten yang memiliki tema terkait
                - Atribut id untuk membuat anchor link (dituju oleh navigasi)
                - Membagi halaman menjadi bagian-bagian logis
            -->
            <h2>Pengenalan HTML</h2>
            <!-- 
                TAG <h2>
                - Heading level 2, subjudul di bawah <h1>
                - Menunjukkan hierarki konten
                - Ada hingga <h6> untuk level yang lebih dalam
            -->
            
            <p>
                <!-- 
                    TAG <p>
                    - Paragraph: paragraf teks
                    - Membuat blok teks terpisah dengan margin otomatis
                    - Elemen block-level (memenuhi lebar kontainer)
                -->
                <strong>HTML</strong> (HyperText Markup Language) adalah 
                <!-- 
                    TAG <strong>
                    - Menandai teks penting dengan penekanan kuat
                    - Ditampilkan tebal secara default
                    - Memiliki makna semantik penting untuk SEO
                -->
                bahasa markup standar untuk membuat halaman web. 
                <em>Markup</em> berarti menggunakan tag untuk menandai konten.
                <!-- 
                    TAG <em>
                    - Emphasis: penekanan pada teks
                    - Ditampilkan miring secara default
                    - Menunjukkan teks yang perlu penekanan
                -->
            </p>
            
            <p>
                HTML menggunakan <mark>tag</mark> untuk memberi struktur dan makna pada konten.
                <!-- 
                    TAG <mark>
                    - Menandai teks yang relevan dalam konteks tertentu
                    - Biasanya ditampilkan dengan latar belakang kuning
                    - Berbeda dengan <strong>, ini untuk highlight kontekstual
                -->
            </p>
        </section>

        <section id="struktur">
            <h2>Struktur Dasar HTML</h2>
            
            <article>
                <!-- 
                    TAG <article>
                    - Konten independen yang bisa berdiri sendiri
                    - Contoh: posting blog, berita, komentar
                    - Bisa memiliki header, footer, dan section sendiri
                -->
                <h3>Elemen Block vs Inline</h3>
                <!-- 
                    TAG <h3>
                    - Heading level 3, sub-subjudul
                    - Hierarki: h1 > h2 > h3 > h4 > h5 > h6
                -->
                
                <p>
                    Elemen <span style="color: blue;">block</span> memulai baris baru dan memenuhi lebar yang tersedia.
                    <!-- 
                        TAG <span>
                        - Inline container untuk menandai bagian teks
                        - Tidak memiliki efek visual sendiri
                        - Biasanya digunakan dengan CSS atau JavaScript
                    -->
                    Contoh: &lt;div&gt;, &lt;p&gt;, &lt;h1&gt;-&lt;h6&gt;.
                    <!-- 
                        Karakter khusus HTML:
                        &lt; = < (less than)
                        &gt; = > (greater than)
                        &amp; = & (ampersand)
                    -->
                </p>
                
                <p>
                    Elemen <span style="color: green;">inline</span> tidak memulai baris baru dan hanya selebar kontennya.
                    Contoh: &lt;span&gt;, &lt;a&gt;, &lt;strong&gt;, &lt;em&gt;.
                </p>
            </article>
            
            <hr>
            <!-- 
                TAG <hr>
                - Horizontal Rule: garis pemisah horizontal
                - Menunjukkan perubahan tema atau pemisah bagian
                - Elemen kosong (self-closing), tidak perlu tag penutup
            -->
        </section>

        <section id="konten">
            <h2>Jenis Konten</h2>
            
            <h3>Daftar (Lists)</h3>
            
            <h4>Daftar Berurutan (Ordered List):</h4>
            <ol>
                <!-- 
                    TAG <ol>
                    - Ordered List: daftar berurutan dengan angka/huruf
                    - Atribut type bisa "1", "A", "a", "I", "i"
                    - Atribut start untuk memulai dari nomor tertentu
                -->
                <li>Item pertama</li>
                <li>Item kedua</li>
                <li>Item ketiga</li>
            </ol>
            
            <h4>Daftar Tak Berurutan (Unordered List):</h4>
            <ul>
                <li>Apel</li>
                <li>Pisang</li>
                <li>Jeruk</li>
            </ul>
            
            <h4>Daftar Definisi (Definition List):</h4>
            <dl>
                <!-- 
                    TAG <dl>
                    - Definition List: daftar istilah dan definisinya
                    - Menggunakan <dt> untuk istilah dan <dd> untuk definisi
                -->
                <dt>HTML</dt>
                <!-- 
                    TAG <dt>
                    - Definition Term: istilah yang akan didefinisikan
                -->
                <dd>Bahasa markup untuk membuat struktur halaman web</dd>
                <!-- 
                    TAG <dd>
                    - Definition Description: penjelasan definisi
                    - Bisa lebih dari satu <dd> untuk satu <dt>
                -->
                
                <dt>CSS</dt>
                <dd>Bahasa stylesheet untuk mendesain tampilan halaman web</dd>
            </dl>
            
            <h3>Link (Tautan)</h3>
            <p>
                <a href="https://www.example.com" target="_blank" rel="noopener noreferrer">
                <!-- 
                    TAG <a> (anchor)
                    - Membuat hyperlink ke halaman lain atau resource
                    - Atribut href: URL tujuan (wajib ada)
                    - Atribut target="_blank": buka di tab baru
                    - Atribut rel="noopener noreferrer": keamanan untuk link eksternal
                -->
                    Kunjungi Example.com
                </a>
            </p>
            
            <p>
                <a href="mailto:email@example.com">Kirim Email</a>
                <!-- 
                    Link email dengan protokol mailto:
                    - Membuka aplikasi email default saat diklik
                    - Bisa ditambahkan subjek: mailto:email@example.com?subject=Halo
                -->
            </p>
            
            <h3>Gambar</h3>
            <img src="https://via.placeholder.com/400x200" 
            <!-- 
                TAG <img>
                - Menampilkan gambar di halaman
                - Atribut src: URL sumber gambar (wajib)
                - Atribut alt: teks alternatif untuk aksesibilitas (wajib)
                - Elemen kosong, tidak perlu tag penutup
            -->
                 alt="Gambar contoh dengan ukuran 400x200 piksel"
                 width="400" 
                 height="200">
                 <!-- 
                     Atribut width dan height:
                     - Menentukan ukuran gambar dalam piksel
                     - Mencegah layout shift saat gambar dimuat
                     - Bisa diatur juga dengan CSS
                 -->
            
            <h3>Tabel</h3>
            <table border="1">
                <!-- 
                    TAG <table>
                    - Membuat tabel data
                    - Atribut border untuk garis pembatas (sebaiknya gunakan CSS)
                -->
                <thead>
                    <!-- 
                        TAG <thead>
                        - Bagian kepala tabel (header)
                        - Biasanya berisi judul kolom
                    -->
                    <tr>
                        <!-- 
                            TAG <tr>
                            - Table Row: baris dalam tabel
                        -->
                        <th>Nama</th>
                        <!-- 
                            TAG <th>
                            - Table Header: sel header (judul kolom/baris)
                            - Ditampilkan tebal dan rata tengah secara default
                        -->
                        <th>Usia</th>
                        <th>Kota</th>
                    </tr>
                </thead>
                <tbody>
                    <!-- 
                        TAG <tbody>
                        - Bagian isi tabel (data utama)
                        - Bisa ada lebih dari satu <tbody> dalam satu tabel
                    -->
                    <tr>
                        <td>Budi</td>
                        <!-- 
                            TAG <td>
                            - Table Data: sel data biasa
                            - Berisi konten aktual tabel
                        -->
                        <td>25</td>
                        <td>Jakarta</td>
                    </tr>
                    <tr>
                        <td>Ani</td>
                        <td>23</td>
                        <td>Bandung</td>
                    </tr>
                </tbody>
                <tfoot>
                    <!-- 
                        TAG <tfoot>
                        - Bagian kaki tabel (footer)
                        - Biasanya berisi ringkasan atau total
                    -->
                    <tr>
                        <td colspan="3">Total: 2 orang</td>
                        <!-- 
                            Atribut colspan:
                            - Menggabungkan beberapa kolom menjadi satu sel
                            - Nilai menunjukkan jumlah kolom yang digabung
                        -->
                    </tr>
                </tfoot>
            </table>
            
            <h3>Formulir</h3>
            <form action="/proses" method="POST">
                <!-- 
                    TAG <form>
                    - Membuat formulir untuk input pengguna
                    - Atribut action: URL tujuan pengiriman data
                    - Atribut method: metode HTTP (GET atau POST)
                -->
                
                <div>
                    <!-- 
                        TAG <div>
                        - Division: kontainer generik tanpa makna semantik
                        - Digunakan untuk mengelompokkan dan styling dengan CSS
                        - Elemen block-level yang sangat fleksibel
                    -->
                    <label for="nama">Nama Lengkap:</label>
                    <!-- 
                        TAG <label>
                        - Label untuk elemen form
                        - Atribut for menghubungkan dengan id elemen input
                        - Meningkatkan aksesibilitas dan area klik
                    -->
                    <input type="text" id="nama" name="nama" placeholder="Masukkan nama" required>
                    <!-- 
                        TAG <input>
                        - Elemen input untuk berbagai jenis data
                        - Atribut type menentukan jenis input (text, email, dll)
                        - Atribut name: nama field saat dikirim ke server
                        - Atribut placeholder: teks petunjuk di dalam input
                        - Atribut required: wajib diisi sebelum submit
                    -->
                </div>
                
                <div>
                    <label for="email">Email:</label>
                    <input type="email" id="email" name="email" placeholder="email@example.com" required>
                    <!-- 
                        type="email" memvalidasi format email secara otomatis
                    -->
                </div>
                
                <div>
                    <label for="pesan">Pesan:</label>
                    <textarea id="pesan" name="pesan" rows="4" cols="50" placeholder="Tulis pesan Anda di sini..."></textarea>
                    <!-- 
                        TAG <textarea>
                        - Area teks multi-baris untuk input panjang
                        - Atribut rows dan cols menentukan ukuran
                        - Bisa diubah ukurannya oleh pengguna (resizeable)
                    -->
                </div>
                
                <div>
                    <label>Jenis Kelamin:</label>
                    <input type="radio" id="laki" name="gender" value="laki-laki">
                    <!-- 
                        type="radio":
                        - Tombol pilihan tunggal (hanya satu bisa dipilih)
                        - Atribut name yang sama mengelompokkan pilihan
                        - Atribut value: nilai yang dikirim saat dipilih
                    -->
                    <label for="laki">Laki-laki</label>
                    
                    <input type="radio" id="perempuan" name="gender" value="perempuan">
                    <label for="perempuan">Perempuan</label>
                </div>
                
                <div>
                    <label>Hobi:</label>
                    <input type="checkbox" id="membaca" name="hobi" value="membaca">
                    <!-- 
                        type="checkbox":
                        - Kotak centang untuk pilihan ganda
                        - Bisa dipilih lebih dari satu
                        - Atribut checked untuk membuat terpilih secara default
                    -->
                    <label for="membaca">Membaca</label>
                    
                    <input type="checkbox" id="olahraga" name="hobi" value="olahraga">
                    <label for="olahraga">Olahraga</label>
                    
                    <input type="checkbox" id="musik" name="hobi" value="musik">
                    <label for="musik">Musik</label>
                </div>
                
                <div>
                    <label for="kota">Kota:</label>
                    <select id="kota" name="kota">
                        <!-- 
                            TAG <select>
                            - Dropdown list untuk memilih satu opsi
                            - Atribut multiple untuk memilih lebih dari satu
                            - Atribut size untuk menampilkan beberapa opsi sekaligus
                        -->
                        <option value="">-- Pilih Kota --</option>
                        <!-- 
                            TAG <option>
                            - Opsi dalam dropdown
                            - Atribut value: nilai yang dikirim saat dipilih
                            - Teks di antara tag adalah yang ditampilkan
                        -->
                        <option value="jakarta">Jakarta</option>
                        <option value="bandung">Bandung</option>
                        <option value="surabaya">Surabaya</option>
                        <option value="yogyakarta">Yogyakarta</option>
                    </select>
                </div>
                
                <button type="submit">Kirim</button>
                <!-- 
                    TAG <button>
                    - Tombol yang bisa diklik
                    - Atribut type="submit": kirim formulir
                    - type="button": tombol biasa (perlu JavaScript)
                    - type="reset": mengosongkan formulir
                -->
                <button type="reset">Reset</button>
            </form>
        </section>
    </main>

    <!-- ==================== SIDEBAR ==================== -->
    <aside>
        <!-- 
            TAG <aside>
            - Konten tambahan yang berhubungan dengan konten utama
            - Biasanya berupa sidebar, iklan, atau link terkait
            - Bisa diletakkan di dalam <article> atau sebagai elemen independen
        -->
        <h3>Informasi Tambahan</h3>
        <p>Sidebar ini berisi konten pelengkap yang tidak terlalu penting tetapi relevan.</p>
        
        <h4>Link Terkait:</h4>
        <ul>
            <li><a href="#pengenalan">Kembali ke Pengenalan</a></li>
            <li><a href="#struktur">Lihat Struktur</a></li>
            <li><a href="#konten">Lihat Konten</a></li>
        </ul>
    </aside>

    <!-- ==================== FOOTER ==================== -->
    <footer>
        <!-- 
            TAG <footer>
            - Bagian bawah halaman
            - Biasanya berisi informasi hak cipta, kontak, dan link penting
            - Bisa digunakan di akhir halaman atau dalam elemen lain
        -->
        <p>&copy; 2024 Contoh HTML Dasar. Semua hak dilindungi.</p>
        <!-- 
            &copy; adalah karakter khusus untuk simbol copyright ©
        -->
        
        <address>
            <!-- 
                TAG <address>
                - Menyediakan informasi kontak
                - Bisa berisi email, alamat fisik, nomor telepon
                - Biasanya ditampilkan dengan gaya miring
            -->
            Hubungi kami di: <a href="mailto:info@example.com">info@example.com</a>
        </address>
    </footer>

</body>
</html>
