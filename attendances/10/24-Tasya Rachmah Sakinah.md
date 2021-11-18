# Pertemuan 10
## Latar Belakang
- Mengemas aplikasi dengan semua dependensi yang dibutuhkannya ke dalam sebuah standar untuk deployment
- Docker membungkus semuanya menjadi sistem file lengkap yang berisi semuanya kebutuhan aplikasi dan yang menjalankan mesin virtual itu sendiri.
- Proses packaging tersebut ke dalam sebuah image lengkap dan menjamin bahwa itu portable, ketika menjalankan dilakukan dengan cara yang sama, tidak memperdulikan
environment deployment yang digunakan.
## Sejarah Docker
- Dimulai sebagai project internal oleh dotCloud.
- 2013 menjadi sebuah project open source.
- dotCloud merupakan penyedia platform as as service yang mengizinkan menjalankan aplikasi tanpa khwatir masalah infrastruktur.
- Mereka membutuhkan sebuah lebih banyak virtual machine dan lebih cepat.
- Untuk meningkatkan waktu start up, mereka menggunakan container dan docker.
- Peluncuran pertama pada bulan Juni 2014 yang dievaluasi lebih dari 10000 developer dan lebih dari 2,75 juta pengguna
- dotCloud berkolaborasi dengan RedHat ataupun Amazon untuk menambahkan layanan sehingga dapat menggunakan Docker untuk mengelola infrastruktur di sana.
## Virtualisasi Vs Containerization
- Docker adalah sebuah container management system yang membantu mengelola container lebih mudah dan universal.
- Memungkinkan membuat container pada virtual environment Mac/Windows di laptop dan menjalankan perintah atau mengoperasikannya.
- Perintah atau operasi yang dilakukan pada container yang dijalankan di local, akan sama seperti yang berjalan di production.
- Setiap membuat sebuah container, tidak membutuhan system operasi secara penuh
- Docker mengandalkan penggunaan kernel Linux Kernel
- Docker menghasilkan sebuah ukuran image yang kecil, compact, dan ringan untuk didistribusikan karena tidak terdapat kernel bahkan sistem operasi
## Keuntungan Docker
- Portability
- Quick deployment/teardown
- Managing infrastructure-like code
- Open source
- Consistency
## Arsitektur Docker
- Docker container: virtual machine atau guest operating system, aplikasi kita berjalan di dalam docker container.
- Docker client: kumpulan perintah command line untuk mengoperasikan docker container, misalkan membuat container, start/stop container, menghapus, dan sebagainya.
- Docker daemon: aplikasi yang berjalan di host machine. Docker server berjalan di background(sebagai daemon) dan menunggu perintah dari docker client.
- Docker engine: gabungan aplikasi yang menjalankan docker container, docker client, dan docker daemon.
- Docker image: template yang digunakan untuk membuat container. Misalkan image ubuntu, CentOS, dan sebagainya.
- Docker registry: tempat yang digunakan untuk menyimpan docker image. Docker hub adalah sebuah registry public yang semua orang dapat menggunakan. Secara default docker akan mencari image pada docker hub.
- Docker compose: sebuah cara yang dapat digunakan untuk mendefinisikan dan menjalankan lebih dari satu container.