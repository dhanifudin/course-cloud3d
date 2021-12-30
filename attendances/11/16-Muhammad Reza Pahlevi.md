# Cloud computing
## Docker 2
### Poin Penting
- Mahasiswa dapat mengetahui secara jelas network di Docker
- Mahasiswa mengetahui konsep volume pada Docker
- Mahasiswa mampu memanfaatkan dan menggunakan volume ataupun network ketika build image docker.
- Mahasiswa bisa menggunakan docker compose dalam pembuatan aplikasi.
### Tipe Docker Network
#### Bridge
- Merupakan jenis network bawaan dari Docker
- Ketika Docker service daemon berjalan, akan melakukan konfigurasi sebuah virtual bridge disebut dengan docker0.
- Jika kita tidak menyebutkan spesifik network yang digunakan, docker run –net=<Network> makaa Docker daemon akan terhubung ke container menggunakan bridge network.
- Masing-masing container yang dibuat, akan dialokasikan sebuah perangkat virtual Ethernet dan dipetakkan sebagai eth0 pada container.
#### Host
- Docker network jenis ini yaitu meletakkan container di dalam stack hostnya network.
- Semua antarmuka jaringan yang telah didefinisikan dapat diakses melalui container.
- Ketika kita menjalankan container menggunakan parameter –net=host, sehingga container akan menggunakan network host.
- Ketika menggunakan host network akan secepat jaringan normal karena tidak ada menggunakan bridge ataupun translation
#### none
- Network None bertujuan untuk tidak mengkonfigurasi networking.
- Tidak ada driver yang digunakan pada Network jenis ini.
- Ketika kita tidak menginginkan container untuk dapat diakses. Perintah yang digunakan dengan menambahkan parameter –net=none
