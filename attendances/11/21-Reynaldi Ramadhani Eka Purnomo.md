# DOCKER 2

# Docker Network 
Docker Network terbagi menjadi 3 yaitu Bridge , Host dan None .
    - Bridge , Network Bawaan dari docker , ketika Docker service daemon berjalan, akan melakukan konfigurasi sebuah virtual bridge disebut dengan docker0.
    - Host , Docker network jenis ini yaitu meletakkan container di dalam stack hostnya network. Semua antarmuka jaringan yang telah didefinisikan dapat diakses melalui container.
    -None , Network None bertujuan untuk tidak mengkonfigurasi networking. Tidak ada driver yang digunakan pada Network jenis ini.

# Perintah Networking Docker
    - Perintah yang dasar digunakan adalah docker network kemudian ditambahkan beberapa parameter setelah perintah dasar.
    - Docker network ls; untuk mengetahui network yang tersedia pada host docker
    - Docker network create; untuk membuat sebuah network pada host docker.
    - Docker network rm; untuk menghapus network yang terdapat pada host docker.
    - Docker network connect; untuk menghubungkan container pada spesifik network
    - Docker network disconnect; memutus network pada container
    - Docker network inspect; untuk mengetahui secara terperinci dari sebuah network, misalkan ip address dan informasi lain

# Presistent Storage (Volume)
    - Persistent storage pada docker bertujuan agar data pada container tetap terjaga walaupun container telah dihapus
    - Persitence storage juga dapat berbagi data antara container yang lain ataupun dengan host docker.
    - Sebagai contoh ketika kita membuat sebuah container yang bertujuan untuk menyimpan data transaksi pada sebuah database transactional, ketika menggunakan volume data yang tersimpan pada database transactional akan tetap persistent walaupun kita sudah menghapus container.

# Perintah DOcker Volume
    - Docker volume create; untuk membuat sebuah volume
    - Docker volume inspect; menampilkan detail informasi pada satu atau lebih dari satu volume.
    - Docker volume ls; menampilkan daftar volume.
    - Docker volume rm; menghapus satu atau lebih volume yang terdapat pada docker host.
    - Docker volume prune; menghapus semua volume yang tidak digunakan, semua volume yang sudah tidak digunakan oleh container akan dihapus.

# Docker Compose 
adalah sebuah tool untuk mendefiniskan, launching, dan mengelola service, dimana sebuah service adalah didefinisikan sebagai satu atau lebih dari sebuah docker container.Service dan sistem service didefinisikan di dalam file YAML dan mengelolanya menggunakan perintah command-line docker-compose.Beberapa hal yang bisa dilakukan menggunakan docker compose adalah build docker image, menjalankan aplikasi container sebagai service, menjalankan full system dari service, mengelola secara individu service pada sebuah sistem, melakukan scaling up atau down, dan melihat log dari kumpulan container yang berjalan sebagai service.

# Perintah Docker Compose
    - Docker-compose up; membuat dan menjalankan container, ketika ditambakan parameter –d maka container akan berjalan sebagai daemon.
    - Docker-compose down; menghentikan dan menghapus semua resource
    - Docker-compose logs; melihat logging pada container
    - Docker-compose ps; melihat container yang sedang berjalan








