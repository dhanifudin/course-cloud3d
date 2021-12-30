# Tipe Docker
Terdapat 3 jenis docker, yaitu :
1. Docker Netwwork Bridge = Network di pakai ketika banyak ethernet atau interface yang akan di jadikan 1 dalam sebuah bridge dalam 1 beridge ini akan dicluster sehingga akan terdapat rule didalamnya.
2. Docker Network Host = Network akan melakukan maping dengan host local lalu akan dipetakkan kedalam container.
3. Docker Network None = Nwtwork dalam container ini tidak ada jaringan yang berperan dan hanya bisa djalan dilokal.

# Docker Volume Driver
Docker Volume Driver berperan sebagai penyimpanan dalam sebuah container yang konsepnya sama dengan sysmlink. 
Terdapat beberapa jenis volume agar mampu terintegrasi dengan jenis penyimpanan yang lain. Beberapa jenis dari Volume, yaitu :
1. Docker volume driver for Azure file storage
2. IPFS(InterPlanetary File System)
3. Keywhiz

# Docker Compose
Docker compose adalah sebuah tool untuk mendefiniskan, melakukan launching, dan mengelola service yang didefinisikan sebagai satu atau lebih dari sebuah docker container. 
Service dan sistem service akan didefinisikan di dalam file YAML yang mana file tersebut akan mengelola perintah command-line docker-compose. 
Berikut beberapa kegunaan Docker Compose diantaranya yaitu :
1. Membuild docker image
2. Menjalankan aplikasi container sebagai service
3. Menjalankan full system dari service
4. Mengelola secara individu service pada sebuah sistem
5. Melakukan scaling up atau down
6. Melihat log dari kumpulan container yang berjalan sebagai service

# Perintah Dasar
Berikut beberapa perintah dasar yang sering digunakan:
1. Docker network ls = Berfungsi untuk mengetahui network yang tersedia pada host docker
2. Docker network create = Berfungsi untuk membuat sebuah network pada host docker.
3. Docker network connect = Berfungsi untuk menghubungkan container pada spesifik network
4. Docker network disconnect = Berfungsi untuk memutus network pada container
