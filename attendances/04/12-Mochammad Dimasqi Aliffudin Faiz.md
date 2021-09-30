# Virtual Cloud Network(VCN)
- Adalah jaringan pribadi virtual yang disiapkan di pusat data Oracle, sangat mirip dengan jaringan konvensional, dengan aturan firewall dan jenis gateway komunikasi tertentu yang dapat dipilih untuk digunakan.

## Goals Pembelajaran
- Mengetahui Layanan OCI Networking
- Mengaktifkan *port* 80 melalui VCN
- Mampu memasang Apache dan Web Server

## Langkah-langkah MwmAnf Apache dan Mengaktifkan Port 80 
- Buat VM Instance dengan **Ubuntu**
- Akses VM Instance dengan **SSH**, dengan memasukan **Public Username, Ip Address, dan SSH Private Key**
- Install Web Server (Apache)
- Cek Status Web Server dengan `systemctl`, apabila belum aktif, aktifkan dengan `systemctl` juga.
- Kembali ke Website OCI, bagian *instance* yang sudah dibuat, masuk ke halaman VCN dan tambahkan **Ingress Rule** baru dengan:
	- Source Type: CIDR
	- Source CIDR: 0.0.0.0/0
	- IP Protocol: TCP
	- Destination Port: 80(HTTP)
- Bukalah Port 80 di VM Instance via SSH dengan mengikuti cara [disini](https://www.cyberciti.biz/faq/how-to-open-firewall-port-on-ubuntu-linux-12-04-14-04-lts/)
- Restart VM Instance-nya dan masuk kembali
- Akses Web server dengan perintah `curl -I 127.0.0.1`. Apabila ada *response* dari *header* HTML-nya, maka berhasil.
- Coba akses secara publik *public port* di VM Instance

## Port Web Server Umum yang biasa digunakan
- 80 = HTTP
- 443 = HTTPS
- 22 = SSH
