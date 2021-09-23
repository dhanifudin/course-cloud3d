# Compute Engine pada OCI
Oracle Cloud Infrastructure menawarkan 2 jenis *instances* yaitu bare metal dan *virtual machine* (VM):
- Bare Metal: merupakan *instances* komputasi bare metal yang memberi Anda akses ke server fisik khusus untuk kinerja tertinggi dan isolasi yang kuat.
- Virtual Machine(VM): VM) adalah lingkungan komputasi independen secara virtual yang berjalan di atas perangkat keras fisik bare metal. Virtualisasi memungkinkan untuk menjalankan beberapa VM yang terisolasi satu sama lain. VM ideal untuk menjalankan
## Langkah Membuat VM di OCI
- Membuka halaman **instances** di website OCI
- Membuat nama *instance* VM harus deskriptif dan menjelaskan apa yang dikerjakan
- Memilih *Image & Shape* disesuaikan dengan kebutuhan dan ketersediaan aplikasi yang ingin digunakan
- Menyimpan *private key* SSH dengan baik untuk *login* ke dalam VM nantinya.
- Koneksikan VM dengan SSH(Via Putty di Windows, atau `ssh` command di UNIX) dengan memasukan *ip address* dan username yang tersedia pada *instance* VM di *website* OCI
- Pastikan *private key's permission* hanya bisa diakses oleh 1 *user* saja.
- Untuk membuat permission tersebut, pada UNIX bisa menggunakan `chmod 600 /file_key`
- Melakukan instalasi salah satu *package* setelah berhasil masuk ke VM, misal NGINX dan mengaktifkannya menggunakan perintah `systemctl`.
