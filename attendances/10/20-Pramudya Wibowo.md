# Docker
Docker adalah sebuah command-line program, sebuah background daemon dan serangkaian remote service dengan mengambil pendekatan logistic untuk memecahkan permasalahan umum perangkat lunak dan menyederhanakan pengalaman kita dalam installing, running, publishing, dan menghapus perangkat lunak.

## Latar Belakang
Mengemas aplikasi dengan semua dependensi yang dibutuhkannya, docker membungkus semuanya menjadi sistem file lengkap serta yang menjalankan mesin virtual itu sendiri. Proses packaging tersebut menjamin bahwa itu portable dan tidak memperdulikan environtment deployment yang digunakan.

## Sejarah
Project internal oleh dotCloud yang merupakan penyedia PaaS hingga pada tahun 2013 menjadi sebuah project open source. Dalam menyediakan PaaS mereka membutuhkan lebih banyak virtual machine serta untuk meningkatkan waktu start up, digunakan container dan docker. Peluncuran pertama pada bulan Juni 2014 dan dotCloud berkolaborasi dengan RedHat serta Amazon untuk menambahkan layanan sehingga dapat menggunakan Docker untuk mengelola infrastruktur.

## Containerization
- Docker menggunakan container linux atauan Linux Container yang biasa disebut LXC.
- Memanfaatkan fungsi cgroups.
- Linux container merupakan virtualisasi untuk menjalankan beberapa sistem linux.

## Virtual vs Container
- Docker adalah sebuah container management system yang lebih mudah dan universal.
- Memungkinkan membuat container pada Mac/Windows dan mengoperasikannya.
- Perintah yang dilakukan di local akan sama seperti saat deployment.
- Setiap membuat container, tidak perlu OS penuh.
- Mengandalkan penggunaan kernel Linux.
- Menghasilkan ukuran image kecil, compact, dan ringan untuk didistribusikan.

## Keuntungan Container
- Portability
- Quick deployment / teardown
- Managing infrastructure-like code
- Open Source
- Consistency

## Dockerfile
Docker dapat membuat sebuah image secara automatis dengan membaca perintah dari Dockerfile. Dockerfile adalah sebuah teks dokumen yang berisi semua perintah yang dapat dipanggil pengguna pada command line untuk membuat sebuah image. Dengan menggunakan Dockerfile kita tidak perlu mengetik perintah satu persatu ketika akan membuat image.
