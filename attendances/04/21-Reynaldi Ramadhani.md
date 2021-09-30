## VIRTUAL CLOUD NETWORK
Dalam Pertemuan kali ini membahas bagaimana cara mengaktifkan port 90 melalui VCN dilayanan Oracle Cloud dan mampu memasang Apache Web Server dan konfigurasi IP Tables Firewalls

## Komponen Networking 
a. Virtual Cloud Network (VCN)
b. Subnets
c. VNIC
d. Private Ip
e. Public IP
f. IPV6
g. Dynamic Routing Gateway
h. Internet Gateway
i. NAT Gateway
j. Service Gateaway
k. LPG
l. RPC
m. Route Tables
n. Security Rules
o. DHCP Option

## Port Web Server
untuk port web server yang sering digunakan ada 3 yaitu HTTP (port 80) , HTTPS (port 443) , SSH (22)

## Langkah Mengaktifkan Port 80 melalui VCN 
1. Membuat VM terlebih dahulu seperti pertemuan minggu 3
2. lalu jika berhasil dibuat , buka VCN dengan cara klik nama 
3. Pilih Security List dan pada Ingress Rulse pilih Add Ingress Rules
4. lalu pastikan mengisi seperti dibawah ini
    - Stateless: Checked
    - Source Type: CIDR
    - Source CIDR: 0.0.0.0/0
    - IP Protocol: TCP
    - Source port range: (biarkan kosong)
    - Destination Port Range: 80
    - Description: Allow HTTP connections
5. Setelah itu akses VM melalui SSH dengan menggunakan private Key dan Host (Windows menggunakan Putty)
6. setelah itu lakukan perintah *sudo apt update* dan *sudo apt -y install*
7. lalu jalankan service Apache dengan menuliskan perintah *sudo systemctl restart apache2*
8. jika menggunakan ubuntu biasanya perlu mengaktifkan firewall yang status nya disabled dengan cara update iptabels dengan perintah *sudo iptables -I INPUT 6 -m state --state NEW -p tcp --dport 80 -j ACCEPT* dan *sudo netfilter-persistent save*
9. Lalu coba akses Server VM menggunakan perintah *curl localhost*
