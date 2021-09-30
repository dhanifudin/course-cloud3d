# Rangkuman Pertemuan Minggu 4

- Jaringan pribadi virtual yang disiapkan di pusat data Oracle. 
  Ini sangat mirip dengan jaringan konvensional, dengan aturan firewall dan 
  jenis gateway komunikasi tertentu yang dapat dipilih untuk digunakan. 
  VCN berada di satu region Oracle Cloud Infrastructure dan mencakup satu 
  atau beberapa blok CIDR (IPv4 dan IPv6, jika diaktifkan) 

- Subdivisi yang ditentukan dalam VCN (misalnya, 10.0.0.0/24, 10.0.1.0/24, atau 2001:DB8::/64). 
  Subnet berisi Virtual Network Interface Cards (VNIC), yang ditautkan ke dalam instance. 
  Setiap subnet terdiri dari rentang alamat IP yang berdekatan (untuk IPv4 dan IPv6, jika diaktifkan) 
  yang tidak tumpang tindih dengan subnet lain dalam VCN.

- Aturan firewall virtual untuk VCN Anda. Anda dapat memilih apakah aturan yang diberikan 
  bersifat stateful atau stateless. Untuk menerapkan aturan keamanan, 
  Anda dapat menggunakan grup keamanan jaringan atau daftar keamanan.
  
- Router virtual (opsional) yang dapat Anda tambahkan ke VCN Anda. Ini menyediakan jalur untuk lalu lintas jaringan pribadi 
  antara VCN Anda dan layanan yang didukung di Oracle Services Network (contoh: Oracle Cloud Infrastructure Object Storage 
  dan Autonomous Database). Misalnya, Sistem DB di subnet pribadi di VCN Anda dapat mencadangkan 
  data ke Object Storage tanpa memerlukan alamat IP publik atau akses ke internet.

- Router virtual (opsional) yang dapat Anda tambahkan ke VCN Anda. 
  Ini menyediakan jalur lalu lintas jaringan pribadi antara VCN Anda dan jaringan lokal.
  Anda dapat menggunakannya dengan komponen Jaringan lain dan router di jaringan 
  lokal Anda untuk membuat koneksi melalui Site-to-Site VPN atau OCI FastConnect. 
  Ini juga dapat menyediakan jalur lalu lintas jaringan pribadi antara VCN Anda dan VCN lain di wilayah yang berbeda.
