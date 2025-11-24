Sistem Pemesanan Makanan Di Kantin Sekolah 
 Berbasis Web


M. Iqbal S1,Salwa Syahratul Aeni2
Program Studi Sistem Informasi, Universitas Muhammadiyah Banten, Indonesia
Salwasyahratul7@gmail.com

Abstract
The rapid development of information technology has provided convenience in various fields, including the education sector. One of its applications is in the school cafeteria food ordering system. Traditionally, the food ordering process in school cafeterias is still carried out manually, which often leads to long queues, service delays, and difficulties in recording transactions. To address these issues, a Web-Based School Canteen Ordering System was developed, allowing students and teachers to place food orders online through computers or smartphones.
This system is designed using the PHP programming language with the Laravel framework and a MySQL database. The main features provided include user registration, food ordering, menu management, payment processing, and transaction reporting. With this system, the ordering process becomes more efficient, waiting times are reduced, and the cafeteria staff can manage sales and stock data more effectively. Based on the testing results, the system runs well and provides convenience for users in conducting food ordering transactions within the school environment.
Keywords: Information System, School Cafeteria, Online Ordering, Web, Laravel, MySQL
Abstrak
Perkembangan teknologi informasi yang semakin pesat memberikan kemudahan dalam berbagai bidang, termasuk dalam sektor pendidikan. Salah satu penerapan teknologi tersebut adalah pada sistem pemesanan makanan di kantin sekolah. Selama ini, proses pemesanan makanan di kantin sekolah masih dilakukan secara manual, yang sering menimbulkan antrean panjang, keterlambatan pelayanan, dan kesulitan dalam pencatatan transaksi. Untuk mengatasi permasalahan tersebut, dibangunlah Sistem Pemesanan Kantin Sekolah Berbasis Web yang memungkinkan siswa dan guru melakukan pemesanan makanan secara online melalui perangkat komputer atau smartphone.
Sistem ini dirancang menggunakan bahasa pemrograman PHP dengan framework Laravel dan database MySQL. Fitur utama yang disediakan meliputi pendaftaran pengguna, pemesanan makanan, manajemen menu, pembayaran, dan pelaporan transaksi. Dengan adanya sistem ini, proses pemesanan di kantin menjadi lebih efisien, waktu tunggu berkurang, serta membantu pihak kantin dalam mengelola data penjualan dan stok secara lebih teratur. Berdasarkan hasil pengujian, sistem dapat berjalan dengan baik dan memberikan kemudahan bagi pengguna dalam melakukan transaksi pemesanan makanan di lingkungan sekolah.
Kata Kunci: Sistem Informasi, Kantin Sekolah, Pemesanan Online, Web, Laravel, MySQL

Pendahuluan
	Kantin sekolah merupakan salah satu fasilitas penting yang menunjang kegiatan belajar mengajar di sekolah. Kantin menyediakan berbagai jenis makanan dan minuman yang dibutuhkan oleh siswa, guru, serta staf sekolah. Namun dalam praktiknya, sistem pemesanan makanan di banyak sekolah masih dilakukan secara manual, yaitu dengan datang langsung ke kantin, memilih menu, dan membayar di tempat. Proses seperti ini sering menyebabkan antrean panjang terutama pada waktu istirahat, sehingga waktu makan menjadi tidak efisien. Selain itu, sistem manual juga sering menimbulkan kesalahan pencatatan pesanan, kesulitan dalam pengelolaan stok, dan keterlambatan dalam pembuatan laporan penjualan.
Perkembangan teknologi informasi saat ini memungkinkan berbagai kegiatan dilakukan secara digital, termasuk dalam proses pemesanan makanan. Dengan adanya sistem berbasis web, kegiatan pemesanan makanan di kantin dapat dilakukan secara online melalui perangkat komputer atau smartphone. Siswa dan guru dapat memilih menu serta melakukan pemesanan sebelum jam istirahat, sedangkan petugas kantin dapat langsung menerima pesanan dan menyiapkannya sesuai jadwal. Hal ini dapat mengurangi antrean, mempercepat pelayanan, dan meningkatkan efisiensi kerja.
Melihat permasalahan yang ada, dibutuhkan sebuah solusi berupa Sistem Pemesanan Kantin Sekolah Berbasis Web yang mampu membantu proses transaksi antara pembeli dan pihak kantin. Sistem ini dirancang untuk memberikan kemudahan kepada pengguna dalam melakukan pemesanan makanan secara daring, serta membantu pihak kantin dalam mengelola data menu, stok, dan laporan keuangan dengan lebih teratur. Dengan adanya sistem ini diharapkan kegiatan di kantin menjadi lebih modern, cepat, dan efisien, sejalan dengan perkembangan teknologi di lingkungan pendidikan.
1.Metode Penelitian 
Metode penelitian yang paling tepat digunakan adalah metode Waterfall. Metode ini dipilih karena proses pemesanan makanan di kantin memiliki alur kerja yang jelas, teratur, dan jarang mengalami perubahan. Lingkungan sekolah yang terstruktur juga mendukung penerapan metode ini, sehingga setiap tahap pembangunan sistem – mulai dari analisis, perancangan, implementasi, pengujian hingga pemeliharaan – dapat dilakukan dengan lebih terkontrol dan mudah dijelaskan dalam laporan penelitian.

  

                                                            




