Komponen-Komponen Networking :

    1.  Virtual Cloud Network (VCN)
    2.  Subnets
    3.  Virtual Network Interface Cards (VNIC)
    4.  Private IP
    5.  Public IP
    6.  IPV6
    7.  Dynamic Routing Gateway (DRG)
    8.  Internet Gateway
    9.  Network Address Translation (NAT) Gateway
    10. Service Gateway
    11. Local Peering Gateway (LPG)
    12. Remote Peering Connection (RPC)
    13. Route Tables
    14. Security Rules
    15. DHCP Optios

Port Web Server Umum yang biasa digunakan itu sebagai berikut :

    80 = HTTP
    443 = HTTPS
    22 = SSH

Langkah-langkah mengaktifkan Apache dan Mengaktifkan Port 80 :

    Buat VM Instance melalui Ubuntu
    Gunakan VM Instance dengan SSH, dengan memasukkan Public Username, Ip Address, dan SSH Private Key
    Lalu install Web Server (Apache)
    Cek Status Web Server dengan systemctl, jika belum aktif aktifkan dengan systemctl
    Lalu back ke Website OCI, bagian instance yang sudah dibuat, masuk ke halaman VCN dan tambahkan Ingress Rule baru dengan:
        Source Type: CIDR
        Source CIDR: 0.0.0.0/0
        IP Protocol: TCP
        Destination Port: 80(HTTP)
    Buka Port 80 di VM Instance via SSH dengan mengikuti cara disini
    Restart VM Instance-nya dan masuk kembali
    Akses Web server dengan perintah curl -I 127.0.0.1. Apabila ada response dari header HTML-nya, maka berhasil.
    Coba akses secara publik public port di VM Instance
