# Write-Up

| Nama | NRP |
|---|---|
|Radella Chesa Syaharani|5027231064|
|Kharisma Fahrun Nisa' |5027231086|

Report PDF: [REPORT FP Ethical Hacking](064_068_ReportFinalProject.pdf)

## Deskripsi Pengerjaan
_Penetration Testing_ merupakan serangkaian kegiatan yang bertujuan untuk menemukan dan memanfaatkan kerentanan keamanan. Hal ini bertujuan untuk memverifikasi seberapa efektif atau tidaknya langkah-langkah keamanan yang telah diterapkan. _Penetration Testing_ terbagi dalam dua metode, yaitu: secara manual dan otomatis. _Penetration Testing_ Manual adalah pengujian yang dilakukan oleh manusia, sementara _penetration testing_ otomatis adalah pengujian yang dijalankan oleh mesin, sehingga tidak memerlukan ahli dan bisa dilakukan oleh siapa saja yang memiliki pengetahuan dalam bidang ini.
Umumnya, _Penetration Testing_ Manual dilakukan dengan metode sebagai berikut:

 • _Data Collection_
  Pengumpulan data sangat penting untuk pengujian. Data dapat dikumpulkan secara manual atau dengan memanfaatkan _tools_ gratis yang dapat ditemukan _online_, seperti: teknik analisis _source code webpage_ dan lain-lain. _Tools-tools_ ini membantu dalam mengumpulkan informasi, seperti nama tabel, versi _database_, _software_, _hardware_, atau bahkan mengenai berbagai plugin pihak ketiga, dan lain-lain.

 • _Vulnerability Assessment_
	 Data yang dikumpulkan dapat  membantu para penguji dalam mengenali celah keamanan dan mengambil tindakan pencegahan yang tepat.

 • _Actual Exploit_
 	Sebelum melakukan serangan, deteksi versi layanan yang aktif pada target menggunakan nmap. Nmap akan mencoba mengidentifikasi nama protokol layanan dan versi dari layanan tersebut dengan menggunakan opsi “-sV” sebagaimana pada gambar ![image](https://github.com/user-attachments/assets/d1fdd6b8-2941-4a42-9ac8-3a55be58f59b)

  Penyerangan dibantu dengan _tool_ hydra, dan untuk melakukan _brute force_ dengan hydra, diperlukan _password_. Terdapat berbagai password yang bisa digunakan; dalam contoh ini, digunakan password bawaan dari _John the Ripper_. Daftar password yang dihasilkan oleh alat peretasan password dapat dimodifikasi dengan opsi: Mausepad password list. Jika ingin mengetahui jumlah baris dalam file daftar password yang sudah didapat, kita gunakan opsi: Wc –l password list. Opsi -l akan menampilkan jumlah baris di dalam file daftar password, dengan output pertama sebagai jumlah dan output kedua sebagai nama file. Setelah daftar password siap, password yang telah disusun akan digunakan untuk melakukan brute force pada server ssh guna mendapatkan password.
  Untuk memastikan seberapa kuat password yang kita gunakan dapat di cek pada website : https://howsecureismypassword.net/, contoh password acak yang saya masukkan pada laman terasebut ternyata dapat dcrack hanya dalam waktu dua menit. 
 
  ![image](https://github.com/user-attachments/assets/29ec094d-69c3-4df4-866c-9eb42bfc801b)

Terakhir,  melakukan _SQL Injection_ dengan bantuan WebGoat. WebGoat adalahproject open source yang memungkinkan individu untuk mempelajari peretasan web, termasuk SQL Injection. Versi WebGoat yang digunakan di sini adalah WebGoat v5.1. WebGoat merupakan aplikasi web J2EE yang dikembangkan oleh OWASP untuk tujuan edukasi tentang keamanan aplikasi web. WebGoat menawarkan pelatihan mengenai masalah celah keamanan di web, yang dapat muncul karena berbagai alasan seperyti halnya salah implementasi. Banyak program yang dikerjakan dengan tergesa-gesa sehingga kurang teliti dalam penulisan kode, akibatnya pengujian sering kali diabaikan. Contoh: _programmer_ sering kali mengabaikan untuk menyaring karakter-karakter aneh yang dimasukkan sebagai input dari sebuah program, contohnya seperti kasus di bawah ini.
Mulai jalankan WebGoat yang telah di download, masuklah ke dalam folder hasil ekstrak, jalankan WebGoat 80 kemudian buka browser dan isilah url dengan http://127.0.0.1/WebGoat/attack. Jika ada pesan untuk memasukkan _username_ dan _password_, masukkan _username_ : gues dengan _password_: gues.

![image](https://github.com/user-attachments/assets/36926b77-58c4-4d9c-a31c-af075e38c3de)
