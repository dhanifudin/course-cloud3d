# Docker
## Latar Belakang Docker
Berawal dari salah satu masalah deployment yang tidak sesuai dengan local dev salah satu penyebabnya adanya package yang belum terinstall Proses packaging tersebut ke dalam sebuah image lengkap dan menjamin bahwa itu portable, ketika menjalankan dilakukan dengan cara yang sama, tidak memperdulikan environment deployment yang digunakan, docker memberikan solusi ini agar deploy production sesuai dengan yang ada di local.
Docker membungkus semuanya menjadi sistem file lengkap yang berisi semuanya kebutuhan aplikasi dan yang menjalankan mesin virtual itu sendiri. Docker bukanlah bahasa pemrograman atau framework, melaikan docker adalah sebuah tool berupa command-line program yang membantu kita dalam menyelesaikan permasalah umum seperti installing, removing, upgrading, distributing, trustring, dan menggelola software.

## Keuntungan Docker
- Portability
- Quick deployment/teardown
- Managing infrastructure-like code
- Open source
- Consistency 

## Istilah pada Docker
- **Docker container**: virtual machine atau guest operating system, aplikasi kita berjalan di dalam docker container
- **Docker client**: kumpulan perintah command line untuk mengoperasikan docker container, misalkan membuat container, 
  start/stop container, menghapus, dan sebagainya.
- **Docker daemon**: aplikasi yang berjalan di host machine. Docker server berjalan di background(sebagai daemon) 
  dan menunggu perintah dari docker client
- **Docker engine**: gabungan aplikasi yang menjalankan docker container, docker client, dan docker daemon
- **Docker image**: template yang digunakan untuk membuat container. Misalkan image ubuntu, CentOS, dan sebagainya. 
- **Docker registry**: tempat yang digunakan untuk menyimpan docker image. Docker hub adalah sebuah registry public 
  yang semua orang dapat menggunakan. Secara default docker akan mencari image pada docker hub
- **Docker compose**: sebuah cara yang dapat digunakan untuk mendefinisikan 
  dan menjalankan lebih dari satu container.

## Perintah dasar docker
- **docker run**: sebuah perintah untuk menjalankan container
- **docker build**: digunakan untuk membuat sebuah docker image dari sebuah Dockerfile
- **docker images**: perintah ini akan menampilkan semua image yang ada
- **docker ps**: akan menampilkan daftar container
- **docker rm**: perintah untuk menghapus satu atau lebih dari satu container.
- **docker rmi**: perintah untuk menghapus sebuah image atau lebih dari satu image
- **docker commit**: digunakan untuk melakukan perubahan atau pengaturan file ke dalam image yang baru. 
- **docker push**: perintah untuk mengupload image ke server, docker hub.
- **docker pull**: perintah untuk mengambil/download image dari server, docker hub

## DockerFile
Dockerfile adalah sebuah teks dokumen yang berisi semua perintah yang dapat dipanggil pengguna pada command line untuk membuat sebuah image. Jadi kita tidak perlu lagi mengetik perintah satu persatu ketika membuat image.

## Perintah DockerFile
- **FROM**: untuk mengambil image dari repository yang sudah ada.
- **MAINTENER**: untuk menginformasikan siapa yang melakukan maintenance pada image yang dibuat.
- **LABEL**: untuk menambahkan tambahan informasi terhadap image.
- **ADD/COPY**: untuk menambahkan file pada lokasi folder tertentu
- **CMD**: untuk menjalankan command tertentu
- **ENTRYPOINT**: untuk menjalankan script tertentu ketika docker booting
