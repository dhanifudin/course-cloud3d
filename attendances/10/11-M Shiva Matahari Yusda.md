# Docker

## Definisi

**Docker** adalah aplikasi untuk menyatukan berbagai file software dan pendukungnya dalam sebuah wadah (container) agar memudahkan proses pengembangan software.

Dalam pengembangan aplikasi, developer memerlukan virtualisasi di server agar aplikasi bisa berjalan di berbagai platform dengan konfigurasi hardware yang berbeda-beda.

Namun, ketika menggunakan virtualisasi, harus menyiapkan satu sistem operasi secara penuh. Jika membutuhkan beberapa virtualisasi, server perlu resource yang besar.

Untuk itu, container bisa digunakan sebagai alternatif virtualisasi sehingga tidak perlu menyiapkan sistem operasi secara penuh. Dengan container, ukuran file menjadi lebih kecil dibandingkan virtualisasi yang biasa digunakan.

## Latar Belakang Docker

Berawal pada saat tidak adanya standarisasi pengembangan aplikasi yang konsisten dan dilakukan dengan cara yang sama pada satu platform, apabila pengembangan dilakukan secara local development, hal ini dapat menyebabkan salah satu package belum terinstall sehingga terjadi error. Docker membungkus semuanya menjadi sistem file lengkap yang berisi semuanya kebutuhan aplikasi dan yang menjalankan mesin virtual itu sendiri. Docker bukanlah bahasa pemrograman atau framework, melaikan docker adalah sebuah tool berupa command-line program yang membantu kita dalam menyelesaikan permasalah umum seperti installing, removing, upgrading, distributing, trustring, dan mengelola software.

## Containerization

Docker menggunakan konsep container yaitu sebuah virtualisasi sistem operasi yang dapat digunakan untuk menjalankan beberapa sistem yang terisolasi pada satu host

## Virtualisasi vs Container

Docker memungkinkan membuat container pada virtual environment Mac/Windows di laptop dan menjalankan perintah atau mengoperasikannya. Perintah atau operasi yang dilakukan pada container yang dijalankan di local, akan sama seperti yang berjalan di production.

## Keuntungan Container

- **Portability** - Dapat memindahkan sebuah aplikasi ke _environtment production_.

- **Quick deployment/teardown** - Memudahkan untuk melakukan pengembangan aplikasi.

- **Managing infrastructure-like code** - konfigurasi docker disimpan pada sebuah file

- **Open Source** - Kode sumbernya terbuka, bebas untuk melakukan modifikasi program.

- **Consistency** - Hasil sama pada semua environtment saat melakukan deployment, hal ini untuk meminimalisir error kompatibilitas apabila dijalankan pada perangkat yang berbeda

## Arsitektur Docker

1. Client

   - docker build

   - docker pull

   - docker run

2. Docker Host

   - Docker daemon

     -> Container

     -> Images

3. Registry

## Istilah pada Docker

- **Docker container** - wadah dimana aplikasi dijalankan

- **Docker client** - kumpulan perintah _command line_ untuk mengoperasikan docker

- **Docker daemon** - aplikasi yang berjalan di host machine

- **Docker engine** - gabungan aplikasi yang menjalankan docker container, docker client, dan docker daemon.

- **Docker image** - template membuat container

- **Docker registry** - tempat menyimpan dokcer image

- **Docker compose** - cara digunakan untuk mendefinisikan dan menjalankan lebih dari satu container.

## Perintah dasar Docker

- `docker run` - menjalankan container

- `docker build` - membuat docker image dari Dockerfile

- `docker images` - mengumpulkan image yang ada

- `docker ps` - menampilkan daftar container

- `docker rm` - mengapus satu atau lebih container

- `docker rmi` - menghapus satu atau lebih image

- `docker commit` - pengaturan file ke dalam image yang baru

- `docker push` - upload image ke server

- `docker pull` - download image dari server

## Dockerfile

Dockerfile adalah sebuah teks dokumen yang berisi semua perintah yang dapat dipanggil pengguna pada command line untuk membuat sebuah image. Dengan menggunakan Dockerfile kita tidak perlu mengetik perintah satu persatu ketika akan membuat image.

## Perintah Dockerfile

- **FROM** - mengambil image dari repository

- **MAINTENER** - author pembuat image

- **LABEL** - tambahan informasi pada image

- **ADD/COPY** - menambah atau menyalin file

- **CMD** - pertintah untuk menjalankan command tertentu

- **ENTRYPOINT** - menjalankan script tertentu ketika docker booting
