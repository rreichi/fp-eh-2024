## PicoCTF — Web Exploitation: Trickster Writeup

#### Langkah Pengerjaan :

1. Buka web yang diberikan

![wx](assets/1wx.png)

2. Buat script yang akan diupload pada web tersebut, saya menggunakan **Visual Studio**

![wx](assets/2wx.png)

Untuk penamaan file diharuskan **.png** dikarenakan web tersebut hanya bisa memroses file dengan format png saja. Lalu upload

![wx](assets/3wx.png)

3. Edit endpoint sebagai berikut, lalu gunakan command **ls**

![wx](assets/4wx.png)

4. Edit lagi tapi gunakan command **cat** untuk menampilkan isi dari file **.txt**

![wx](assets/5wx.png)
**Flag: picoCTF{c3rt!fi3d_Xp3rt_tr1ckst3r_48785c0e}**