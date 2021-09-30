# Pertemuan 04

## Layanan Networking
Komponen - komponen Networking
- VIRTUAL CLOUD NETWORK (VCN)
- SUBNETS
- VNIC (Virtual Network Interface Cards)
- PRIVATE IP
- PUBLIC IP
- IPV6
- DYNAMIC ROUTING GATEWAY (DRG)
- INTERNET GATEWAY
- NETWORK ADDRESS TRANSLATION (NAT) GATEWAY
- SERVICE GATEWAY
- LOCAL PEERING GATEWAY (LPG)
- REMOTE PEERING CONNECTION (RPC)
- ROUTE TABLES
- SECURITY RULES
- DHCP OPTIONS

## VIRTUAL CLOUD NETWORK (VCN)
VCN berada di satu region Oracle Cloud Infrastructure dan mencakup satu atau beberapa blok CIDR (IPv4 dan IPv6, jika diaktifkan) 

## SUBNETS
Subdivisi yang ditentukan dalam VCN (misalnya, 10.0.0.0/24, 10.0.1.0/24, atau 2001:DB8::/64). Subnet berisi Virtual Network Interface Cards (VNIC), yang ditautkan ke dalam instance.

## VNIC (Virtual Network Interface Cards)
VNIC melekat pada sebuah instance dan berada di subnet untuk mengaktifkan koneksi ke VCN subnet. VNIC menentukan bagaimana instances terhubung dengan endpoints di dalam dan di luar VCN.

## PRIVATE IP
Alamat IPv4 pribadi dan informasi terkait untuk menangani instance (misalnya, nama host untuk DNS). Setiap VNIC memiliki IP pribadi primer, dan Anda dapat menambah dan menghapus IP pribadi sekunder. 

## PUBLIC IP
Alamat IPv4 publik dan informasi terkait. Anda dapat secara opsional menetapkan IP publik ke instances Anda atau sumber daya lain yang memiliki IP pribadi. 

## DYNAMIC ROUTING GATEWAY (DRG)
Router virtual (opsional) yang dapat Anda tambahkan ke VCN Anda. Ini menyediakan jalur lalu lintas jaringan pribadi antara VCN Anda dan jaringan lokal.

## Service Gateway
Router virtual (opsional) yang dapat Anda tambahkan ke VCN Anda. Ini menyediakan jalur untuk lalu lintas jaringan pribadi antara VCN Anda dan layanan yang didukung di Oracle Services Network (contoh: Oracle Cloud Infrastructure Object Storage dan Autonomous Database). 

## LOCAL PEERING GATEWAY (LPG)
Router virtual (opsional) yang dapat Anda tambahkan ke VCN Anda. Ini memungkinkan mengaitkan satu VCN dengan VCN lain di wilayah yang sama. 

## REMOTE PEERING CONNECTION (RPC)
Komponen yang dapat Anda tambahkan ke DRG. Ini memungkinkan mengaitkan satu VCN dengan VCN lain di wilayah yang berbeda.

## ROUTE TABLES
Virtual route tables untuk VCN Anda. Mereka memiliki aturan untuk merutekan lalu lintas dari subnet ke tujuan di luar VCN melalui gateway atau instance yang dikonfigurasi secara khusus.

## SECURITY RULES
Aturan firewall virtual untuk VCN Anda. Ini untuk aturan masuk dan keluar yang menentukan jenis lalu lintas (protokol dan port) yang diizinkan masuk dan keluar dari instance

## DHCP OPTIONS
Informasi konfigurasi yang secara otomatis diberikan ke instances saat dilakukan booting.