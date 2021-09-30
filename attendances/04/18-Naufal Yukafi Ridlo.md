# 04 - Virtual Cloud Network(VCN)
VCN adalah jaringan pribadi virtual yang disiapkan di pusat data Oracle, dengan aturan firewall dan jenis gateway komunikasi tertentu yang dapat dipilih untuk digunakan.

## Komponen jaringan
Layanan jaringan menggunakan versi virtual komponen dari jaringan konvensional yaitu sebagai berikut:

<ol>
  <li>Subnets</li>
  <li>VNIC (Virtual Network Interface Cards)</li>
  <li>Private IP</li>
  <li>Public IP</li>
  <li>IPv6</li>
  <li>Dynamic Routing Gateway (DRG)</li>
  <li>Internet Gateway</li>
  <li>Network Address Translation (NAT) Gateway</li>
  <li>Service Gateway</li>
  <li>Local Peering Gateway (LPG)</li>
  <li>Remote Peering Connection (RPC)</li>
  <li>Route Tables</li>
  <li>Security Rules</li>
  <li>DHCP Options</li>
</ol>

## Apache di Virtual Machine dan Mengaktifkan Port 80
Untuk melakukan setup apache di vm pastikan sudah membuat VM instance menggunakan image ubuntu.
<ol>
  <li>Akses virtual machine instance melalui SSH</li>
  <li>Instal web server(Apache) kemudian melakukan cek status web server</li>
  <li>Menambahkan port pada Ingress Rules</li>
  <li>Membuka Port 80 di VM Instance dengan menggunakan SSH</li>
  <li>Uji akses server Virtual Machine dengan perintah "curl http://(ip public)"</li>
</ol>

## Port Yang Sering Digunakan
<ul>
  <li><b>Port 80</b> digunakan untuk konektivitas web server dan merupakan port default untuk koneksi HTTP</li>
  <li><b>Port 22</b> merupakan port Standard Secure Shell(SSH)</li>
  <li><b>Port 433</b> port default dari koneksi dengan protokol HTTPS</l>
</ul>
