BAB III
ANALISIS DAN PERANCANGAN

3.1 	Analisis
	Sebelum merancang sebuah aplikasi yang akan dibangun, factor yang harus diperhatikan adalah tahap analisis. Tahap analisis merupakan tahap pemahaman dengan perangkat lunak yang akan dibangun, kebutuhan fungsional, diagram alir data, kamus alir data, dan enkripsi proses. Tahap analisis bertujuan untuk mengetahui mekanisme system, proses-proses yang terlibat dalam system, serta hubungan antara proses tersebut.
	Analisis adalah tahap yang sangat penting karena suatu kesalahan dalam tahap ini akan mempengaruhi pada tahap berikutnya. Penelitian membuktikan bahwa kesalahan yang diperbaiki setelah tahap analisis akan memakan biaya yang lebih besar daripada jika diperbaiki saat dilakukan analisis.
3.1.1 	Analisis Sistem Yang Sedang Berjalan
	Analisis system yang sedang berjalan sekarang meliputi :
1.	Pencatatan dan pendataan penjualan di Butik Puspa masih tersimpan dalam bentuk faktur marvel, buku catatan, hingga buku buku besar oleh bagian manajemen.
2.	Aplikasi yang memiliki fungsi disposisi arsip yang belum dimiliki oleh bagian Butik Puspa.
3.	Lamanya dalam proses pencarian data dokumen oleh bagian pegawai, karena pegawai harus memeriksa tempat penyimpanan arsip satu persatu.
4.	Kurangnya informasi pada pengrajinnya, yang berkaitan pada stok batik tersebut.

3.1.1.1 Alur yang sedang berjalan
Keterangan : 
1.	Pelanggan mendatangi butik.
2.	Pelanggan memilih barang yang di inginkan.
3.	Butik menyediakan barang yang akan di beli oleh pelanggan dengan cara melakukan cek barang.
4.	Setelah melakukan pengecekan barang, jika tersedia maka pihak butik akan membuatkan nota penjualan. 
5.	Kemudian pelanggan akan mendapatkan nota penjulaan. 
6.	Pihak butik akan membuat sebuah laporan penjualan ketika transaksi sudah terjadi.
7.	Pihak gudang akan membuat batik dan akan membuat laporan data batik untuk di kirim ke butik.
3.1.2 	Analisis Sistem Yang akan Dibangun
	Analisis system yang akan dibangun digunakan untuk proses manajemen pengelolaan penjualan dimana aplikasi tersebut dapat mengikuti prosedur yang telah kami buat sehingga dapat mempermudah pengelolaan data gudang dan data pembelian. Adapun alur manajemen system aplikasi Batik di Butik Puspa Berbasis Framework dan SMS Gateway yang akan dibangun adalah sebagai berikut:
