#Latihan 1


**TUTORIAL CARA MENGGUNAKAN GIT**

**A. Download dan Install Git**  
+ Download Git, buka website resminya Git (git-scm.com).  
+ Kemudian unduh Git sesuai dengan arsitektur komputer kita. Kalau menggunakan 64bit, unduh yang 64bit. Begitu juga kalau menggunakan 32bit, unduh yang 32bit.  
  
![Download Git-image](https://user-images.githubusercontent.com/56189248/66376538-1a9ab680-e9da-11e9-8342-df8d66fb971e.png)  
  
+ Install Git yang telah terunduh!. Selamat, Git sudah terinstal di Windows. Untuk mencobanya, silahkan buka **CMD** atau **PowerShell**, kemudian ketik perintah "__git --version__".  
  
![Check Git Version-cmd](https://user-images.githubusercontent.com/56189248/66382918-3d32cc80-e9e6-11e9-83a2-734fd4c66829.png)
  
**B. Menambahkan Global Config**  
+ Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi *__user.name__* dan *__user.email__*.  
+ Konfigurasi ini bisa dilakukan untuk global repostiry atau individual repository.  
+ Apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi kegagalan saat menjalankan perintah *__git commit__*.  
+ Config Global Repository
    
![Editing Global Config](https://user-images.githubusercontent.com/56189248/66390848-c1408080-e9f5-11e9-969a-b09ae216fed7.png)  
  
  
**C. Perintah Dasar Pada Git**  
_Pada Git, ada beberapa perintah dasar yang sering digunakan seperti di bawah ini berikut fungsinya :_  
  
![Perintah Dasar Git](https://user-images.githubusercontent.com/56189248/66391500-84758900-e9f7-11e9-813a-d110c2711fa7.png)  
  
**B. Membuat Repository Local**  
+ Buka directory aktif yang akan kita jadikan tempat penyimpanan file latihan atau project kita *dengan menggunakan Windows Explorer*. Misal, kita buka di **d:\labs_pemrograman1**.  
+ Klik kanan pada directory aktif tersebut, klik **Git Bash** pada menu yang muncul, sehingga akan muncul *git bash command*.  
+ Buatlah directory praktikum project pertama dengan nama **latihan1**, caranya adalah dengan mengetik perintah berikut pada git bash commad.  
  
![Membuat Repository Local](https://user-images.githubusercontent.com/56189248/66398630-52205780-ea08-11e9-9055-3098fc83f554.png)  
  
+ Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya masuk kedalam direktori tersebut dengan perintah **cd latihan1** (change directory ke latihan1) seperti pada gambar di atas.
+ Directory aktif menjadi: **d:\labs_pemrograman1\latihan1** .
+ Jalankan perintah **git init**, untuk membuat repository local pada directory aktif yang sudah kita pilih tadi. Jadi segala perubahan pada directory tersebut akan selalu terpantau oleh git.  
  
![Ketik Git Init](https://user-images.githubusercontent.com/56189248/66399365-ae37ab80-ea09-11e9-8fd5-1ac6ac5f0ee6.png)  
