<div align="center">
  <h3 align="center">PEMROGRAMAN MOBILE</h3>
  <h3 align="center">Pemrograman Asynchronous</h3>
  <a href="https://github.com/othneildrew/Best-README-Template">
    <img src="img/logo_polinema.png" alt="Logo" width="300" height="300">
  </a>

  <h3 align="center">Abiyasa Putra Prasetya</h3>
  <h3 align="center">3G - D4TI</h3>
  <h3 align="center">01</h3>
  <h3 align="center">2141720203</h3>
</div>

# Praktikum 1: Mengunduh Data dari Web Service (API)

Langkah 1: Buat Project Baru

Buatlah sebuah project flutter baru dengan nama books di folder src week-12 repository GitHub Anda.

Kemudian Tambahkan dependensi http dengan mengetik perintah berikut di terminal.

Soal 1:

Tambahkan nama panggilan Anda pada title app sebagai identitas hasil pekerjaan Anda.

<p align="center">
  <img src="img/praktikum_1/soal1.png" alt="Alt text">
</p>

<p align="center">
  <img src="img/praktikum_1/1.png" alt="Alt text">
</p>

Langkah 2: Cek file pubspec.yaml

Jika berhasil install plugin, pastikan plugin http telah ada di file pubspec ini seperti berikut.

<p align="center">
  <img src="img/praktikum_1/2.png" alt="Alt text">
</p>

Langkah 3: Buka file main.dart

Ketiklah kode seperti berikut ini.

<p align="center">
  <img src="img/praktikum_1/3.png" alt="Alt text">
</p>

Langkah 4: Tambah method getData()

Tambahkan method ini ke dalam class _FuturePageState yang berguna untuk mengambil data dari API Google Books.

<p align="center">
  <img src="img/praktikum_1/4.png" alt="Alt text">
</p>

Langkah 5: Tambah kode di ElevatedButton

Tambahkan kode pada onPressed di ElevatedButton seperti berikut.

<p align="center">
  <img src="img/praktikum_1/5.png" alt="Alt text">
</p>

Lakukan run aplikasi Flutter Anda. Anda akan melihat tampilan akhir seperti gambar berikut. Jika masih terdapat error, silakan diperbaiki hingga bisa running.

<p align="center">
  <img src="img/praktikum_1/run.png" alt="Alt text">
</p>

Soal 3:

Jelaskan maksud kode langkah 5 tersebut terkait substring dan catchError!

Jawab:

-  Aplikasi melakukan permintaan untuk mendapatkan data.

-  Jika berhasil, ambil 450 karakter pertama dari data yang diterima dan tampilkan.

-  Jika ada masalah saat ambil data, tampilkan pesan 'An error occured'.

# Praktikum 2: Menggunakan await/async untuk menghindari callbacks

Langkah 1: Buka file main.dart

Tambahkan tiga method berisi kode seperti berikut di dalam class _FuturePageState.

<p align="center">
  <img src="img/praktikum_2/1.png" alt="Alt text">
</p>

Langkah 2: Tambah method count()

Lalu tambahkan lagi method ini di bawah ketiga method sebelumnya.

<p align="center">
  <img src="img/praktikum_2/2.png" alt="Alt text">
</p>

Langkah 3: Panggil count()

Lakukan comment kode sebelumnya, ubah isi kode onPressed() menjadi seperti berikut.

<p align="center">
  <img src="img/praktikum_2/3.png" alt="Alt text">
</p>

Langkah 4: Run

Akhirnya, run atau tekan F5 jika aplikasi belum running. Maka Anda akan melihat seperti gambar berikut, hasil angka 6 akan tampil setelah delay 9 detik.

<p align="center">
  <img src="img/praktikum_2/run.png" alt="Alt text">
</p>

# Praktikum 3: Menggunakan Completer di Future

Langkah 1: Buka main.dart

Pastikan telah impor package async berikut.

<p align="center">
  <img src="img/praktikum_3/1.png" alt="Alt text">
</p>

Langkah 2: Tambahkan variabel dan method

Tambahkan variabel late dan method di class _FuturePageState seperti ini.

<p align="center">
  <img src="img/praktikum_3/2.png" alt="Alt text">
</p>

Langkah 3: Ganti isi kode onPressed()

Tambahkan kode berikut pada fungsi onPressed(). Kode sebelumnya bisa Anda comment.

<p align="center">
  <img src="img/praktikum_3/3.png" alt="Alt text">
</p>

Langkah 4:

Terakhir, run atau tekan F5 untuk melihat hasilnya jika memang belum running. Bisa juga lakukan hot restart jika aplikasi sudah running. Maka hasilnya akan seperti gambar berikut ini. Setelah 5 detik, maka angka 42 akan tampil.

<p align="center">
  <img src="img/praktikum_3/run.png" alt="Alt text">
</p>

