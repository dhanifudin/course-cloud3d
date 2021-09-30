# Virtual Cloud Network (VCN)
Virtual cloud network (VCN) (Indonesia : Jaringan pribadi virtual) yaitu jaringan yang disiapkan di
pusat data Oracle. VCN mirip dengan jaringan konvensional dan memiliki firewall dan gateway tertentu.
## Subnet
ubnet ditentukan dalam VCN (misal 10.0.0.0/24) dan diterapkan dalam VNIC (Virtual Network Interface Card)
yang dipasangkan ke dalam instance. 
## VNIC
VNIC digunakan untuk menghubungkan instance dan endpoints di dalam
dan di luar VCN dan VNIC tersebut tidak dapat dihapus.
## Private IPv4
Yaitu alamat IPv4 yang dimiliki oleh setiap instance untuk dapat terhubung ke jaringan dalam VNC. VNIC
memiliki alamat IP primer yang tidak dapat dihapus, tetapi dapat ditambahkan IP sekunder yang dinamis.
## Public IP
Alamat ini menghubungkan alamat IP Private dengan alamat IP internet.
## Dynamic Routing Gateway (DRG)
Router virtual (Opsional) yang dapat ditambahkan ke VCN. Router virtual ini digunakan untuk menghubungkan
jaringan pribadi antara VCN dan jaringan lokal. Ini juga dapat difungsikan untuk menghubungkan jaringan 
VCN anda dan VCN di wilayah lain yang berbeda.
## Service Gateway
Router virtual (Opsional) yang dapat ditambahkan ke VCN. Berfungsi untuk menghubungkan instance dengan
database dalam layanan oracle tanpa melewati jaringan internet.
## Local Peering Gateway (LPG)
Router virtual (Opsional) yang dapat ditambahkan ke VCN. Berfungsi untuk menghubungkan satu VCN dengan VCN
lain di wilayah yang sama tanpa melewati jaringan internet.
## Remote Peering Connection (RPC)
Komponen yang dapat Anda tambahkan ke DRG. Ini memungkinkan mengaitkan satu VCN dengan VCN lain di wilayah
yang berbeda.
## Virtual route tables.
Oracle memiliki tabel aturan yang digunakan untuk merutekan lalu lintas dari subnetke tujuan di luar 
VCN melalui gateway atau instance yang dikonfigurasi secara khusus. VCN dilengkapi dengan tabel rute default
yang kosong dan dapat ditambah dengan aturan rute sendiri.
## Security Rules
Aturan firelwall yang digunakan untuk mengatur lalu lintas keluar masuk berdasarkan komponen-komponen jaringan.
Misalkan mengatur untuk aturan ingress dari SSH bersumber dari mana dan port apa yang digunakan.
## DHCP Options
Informasi konfigurasi IP yang akan diberikan secara otomatis ke instance saat dilakukan booting.
