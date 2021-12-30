<h1>Docker 2</h1>

**Tipe Docker Network**
- Bridge
- Host
- None

**Docker Network Bridge**
- Jenis network bawaan dari Docker.
- Ketika Docker service daemon berjalan, akan melakukan konfigurasi sebuah virtual bridge disebut dengan docker0.
- Jika tidak menyebutkan spesifik network yang digunakan, docker run –net=<Network> makaa Docker daemon akan terhubung ke container menggunakan bridge network.

**Docker Network Host**
- Docker network jenis ini yaitu meletakkan container di dalam stack hostnya network.
- Semua antarmuka jaringan yang telah didefinisikan dapat diakses melalui container.
- Ketika menjalankan container menggunakan parameter –net=host, sehingga container akan menggunakan network host.

**Docker Network None**
- Network None bertujuan untuk tidak mengkonfigurasi networking.
- Tidak ada driver yang digunakan pada Network jenis ini.
- Ketika tidak menginginkan container untuk dapat diakses. Perintah yang digunakan dengan menambahkan parameter –net=none.

**Perintah Networking Docker**
- Perintah yang dasar yaiut docker network kemudian ditambahkan beberapa parameter setelah perintah dasar.
- Docker network ls; untuk mengetahui network yang tersedia pada host docker.
- Docker network create; untuk membuat sebuah network pada host docker.
- Docker network rm; untuk menghapus network yang terdapat pada host docker.
- Docker network connect; untuk menghubungkan container pada spesifik network.
- Docker network disconnect; memutus network pada container.
- Docker network inspect; untuk mengetahui secara terperinci dari sebuah network.

**Expose dan mapping port**
- Skenario yang umum digunakan ketika menginginkan container menerima koneksi yang datang, salah satunya dari container yang lain atau dari luar docker.
- Aplikasi server yang listening pada port 80 atau sebuah database yang menerima request yang datang.
- Sebuah image dapat juga melakukan expose port.

**Persistent Storage (Volume)**
- Persistent storage pada docker bertujuan agar data pada container tetap terjaga walaupun container telah dihapus
- Persitence storage juga dapat berbagi data antara container yang lain ataupun dengan host docker.

**Perintah Docker Volume**
- Docker volume create; untuk membuat sebuah volume
- Docker volume inspect; menampilkan detail informasi pada satu atau lebih dari satu volume.
- Docker volume ls; menampilkan daftar volume.
- Docker volume rm; menghapus satu atau lebih volume yang terdapat pada docker host.
- Docker volume prune; menghapus semua volume yang tidak digunakan, semua volume yang sudah tidak digunakan oleh container akan dihapus.

**Docker Volume Driver**
- Sama dengan network yang memiliki driver, volume juga memiliki jenis-jenis volume agar mampu terintegrasi dengan jenis penyimpanan yang lain.
- Docker volume driver for Azure file storage; sebuah driver docker volume yang digunakan Azure file storage untuk mount file yang dishare pada cloud ke Docker container sebagai volume.

**Docker Compose**
- Docker compose adalah sebuah tool untuk mendefiniskan, launching, dan mengelola service, dimana sebuah service adalah didefinisikan sebagai satu atau lebih dari sebuah docker container.
- Service dan sistem service didefinisikan di dalam file YAML dan mengelolanya menggunakan perintah command-line docker-compose.

**Perintah Dasar Docker Compose**
- Docker-compose up; membuat dan menjalankan container, ketika ditambakan parameter –d maka container akan berjalan sebagai daemon.
- Docker-compose down; menghentikan dan menghapus semua resource.
- Docker-compose logs; melihat logging pada container.
- Docker-compose ps; melihat container yang sedang berjalan.
