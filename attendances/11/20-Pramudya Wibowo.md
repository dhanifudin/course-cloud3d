# Docker 2
## Tipe Docker Network
### Bridge
Merupakan jenis network bawaan docker dan ketika docker berjalan akan melakukan konfigurasi virtual bridge yang disebut dengan docker0. Masing-masing container akan dialokasikan sebuah virtual Ethernet eth0. Interface ethh0 akan diberikan sebuah IP address dari range bridge. Docker akan mencari sebuah IP yang tersedia dan akan mengkonfigurasi eth0. Ketika container terhubung dengan internet, bridge akan otomatis meneruskan paket antar interface asalkan terhubung dan diizinkan untuk berkomunikasi dengan mesin host.
### Host
Network ini meletakkan container dalam stack host network. Semua interface dapat diakses melalui container. Menggunakan host network sama seperti jaringan aslinya sehingga dapat melakukan performa jaringan terbaik, bahkan akan lebih cepat daripada container yang menggunakan bridge. Container akan membagi network dari host yang langsung ke internet. Ketika menggunakan network ini, container akan dapat diakses melalui IP host. Network ini cenderung tidak aman karena langsung terekspos ke internet.
### None
Network ini bertujuan untuk tidak mengkonfigurasi networking.

## Expose dan Mapping port
Yaitu skenario yang umum digunakan ketika menginginkan container diakses dari luar docker. Sebuah image juga dapat melakukan expose port, yaitu container akan melakukan listen pada port yang diekspos. Contoh, aplikasi server Tomcat akan listen pada port 8080 maka nantinya semua container yang berjalan pada host yang sama akan berkomunikasi dengan Tomcat pada port 8080.

## Persistent Storage (Volume)
Bertujuan untuk menjaga data meskipun container dihapus. Persistent storage juga dapat berbagi data antar container atau host docker. Sebagai contoh container data transaksi ketika dihapus maka data tersbut akan tetap ada meskipun telah menghapus container.

## Docker Volume Driver
Terdapat jenis-jenis volume agar dapat terintegrasi dengan jenis penyimpanan lain.
- Docker volume driver for Azure file storage, yaitu driver untuk docker yang digunakan Azure.
- IPFS (InterPlanetary File System) yaitu plugin volume open source yang mengizinkan filesystem menjadi volume.
- Keywhiz, sistem ang digunakan untuk mengelola dan mendistribusikan data yang rahasia seperti TLS certificate, GPG keys, API tokens, dan database credentials.

## Docker Compose
Yaitu tool untuk mendefinisikan, launching, dan mengelola service, dimana service tesebut didefinisikan sebagai satu atau lebih docker container. Service dan sistem didefinisikan dalam file YAML. Hal yang dapat dilakukan docker compose adalah build docker image, menjalankan aplikasi sebagai service, menjalankan full system service, mengelola service, scaling up/down dan melihat log container.
