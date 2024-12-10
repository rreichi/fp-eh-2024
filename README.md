# Write-Up

| Nama | NRP |
|---|---|
|Radella Chesa Syaharani|5027231064|
|Kharisma Fahrun Nisa' |5027231086|


## Deskripsi Pengerjaan
Penetration Testing merupakan serangkaian kegiatan yang bertujuan untuk menemukan dan memanfaatkan kerentanan keamanan. Hal ini bertujuan untuk memverifikasi seberapa efektif atau tidaknya langkah-langkah keamanan yang telah diterapkan. Penetration Testing terbagi dalam dua metode, yaitu: secara manual dan otomatis. Penetration Testing Manual adalah pengujian yang dilakukan oleh manusia, sementara penetration testing otomatis adalah pengujian yang dijalankan oleh mesin, sehingga tidak memerlukan ahli dan bisa dilakukan oleh siapa saja yang memiliki pengetahuan dalam bidang ini.
Umumnya, Penetration Testing Manual dilakukan dengan metode sebagai berikut:

 • Data Collection
  Pengumpulan data sangat penting untuk pengujian. Data dapat dikumpulkan secara manual atau dengan memanfaatkan tools gratis yang dapat ditemukan online, seperti: teknik analisis source code webpage dan lain-lain. Tools ini   membantu dalam mengumpulkan informasi, seperti nama tabel, versi database, software, hardware, atau bahkan mengenai berbagai plugin pihak ketiga, dan lain-lain.

 • Vulnerability Assessment
	 Data yang dikumpulkan dapat  membantu para penguji dalam mengenali celah keamanan dan mengambil tindakan pencegahan yang tepat.

 • Actual Exploit
 	Sebelum melakukan serangan, deteksi versi layanan yang aktif pada target menggunakan nmap. Nmap akan mencoba mengidentifikasi nama protokol layanan dan versi dari layanan tersebut dengan menggunakan opsi “-sV” sebagaimana pada gambar ![image](https://github.com/user-attachments/assets/d1fdd6b8-2941-4a42-9ac8-3a55be58f59b)

  Penyerangan dibantu dengan tool hydra, dan untuk melakukan brute force dengan hydra, diperlukan password. Terdapat berbagai password yang bisa digunakan; dalam contoh ini, digunakan password bawaan dari John the Ripper. Daftar password yang dihasilkan oleh alat peretasan password dapat dimodifikasi dengan opsi: Mausepad password list. Jika ingin mengetahui jumlah baris dalam file daftar password yang sudah didapat, kita gunakan opsi: Wc –l password list. Opsi -l akan menampilkan jumlah baris di dalam file daftar password, dengan output pertama sebagai jumlah dan output kedua sebagai nama file. Setelah daftar password siap, password yang telah disusun akan digunakan untuk melakukan brute force pada server ssh guna mendapatkan password.
  Untuk memastikan seberapa kuat password yang kita gunakan dapat di cek pada website : https://howsecureismypassword.net/, contoh password acak yang saya masukkan pada laman terasebut ternyata dapat dcrack hanya dalam waktu dua menit. 
 
  ![image](https://github.com/user-attachments/assets/29ec094d-69c3-4df4-866c-9eb42bfc801b)

