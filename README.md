# Build-APK
## Berikut Merupakan Run Build APK <br>

#### Cara Build APK
Salah satu langkah terakhir yang perlu dilakukan setelah mengembangkan aplikasi Android adalah membuat berkas executable dalam format APK (Android Application Package). Berkas ini yang akan didistribusikan oleh Google Play ke pengguna. Jadi, ketika Anda hendak mempublikasikan Aplikasi Anda ke Google Play, berkas inilah yang harus Anda unggah. <br>
Jika Anda belum memahami berkas APK, Anda dapat menyamakannya dengan berkas exe di windows atau ipa di iOS.<br>
Cara membuat file APK di Android terbilang cukup mudah. Anda dapat menggunakan sebuah wizard atau melalui command line. Pada modul ini, kita akan fokus menggunakan wizard. <br>

Membuat APK terbagi menjadi 2 yakni dengan menggunakan: <br>
1.	Default keystore <br>
2.	Custom keystore <br>


Keystore adalah sebuah berkas biner yang berisi informasi tentang satu atau lebih private key. Private key ini digunakan untuk mencegah pemalsuan aplikasi. Konsep umumnya adalah: <br>
•	Sistem Operasi Android mewajibkan semua APK di-sign sebelum terpasang ke dalam device. <br>
•	Proses signing ini membutuhkan Public dan Private Key. <br>
•	Proses signing ini berlangsung selama pembuatan APK dalam mode debug maupun released. <br>
•	Sebuah sertifikat digital public key, atau identity certificate, berisi informasi mengenai sertifikat itu sendiri dan metadata dari pemilik sertifikat tersebut. Pemilik sertifikat ini biasanya adalah developer yang mengembangkan aplikasi. <br>
•	Public key yang digunakan dalam proses signing di atas akan dilampirkan di dalam berkas APK. Proses ini dilakukan secara otomatis oleh Android Studio. <br>
•	Ketika Anda hendak memperbarui Aplikasi Anda pada Google Play, maka Google Play hanya akan menerimanya bila keystore yang digunakan sama dengan keystore yang pertama kali Anda gunakan ketika mengunggah Aplikasi tersebut ke Google Play. <br>


Kegunaan lain dari Keystore : <br>
•	Untuk integrasi ke layanan Google seperti Google Maps dengan menggunakan nilai hash (digest SHA1) di dalamnya. <br>
•	Untuk integrasi ke layanan API Facebook dengan menggunakan key hash base64 yang terkandung di dalam keystore. <br>


Keystore merupakan sebuah berkas penting yang harus Anda jaga, terlebih ketika aplikasi Anda memiliki jumlah unduhan pengguna yang banyak. Sebabnya, kelalaian menjaga keystore ini dapat menghalangi Anda untuk memperbarui aplikasi. Akibat terburuk adalah Anda harus melakukannya dari awal lagi. <br>
Berikut adalah tips yang bisa Anda gunakan untuk mengamankan keystore : <br>
1.	Pilih kata kunci (password) yang sulit ditebak. Kombinasikan angka, alfabet dan simbol dalam membuatnya. <br>
2.	Bedakan antara keystore password dan key password ketika membuat berkas APK dengan custom keystore. <br>
3.	Jangan memberikan keystore kepada orang yang tidak dipercaya apalagi meletakkannya di dalam berkas proyek aplikasi. <br>
4.	Letakan di tempat yang Anda ingat dan aman tentunya. <br>

Untuk pengguna Windows bisa menemukannya di  C:\User\YourUser\.android\debug.keystore.

### Code LAB Build APK <br>
Untuk mulai melakukan proses build APK, Anda dapat mengikuti langkah berikut: <br>
1. Buka kembali proyek kosong yang telah kita buat sebelumnya, kemudian klik build Dan pilih Bundle's APK. <br>
![Alt Text](https://github.com/adam033/Build-APK/blob/master/Screenshot%20(237).png) <br>
2. Apabila sudah terinstall maka akan muncul di bawah kanan dan klik locate untuk mengetahui lokasi file nya. <br>
![Alt Text](https://github.com/adam033/Build-APK/blob/master/Screenshot%20(238).png) <br>
3. Ini adalah tampilan penyimpanan di folder kita.
![Alt Text](https://github.com/adam033/Build-APK/blob/master/Screenshot%20(239).png) <br>
4. 