Soal 5:

Jelaskan maksud kode langkah 2 tersebut!

Jawab:

Membuat Objek Completer: Kode completer = Completer<int>(); membuat objek Completer yang bertindak sebagai penanda atau penyelesaian (completion) untuk Future yang akan diselesaikan suatu saat nanti.
Objek Completer ini adalah seperti janji untuk memberikan nilai int di masa mendatang yang akan digunakan oleh Future. Saat fungsi calculate() selesai dijalankan, completer.complete(42); akan menandai bahwa nilai yang dijanjikan telah tersedia dan akan menyelesaikan Future yang sebelumnya dibuat.

Jadi, secara sederhana, objek Completer digunakan untuk memberikan nilai ke Future di suatu waktu nanti ketika proses perhitungan selesai dilakukan.

<p align="center">
  <img src="img/praktikum_3/2.png" alt="Alt text">
</p>

# Praktikum 4: Memanggil Future secara paralel

Langkah 1: Buka file main.dart

Tambahkan method ini ke dalam class _FuturePageState

<p align="center">
  <img src="img/praktikum_4/1.png" alt="Alt text">
</p>

Langkah 2: Edit onPressed()

Anda bisa hapus atau comment kode sebelumnya, kemudian panggil method dari langkah 1 tersebut.

<p align="center">
  <img src="img/praktikum_4/2.png" alt="Alt text">
</p>

Langkah 3: Run

Anda akan melihat hasilnya dalam 3 detik berupa angka 6 lebih cepat dibandingkan praktikum sebelumnya menunggu sampai 9 detik.

<p align="center">
  <img src="img/praktikum_4/run.png" alt="Alt text">
</p>

Soal 7:

Capture hasil praktikum Anda berupa GIF dan lampirkan di README

Langkah 4: Ganti variabel futureGroup

Anda dapat menggunakan FutureGroup dengan Future.wait seperti kode berikut.

<p align="center">
  <img src="img/praktikum_4/4.png" alt="Alt text">
</p>

Soal 8:

Jelaskan maksud perbedaan kode langkah 1 dan 4!

Jawab:

-  FutureGroup: Pada langkah 1, FutureGroup digunakan untuk mengelompokkan beberapa Future menjadi satu kelompok sehingga dapat ditangani secara bersamaan. Dalam kasus ini, ketika semua Future yang ditambahkan ke dalam FutureGroup sudah selesai, futureGroup.future akan menghasilkan List<int> dari hasil Future yang terkumpul. Kemudian, hasilnya dijumlahkan dan diperbarui ke dalam setState.

-  Future.wait: Pada langkah 4, Future.wait digunakan untuk menunggu sejumlah Future sekaligus dan mengembalikan List dari hasil Future yang sudah selesai. Ini berguna ketika kamu hanya perlu menunggu sekelompok Future selesai tanpa memerlukan manipulasi lain pada kelompok tersebut. Kemudian, ketika semua Future selesai, Future.wait akan mengembalikan List<int> dengan hasil dari masing-masing Future.

Jadi, perbedaannya terletak pada penggunaan FutureGroup untuk mengelompokkan Future dan kemudian mendapatkan hasilnya sebagai satu List di langkah 1, sedangkan pada langkah 4, Future.wait langsung menunggu sekelompok Future dan mengembalikan hasilnya sebagai List ketika semuanya selesai.

# Praktikum 5: Menangani Respon Error pada Async Code

Langkah 1: Buka file main.dart

Tambahkan method ini ke dalam class _FuturePageState

<p align="center">
  <img src="img/praktikum_5/1.png" alt="Alt text">
</p>

Langkah 2: ElevatedButton

Ganti dengan kode berikut

<p align="center">
  <img src="img/praktikum_5/2.png" alt="Alt text">
</p>

Langkah 3: Run

Lakukan run dan klik tombol GO! maka akan menghasilkan seperti gambar berikut.

<p align="center">
  <img src="img/praktikum_5/run.png" alt="Alt text">
</p>

Pada bagian debug console akan melihat teks Complete seperti berikut.

<p align="center">
  <img src="img/praktikum_5/debug.png" alt="Alt text">
</p>


Langkah 4: Tambah method handleError()

Tambahkan kode ini di dalam class _FutureStatePage

<p align="center">
  <img src="img/praktikum_5/4.png" alt="Alt text">
</p>

Soal 10:

Panggil method handleError() tersebut di ElevatedButton, lalu run. Apa hasilnya? Jelaskan perbedaan kode langkah 1 dan 4!

Jawab:

<p align="center">
  <img src="img/praktikum_5/4.png" alt="Alt text">
</p>

-  returnError() dipanggil sebagai Future.

-  Jika returnError() berjalan tanpa masalah, maka kode di dalam then akan dieksekusi. Ini mengatur result menjadi 'Success' dan memperbarui tampilan.