1.	Pihak Manajemen dapat memonitoring kegiatan yang ada di Butik Puspa mulai dari menerima sms untuk persedian barang, mengirim data pemesanan ke pengrajin hingga melihat aktivitas transaksi penjualan di Butik Puspa.
2.	Pegawai Butik Puspa dapat melakukan pengecekan data barang, membuat faktur penjualan hingga pembuatan laporan.
3.	Data laporan penjualan yang dibuat oleh pegawai Butik Puspa akan dikirim ke pihak.
3.1.2.1 Flowmap Aplikasi Yang Akan Dibangun
Keterangan:
1.	Pelanggan melihat dan memilih batik
2.	Butik login, melihat persediaan dan data akan ditampilkan. 
3.	Jika tidak ada batik yang diingkan maka pelanggan memilih kembali.
4.	Setelah butik menampilkan data maka membuat faktur penjualan dan langsung mengecek ketersediaan barang.
5.	Laporan sisa batik dari butik langsung konfirmasi ke manajemen dengan sms gateway.
6.	Maka manajemen akan menerima sms barang yang sudah habis dijual di butik.
7.	Lalu, manajemen akan mengirim sms pemesanan ke bagian pengrajin atau gudang untuk membuat batik yang sudah habis.
8.	Setelah pembuatan batik selesai maka pengrajin akan penginputkan batik yang sudah jadi.
9.	Manajemen dapat melihat hasil penjualan ke bagian butik memalui system.
3.1.1	Deskripsi Kebutuhan Aplikasi
Pembuatan manajemen system aplikasi Batik di Butik Puspa Berbasis Framework Codeigniter dan SMS Gateway (Sub: Pengelolaan Penjualan) ini dibangun untuk membantu pemilik mudah mengelola persedian barang.
Sistem yang dibuat ini memberikan hak akses yaitu :
Tabel 3.1 Hak Akses Untuk Pengguna Aplikasi
Kategori Pengguna	Tugas
Manajemen
Gudang/Pengrajin
Butik
Pembeli	Mengontrol persedian barang di butik dan di gudang.
Mendesain dan membuat batik.
Menjual stok batik.
Memilih dan membeli batik yang sudah disediakan di butik.
3.1.3.1 Analisis Kebutuhan Perangkat Lunak Dan Perangkat Keras
Spesifikasi perangkat lunak yang dibutuhkan adalah sebagai berikut :
Tabel 3.2 spesifikasi perangkat lunak
Administrator
Operating Sistem	:	Microsoft Windows 7
Development Tools	:	Sublime Text 2, Bizagi Modeler
DBMS / Bahasa Pemrograman	:	Microsoft SQL Server 2008
Aplikasi	:	CodeIgniter, SMS Gateway
3.1.3.2	Analisis Kebutuhan Perangkat Keras yang dibutuhkan untuk Membangun Aplikasi ini
Spesifikasi Perangkat keras yang dibutuhkan adalah sebagai berikut :
Tabel 3.3 Spesifikasi Perangkat Keras
Administrator
Procesor	:	Intel® Core™ i3-3217U 
Memory	:	4.00 GB
Hardisk	:	SATA 1.00 GB
VGA	:	2024 MB
3.2 	Perancangan 
Berikut ini adalah suatu gambar analisis sistem pada perancangan dan Pembuatan manajemen system aplikasi Batik di Butik Puspa menggunakan UML, yang terdiri dari usecase Diagram, class Diagram, sequence diagram, collaboration diagram, activity diagram, statechart diagram, component diagram, dan deployment diagram. 
3.2.1 Usecase Diagram
3.2.1.1 Definisi Use Case Diagram
Use Case diagram merupakan model diagaram yang akan digunakan untuk menggambarkan requirement fungsional dari sistem yang akan dibuat. Pada use case diagram ini akan menekankan “siapa” melakukan “apa” dalam sistem yang akan dibuat.
Keterangan:
1.	Butik mengelola penjualan dan membuat laporan penjualan.
2.	Pengrajin membuat batik, mengelola pergudangan, dan membuat laporan pergudangan.
3.	Manajemen dapat mengelola gudang dan butik.
4.	Pelanggan dapat memilih batik, membeli batik, dan mendapat nota.
5.	Butik, pengrajin, dan manajemen sebelum mengelola harus login terlebih dahulu.
6.	Butik, pengrajin, dan manajemen saling berkomunikasi menggunakan SMS Gateway.
3.2.2.1 Definisi Class Diagram
Class Diagram digunakan untuk menunjukan atau menggambarkan kelas-kelas yang ada pada sistem yang akan dibangun dan juga hubungannya antara satu dengan yang lainnya, yang juga di dalamnya terdapat atribut dan juga oprasi yang akan dilakukan oleh sistem
Pada Gambar 3.6 merupakan class diagram dari sistem yang sedang dibangun. Pada class diagram tersebut terdapat kelas yang saling berhubungan satu sama lain. Pada kelas “Pelanggan, Butik, Gudang/Pengrajin, Administrasi dan Manajemen” terdapat kelas yang mempunya fungsi masing-masing.
3.2.3	Sequence Diagram
Sequence diagram adalah suatu diagram yang menggambarkan interaksi antar obyek dan mengindikasikan komunikasi diantara objek-objek tersebut. Diagram ini juga menunjukkan serangkaian pesan yang dipertukarkan oleh objek-objek yang melakukan suatu tugas atau aksi tertentu. Objek-objek tersebut kemudian diurutkan dari kiri ke kanan, aktor yang menginisiasi interaksi biasanya ditaruh di paling kiri dari diagram.
3.2.3.1 Sequence Diagram Login
Keterangan:
Pada gambar diatas terdapat Sequence diagram login yakni Manajemen, Butik dan Gudang/Pengrajin melakukan input username dan password kemudian masuk ke form login, kemudian setelah username dan password masuk ke dalam database maka system akan melakukan validasi data login kemudian masuk ke halaman menu utama. Jika gagal system akan kembali ke form login.

