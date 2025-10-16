CampusIntern


Merupakan sebuah website penyedia lowongan magang yang dapat membantu para mahasiswa dalam mencari dan melakukan magang. 


bahasa pemrograman yang digunakan yaitu:
- html
- css
- javascript


Fitur:
1. Navigasi bar
merupakan sebuah fitur yg terdapat di bagian atas website tiap halaman, yg membantu kita untuk mengarahkan ke masing-masing halaman yang tersedia. terdapat dua halaman yg berarti ada dua opsi di bagian navbar. yg pertama yaitu homepage, dan yg kedua adalah informasi.

2. Dark mode & Light mode
fitur ini akan mengatur tampilan warna dalam website. dark mode yg berarti tampilan web kami akan dominan berwarna gelap, dan light mode yg berarti tampilan web akan dominan berwarna terang. 

3. Button "Cari Magang"
sebuah fitur simple yg akan mengarahkan kita ke halaman ke dua (informasi magang) setelah kita menekan button "cari magang".

4. FAQ (Frequently Asked Question)
fitur yg memberikan jawaban atas pertanyaan-pertanyaan yg sering ditanyakan oleh para user. dengan tampilan awal pertanyaan yg bisa didropdown sehingga muncul jawaban yg diinginkan.

5. button dropdown informasi magang
merupakan fitur yg jika kita tekan buttonnya, sistem akan menjabarkan informasi detail mengenai lowongan magang yg tersedia di suatu perusahaan tersebut. awalnya, jika kita tidak tekan button dropdownnya, maka hanya menampilkan informasi sekilas tentang lowongan pekerjaannya.

6. Button Website dan Instagram perusahaan
merupakan button yg akan mengarahkan ke website dan social media instagram dari perusahaan yg membuka lowongan magang tersebut.

7. button daftar
merupakan fitur untuk para user dapat melakukan pendaftaran pada suatu perusahaan yg membuka lowongan magang. button ini akan mengarahkan kita ke formulir pendafaran magang yg bisa kita isi sesuai dengan data pribadi.

8. input user
pada halaman formulir pendaftaran magang. user dapat melakukan input data seperti:
- nama lengkap, alamat domisili, nomor handphone, asal sekolah/universitas, program studi, jurusan, semester, ipk, posisi/jabatan yg dilamar, alasan mengikuti magang (text)
- jenis kelamin, pendidikan terakhir, sumber info lowongan (option)
- tanggal lahir (date)
- email (email)
- upload cv, portofolio (file)

9. button kembali
yg akan muncul saat kita sudah selesai mengisi formulir pendaftaran magang, yg berguna untuk kembali ke halaman utama.


Cara instalasi dan penggunaan

Instalasi:
Tidak perlu instalasi.  
Website sudah bisa diakses langsung melalui link berikut:  
https://zaryan19.github.io/Project-UTS-Campus-Intern-Web-Kelompok-5-/index.html

Cara penggunaan:
1. membuka halaman utama web yg bisa diakses melalui link ini: https://zaryan19.github.io/Project-UTS-Campus-Intern-Web-Kelompok-5-/index.html 
2. Jika:
- ingin langsung mencari lowongan magang: bisa langsung menekan tombol "cari magang" yg ada halaman utama atau bisa menekan navigasi bar bernama "informasi" yg fungsinya sama akan mengarahkan ke halaman lowongan magang yg tersedia
- mempunyai pertanyaan tentang website kami: bisa langsung ke bagian bawah dari halaman utama, terdapat fitur FAQ yg akan membantu kita dalam menjawab pertanyaan yg familiar/sering ditanyakan.
3. setelah ke halaman informasi lowongan magang, bisa dilihat-lihat terlebih dahulu lowongan mana yg ingin ditelusuri. jika ingin melihat detail, tekan button "selengkapnya/icon segitiga dropdown".
4. jika ingin melihat profile dari perusahaan, bisa menekan button website ataupun instagram yg akan mengarahkan sesuai tujuan.
5. klik tombol daftar, untuk mengisi formulir pendaftaran pada suatu perusahaan
6. mengisi semua data yg diperlukan untuk pendaftaran
7. setelah selesai, pengumuman lowongannya akan disampaikan melalui email masing-masing pendaftar.


