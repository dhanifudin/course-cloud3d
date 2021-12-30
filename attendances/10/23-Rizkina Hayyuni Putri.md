# DOCKER

## Latar Belakang Docker
Docker membungkus semuanya menjadi sistem file lengkap yang berisi semuanya kebutuhan aplikasi dan yang menjalankan mesin virtual itu sendiri. Hasilnya akan beripa sebuah image lengkap yang bersifat portable, yang memiliki kelebihan yaitu bisa dijalankan dengan cara yang sama, tidak memperdulikan environment deployment yang digunakan.

## Virtualisasi Vs Containerization 
Container adalah sebuah virtualisasi tidak penuh. Container mirip seperti virtualisasi tetapi tidak selengkap virtualisasi. 
Docker adalah sebuah container management system yang membantu mengelola container lebih mudah dan universal.
Docker dapat berjalan disemua OS(Windows, Linux atau MacOS).

## Keuntungan Docker
1. **Portability** = Dapat memindahkan aplikasi dengan mudah ke environment deployment manapun
2. **Quick deployment/teardown** = Mudah mendeploy dan un-deploy atau mendeploy ke versi tertentu
3. **Managing infrastructure-like code** = semua konfigurasi disimpan dalam file lalu saat dideploy akan dilakukan
4. **Open source** = Kode sumber terbuka
5. **Consistency** = disemua environment deployment akan menghasilkan hasil yang sama

## Arsitektur Docker
Docker bukanlah bahasa pemrograman atau framework, melaikan docker adalah sebuah tool berupa command-line program yang membantu kita dalam menyelesaikan permasalah umum seperti installing, removing, upgrading, distributing, trustring, dan menggelola software.

## Istilah dalam Docker
- **Docker container**: virtual machine tempat dimana aplikasi berjalan di dalam docker container.
- **Docker client**: kumpulan perintah command line untuk mengoperasikan docker container.
- **Docker daemon**: aplikasi yang berjalan di host machine.
- **Docker engine**: gabungan docker container, docker client, dan docker daemon. 
- **Docker image**: template yang digunakan untuk membuat container.  
- **Docker registry**: tempat yang digunakan untuk menyimpan docker image.
- **Docker compose**: cara untuk mendefinisikan dan menjalankan lebih dari satu container.

## Perintah sadar Docker
- **docker run**: untuk menjalankan container.
- **docker build**: untuk membuat sebuah docker image dari sebuah Dockerfile.
- **docker images**: untuk menampilkan semua image dan informasi lainnya seputar image.
- **docker ps**: untuk menampilkan daftar container
- **docker rm**: untuk menghapus container.
- **docker rmi**: untuk menghapus image.
- **docker commit**: untuk melakukan perubahan atau pengaturan file ke dalam image yang baru. 
- **docker push**: untuk mengupload image ke server(docker hub).
- **docker pull**: untuk mengambil/download image dari server(docker hub).

## Dockerfile 
Dockerfile adalah sebuah teks dokumen yang berisi semua perintah yang dapat dipanggil pengguna pada command line untuk membuat sebuah image.

## Perintah Dockerfile
- **FROM**: untuk mengambil image dari repository yang sudah ada.
- **MAINTENER**: untuk menginformasikan siapa yang melakukan maintenance pada image yang dibuat.
- **LABEL**: untuk menambahkan tambahan informasi terhadap image.
- **ADD/COPY**: untuk menambahkan file pada lokasi folder tertentu
- **CMD**: untuk menjalankan command tertentu
- **ENTRYPOINT**: untuk menjalankan script tertentu ketika docker booting
