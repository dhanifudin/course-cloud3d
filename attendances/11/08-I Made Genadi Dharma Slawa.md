# Docker Network Bridge
 Merupakan jenis network bawaan dari Docker. Ketika Docker service daemon berjalan, akan melakukan
konfigurasi sebuah virtual bridge disebut dengan docker0. Jika kita tidak menyebutkan spesifik network yang digunakan, docker run –net=<Network> makaa Docker daemon akan terhubung ke container menggunakan bridge network. Masing-masing container yang dibuat, akan dialokasikan sebuah perangkat virtual Ethernet dan dipetakkan sebagai eth0 pada container.

# Docker Network Host
Docker network jenis ini yaitu meletakkan container di dalam stack hostnya network. Semua antarmuka jaringan yang telah didefinisikan dapat diakses melalui container. Ketika kita menjalankan container menggunakan parameter –net=host, sehingga container akan menggunakan network host. Ketika menggunakan host network akan secepat jaringan normal karena tidak ada menggunakan bridge ataupun translation

# Perintah Networking Docker
- Perintah yang dasar digunakan adalah docker network kemudian ditambahkan beberapa parameter setelah perintah dasar.
- Docker network ls; untuk mengetahui network yang tersedia pada host docker
- Docker network create; untuk membuat sebuah network pada host docker
- Docker network rm; untuk menghapus network yang terdapat pada host docker
- Docker network connect; untuk menghubungkan container pada spesifik network
- Docker network disconnect; memutus network pada container
- Docker network inspect; untuk mengetahui secara terperinci dari
sebuah network, misalkan ip address dan informasi lain
