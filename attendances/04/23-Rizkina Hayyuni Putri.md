# VIRTUAL CLOUD NETWORK (VCN)
VCN memiliki aturan tentang firewall dan gateway komunikasi. Jadi dengan adanya VCN memungkinkan untuk mengatur jaringan cloud, seperti IP, Subnet, Routing dan Firewall.

# Hal yang perlu dipelajari dalam Networking VCN
1. Subnets
2. VNIC (Virtual Network Interface Cards)
3. Private IP
4. Public IP
5. IPv6
6. Dynamic Routing Gateway (DRG)
7. Internet Gateway
8. Network Address Translation (NAT) Gateway
9. Service Gateway
10. Local Peering Gateway (LPG)
11. Remote Peering Connection (RPC)
12. Route Tables
13. Security Rules
14. DHCP Options



# Proses Praktikum Secara Garis Besar
## Mengaktifkan port 80 melalui VCN
1. Pastikan sudah memiliki VM di oracle cloud
2. Buka VCN dari VM
3. Menambahkan "Ingress Rules" di Security. Dengan settingan bahwa semua IP(0.0.0.0/0) dapat mengakses, IP Protocol adalah TCP karena HTTP termasuk dalam TCP, dan Destination port adalah 80 yaitu port dari HTTP.

## Setup Apache di VM
1. Akses VM melalui SSH
2. Install apache
3. Restart service apache
4. Pastikan firewall aktif
5. Uji akses server VM dengan perintah "curl http://(ip public)"

# Jenis Port yang Umum Digunakan secara Public
1. HTTP = Port 80(TCP)
2. HTTPS = Port 443(TCP)
3. SSH = Port 22(TCP)
