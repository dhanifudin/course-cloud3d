# Rangkuman Pertemuan 11
# Docker 2
Dockerfile untuk setting kebutuhan aplikasi yang akan ditaruh di container
Docker.yml untuk kebutuhan component atau config dari project dan juga kebutuhan service dari aplikasi.
# Docker Network
1. Bridge 
* Merupakan jenis network bawaan dari Docker.
* Jika kita tidak menyebutkan spesifik network yang digunakan, docker run –net=Network maka Docker daemon akan terhubung ke container menggunakan bridge network.
* Masing-masing container yang dibuat, akan dialokasikan sebuah perangkat virtual Ethernet dan dipetakkan sebagai eth0 pada container
2. Host
* Docker network jenis ini yaitu meletakkan container di dalam stack hostnya network. 
* Semua antarmuka jaringan yang telah didefinisikan dapat diakses melalui container.
* Ketika kita menjalankan container menggunakan parameter –net=host, sehingga container akanmenggunakan network host.
* Ketika menggunakan host network akan secepat jaringan normal karena tidak ada menggunakan bridge ataupun translation. 
* Container yang berjalan di dalam stack hostnya network akan mendapatkan jauh lebih cepat dibandingkan container yang berjalan menggunakan network bridge, tidak membutuhkan traverse pada docker0 bridge dan mappings port iptables.
* Container membagi networknya dari host yang langsung ter-expose ke dunia luar.
* Ketika menggunakan perintah –net=host, container kita akan dapat diakses melalui hostnya IP address.
* Kita butuh berhati-hati ketika menggunkaan network host karena berbahaya.
3. None
* Network None bertujuan untuk tidak mengkonfigurasi networking.
* Tidak ada driver yang digunakan pada Network jenis ini.
* Ketika kita tidak menginginkan container untuk dapat diakses. Perintah yang digunakan dengan menambahkan parameter –net=none
# Expose dan mapping port
* Skenario yang umum digunakan ketika kita menginginkan container menerima koneksi yang datang, salah satunya dari container yang lain atau dari luar docker.
* Expose port adalah container aplikasi kita akan listen pada port yang ter-expose. Sebagai contoh, aplikasi server Tomcat akan listen pada port default yaitu 8080.
* Expose port dapat dilakukan menggunakan 2 cara yaitu salah satunya adalah menggunakan Dockerfile dengan perintah EXPOSE dan menggunakan perintah docker run –expose.
* Ketika container berbeda host atau network agar tetap bisa berkomunikasi menggunakan maping port.
* Mapping port dilakuan dengan menambahkan parameter –p ketika menjalankan container.
# Persistent Storage (Volume)
* Persistent storage pada docker bertujuan agar data pada container tetap terjaga walaupun container telah dihapus
* Persitence storage juga dapat berbagi data antara container yang lain ataupun dengan host docker.
# Docker Compose
Docker compose adalah sebuah tool untuk mendefiniskan, launching, dan mengelola service,
dimana sebuah service adalah didefinisikan sebagai satu atau lebih dari sebuah docker
container.
Beberapa hal yang bisa dilakukan menggunakan docker compose adalah:
* Build docker image
* Menjalankan aplikasi container sebagai service
* Menjalankan full system dari service
* Mengelola secara individu service pada sebuah sistem
* Melakukan scaling up atau down
* Melihat log dari kumpulan container yang berjalan sebagai service

