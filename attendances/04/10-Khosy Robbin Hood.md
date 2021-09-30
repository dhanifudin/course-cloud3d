# Pertemuan 4

### VCN(Virtual cloud Network)
VCN adalah sistem yang memiliki perangkat, mesin virtual(VM), server, dan pusat data yang terhubung dan dikendalikan menggunakan teknologi dan perangkat lunak nirkabel. Dengan jaringan cloud virtual, organisasi dapat memperluas jaringan mereka sesuai keinginan, tanpa harus mengorbankan efisiensi dan fungsionalitas.

### SUBNET
Cara untuk memisahkan suatu jaringan fisik menjadi lebih dari satu sub-jaringan logis yang lebih kecil

### VNIC (Virtual Network Interface Cards)
cara instance terhubung agar koneksi ke vcn aktif.

### Jenis port : 
* 80(http) 
* 443(https) 
* 22(SSH)

### Komponen-komponen Networking :
* VIRTUAL CLOUD NETWORK (VCN)
* SUBNETS
* VNIC (Virtual Network Interface Cards)
* PRIVATE IP
* PUBLIC IP
* IPV6
* DYNAMIC ROUTING GATEWAY (DRG)
* INTERNET GATEWAY
* NETWORK ADDRESS TRANSLATION (NAT) GATEWAY
* SERVICE GATEWAY
* LOCAL PEERING GATEWAY (LPG)
* REMOTE PEERING CONNECTION (RPC)
* ROUTE TABLES
* SECURITY RULES
* DHCP OPTIONS

## Langkah-langkah Mengaktifkan Port 80 melalui VCN
1. Membuat VM terlebih dahulu.
2. Lalu jika berhasil , buka VCN dengan cara klik nama.
3. Pilih Security List yang tersedia lalu pilih, Klik Add Ingress Rules untuk menambahkan port.
4. Lalu pastikan mengisi seperti dibawah ini :
* Stateless: Checked
* Source Type: CIDR
* Source CIDR: 0.0.0.0/0
* IP Protocol: TCP
* Source port range: (biarkan kosong)
* Destination Port Range: 80
* Description: Allow HTTP connections
5. Terakhir, klik tombol Add Ingress Rules. Sekarang koneksi HTTP telah diizinkan. VCN Anda telah dikonfigurasi untuk Apache server 




