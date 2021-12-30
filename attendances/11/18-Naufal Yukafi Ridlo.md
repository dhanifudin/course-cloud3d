# Docker 2
### Docker Network Bridge
Docker Network Bridge merupakan jenis network bawaan dari Docker. Ketika Docker service daemon berjalan, akan melakukan konfigurasi sebuah virtual bridge disebut dengan docker0. Jika kita tidak menyebutkan spesifik network yang digunakan, docker run –net= makaa Docker daemon akan terhubung ke container menggunakan bridge network. Masing-masing container yang dibuat, akan dialokasikan sebuah perangkat virtual Ethernet dan dipetakkan sebagai eth0 pada container.

### Docker Network Host
Network ini meletakkan container dalam stack host network. Semua interface dapat diakses melalui container. 
Menggunakan host network sama seperti jaringan aslinya sehingga dapat melakukan performa jaringan terbaik, 
bahkan akan lebih cepat daripada container yang menggunakan bridge. Container akan membagi network dari host yang langsung ke internet. 
Ketika menggunakan network ini, container akan dapat diakses melalui IP host.

### Perintah Networking Docker
- Docker network ls: untuk mengetahui network yang tersedia pada host docker

- Docker network craete: untuk membuat sebuah network pada host docker

- Docker network rm: untuk menghapus network yang terdapat pada host docker

- Docker network connect: untuk menghubungkan container spesifik network

- Docker network disconnect: untuk memutus network pada container

- Docker network inspect: untuk mengetahui secara rinci dari sebuah network

### Docker Compose
Docker compose adalah sebuah tool untuk mendefiniskan, launching, dan mengelola service, dimana sebuah service adalah didefinisikan sebagai satu atau lebih dari sebuah docker container. Service dan sistem service didefinisikan di dalam file YAML dan mengelolanya menggunakan perintah command-line docker-compose.