![alt text](https://github.com/salwasyahratul/UTS-RPL-/blob/main/WATERFALL.SALWA.jpg?raw=true)


Gambar 1.Metode Waterfall 
Metode Waterfall adalah metode pengembangan sistem yang berjalan secara berurutan, dari langkah pertama sampai langkah terakhir, seperti air terjun yang mengalir ke bawah. Setiap tahap harus diselesaikan dulu sebelum masuk ke tahap berikutnya.


1.	Analisis & Perancangan Sistem
A.	Sistem Design
Aktor Utama
1.	Siswa → pengguna yang memesan makanan.
2.	Admin Kantin → mengelola menu, stok, dan validasi pesanan.
3.	Kasir → melakukan konfirmasi pembayaran.
4.	Sistem Pembayaran (opsional) → jika ada metode e-wallet.
Aktivitas Masing-Masing Aktor
Siswa
•	Melihat daftar menu.
•	Memesan makanan/minuman.
•	Melihat status pesanan.
•	Melakukan pembayaran.
•	Membatalkan pesanan.
Admin Kantin
•	Menambah/mengubah/menghapus menu.
•	Mengelola stok makanan.
•	Melihat daftar pesanan.
•	Mengubah status pesanan (diproses, selesai, dibatalkan).
Kasir
•	Menerima notifikasi pesanan masuk.
•	Memverifikasi pembayaran siswa.
•	Mengubah status pembayaran (lunas/belum lunas).

![alt text](https://github.com/salwasyahratul/UTS-RPL-/blob/main/USE.CASE%20SALWA.png?raw=true)
 Gambar 2. Use Case Diagram Sistem pemesanan makanan

                                            
                                        






















![alt text](https://github.com/salwasyahratul/UTS-RPL-/blob/main/CLASSDIAGRAM.SALWA.png?raw=true)

Gambar 3. Class diagram pemesanan makan
2.	ALUR SISTEM PEMESANAN – PEMBAYARAN (Berdasarkan UML)
•	User Login
a.	User (Admin atau Kasir) membuka aplikasi.
b.	User mengisi username dan password.
c.	Sistem memanggil fungsi login() pada class User.
d.	Jika valid, user diarahkan ke halaman sesuai role‐nya:
i.	Admin → Kelola Menu
ii.	Kasir → Buat Pesanan & Pembayaran
•	Admin Mengelola Menu
(Hanya role Admin)
a.	Admin menambah menu baru → tambahMenu() pada Menu.
b.	Admin bisa mengupdate menu → updateMenu().
c.	Admin bisa menghapus menu → hapusMenu().
•	Kasir Membuat Pesanan
a.	Kasir membuat pesanan baru → buatPesanan() pada Pesanan.
b.	Sistem menyimpan:
o	pesananId
o	userId (kasir)
o	statusPesanan = "baru"
c.	Kasir memilih menu → aplikasi membuat beberapa record di DetailPesanan:
o	detailId
o	pesananId
o	menuId
o	qty
o	subTotal
d.	Sistem menghitung totalHarga pesanan berdasarkan sum(subTotal).
•	Update Status Pesanan
a.	Setelah pesanan selesai dibuat, sistem dapat mengubah status melalui updateStatus() pada Pesanan.
Contoh status:
o	“Menunggu Pembayaran”
o	“Dibayar”
o	“Selesai”
•	Pembayaran
a.	Kasir membuka pesanan yang sudah selesai dibuat.
b.	Kasir melakukan pembayaran → sistem membuat objek Pembayaran:
o	pembayaranId
o	pesananId
o	jumlahBayar
o	statusBayar = "menunggu"
c.	Sistem memverifikasi pembayaran → verifikasiPembayaran():
o	Jika berhasil → statusBayar = "lunas", statusPesanan = "selesai"
o	Jika gagal → tetap “menunggu”
 Ringkasan Alur Utama
1.	User login
2.	Admin kelola menu (opsional)
3.	Kasir membuat Pesanan
4.	Kasir menambah DetailPesanan
5.	Sistem menghitung total harga
6.	Pembayaran dibuat
7.	Pembayaran diverifikasi
8.	Pesanan selesai
3.Penerapan prinsip SRP sangat sesuai untuk sistem pemesanan makanan kantin karena setiap bagian dari sistem memiliki tanggung jawab yang berbeda dan tidak saling tumpang-tindih. Pengelolaan menu makanan oleh admin memerlukan kelas yang fokus pada penambahan, pembaruan, dan penghapusan menu tanpa terganggu oleh proses lain. Proses pemesanan makanan oleh siswa adalah tanggung jawab berbeda, sehingga kelas Pesanan hanya mengelola pencatatan pesanan dan statusnya saja. 
Berikut tiga contoh pola desain( creational desaig patterns)











1.	Order Service
OrderService pada gambar merupakan contoh penerapan Single Responsibility Principle (SRP), di mana satu kelas hanya menangani satu jenis tanggung jawab, yaitu pengelolaan data dan proses terkait pemesanan. Kelas ini berfokus sepenuhnya pada operasi order, seperti membuat pesanan baru melalui fungsi createOrder, menghitung total harga item dengan calculateTotal, serta mengubah status pesanan menggunakan updateStatus. Dengan hanya menangani logika yang berhubungan langsung dengan order, kelas ini menjadi lebih terstruktur, mudah dikelola, serta lebih mudah diuji karena tidak bercampur dengan logika lain seperti pembayaran, notifikasi, atau manajemen pengguna.


![alt text](https://github.com/salwasyahratul/UTS-RPL-/blob/main/orderservice.salwa.drawio.png?raw=true)







2.Order Repository
OrderRepository adalah kelas yang bertanggung jawab khusus untuk melakukan operasi data terkait pesanan (order) pada lapisan penyimpanan, seperti database. Dengan menerapkan Single Responsibility Principle (SRP), kelas ini hanya berfokus pada tugas mengelola akses data, sehingga semua proses pengambilan, penyimpanan, dan pembaruan order dilakukan melalui metode seperti save(order), findById(orderId), dan update(order). OrderRepository tidak menangani logika bisnis seperti perhitungan total atau pengubahan status; tugas tersebut tetap berada di OrderService. Pemisahan ini membuat arsitektur lebih bersih, memudahkan pengujian, serta mempermudah penggantian sistem penyimpanan di masa depan tanpa mengubah logika utama aplikasi.


![alt text](https://github.com/salwasyahratul/UTS-RPL-/blob/main/OrderResopotory.salwa.drawio.png?raw=true)














3.Notification Service
NotificationService adalah kelas yang memiliki satu tanggung jawab utama, yaitu mengirimkan notifikasi kepada pengguna ketika terjadi suatu peristiwa dalam sistem, seperti pesanan dibuat, status berubah, atau pembayaran berhasil. Dengan menerapkan Single Responsibility Principle (SRP), kelas ini hanya fokus pada pengelolaan proses pengiriman notifikasi tanpa mencampurkannya dengan logika bisnis lain seperti pembuatan order atau pengelolaan data. Metode-metode seperti sendEmail(user, message) atau sendSMS(user, message) berada di dalam kelas ini karena semuanya berkaitan dengan tugas pengiriman pemberitahuan. Pemisahan ini membuat aplikasi lebih modular, mudah diperluas, dan memungkinkan perubahan pada mekanisme notifikasi—misalnya dari email ke push notification—tanpa memengaruhi bagian sistem lainnya


![alt text](https://github.com/salwasyahratul/UTS-RPL-/blob/main/NotificationServer.Salwa.drawio.png?raw=true)







4.Tahapan tahapan pada salah satu proses penting dalam sistem

![alt text](https://github.com/salwasyahratul/UTS-RPL-/blob/main/TAHAPAN.SALWA.drawio.png?raw=true)




















Berikut tahapan-tahapan proses dari Activity Diagram – Proses Pemesanan Makanan berdasarkan gambar yang kamu kirim.

Tahapan-Tahapan Proses Pemesanan Makanan di Kantin Sekolah
1.	User membuka halaman menu
– Sistem menampilkan daftar makanan yang tersedia.
2.	User memilih makanan
– User memilih salah satu menu yang ingin dipesan.
3.	User memasukkan jumlah pesanan
– User menentukan berapa porsi yang ingin dipesan.
4.	User memutuskan apakah menambah item ke keranjang
– Jika Ya: item ditambahkan ke keranjang.
– Jika Tidak: kembali memilih menu lain.
5.	User membuka keranjang
– User melihat semua item yang sudah dipilih.
6.	User melakukan pengecekan pesanan
– User memastikan daftar pesanan sudah sesuai.
7.	Keputusan apakah pesanan sudah benar
– Jika Ya: user klik tombol "Pesan".
– Jika Belum: user kembali ke menu untuk mengubah pesanan.
8.	Sistem menghitung total harga
– Sistem menghitung harga seluruh item beserta jumlahnya.
9.	Sistem menyimpan pesanan ke database
– Sistem mencatat data pesanan ke dalam sistem.
10.	Sistem mengirim notifikasi status pesanan ke user
– Misalnya status: “Pesanan diterima / sedang diproses”.
11.	Proses selesai


State Machine 
![alt text](https://github.com/salwasyahratul/UTS-RPL-/blob/main/state%20machine.salwa.drawio.png?raw=true)


