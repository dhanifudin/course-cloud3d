<h1>Virtual Cloud Network</h1>

**Komponen-Komponen Networking**

1. Virtual Cloud Network (VCN)
2. Subnets
3. Virtual Network Interface Cards (VNIC)
4. Private IP
5. Public IP
6. IPV6
7. Dynamic Routing Gateway (DRG)
8. Internet Gateway
9. Network Address Translation (NAT) Gateway
10. Service Gateway
11. Local Peering Gateway (LPG)
12. Remote Peering Connection (RPC)
13. Route Tables
14. Security Rules
15. DHCP Optios

**Langkah Mengaktifkan Port 80 melalui VCN**
1. Membuat VM terlebih dahulu seperti pertemuan minggu 3.
2. Lalu jika berhasil dibuat, buka VCN dengan cara klik nama.
3. Pilih Security List dan pada Ingress Rulse pilih Add Ingress Rules.
4. Lalu pastikan mengisi seperti dibawah ini :
	- Stateless: Checked
	- Source Type: CIDR
	- Source CIDR: 0.0.0.0/0
	- IP Protocol: TCP
	- Source port range: (biarkan kosong)
	- Destination Port Range: 80
	- Description: Allow HTTP connections
5. Setelah itu akses VM melalui SSH dengan menggunakan private Key dan Host (Windows menggunakan Putty).
6. Setelah itu lakukan perintah sudo apt update dan sudo apt -y install.
7. Lalu jalankan service Apache dengan menuliskan perintah sudo systemctl restart apache2.
8. Jika menggunakan ubuntu biasanya perlu mengaktifkan firewall yang status nya disabled dengan cara update iptabels dengan perintah sudo iptables -I INPUT 6 -m state --state NEW -p tcp --dport 80 -j ACCEPT dan sudo netfilter-persistent save.
9. Coba akses secara publik public port di VM Instance.
