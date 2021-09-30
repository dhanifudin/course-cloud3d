Pertemuan 4 - VCN

Komponen-komponen dalam Networking :
1. VIRTUAL CLOUD NETWORK (VCN)
2. SUBNETS
3. VNIC (Virtual Network Interface Cards)
4. PRIVATE IP
5. PUBLIC IP
6. IPV6
7. DYNAMIC ROUTING GATEWAY (DRG)
8. INTERNET GATEWAY
9. NETWORK ADDRESS TRANSLATION (NAT) GATEWAY
10. SERVICE GATEWAY
11. LOCAL PEERING GATEWAY (LPG)
12. REMOTE PEERING CONNECTION (RPC)
13. ROUTE TABLES
14. SECURITY RULES
15. DHCP OPTIONS

- VCN atau Virtual Cloud Network merupakan jaringan pribadi virtual pada Oracle. 
Mirip dengan jaringan konvensional yang didalamnya itu terdapat aturan firewall juga jenis gateway tertentu yang dapat dipilih untuk nantinya digunakan. 
- Subnet, berisi Virtual Network Interface Cards yang ditautkan ke dalam instance. Yang mana pada tiap-tiap subnet terdiri dari rentang alamat IP yang berdekatan (untuk IPv4 dan IPv6, jika diaktifkan) yang tidak tumpang tindih dengan subnet lain dalam VCN.
- VNIC atau Virtual Network Interface Cards berhubungan dengan instance yang berada pada subnet berguna untuk mengaktifkan koneksi ke VCN subnet.
- Private IP, Alamat IPv4 pribadi dan informasi terkait untuk menangani instance (misalnya, nama host untuk DNS).
- Public IP,  Alamat IPv4 publik dan informasi terkait, bersifat sementara atau dilindungi oleh undang-undang.
- DRG, merupakan router virtual yang menyediakan lalu lintas jaringan pribadi VCN dengan jaringan lokal.
- Services Gateway, menyediakan jalur lalu lintas VCN dengan layanan Oracle Services Network.
- LPG, router opsional yang memungkinkan mengaitkan VCN satu dengan lainnya pada wilayah yang sama (contoh peering yakni menggunakan alamat IP pribadi sehingga tanpa lalu lintas internet / hanya melalui jaringan lokal di cloud).
- RPC, dapat ditambahkan ke DRG dimana memungkinkan VCN satu dengan yang lain di wilayah yang berbeda.
- Route Tables, virtual route yang berhubungan dengan aturan rute lalu lintas subnet ke tujuan melalui gateway.
- Security Rules, merupakan aturan firewall virtual untuk VCN (menentukan protocol dan port).
- DHCP Options, informasi konfigurasi otomatis saat melakukan booting instances.

Port yang umum digunakan :
port 22 -> SSH
port 80 -> http
port 443 -> https

Komponen pyshical network juga dapat diaplikasikan pada cloud.
