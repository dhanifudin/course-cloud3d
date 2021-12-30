# PERTEMUAN 10
### Docker
Docker adalah sebuah command-line program, sebuah background daemon dan serangkaian remote service dengan mengambil pendekatan logistic untuk memecahkan permasalahan umum perangkat lunak dan menyederhanakan pengalaman kita dalam installing, running, publishing, dan menghapus perangkat lunak. Docker bukan bahasa pemrograman dan bukan sebuah framework untuk membangun perangkat lunak. Docker adalah sebuah tool yang membantu kita dalam menyelesaikan permasalah umum seperti installing, removing, upgrading, distributing, trustring, dan menggelola software.
### Perintah Dasar Docker
* docker run: sebuah perintah untuk menjalankan container, ketika baru dijalankan pertama kali maka akan mencari/download image.
* docker build: digunakan untuk membuat sebuah docker image dari sebuah Dockerfile. Perintah ini secara default akan mencari di direktori saat ini tetapi dapat juga menggunakan spesifik PATH atau URL.
* docker images: perintah ini akan menampilkan semua image yang ada, informasi seperti tag dan ukuran akan ditampilkan.
* docker ps: akan menampilkan daftar container
* docker rm: perintah untuk menghapus satu atau lebih dari satu container.
* docker rmi: perintah untuk menghapus sebuah image atau lebih dari satu image.
* docker commit: digunakan untuk melakukan perubahan atau pengaturan file ke dalam image yang baru. 
* docker push: perintah untuk mengupload image ke server, docker hub.
* docker pull: perintah untuk mengambil/download image dari server, docker hub.
### Dockerfile
Dockerfile adalah sebuah teks dokumen yang berisi semua perintah yang dapat dipanggil pengguna pada command line untuk membuat sebuah image. Dengan menggunakan Dockerfile kita tidak perlu mengetik perintah satu persatu ketika akan membuat image.
### Perintah Dockerfile
* FROM: sebuah perintah inisialisasi untuk mengambil image dari repository yang sudah ada.
* MAINTENER: menginformasikan siapa yang melakukan maintenance pada image yang dibuat.
* LABEL: menambahkan tambahan informasi terhadap image.
* ADD/COPY: digunakan untuk menambahkan file pada lokasi folder tertentu
* CMD: perintah untuk menjalankan command tertentu
* ENTRYPOINT: menjalankan script tertentu ketika docker booting
### Containerization
Docker menggunakan Container Linux.Linux container biasanya disebut LXC yang pada Agustus 2018. Memanfaatkan fungsi cgroups kernel linux dari kernel linux versi 2.6.24. Linux container adalah sebuah virtualisasi sistem operasi yang dapat digunakan untuk menjalankan beberapa sistem Linux yang terisolasi pada satu host