-  Namun, jika returnError() mengalami masalah atau error, maka blok kode di dalam catchError akan dieksekusi. Ini mengatur result menjadi pesan error yang dihasilkan dan memperbarui tampilan.

-  Setelah selesai, kode di dalam .whenComplete() akan dieksekusi, dalam hal ini, akan mencetak 'Complete'. Ini terjadi setelah Future selesai, baik berhasil atau terjadi kesalahan.

# Praktikum 6: Menggunakan Future dengan StatefulWidget

Langkah 1: install plugin geolocator

Tambahkan plugin geolocator dengan mengetik perintah berikut di terminal.

<p align="center">
  <img src="img/praktikum_6/1.png" alt="Alt text">
</p>

Langkah 2: Tambah permission GPS

Jika Anda menargetkan untuk platform Android, maka tambahkan baris kode berikut di file android/app/src/main/androidmanifest.xml

<p align="center">
  <img src="img/praktikum_6/2.png" alt="Alt text">
</p>

Langkah 3: Buat file geolocation.dart

Tambahkan file baru ini di folder lib project Anda.

<p align="center">
  <img src="img/praktikum_6/3.png" alt="Alt text">
</p>

Langkah 4: Buat StatefulWidget

Buat class LocationScreen di dalam file geolocation.dart

<p align="center">
  <img src="img/praktikum_6/4.png" alt="Alt text">
</p>

Langkah 5: Isi kode geolocation.dart

<p align="center">
  <img src="img/praktikum_6/5.png" alt="Alt text">
</p>

Soal 11:

Tambahkan nama panggilan Anda pada tiap properti title sebagai identitas pekerjaan Anda.

Jawab:

<p align="center">
  <img src="img/praktikum_6/soal11.png" alt="Alt text">
</p>

Langkah 6: Edit main.dart

Panggil screen baru tersebut di file main Anda seperti berikut.

<p align="center">
  <img src="img/praktikum_6/6.png" alt="Alt text">
</p>

Langkah 7: Run

Run project Anda di device atau emulator (bukan browser), maka akan tampil seperti berikut ini.

<p align="center">
  <img src="img/praktikum_6/run.png" alt="Alt text">
</p>

Langkah 8: Tambahkan animasi loading

Tambahkan widget loading seperti kode berikut. Lalu hot restart, perhatikan perubahannya.

<p align="center">
  <img src="img/praktikum_6/8.png" alt="Alt text">
</p>

Soal 12:

Jika Anda tidak melihat animasi loading tampil, kemungkinan itu berjalan sangat cepat. Tambahkan delay pada method getPosition() dengan kode await Future.delayed(const Duration(seconds: 3));

Jawab: 

<p align="center">
  <img src="img/praktikum_6/loading.png" alt="Alt text">
</p>

Output:

<p align="center">
  <img src="img/praktikum_6/soal12.gif" alt="Alt text">
</p>

Apakah Anda mendapatkan koordinat GPS ketika run di browser? Mengapa demikian?

Jawab:

<p align="center">
  <img src="img/praktikum_6/rungps.png" alt="Alt text">
</p>

Saat menjalankan aplikasi Flutter di browser, peramban menyediakan koordinat palsu atau disimulasikan sebagai pengganti nilai GPS yang sebenarnya. Ini memungkinkan aplikasi untuk mengakses "lokasi palsu" yang diberikan oleh peramban untuk keperluan pengembangan dan pengujian, bukan nilai koordinat GPS yang sebenarnya dari perangkat.

# Praktikum 7: Manajemen Future dengan FutureBuilder

Langkah 1: Modifikasi method getPosition()

Buka file geolocation.dart kemudian ganti isi method dengan kode ini.

<p align="center">
  <img src="img/praktikum_7/1.png" alt="Alt text">
</p>

Langkah 2: Tambah variabel

Tambah variabel ini di class _LocationScreenState

<p align="center">
  <img src="img/praktikum_7/2.png" alt="Alt text">
</p>

Langkah 3: Tambah initState()

Tambah method ini dan set variabel position

<p align="center">
  <img src="img/praktikum_7/3.png" alt="Alt text">
</p>

Langkah 4: Edit method build()

Ketik kode berikut dan sesuaikan. Kode lama bisa Anda comment atau hapus.

<p align="center">
  <img src="img/praktikum_7/4.png" alt="Alt text">
</p>

Soal 13:

Apakah ada perbedaan UI dengan praktikum sebelumnya? Mengapa demikian?

Jawab:

Tidak ada perubahan UI

<p align="center">
  <img src="img/praktikum_7/soal13.gif" alt="Alt text">
</p>

Langkah 5: Tambah handling error

Tambahkan kode berikut untuk menangani ketika terjadi error. Kemudian hot restart.

<p align="center">
  <img src="img/praktikum_7/5.png" alt="Alt text">
