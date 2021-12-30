# PERTEMUAN 11
## Docker Network
### Docker Network Bridge
  * Merupakan jenis network bawaan dari Docker
  * Jika kita tidak menyebutkan spesifik network yang digunakan, docker run –net=<Network> makaa Docker daemon akan terhubung ke container menggunakan bridge network.
  * Masing-masing container yang dibuat, akan dialokasikan sebuah perangkat virtual Ethernet dan dipetakkan sebagai eth0 pada container.
### Docker Network Host
  * Docker network jenis ini yaitu meletakkan container di dalam stack hostnya network.
  * Semua antarmuka jaringan yang telah didefinisikan dapat diakses melalui container.
  * Ketika kita menjalankan container menggunakan parameter –net=host, sehingga container akan menggunakan network host.
  * Ketika menggunakan host network akan secepat jaringan normal karena tidak ada menggunakan bridge ataupun translation
### Docker Network None
  * Network None bertujuan untuk tidak mengkonfigurasi networking.
  * Tidak ada driver yang digunakan pada Network jenis ini.
  * Ketika kita tidak menginginkan container untuk dapat diakses. Perintah yang digunakan dengan menambahkan parameter –net=none
### Expose dan mapping port
  Expose port adalah container aplikasi kita akan listen pada port yang ter-expose. Sebagai contoh, aplikasi server Tomcat akan listen pada port default yaitu 8080. Semua container yang berjalan pada host yang sama dan network yang sama dapat berkomunikasi dengan Tomcat pada port 8080.Expose port dapat dilakukan menggunakan 2 cara yaitu salah satunya adalah menggunakan Dockerfile dengan perintah EXPOSE dan menggunakan perintah docker run –expose. Ketika container berbeda host atau network agar tetap bisa berkomunikasi menggunakan maping port. Mapping port dilakuan dengan menambahkan parameter –p ketika menjalankan container. 
## Docker Volume
### Docker Volume Driver
Docker volume driver for Azure file storage; sebuah driver docker volume yang digunakan Azure file storage untuk mount file yang dishare pada cloud ke Docker container sebagai volume.
IPFS(InterPlanetary File System); sebuah plugin volume open source yang mengizinkan menggunakan sebuah IPFS filesystem sebagai sebuah volume. IPFS adalah sebuah sistem storage yang sangat menarik dan menjanjikan, memungkinkan dalam mendistribusikan high volume data dengan efisiensi yang tinggi.
## Docker Compose
  Docker compose adalah sebuah tool untuk mendefiniskan, launching, dan mengelola service, dimana sebuah service adalah didefinisikan sebagai satu atau lebih dari sebuah docker container. Beberapa hal yang bisa dilakukan menggunakan docker compose adalah build docker image, menjalankan aplikasi container sebagai service, menjalankan full system dari service, mengelola secara individu service pada sebuah sistem, melakukan scaling up atau down, dan melihat log dari kumpulan container yang berjalan sebagai service.
### Perintah Dasar Docker Compose
  * Docker-compose up; membuat dan menjalankan container, ketika ditambakan parameter –d maka container akan berjalan sebagai daemon.
  * Docker-compose down; menghentikan dan menghapus semua resource
  * Docker-compose logs; melihat logging pada container
  * Docker-compose ps; melihat container yang sedang berjalan

