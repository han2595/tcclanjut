## Deploy Containers Using YAML


> Step 1 - Create Deployment

Salah satu objek Kubernetes yang paling umum adalah objek penyebaran. Objek penyebaran mendefinisikan spesifikasi kontainer yang diperlukan, bersama dengan nama dan label yang digunakan oleh bagian lain dari Kubernetes untuk menemukan dan menghubungkan ke aplikasi.

 > Tugas : 


Salin definisi berikut ke editor. Definisi tersebut mendefinisikan cara meluncurkan aplikasi yang disebut webapp1 menggunakan Docker Image katacoda / docker-http-server yang berjalan pada Port 80.


 ![16](images/README.16.jpg)

 Ini digunakan untuk cluster dengan perintah

 ```kubectl create -f deployment.yaml```

 ![17](images/README.17.jpg)

 Karena ini adalah objek Penerapan, daftar semua objek yang digunakan dapat diperoleh melalui

 ```kubectl get deployment```

 ![18](images/README.18.jpg)

 Detail dari masing-masing penyebaran dapat ditampilkan

 ```kubectl describe deployment webapp1```

  ![19](images/README.19.jpg)



> Step 2 - Create Service

Kubernetes memiliki kemampuan jaringan yang kuat yang mengontrol cara aplikasi berkomunikasi. Konfigurasi jaringan ini juga dapat dikontrol melalui YAML.


 > Tugas : 


Salin definisi Layanan ke editor. Layanan memilih semua aplikasi dengan label webapp1. Saat banyak replika, atau contoh, ditempatkan, mereka akan secara otomatis memuat seimbang berdasarkan label umum ini. Layanan menyediakan aplikasi melalui NodePort.


 ![20](images/README.20.jpg)

 Semua objek Kubernetes dikerahkan secara konsisten menggunakan kubectl.

Menyebarkan Layanan dengan cara

 ```kubectl create -f service.yaml```

 ![21](images/README.21.jpg)

 Seperti sebelumnya, detail semua objek Layanan yang dikerahkan dengan ```kubectl get svc```
 ![22](images/README.22.jpg)

Dengan menjelaskan objek, Anda dapat menemukan detail lebih lanjut tentang konfigurasi

 ```kubectl describe svc webapp1-svc.```

 ![23](images/README.23.jpg)


 ```curl host01:30080```

  ![24](images/README.24.jpg)


 
 > Step 3 - Scale Deployment

Rincian YAML dapat diubah karena konfigurasi yang berbeda diperlukan untuk penerapan. Ini mengikuti infrastruktur sebagai pola pikir kode. Manifes harus disimpan di bawah kendali sumber dan digunakan untuk memastikan bahwa konfigurasi dalam produksi cocok dengan konfigurasi dalam kontrol sumber.


 > Tugas : 



Perbarui file deployment.yaml untuk meningkatkan jumlah instance yang berjalan. Misalnya, file tersebut akan terlihat seperti ini:

 ```replicas: 4```

 Pembaruan definisi yang ada diterapkan menggunakan kubectl apply. Untuk skala jumlah replika, gunakan file YAML yang diperbarui menggunakan

 ```kubectl apply -f deployment.yaml```

 ![25](images/README.25.jpg)

 Seketika, keadaan yang diinginkan dari kluster kami telah diperbarui, dapat dilihat dengan

 ```kubectl get deployment```

 ![26](images/README.26.jpg)

Pod tambahan akan dijadwalkan agar sesuai dengan permintaan

 ```kubectl get pods```

 ![27](images/README.27.jpg)

 Karena semua Pods memiliki pemilih label yang sama, mereka akan dimuat dengan seimbang di belakang Service NodePort yang digunakan.

Mengeluarkan permintaan ke pelabuhan akan menghasilkan berbagai kontainer memproses permintaan


 ```curl host01:30080```

  ![28](images/README.28.jpg)

  Rincian Jaringan Kubernetes tambahan dan Definisi Objek akan dibahas dalam skenario mendatang.25

 


 * [<<= Back](README.md)