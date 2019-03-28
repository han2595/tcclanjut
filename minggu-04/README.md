# tcclanjut minggu -04
### Katacoda Scenario -04

:mortar_board: han2595 	:one::six::five::four::one::zero::two::one::two:


> Docker - Communicating Between Containers

Skenario ini mengeksplorasi cara mengizinkan beberapa Kontainer untuk berkomunikasi satu sama lain. Langkah-langkah ini akan menjelaskan cara menghubungkan penyimpanan data, dalam hal ini, Redis, ke aplikasi yang berjalan dalam kontainer terpisah.
Lingkungan ini telah dikonfigurasikan dengan klien Docker dan daemon.
Nama mesin yang digunakan Docker daemon dinamakan docker. Jika Anda ingin mengakses salah satu layanan, gunakan docker di localhost atau 0.0.0.0.

> Docker - Docker Networks

Skenario ini mengeksplorasi cara membuat sebuah jaringan docker yang memungkinkan Kontainer untuk berkomunikasi. Kami juga akan menjelajahi Server DNS Tertanam yang ditambahkan di Docker 1.10.

Docker memiliki dua pendekatan untuk jaringan. Yang pertama mendefinisikan hubungan antara dua kontainer. Tautan ini memperbarui / etc / hosts dan variabel lingkungan untuk memungkinkan Kontainer untuk di temukan dan berkomunikasi.

Pendekatan alternatif adalah membuat jaringan docker yang terhubung dengan Kontainer. Jaringan memiliki atribut yang mirip dengan jaringan fisik, memungkinkan Kontainer untuk datang dan pergi lebih bebas daripada saat menggunakan Link.

Yang akan kita bahas dari [Skenario Katacoda](https://www.katacoda.com/) adalah sebagai berikut :

 * [Communicating Between Containers](01-Communicating_Between_Containers.md) 

 Link Skenario  [Katacoda](https://www.katacoda.com/courses/docker/5)
  Communicating Between Containers 
  * [Docker Networks](02-Docker_Networks.md) 

  Link Skenario [Katacoda](https://www.katacoda.com/courses/docker/networking-intro) Docker Networks 