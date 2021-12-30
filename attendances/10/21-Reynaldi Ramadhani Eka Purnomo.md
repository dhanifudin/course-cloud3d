# PENGERTIAN DOCKER
Docker adalah sebuah container , digunakan untuk membungkus file file yang dibutuhkan
untuk sebuah software . Docker biasanya digunakan oleh developer untuk pengembangan software
karena setiap pc atau os memiliki konfigurasi yang berbeda jadi memungkinkan sebuah software
tidak bisa berjalan di lain pc atau os .
Docker bisa memiliki banyak container dan memindahkan ke web server lebih mudah dibandingankan
Virtual Machine sendiri .

# Containerization
    - Docker menggunakan container linux
    - Linux Container biasanya disebut LXC yang pada agustus 2018
    - Memanfaatkan fungsi cgroups kernel linux dari kernel linux versi 2.6.24
    - Linux container adalah sebuah virtualisasi sistem operasi yang dapat digunakan untuk menjalankan beberapa sistem Linux yang terisolasi pada satu host

# Keuntungan Container
    - Portability
    - Deployment yang cepat
    - memanaged infrastructure seperti code
    - open source
    - Konsisten 

# Produk Virtualisasi
    * Berbasis HyperVisor
        - Oracle Virtual Box
        - VMWare
        - KVM
        - Microsoft Hyper-V
    * Berbasis Container
        - Open VZ
        - LXC

# Istilah DOcker
    - Docker container: virtual machine atau guest operating system, aplikasi kita berjalan di dalam docker container.
    - Docker client: kumpulan perintah command line untuk mengoperasikan docker container, misalkan membuat container, start/stop container, menghapus, dan sebagainya.
    - Docker daemon: aplikasi yang berjalan di host machine. Docker server berjalan di background(sebagai daemon) dan menunggu perintah dari docker client.
    - Docker engine: gabungan aplikasi yang menjalankan docker container, docker client, dan docker daemon. 
    - Docker image: template yang digunakan untuk membuat container. Misalkan image ubuntu, CentOS, dan sebagainya. 
    - Docker registry: tempat yang digunakan untuk menyimpan docker image. Docker hub adalah sebuah registry public yang semua orang dapat menggunakan. Secara default docker akan mencari image pada docker hub.
    - Docker compose: sebuah cara yang dapat digunakan untuk mendefinisikan dan menjalankan lebih dari satu container.

# Perintah Dasar Docker
    - docker run: sebuah perintah untuk menjalankan container, ketika baru dijalankan pertama kali maka akan mencari/download image.
    - docker build: digunakan untuk membuat sebuah docker image dari sebuah Dockerfile. Perintah ini secara default akan mencari di direktori saat ini tetapi dapat juga menggunakan spesifik PATH atau URL.
    - docker images: perintah ini akan menampilkan semua image yang ada, informasi seperti tag dan ukuran akan ditampilkan.
    - docker ps: akan menampilkan daftar container
    - docker rm: perintah untuk menghapus satu atau lebih dari satu container.
    - docker rmi: perintah untuk menghapus sebuah image atau lebih dari satu image.
    - docker commit: digunakan untuk melakukan perubahan atau pengaturan file ke dalam image yang baru. 
    - docker push: perintah untuk mengupload image ke server, docker hub.
    - docker pull: perintah untuk mengambil/download image dari server, docker hub.


