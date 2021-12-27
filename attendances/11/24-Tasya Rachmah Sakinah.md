# Pertemuan 11
## Docker Network Bridge
- Merupakan jenis network bawaan dari Docker
- Ketika Docker service daemon berjalan, akan melakukan konfigurasi sebuah virtual bridge disebut dengan docker0.
- Jika kita tidak menyebutkan spesifik network yang digunakan, docker run –net=<Network> maka Docker daemon akan terhubung ke container menggunakan bridge network.
- Masing-masing container yang dibuat, akan dialokasikan sebuah perangkat virtual Ethernet dan dipetakkan sebagai eth0 pada container.
- Dalam container interface eth0 akan diberi sebuah IP address dari rentang alamat bridge.
- Docker akan mencari sebuah IP address yang tersedia pada bridge dan akan mengkonfigurasi interface eth0 container dengan IP address.
- Ketika container ingin terhubung ke internet akan menggunakan bridge. Bridge akan secara automatis meneruskan paket antara interface network yang lain asalkan terhubung dan juga diizinkan container berkomunikasi dengan mesin host.

## Docker Network Host
- Docker network jenis ini yaitu meletakkan container di dalam stack hostnya network.
- Semua antarmuka jaringan yang telah didefinisikan dapat diakses melalui container.
- Ketika kita menjalankan container menggunakan parameter –net=host, sehingga container akan menggunakan network host.
- Ketika menggunakan host network akan secepat jaringan normal karena tidak ada menggunakan bridge ataupun translation

## Docker Network None
- Network None bertujuan untuk tidak mengkonfigurasi networking.
- Tidak ada driver yang digunakan pada Network jenis ini.
- Ketika kita tidak menginginkan container untuk dapat diakses. Perintah yang digunakan dengan menambahkan parameter –net=none

## Perintah Networking Docker
- Perintah yang dasar digunakan adalah docker network kemudian ditambahkan beberapa parameter setelah perintah dasar.
- Docker network ls; untuk mengetahui network yang tersedia pada host docker
- Docker network create; untuk membuat sebuah network pada host docker.
- Docker network rm; untuk menghapus network yang terdapat pada host docker.
- Docker network connect; untuk menghubungkan container pada spesifik network
- Docker network disconnect; memutus network pada container
- Docker network inspect; untuk mengetahui secara terperinci dari sebuah network, misalkan ip address dan informasi lain

## Expose dan mapping port
- Skenario yang umum digunakan ketika kita menginginkan container menerima koneksi yang datang, salah satunya dari container yang lain atau dari luar docker.
- Aplikasi server yang listening pada port 80 atau sebuah database yang menerima request yang datang.
- Sebuah image dapat juga melakukan expose port.
- Expose port adalah container aplikasi kita akan listen pada port yang ter-expose. Sebagai contoh, aplikasi server Tomcat akan listen pada port default yaitu 8080.
- Semua container yang berjalan pada host yang sama dan network yang sama dapat berkomunikasi dengan Tomcat pada port 8080.

## Perintah Docker Volume
- Docker volume create; untuk membuat sebuah volume
- Docker volume inspect; menampilkan detail informasi pada satu atau lebih dari satu volume.
- Docker volume ls; menampilkan daftar volume.
- Docker volume rm; menghapus satu atau lebih volume yang terdapat pada docker host.
- Docker volume prune; menghapus semua volume yang tidak digunakan, semua volume yang sudah tidak digunakan oleh container akan dihapus.
