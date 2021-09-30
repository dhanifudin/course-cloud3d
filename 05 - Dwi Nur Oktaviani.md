# Pertemuan 04
VCN adalajh jaringan cloud virtual yang di OCI yang memungkinkan instance untuk berkomunikasi seolah-olah beroperasi pada jaringan konvensional. VCN mencakup komponen seperti subnet public dan private, table route, internet gateways, DNS support, Security List, dsb. Pembuatan instance harus dikaitkan dengan subnet, jadi VCN dibuat menyediakan layanan jaringan ke instance. Dikonfigurasi setidaknya satu subnet sehingga instance memiliki sumber daya jaringan untuk digunakan saat launch. Membuat VCN dapat dilakukan secara manual dan dengan wizard. Dimulai dengan membuat VCN. Mulai dari konsol OCI, navigasikan melalui menu utama, ke Networking dan kemudian ke Virtual Cloud Networks. Klik create VCN untuk memunculkan dialog konfigurasi VCN. Setelah pembuatan selesai akan didapat kompartemen, rentang blok CIDR, nama domain yang dihasilkan, dan OCID yang unik. Beberapa sumber daya nomor 1 dalam tanda kurung di samping nama, yang menunjukkan sumber day aini sibuat secara otomatis Ketika VCN dibangun. Kita melihat block CIDR, Tabel Route, Security List, dan Opsi DHCP telah ditetapkan atau dibuat. VCN secara otomatis akan mendapat route table default, security list, dan pengaturan opsi DHCP tapi tidak termasuk subnet default.
Security list, kita melihat ada 3 Ingress Rules., yaitu ada aturan untuk port 22, yang akan mendukung koneksi SSH ke instance yang dilampirkan ke subnet VCN ini. Ada juga 2 aturan tambahan yang mendukung ICMP untuk komunikasi internal. Mengklik Egress Rules, dapat dilihat ada 1 aturan yang mendukung semua lalu lintas keluar untuk semua protocol di semua port. Pada table route table tidak ada rule sampai dibuat untuk tujuan khusus. Blok CIDR berfungsi untuk penetapan alamat IP. 










