# Rangkuman Pertemuan 10
# Docker
Docker adalah aplikasi untuk menyatukan berbagai file software dan pendukungnya dalam 
sebuah wadah (container) agar memudahkan proses pengembangan software.Dalam pengembangan 
aplikasi, developer memerlukan virtualisasi di server agar aplikasi bisa berjalan di 
berbagai platform dengan konfigurasi hardware yang berbeda-beda.
Ketika menggunakan virtualisasi, Anda harus menyiapkan satu sistem operasi secara penuh. 
Jika membutuhkan beberapa virtualisasi, server perlu resource yang besar. Nah, container
bisa digunakan sebagai alternatif virtualisasi sehingga tidak perlu menyiapkan sistem 
operasi secara penuh. Dengan container, ukuran file menjadi lebih kecil dibandingkan 
virtualisasi yang biasa digunakan.

# Arsitektur Docker
1. Docker image — Kumpulan file yang menunjang sebuah aplikasi.
2. Docker container — Wadah untuk mengemas dan menjalankan aplikasi. Wadah ini mencakup
kode, runtime, system tools, dan pengaturan. Container hanya bisa mengakses resource
yang telah ditentukan dalam Docker image.
3. Docker client — Tempat di mana pengguna dapat mengirimkan perintah seperti Docker 
build, Docker pull, dan Docker run kepada Docker daemon.
4. Docker Engine Rest API — Komponen yang digunakan untuk berinteraksi dengan Docker 
daemon. Komponen ini bisa diakses klien melalui HTTP.
5. Docker daemon — Proses pengelolaan Docker images, container, network, dan storage 
volumes. Docker daemon menerima request dari Docker API dan akan memprosesnya.
6. Docker host — Komponen yang menyediakan lingkungan untuk menjalankan aplikasi. Docker 
host bertanggung jawab menerima perintah yang diberikan Docker client.
7. Docker registry — Wadah untuk menyimpan Docker image. Docker image akan memberi 
reaksi sesuai perintah yang diberikan. Misalnya, saat diberi perintah docker push, 
docker image akan didorong atau dibagikan ke registry Docker Hub.
8. Docker Hub — Layanan yang disediakan untuk menemukan dan berbagi Docker image.

Docker build -> Images
Docker pull -> Registri
Docker run -> Images->registri->container

# Virtualisasi Vs Containerization
Virtualisasi memungkinkan Anda untuk menjalankan beberapa sistem operasi pada perangkat 
keras dari satu server fisik, sedangkan containerization memungkinkan Anda untuk 
menyebarkan beberapa aplikasi menggunakan sistem operasi yang sama pada satu mesin 
virtual atau server.

# Keuntungan Docker
Sistem kontainer berbasis open source, mudah dibuat dan mendistribusikan images, dapat 
menjalankan images yang sama di setiap kontainer yang telah dibuat, dan pemanfaatan 
sumber daya yang lebih baik.