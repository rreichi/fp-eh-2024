## Hack The Box — Hardware: Critical Flight Writeup

#### Langkah Pengerjaan :
1. Download file yang disertakan pada *challenge*
![cf](assets/1.png)
Setelah download, buka folder **flight_control_board**. Terdapat file dengan format **.gbr** yang merupakan format untuk PCBs (Printed Circuit Board)
![cf](assets/2.png)
2. Kita memerlukan tools untuk menganalisis *circuit board*. Disini saya menggunakan ![Online Gerber Viewer](https://www.pcbway.com/project/OnlineGerberViewer.html)
- Upload file **.zip** yang didownload tadi lalu akan ditampilkan layout PCB seperti ini
![cf](assets/3.png)
- Pindah ke tab layers lalu hide semua layer kecuali **bottom > copper** dan **inner > copper** 
![cf](assets/4.png)
![cf](assets/5.png)
**Flag : HTB{533_7h3_1nn32_w02k1n95_0f_313c720n1c5#$@}**