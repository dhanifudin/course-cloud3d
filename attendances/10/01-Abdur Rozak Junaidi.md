<h1>Docker</h1>

**Latar Belakang Docker**

Mengemas aplikasi dengan semua dependensi yang dibutuhkannya ke dalam sebuah standar untuk deployment. Docker membungkus semuanya menjadi sistem file lengkap yang berisi semuanya kebutuhan aplikasi dan yang menjalankan mesin virtual itu sendiri.

**Docker**

Docker adalah sebuah command-line program, sebuah background daemon dan serangkaian remote service dengan mengambil pendekatan logistic untuk memecahkan permasalahan umum perangkat lunak dan menyederhanakan pengalaman kita dalam installing, running, publishing, dan menghapus perangkat lunak. Docker bukan bahasa pemrograman dan bukan sebuah framework untuk membangun perangkat lunak

**Istilah pada Docker**
- Docker container : virtual machine berjalan di dalam docker container.
- Docker client : kumpulan perintah command line untuk mengoperasikan docker container.
- Docker daemon : aplikasi yang berjalan di host machine.
- Docker engine : gabungan aplikasi yang menjalankan docker container, docker client, dan docker daemon. 
- Docker image : template yang digunakan untuk membuat container. 
- Docker registry : tempat yang digunakan untuk menyimpan docker image. 
- Docker compose : sebuah cara yang dapat digunakan untuk mendefinisikan dan menjalankan lebih dari satu container.

**Perintah Dasar Docker**
- Docker run: Perintah untuk menjalankan containersaat pertama kali maka akan mencari/download image.
- Docker build: Perintah untuk membuat sebuah docker image dari sebuah Dockerfile. 
- Docker images: Perintah untuk menampilkan semua image yang ada, informasi seperti tag dan ukuran akan ditampilkan.
- Docker ps: Untukmenampilkan daftar container.
- Docker rm: Perintah untuk menghapus satu atau lebih dari satu container.
- Docker rmi: Perintah untuk menghapus sebuah image atau lebih dari satu image.
- docker commit: Perintah untuk melakukan perubahan atau pengaturan file ke dalam image yang baru. 
- Docker push: perintah untuk mengupload image ke server, docker hub.
- Docker pull: perintah untuk mengambil/download image dari server, docker hub.

**Dockerfile**

Dockerfile adalah sebuah teks dokumen yang berisi semua perintah yang dapat dipanggil pengguna pada command line untuk membuat sebuah image. Docker dapat membuat sebuah image secara automatis dengan membaca perintah dari Dockerfile.

**Perintah Dockerfile**
- FROM : Perintah inisialisasi untuk mengambil image dari repository yang sudah ada.
- MAINTENER : Menginformasikan siapa yang melakukan maintenance pada image yang dibuat.
- LABEL : Menambahkan tambahan informasi terhadap image.
- ADD/COPY : Untuk menambahkan file pada lokasi folder tertentu.
- CMD : Untuk menjalankan command tertentu.
- ENTRYPOINT : menjalankan script tertentu ketika docker booting.