Penjelasan Code Html, css, dan javascript pada tiap fitur:

1. navigasi bar
**html:**
<nav class="navbar">
      <div class="nav-brand">CampusIntern</div>
      <ul class="nav-menu">
        <li><a href="index.html">Beranda</a></li>
        <li><a href="info.html">Informasi</a></li>
      </ul>
    </nav>
    
a.	<nav>
Menandakan bahwa bagian ini adalah navigasi utama pada halaman web. Browser, pembaca layar, dan mesin pencari (seperti Google) bisa langsung tahu bahwa bagian ini berisi tautan penting untuk berpindah antar halaman.
b.	<div class="nav-brand">CampusIntern</div>
Ini bagian logo atau nama merek dari websitenya, yaitu CampusIntern. nav-brand bisa digunakan di CSS untuk mengatur posisi (misal di kiri navbar) dan gaya teks (misalnya ukuran besar atau tebal).
c.	Menu navigasi
Elemen <ul> menandakan sebuah daftar tidak berurutan (unordered list). Di dalamnya terdapat dua item <li> yang masing-masing berisi elemen <a> (tautan). Tautan tersebut mengarahkan pengguna ke halaman:
•	index.html → Halaman Beranda
•	info.html → Halaman Informasi

**css:**
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 15px 40px;
  background: #343a41;
  color: #fff;
  flex-wrap: wrap;
}
#Bagian ini mengatur tata letak utama dari navigasi agar rapi dan sejajar menggunakan Flexbox.
#Elemen-elemen di dalamnya seperti nama brand dan menu ditempatkan secara horizontal dan berjarak seimbang di kiri dan kanan.
Warna latar belakangnya menggunakan warna gelap (#343a41), dengan teks berwarna putih agar kontras dan mudah dibaca.
Padding juga ditambahkan untuk memberi jarak antara isi dengan tepi navbar.

.nav-brand {
  font-weight: bold;
  font-size: 1.5em;
}
#Bagian ini mengatur tampilan nama atau logo website, yaitu CampusIntern.
Huruf dibuat tebal dan berukuran lebih besar supaya terlihat menonjol di bagian kiri navbar.

.nav-menu {
  list-style: none;
  display: flex;
  gap: 20px;
}
#Kelas ini digunakan untuk mengatur daftar menu navigasi, seperti “Beranda” dan “Informasi”.
#Dengan display: flex;, menu ditampilkan secara horizontal, bukan vertikal.
gap: 20px; memberi jarak antar item menu agar tidak saling menempel, dan list-style: none; menghilangkan titik daftar bawaan.

.nav-menu li a {
  color: white;
  text-decoration: none;
  font-weight: 500;
}
#Mengatur gaya tampilan tautan dalam menu. Warna teks diatur menjadi putih agar sesuai dengan tema navbar, dan text-decoration: none; menghapus garis bawah pada link supaya tampil lebih bersih. Selain itu, font-weight: 500; memberi ketegasan pada teks agar terlihat profesional tapi tetap ringan.


2. Dark mode dan Light mode
**html:**

     <button id="darkModeToggle" class="dark-mode-toggle">Dark Mode</button>
     
#Elemen <button> berfungsi sebagai tombol interaktif yang dapat diklik oleh pengguna. id="darkModeToggle" digunakan agar tombol ini bisa dikenali oleh JavaScript dan diberi fungsi untuk mengganti tema situs ke mode gelap (dark mode). Elemen <button> bersifat semantik interaktif, menandakan bahwa elemen ini digunakan untuk melakukan suatu aksi, bukan hanya berpindah halaman.

**css:**
body.dark {
  background-color: #1e1e1e;
  color: #f5f5f5;
}

body.dark .faq {
  background-color: #2a2a2a;
  box-shadow: 0 4px 8px rgba(255, 255, 255, 0.1);
}

body.dark .faq-question {
  color: #fff; /* tulisan pertanyaan jadi putih */
  border-color: #444;
}
#body.dark digunakan untuk mengaktifkan mode gelap pada website. Bagian ini mengubah warna background menjadi gelap dan warna teks menjadi lebih terang agar tetap terbaca. body.dark .faq mengubah tampilan kotak FAQ saat dark mode dengan memberi background abu gelap dan bayangan terang agar tetap kontras. body.dark .faq-question mengubah warna teks pertanyaan menjadi putih dan memberi border lebih gelap agar tetap jelas terlihat dalam mode gelap.

**javascript:**
const toggleBtn = document.getElementById('darkModeToggle');

// Cek preferensi dark mode sebelumnya dari localStorage
if (localStorage.getItem('darkMode') === 'enabled') {
  document.body.classList.add('dark');
  toggleBtn.textContent = 'Light Mode';
} else {
  toggleBtn.textContent = 'Dark Mode';
}

// Tombol toggle
toggleBtn.addEventListener('click', () => {
  document.body.classList.toggle('dark');

  // Simpan preferensi di localStorage
  if (document.body.classList.contains('dark')) {
    localStorage.setItem('darkMode', 'enabled');
    toggleBtn.textContent = 'Light Mode';
  } else {
    localStorage.setItem('darkMode', 'disabled');
    toggleBtn.textContent = 'Dark Mode';
  }
});
#a.	toggleBtn mengambil tombol pengaktif dark mode.
#b.	Bagian cek localStorage digunakan untuk mengecek apakah sebelumnya dark mode sudah aktif. Kalau iya, saat halaman dibuka dark mode langsung aktif lagi.
#c.	Event toggleBtn.addEventListener('click') dipakai untuk mengubah mode saat tombol diklik dengan menambah atau menghapus class dark pada <body>.
#d.	localStorage.setItem menyimpan status dark mode (enabled atau disabled) supaya pilihan pengguna tidak hilang saat reload.
#e.	textContent tombol ikut diganti agar tulisan berubah sesuai mode (Dark Mode / Light Mode).


3. Button "cari magang"
**html:**
<div class="search-box">
        <button><a href="info.html">🔍Cari Magang</a></button>
      </div>

#Elemen <div class="search-box">
Elemen ini berfungsi sebagai wadah untuk tombol pencarian magang. Biasanya diberi gaya CSS agar tampil menonjol, seperti tombol besar di tengah halaman.

#Elemen <button><a href="info.html">🔍 Cari Magang</a></button>
Bagian ini menampilkan tombol bertuliskan “Cari Magang” dengan ikon 🔍 (lup). Di dalam tombol terdapat elemen <a> yang mengarahkan pengguna ke halaman info.html, yaitu halaman berisi daftar informasi magang. Kombinasi ini memberikan kesan interaktif dan memudahkan pengguna untuk langsung menuju ke halaman pencarian magang.

**css:**
.search-box {
  position: relative;
  z-index: 2;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  background: rgba(255, 255, 255, 0.9);
  padding: 15px;
  border-radius: 10px;
  max-width: 170px;
  margin: 30px auto 0;
  gap: 10px;
}
#Bagian utama pembungkus kotak pencarian. Menggunakan flexbox supaya isi (input, select, button) sejajar dan responsif. justify-content: center membuat semua elemen berada di tengah. Latar belakangnya putih transparan (rgba(255, 255, 255, 0.9)) agar terlihat lembut di atas background lain. Diberi padding dan border-radius supaya tampilannya tidak kaku (membulat di tepi). margin: 30px auto 0 membuatnya berada di tengah halaman dengan jarak ke atas. gap: 10px memberi jarak antar elemen di dalamnya.


3. 






