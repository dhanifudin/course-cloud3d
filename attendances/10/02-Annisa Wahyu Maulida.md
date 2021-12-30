Pertemuan 10 - Docker

1. Sejarah Docker
- Docker merupakan project internal (oleh dotCloud) kemudian di open source kan
- DotCloud berkolaborasi dengan Redhat dan Amazon untuk menambah layanan sehingga docker dapat digunakan untuk mengelola infrastruktur disana
- Docker sedang populer
- Docker : membungkus aplikasi dengan semua dependensi kedalam sistem file lengkap
- Docker menggunakan Container Linux yang standar untuk deployment (dengan menjalankan VM itu sendiri)

2. Virtualisasi Vs. Container
- Docker merupakan container management system -> membantu mengelola container
- Memungkinkan membuat container pada virtual environment Mac/Windows di laptop dan menjalankan perintah atau mengoperasikannya.
- Setiap membuat sebuah container, tidak membutuhan system operasi secara penuh
- Docker mengandalkan penggunaan kernel Linux Kernel
- Docker menghasilkan sebuah ukuran image yang kecil, compact, dan ringan untuk didistribusikan karena tidak terdapat kernel bahkan sistem operasi

3. Keuntungan Container
- portability
- quick deployment/teardown (mudah dg docker)
- managing infrastructure like code 
- open source
- consistency

4. Produk Virtualisasi
- Berbasis Hypervisor (Oracle Virtualbox, VMWare, KVM, Microsoft Hyper-V)
- Berbasis Container (OpenVZ, LXC)

5. Pengertian Docker 
- Docker merupakan command line program dan bukan merupakan bahasa pemrograman maupun framework
- Docker merupakan tool dalam membantu menyelesaikan permasalah umum seperti installing, removing, upgrading, distributing, trustring, dan menggelola software
- Docker jalan disemua OS (Windows, Linux, Mac)

6. Istilah Pada Docker
- Docker container : virtual machine dimana aplikasi kita berjalan didalam docker container
- Docker client : kumpulan perintah command line untuk mengoperasikan docker container (misal membuat container, start/stop, menghapus, dll)
- Docker daemon : aplikasi yang berjalan di host machine. Docker server berjalan di background(sebagai daemon) dan menunggu perintah dari docker client
- Docker engine : gabungan aplikasi yang menjalankan docker container, docker client, dan docker daemon
- Docker image : template yang digunakan untuk membuat container
- Docker registry : tempat yang digunakan untuk menyimpan docker image
- Docker compose: cara yang dapat digunakan untuk mendefinisikan dan menjalankan lebih dari satu container

7. Perintah Dasar Docker
- docker run : sebuah perintah untuk menjalankan container
- docker build : digunakan untuk membuat sebuah docker image dari sebuah 
Dockerfile (teks dokumen yang berisi semua perintah yang dapat 
dipanggil pengguna pada command line untuk membuat sebuah image)
- docker images: menampilkan semua image yang ada, informasi tag dan ukuran
- docker ps: akan menampilkan daftar container
- docker rm : perintah untuk menghapus satu atau lebih dari satu container
- docker rmi: perintah untuk menghapus sebuah image atau lebih dari satu image
- docker commit: digunakan untuk melakukan perubahan atau pengaturan file ke dalam image yang baru
- docker push: perintah untuk mengupload image ke server, docker hub
- docker pull: perintah untuk mengambil/download image dari server, docker hub

8. Perintah Dockerfile
- FROM : sebuah perintah inisialisasi untuk mengambil image dari repository yang sudah ada
- MAINTENER : menginformasikan siapa yang melakukan maintenance pada image yang dibuat
- LABEL: menambahkan tambahan informasi terhadap image
- ADD/COPY : digunakan untuk menambahkan file pada lokasi folder tertentu
- CMD : perintah untuk menjalankan command tertentu
- ENTRYPOINT : menjalankan script tertentu ketika docker booting