</p>

Soal 14:

Apakah ada perbedaan UI dengan langkah sebelumnya? Mengapa demikian?

Tidak ada perubahan UI

<p align="center">
  <img src="img/praktikum_7/soal13.gif" alt="Alt text">
</p>

# Praktikum 8: Navigation route dengan Future Function

Langkah 1: Buat file baru navigation_first.dart

Buatlah file baru ini di project lib Anda.

<p align="center">
  <img src="img/praktikum_8/1.png" alt="Alt text">
</p>

Langkah 2: Isi kode navigation_first.dart

<p align="center">
  <img src="img/praktikum_8/2.png" alt="Alt text">
</p>

Soal 15:

Tambahkan nama panggilan Anda pada tiap properti title sebagai identitas pekerjaan Anda.

<p align="center">
  <img src="img/praktikum_8/soal15.png" alt="Alt text">
</p>

Langkah 3: Tambah method di class _NavigationFirstState

Tambahkan method ini.

<p align="center">
  <img src="img/praktikum_8/3.png" alt="Alt text">
</p>

Langkah 4: Buat file baru navigation_second.dart

Buat file baru ini di project lib Anda. Silakan jika ingin mengelompokkan view menjadi satu folder dan sesuaikan impor yang dibutuhkan.

<p align="center">
  <img src="img/praktikum_8/4.png" alt="Alt text">
</p>

Langkah 5: Buat class NavigationSecond dengan StatefulWidget

<p align="center">
  <img src="img/praktikum_8/5.png" alt="Alt text">
</p>

Langkah 6: Edit main.dart

Lakukan edit properti home.

<p align="center">
  <img src="img/praktikum_8/6.png" alt="Alt text">
</p>

Langkah 8: Run

Lakukan run, jika terjadi error silakan diperbaiki.

<p align="center">
  <img src="img/praktikum_8/run.gif" alt="Alt text">
</p>

Soal 16:

Cobalah klik setiap button, apa yang terjadi ? Mengapa demikian ?

Jawab:

Saat menekan tombol 'Change Color' pada layar pertama, aplikasi beralih ke layar kedua yang memiliki tiga tombol: 'Red', 'Green', dan 'Blue' untuk memilih warna.

Namun, ada kesalahan dalam kode yang membuatnya tidak berfungsi sebagaimana mestinya. Variabel yang menyimpan warna pada layar kedua tidak diatur dengan benar, sehingga pemilihan warna tidak berdampak pada layar pertama. Jadi, saat tombol dipilih, perubahan warna tidak tercermin kembali di layar pertama.

Gantilah 3 warna pada langkah 5 dengan warna favorit Anda!

Jawab:

<p align="center">
  <img src="img/praktikum_8/soal16.png" alt="Alt text">
</p>

Output:

<p align="center">
  <img src="img/praktikum_8/soal16run.gif" alt="Alt text">
</p>

# Praktikum 9: Memanfaatkan async/await dengan Widget Dialog

Langkah 1: Buat file baru navigation_dialog.dart

Buat file dart baru di folder lib project Anda.

<p align="center">
  <img src="img/praktikum_9/1.png" alt="Alt text">
</p>

Langkah 2: Isi kode navigation_dialog.dart

<p align="center">
  <img src="img/praktikum_9/2.png" alt="Alt text">
</p>

Langkah 3: Tambah method async

<p align="center">
  <img src="img/praktikum_9/3.png" alt="Alt text">
</p>

Langkah 4: Panggil method di ElevatedButton

<p align="center">
  <img src="img/praktikum_9/4.png" alt="Alt text">
</p>

Langkah 5: Edit main.dart

Ubah properti home

<p align="center">
  <img src="img/praktikum_9/5.png" alt="Alt text">
</p>

Langkah 6: Run

Coba ganti warna background dengan widget dialog tersebut. Jika terjadi error, silakan diperbaiki. Jika berhasil, akan tampil seperti gambar berikut.

<p align="center">
  <img src="img/praktikum_9/run.gif" alt="Alt text">
</p>

Soal 17:

Cobalah klik setiap button, apa yang terjadi ? Mengapa demikian ?

Jawab:

Ketika menekan tombol 'Change Color', muncul dialog dengan tiga pilihan warna: 'Red', 'Green', dan 'Blue'. Meskipun memilih warna dari dialog, perubahan warna tidak terjadi di layar utama. Hal ini terjadi karena nilai warna yang dipilih dari dialog tidak diteruskan kembali ke layar utama untuk mengubah warna latar belakangnya.

Gantilah 3 warna pada langkah 3 dengan warna favorit Anda!

Jawab:

<p align="center">
  <img src="img/praktikum_9/soal17.png" alt="Alt text">
</p>

Output:

<p align="center">
  <img src="img/praktikum_9/run17.gif" alt="Alt text">
</p>