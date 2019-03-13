# tcclanjut minggu-02
# Pull Request-02

Melakukan Pull Request di GitHub ,
Pull-request merupakan fitur yang memungkinkan kita memberitahukan kepada para pengembang 
di pusat bahwa kita memiliki perubahan yang ingin dikirimkan ke mereka.
Tombol pull-request ada pada kiri atas repositori:
 
1.Yang pertama dilakukan adalah mencari teman atau partner untuk berkolaborasi atau para pengembang 
di pusat bahwa kita memiliki perubahan yang ingin dikirimkan ke mereka.

![01](images/README-01.jpg)
 
2.Setelah itu Mengambil Kode dari pemilik repo atau biasa disebut Fork 
 
 ![02](images/README-02.jpg)
 
3.Kemudian proses forking berlangsung dan tunggu hingga selesai 

![03](images/README-03.jpg)

 
4.Kemudian jika forking berhasil , ketika kita kembali ke repo milik kita akan terdapat repo milik teman yang sudah kita fork , dalam kasus ini "tcclanjut-1"

![04](images/README-04.jpg)
 
5.Setelah itu kita akan meng Clone repo tersebut ke komputer lokal 

![05](images/README-05.jpg)


6.Kemudian mengkonfigurasi repo lokal kontributor gunanya  untuk memudahkan kita dalam memastikan perubahan yang dilakukan tidak mengalami konflik dengan kontributor lainnya

origin: menunjuk ke repo milik kontributor di GitHub, hasil dari fork.

![06](images/README-06.jpg)

upstream: menunjuk ke repo milik upstream author (repo asli) dan inilah yang akan kita konfigurasi 
 
![06.1](images/README-06.1.jpg)

kemudian kita lakukan pengecekan dengan cara mengetikan'$ git remote -v' di git bash

![06.2](images/README-06.2.jpg)

7.Nah pada poin ini kita akan melakukan perubahan atau mengirim kontribusi ke repo milik si pemilik dalam kasus ini repo dari teman saya 'yudhiwae'
 tapi sebelum itu pastikan bahwa isi repo lokal tersinkronisasi dengan repo dari upstream author.

![07](images/README-07.jpg)
 
 ini adalah perubahan yang saya lakukan di repo milik 'yudhiwae' mungkin terlihat simple , tapi kembali lagi ini hanya sedikit pembelajaran dari Pull Request di GitHub
 
 ![07.1](images/README-07.1.jpg)
 
kemudian kita lakukan Push ke repo origin (milik kontributor) langkahnya dapat dilihat dibawah

![07.2](images/README-07.2.jpg)

selanjutnya

![07.3](images/README-07.3.jpg)

kemudian 

![07.4](images/README-07.4.jpg)
 
8.Setelah itu,cek halaman Web dari repo kontributor dalam hal ini adalah akun git saya sendiri https://github.com/han2595/tcclanjut-1.git

![08](images/README-08.jpg)
 
9.Kemudian Pilih 'Compare and pull request', setelah itu isikan deskripsi PR(Pull Request) dan klik pada Create pull request:

![09](images/README-09.jpg)

setelah selesai kita harus menunggu persetujuan dari pemilik repo , di kasus ini adalah 'yudhiwae'
 
 ![09.1](images/README-09.1.jpg)
 
10.Untuk diketahui bahwasalnya Upstream author bisa menyetujui setelah melakukan review: klik pada Pull requests, akan muncul PR dengan message seperti yang ditulis oleh kontributor (Add: contributor). Klik pada PR tersebut, review kemudian klik Merge pull request diikuti dengan Confirm merge. Setelah itu, status akan berubah menjadi Merged.


 
11.kemudian melakukan sinkron repo (lokal maupun GitHub kontributor)

![11](images/README-11.jpg)
 

 
 
 Sekian Cara atau Proses Pull-request di GitHub 
