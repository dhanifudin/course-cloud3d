# Resume Pertemuan 9
## Docker
Docker adalah sebuah command-line program, sebuah background daemon dan serangkaian 
remote service dengan mengambil pendekatan logistic untuk memecahkan permasalahan 
umum perangkat lunak dan menyederhanakan pengalaman kita dalam installing, running, 
publishing, dan menghapus perangkat lunak.
Docker adalah sebuah tool. Docker bukan bahasa pemrograman dan bukan sebuah framework 
untuk membangun perangkat lunak.

## Arsitektur Docker
Terdapat istilah pada Docker :
1. Docker container
2. Docker client
3. Docker daemon
4. Docker engine
5. Docker image
6. Docker registry
7. Docker compose

Perintah dasar pada Docker :
1. docker run
2. docker build
3. docker images
4. docker ps
5. docker rm
6. docker rmi
7. docker commit
8. docker push
9. docker pull

## Dockerfile
Docker dapat membuat sebuah image secara automatis dengan membaca perintah dari Dockerfile.
Dockerfile adalah sebuah teks dokumen yang berisi semua perintah yang dapat dipanggil pengguna 
pada command line untuk membuat sebuah image.
Dengan menggunakan Dockerfile kita tidak perlu mengetik perintah satu persatu ketika akan membuat image.

Perintah Dockerfile :
- FROM
- MAINTENER
- LABEL
- ADD/COPY
- CMD
- ENTRYPOINT

## Containerization
Docker menggunakan Container Linux. Linux container biasanya disebut LXC yang pada Agustus 2018.
Memanfaatkan fungsi cgroups kernel linux dari kernel linux versi 2.6.24. Linux container adalah 
sebuah virtualisasi sistem operasi yang dapat digunakan untuk menjalankan beberapa sistem Linux yang terisolasi pada satu host

## Virtualisasi vc Container
- Docker adalah sebuah container management system yang membantu mengelola container lebih mudah dan universal.
- Memungkinkan membuat container pada virtual environment Mac/Windows di laptop dan menjalankan perintah atau mengoperasikannya.
- Perintah atau operasi yang dilakukan pada container yang dijalankan di local, akan sama seperti yang berjalan di production.
- Setiap membuat sebuah container, tidak membutuhan system operasi secara penuh
- Docker mengandalkan penggunaan kernel Linux Kernel
- Docker menghasilkan sebuah ukuran image yang kecil, compact, dan ringan untuk didistribusikan karena tidak terdapat kernel bahkan sistem operasi

## Keuntungan Container
- Portability
- Quick deployment/teardown
- Managing infrastructure-like code
- Open source
- Consistency 








