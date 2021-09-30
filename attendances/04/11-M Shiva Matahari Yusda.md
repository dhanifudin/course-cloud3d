# 04 - Virtual Cloud Network (VCN)

## Tujuan Pembelajaran

1. Mengetahui layanan _Oracle Cloud Infrastructure Networking_.

2. Mengaktifkan port 80 melalui Virtual Cloud Network (VCN) di layanan _Oracle Cloud_.

3. Mampu memasang _Apache Server_ dan mengkonfigurasi _IP tables Firewalls_.

## Jenis-jenis Port Web Server

- Port 22 -> merupakan port standar _Secure Shell_ atau sering disebut dengan SSH.

- Port 80 -> digunakan untuk konektivitas web _server_ secara umum dengan _client_.

- Port 433 -> memiliki fungsi keamanan yang lebih kuat sehingga _client_ merasa aman dalam mengakses berbagai konten web.

## Mengaktifkan _port_ 80.

- Membuat _Instance VM_ menggunakan _image Ubuntu_.

- Membuka _Virtual Cloud Network_.

- Menambahkan _port_ pada _Ingress Rules_.

## Menginstall Apache Server.

- Mengakses VM menggunakan SSH dengan menggunakan _private key_ dan _IP Address Public Instance_ VM.

- Menginstall _Apache Server_.

- Menjalankan _service Apache server_.

- Menambahkan _iptables_ untuk mengaktifkan _firewall_ pada VM _Ubuntu_.

- Menguji server VM dengan perintah _curl localhost_ atau membuka _browser_ dan arahkan ke _IP Public_ VM yang dimiliki. Jika berhasil, maka akan muncul halaman _Apache Server_.
