# Apa itu Docker
Docker adalah sebuah command-line program, sebuah background daemon dan serangkaian remote 
service dengan mengambil pendekatan logistic untuk memecahkan permasalahan umum perangkat lunak 
dan menyederhanakan pengalaman kita dalam installing, running, publishing, dan menghapus perangkat lunak.
Docker bukan bahasa pemrograman dan bukan sebuah framework untuk membangun perangkat lunak
Docker adalah sebuah tool yang membantu kita dalam menyelesaikan permasalah umum seperti installing, 
removing, upgrading, distributing, trustring, dan menggelola software.


# Latar Belakang Docker
Docker Mengemas aplikasi dengan semua dependensi yang dibutuhkannya 
ke dalam sebuah standar untuk deployment

Docker membungkus semuanya menjadi sistem file lengkap yang 
berisi semuanya kebutuhan aplikasi dan yang menjalankan mesin virtual itu sendiri.

# Sejarah Docker
Dikeluarkan pada tahun 2013 sebagai open source, dotCloud merupakan penyedia platform 
as as service yang mengizinkan menjalankan aplikasi tanpa khwatir masalah infrastruktur.
Untuk meningkatkan waktu start up, mereka menggunakan container dan docker

# Virtualisasi Vs Containerization 
Memungkinkan membuat container pada virtual environment Mac/Windows di laptop dan menjalankan perintah atau mengoperasikannya.
Perintah atau operasi yang dilakukan pada container yang dijalankan di local, akan sama seperti yang berjalan di production.

# Keuntungan Docker
- Portability
- Quick deployment/teardown
- Managing infrastructure-like code
- Open source
- Consistency 

# Istilah pada Docker
- Docker container: virtual machine atau guest operating system, aplikasi kita berjalan di dalam docker container
- Docker client: kumpulan perintah command line untuk mengoperasikan docker container, misalkan membuat container, 
  start/stop container, menghapus, dan sebagainya.
- Docker daemon: aplikasi yang berjalan di host machine. Docker server berjalan di background(sebagai daemon) 
  dan menunggu perintah dari docker client
- Docker engine: gabungan aplikasi yang menjalankan docker container, docker client, dan docker daemon
- Docker image: template yang digunakan untuk membuat container. Misalkan image ubuntu, CentOS, dan sebagainya. 
- Docker registry: tempat yang digunakan untuk menyimpan docker image. Docker hub adalah sebuah registry public 
  yang semua orang dapat menggunakan. Secara default docker akan mencari image pada docker hub
- Docker compose: sebuah cara yang dapat digunakan untuk mendefinisikan 
  dan menjalankan lebih dari satu container.

# Perintah dasar docker
- docker run: sebuah perintah untuk menjalankan container
- docker build: digunakan untuk membuat sebuah docker image dari sebuah Dockerfile
- docker images: perintah ini akan menampilkan semua image yang ada
- docker ps: akan menampilkan daftar container
- docker rm: perintah untuk menghapus satu atau lebih dari satu container.
- docker rmi: perintah untuk menghapus sebuah image atau lebih dari satu image
- docker commit: digunakan untuk melakukan perubahan atau pengaturan file ke dalam image yang baru. 
- docker push: perintah untuk mengupload image ke server, docker hub.
- docker pull: perintah untuk mengambil/download image dari server, docker hub



