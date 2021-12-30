# Docker 2

## Docker Network

1. Docker Network Bridge

   - Jenis network bawaan Docker.

   - Ketika Docker service daemon berjalan, akan melakukan konfigurasi sebuah virtual bridge disebut dengan docker0.

   - Jika kita tidak menyebutkan spesifik network yang digunakan, docker run –net = Network maka Docker daemon akan terhubung ke container menggunakan bridge network.

   - Masing-masing container yang dibuat, akan dialokasikan sebuah perangkat virtual Ethernet dan dipetakkan sebagai eth0 pada container.

2. Docker Network Host

   - Meletakkan _container_ didalam stack hostnya network.

   - Antarmuka yang didefinisikan dapat diakses melalui container.

   - Container akan menggunakan network host apabila parameter -net=host dijalankan

3. Docker Network None

   - Bertujuan untuk tidak mengkonfigurasi networking.

   - Driver tidak digunakan pada network ini.

   - Perintah parameter -net=none digunakan ketika container tidak ingin diakses.

### Perintah Networking Docker

- Docker network ls -> mengetahui network yang tersedia pada host docker

- Docker network craete -> membuat sebuah network pada host docker

- Docker network rm -> untuk menghapus network yang terdapat pada host docker

- Docker network connect -> menghubungkan container spesifik network

- Docker network disconnect -> memutus network pada container

- Docker network inspect -> mengetahui secara rinci dari sebuah network

### Expose dan Mapping Port

Skenario yang umum digunakan ketika kita menginginkan container menerima koneksi yang datang, salah satunya dari container yang lain atau dari luar docker. Expose port adalah container aplikasi kita akan listen pada port yang ter-expose. Sebagai contoh, aplikasi server Tomcat akan listen pada port default yaitu 8080. Semua container yang berjalan pada host yang sama dan network yang sama dapat berkomunikasi dengan Tomcat pada port 8080.

### Persistent Storage (Volume)

Persistent storage pada docker bertujuan agar data pada container tetap terjaga walaupun container telah dihapus. Persitence storage juga dapat berbagi data antara container yang lain ataupun dengan host docker.

## Docker Volume

- Docker volume create -> membuat sebuah volume

- Docker volume inspect -> menampilkan detail informasi volume

- Dcoker volume ls -> menampilkan daftar volume

- Docker volume rm -> menghapus volume yang terdapat pada docker host

- Docker volume prune -> menghapus semua volume yang tidak digunakan oleh container

### Docker Volume Driver

Digunakan agar volume dapat terintegrasi dengan jenis penyimpanan lain, antara lain sebagai berikut :

- Docker volume driver for Azure file storage

- IPSF (InterPlanetary File System)

- Keywhiz

## Docker Compose

Docker compose adalah sebuah tool untuk mendefiniskan, launching, dan mengelola service, dimana sebuah service adalah didefinisikan sebagai satu atau lebih dari sebuah docker container. Service dan sistem service didefinisikan di dalam file YAML dan mengelolanya menggunakan perintah command-line docker-compose.

### Perintah Docker Compose

- Docker-compose up -> membuat dan menjalankan container

- Docker-compose down -> menghentikan dan menghapus semua resource

- Docker-compose logs -> melihat logging pada container

- Docker-compose ps -> melihat container yang sedang berjalan

Untuk melakukan setting terkait deengan kebutuhan komponen atau konfigurasi dari aplikasi yang akan diintegrasikan pada container, maka dapat dilakukan pada Dockerfile.
