Pertemuan 11 - Docker (2)

1. Tipe Network Docker & Perintah Dasar Docker
- Bridge
Merupakan jenis network bawaan dari Docker. Ketika Docker service daemon berjalan, akan melakukan konfigurasi sebuah virtual bridge disebut dengan docker0. Masing-masing container yang dibuat, akan dialokasikan sebuah perangkat virtual Ethernet dan dipetakkan sebagai eth0 pada container yang kemudian akan diberi sebuah IP address dari rentang alamat bridge. Ketika container ingin terhubung ke internet akan menggunakan bridge. Bridge akan secara automatis meneruskan paket antara interface network yang lain.
- Host
Merupakan jenis yang meletakkan container di dalam stack hostnya network. Dimana semua antarmuka jaringan yang telah didefinisikan dapat diakses melalui container. Container yang berjalan di dalam stack hostnya network akan mendapatkan jauh lebih cepat dibandingkan container yang berjalan menggunakan network bridge, tidak membutuhkan traverse pada docker0 bridge dan mappings port iptables.
- none
Network None bertujuan untuk tidak mengkonfigurasi networking serta tidak ada driver yang digunakan pada network jenis ini. Ketika kita tidak menginginkan container untuk dapat diakses. Perintah yang digunakan dengan menambahkan parameter –net=none.

Perintah pada docker :
- Docker network ls : mengetahui network yang tersedia pada host docker
- Docker network create : membuat sebuah network pada host docker.
- Docker network rm : untuk menghapus network yang terdapat pada host docker.
- Docker network connect : menghubungkan container pada spesifik network
- Docker network disconnect : memutus network pada container
- Docker network inspect : mengetahui secara terperinci dari sebuah network, misalkan ip address dan informasi lain

2. Expose dan Mapping Port
- Expose port adalah container aplikasi kita akan listen pada port yang ter-expose. Sebagai contoh, Semua container yang berjalan pada host yang sama dan network yang sama dapat berkomunikasi dengan Tomcat pada port 8080. Expose port dapat dilakukan menggunakan 2 cara yaitu salah satunya adalah menggunakan Dockerfile dengan perintah EXPOSE dan menggunakan perintah docker run –expose
- Mapping port dilakuan dengan menambahkan parameter –p ketika menjalankan container. Ketika container berbeda host atau network agar tetap bisa berkomunikasi menggunakan maping port.

3. Persistent Storage (volume) & Perintah Docker Volume
Persistent storage pada docker bertujuan agar data pada container tetap terjaga walaupun container telah dihapus. Persitence storage juga dapat berbagi data antara container yang lain ataupun dengan host docker. 

Perintah pada docker volume :
- Docker volume create : membuat sebuah volume
- Docker volume inspect : menampilkan detail informasi pada satu atau lebih dari satu volume.
- Docker volume ls : menampilkan daftar volume.
- Docker volume rm : menghapus satu atau lebih volume yang terdapat pada docker host.
- Docker volume prune : menghapus semua volume yang tidak digunakan, semua volume yang sudah tidak digunakan oleh container akan dihapus.

4. Docker Compose & Perintah Docker Compose
Docker compose adalah tool untuk mendefiniskan, launching, dan mengelola service (yang merupakan satu atau lebih  dari sebuah docker container) seperti melakukan build docker image, menjalankan aplikasi container sebagai service, menjalankan full system dari service, mengelola secara individu service pada sebuah sistem, melakukan scaling up atau down, dan melihat log dari kumpulan container yang berjalan sebagai service. Service dan sistem service didefinisikan di dalam file YAML dan mengelolanya menggunakan perintah command-line docker-compose.

Perintah docker compose :
- Docker-compose up : membuat dan menjalankan container, ketika ditambakan parameter –d maka container akan berjalan sebagai daemon.
- Docker-compose down : menghentikan dan menghapus semua resource
- Docker-compose logs : melihat logging pada container
- Docker-compose ps : melihat container yang sedang berjalan