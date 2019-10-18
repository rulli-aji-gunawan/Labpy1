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
+ Sesuai dengan istilahnya, maka kita akan belajar cara membuat repository local, yaitu repository yang akan disimpan di ruang penyimpanan komputer kita.
+ Buka directory aktif yang akan kita jadikan tempat penyimpanan file latihan atau project kita *dengan menggunakan Windows Explorer*. Misal, kita buka di **d:\labs_pemrograman1**.  
+ Klik kanan pada directory aktif tersebut, klik **Git Bash** pada menu yang muncul, sehingga akan muncul *git bash command*.  
+ Buatlah directory praktikum project pertama dengan nama **latihan1**, caranya adalah dengan mengetik perintah berikut pada git bash commad.  
  
![Membuat Repository Local](https://user-images.githubusercontent.com/56189248/66398630-52205780-ea08-11e9-9055-3098fc83f554.png)  
  
+ Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya masuk kedalam direktori tersebut dengan perintah **cd latihan1** (change directory ke latihan1) seperti pada gambar di atas.
+ Directory aktif menjadi: **d:\labs_pemrograman1\latihan1** .
+ Jalankan perintah **git init**, untuk membuat repository local pada directory aktif yang sudah kita pilih tadi. Jadi segala perubahan pada directory tersebut akan selalu terpantau oleh git.  
  
![Ketik Git Init](https://user-images.githubusercontent.com/56189248/66399365-ae37ab80-ea09-11e9-8fd5-1ac6ac5f0ee6.png)  
  
+ Repository baru berhasil di inisialisasi, dengan terbentuknya satu directory hidden dengan nama **.git**  
  
![Directory.git](https://user-images.githubusercontent.com/56189248/66400022-e7245000-ea0a-11e9-9e19-24f22f97cd22.png)  
  
+ Jadi, semua perubahan pada directory yang sudah di-repository tersebut atau bisa disebut juga dengan *working directory* akan selalu terekam dan sisimpan oleh git.  
  
**D. Menambah File Baru Pada Repository**  
+ Dalam repository (directory aktif) yang sudah kita buat tadi, kita bisa menambahkan file yang akan kita olah. Salah satu cara membuat file adalah bisa menggunakan text editor, lalu file tersebut disimpan pada repository.
+ Sebagai contoh dan latihan, kita akan mencoba membuat text file yang diberi nama README.md  , cara membuatnya adalah dengan memberikan perintah pada git seperti berikut :  
**$ echo "#Latihan 1" >> README.md**  
  
![Perintah menambah file baru pada repository](https://user-images.githubusercontent.com/56189248/67097328-134a8880-f1e4-11e9-854f-0c1a262d4ca5.png)
  
+ Dan file **README.md** pun berhasil dibuat.  
+ Untuk menambahkan file tersebut kedalam repository supaya bisa terdeteksi oleh Git, gunakan perintah **$ git add README.md**  .  
+ Untuk menyimpan perubahan yang ingin kita rekam dan ingin diberikan keterangan ke dalam database repository local, maka gunakanlah perintah: **$ git commit -m "komentar /catatan commit"**. Contoh : **$ git commit -m "file dalam repository pertama saya"** . Dan perubahan pun berhasil disimpan.  
  
**E. Membuat Repository Server**  
+ Sesuai dengan istilahnya, maka kali ini kita akan belajar cara membuat repository di server (di luar ruang penyimpanan komputer yang kita gunakan).  
+ Sever repository yang akan kita gunakan adalah **http://github.com**  
+ Pertama kita harus membuat akun terlebih dahulu dengan email dan password yang akan kita gunakan.  
+ Pada halaman utama github.com, klik tombol *Start a project* atau  
+ Dari menu (icon +) klik *New Repository*  
  
![Membuat akun di github1](https://user-images.githubusercontent.com/56189248/66759797-1b948200-eecb-11e9-9db8-c3585aacf7dd.png)       ![Membuat akun di github2](https://user-images.githubusercontent.com/56189248/66759251-1aaf2080-eeca-11e9-9e2d-7e43c7623bde.png)  
  
+ Isi nama repository-nya, misalkan kita beri nama : **Labpy1**  
+ Lalu klik tombol *Create Repository*.  
  
![Membuat nama repo di github](https://user-images.githubusercontent.com/56189248/66760354-226fc480-eecc-11e9-894a-c0b0e9321aab.png)  
  
**F. Menambahkan Reomote Repository**  
+ Remote Repository merupakan repository server yang akan digunakan untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses oleh banyak user atau bisa diakses dari mana saja.  
+ Untuk menambahkan remote repository server, gunakan perintah **$ git remote add origin [*url repository di github*]**  
  
![Remote repo](https://user-images.githubusercontent.com/56189248/66760700-d2ddc880-eecc-11e9-8f2a-a0397bbe756d.png)  
  
**G. Push (mengirim perubahan ke server)**  
+ Untuk mengirim perubahan pada local repository yang sudah kita *commit* ke server, gunakan perintah git push seperti berikut,  
  
![Git Push](https://user-images.githubusercontent.com/56189248/66761232-c7d76800-eecd-11e9-91f8-3a6835996273.png)  
+ Saat pertama kali menggunakan perintah ini, maka kita akan diminta memasukkan username dan password pada akun github.com.  
+ Masukkan username dan password sesuai dengan yang kita daftarkan saat membuat akun di github.com seperti yang sudah dijelaskan sebelumnya.  
+ Buka laman github.com, arahkan pada repositori-nya, maka perubahan akan terlihat pada laman tersebut.  
  
![hasil git push](https://user-images.githubusercontent.com/56189248/66761717-bb9fda80-eece-11e9-89c8-cc1ea78ab65b.png)  
  
**H. Clone Repository**  
+ Clone repository, pada dasarnya adalah **_meng-copy_** repository server dan secara otomatis membuat satu directory sesuai dengan nama repository-nya (_working directory_).  
+ Untuk melakukan cloning, gunakan perintah git **clone [*url repository yang akan kita copy di github*]**  
  
**I. Kegunaan File README.md**  
+ Apabila kita menggunakan github, untuk memberikan penjelasan awal pada project yang kita buat, maka dapat menggunakan sebuah file yang bernama README.md  
+ Pada file tersebut kita dapat membuat dokumentasi awal dari setiap project yang kita buat untuk memberikan penjelasan atau sekedar cara penggunaan dari aplikasi yang kita kembangkan.  
+ Penulisan file README.md berbasis teks, dan untuk pemformatannya menggunakan Markdown format.  
Untuk lebih jelasnya, dapat anda pelajari cara penggunaan markdown pada url berikut: https://guides.github.com/features/mastering-markdown/
  
  


Terima kasih  
  
**_Disclaimer : Ini hanya file latihan pribadi saya, jika ada kekurangan dan kesalahan, itu semata-mata karena keterbatasan ilmu dari saya_**