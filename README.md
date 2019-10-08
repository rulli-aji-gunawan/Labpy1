#Latihan 1


**== TUTORIAL CARA MENGGUNAKAN GIT == **

**A. Download dan Install Git**;
     Download Git, buka website resminya Git (git-scm.com).;
buka aplikasi git dan jalankan perintah "git config --global user.nama "nama anda" lalu enter dan tulis "git config --global user.email "email anda"
menggunakan git

buka github.com
tambahkn repository baru untuk mengisi ada beberapa hal yang harus diperhatikan : a. repository name : nama repository (latihan1) b. description : deskripsi repository (biasanya berupa siapa saja yang terlibat) c. public/private : kondisi repository mau di publikasikan atau pribadi d. initiallize the repository with README : ini adalah isi dokumentasi pada project yang dikerjakan, saya sarankan tidak usah dicentang. setelah diisi sesuai keinginan, klik tombol "create repository" maka tampilan selanjutnya adalah repository yang sudah dibuat, tahap selanjutnya adalah upload project ke repository online.
buka aplikasi git bash. pertama kalian konfigurasi seperti yng sudah dijelaskan diatas
buat directory project praktikum pertama dengan nama latihan1
sehingga terbentuk satu direktori baru dibawahnya,selanjutnya masuk kedalam direktori tersebut dengan perintah cd
direktori aktif menjadi d/latihan1
jalankan perintah git init, untuk membuat repository lokal
repository baru berhasil diinisialisasi, dengan terbentuknya satu direktori hidden dengan nama .git
pada direktori tersebut semua perubahan akan tersimpan
untuk membuat file dapat menggunakan text editor, lalu menyimpan filenya pada direktori aktif (repository)
buat satu file bernama README.md
file README.md berhasil dibuat untuk menambahkan file yang baru dibuat tersebut gunakan perintah git add
file README.md berhasil ditambahkan
untuk menyimpan perubahan yang ada kedalam database repository lokal, gunakan perintah git commit -m "komentar commit"
perubahan berhasil disimpan
server repo yang akan digunakan adalah https:/github.com
remote repository adalah repository server yang akan digunakan untuk menyimpan setiap perubahan pada lokal repository, sehingga dapat diakses oleh banyak user
untuk mengirim perubahan pada lokal repository ke server gunakan perintah git push
perintah ini akan meminta anda memasukkan username dan password pada akun github.com
buka halaman github.com, arahkan pada repository lalu refresh. maka hasilnya akan ditampilkan.

![Contoh memasukkan image](https://user-images.githubusercontent.com/56189248/66370074-09957980-e9c9-11e9-92b1-e554bc2d4704.png)