Oracle cloud Infrastruktur digunakan untuk mengelola host komputasi atau bisa disebut instance , terdapat 2 jenis yaitu instance yaitu bare metal dan VM 
    -Bare metal digunakan untuk memberi akses ke server fisik khusus untuk kinerja tertinggi dan isolasi yang kuat
    - VM berjalan di atas perangkat keras fisik bare metal. Ideal untuk menjalankan 
    aplikasi yang tidak memerlukan kinerja dan sumber daya. 

lalu OCI sendiri ada berbagai variasi shape , sebuah tempat yang menentukan kebutuhan jumlah cpu , volume memori dan sumber daya lainya.
ada beberapa jenis shape yaitu :
    1.Standart Shape
    2.DenseIO shapes
    3.GPU shapes
    4.High Performance Computing (HPC)
    5.Optimized Shapes

Cara membuat VM pada oracle
1.pada bar sebelah kiri pilih compute
2.lalu pilih instance 
3.setelah itu create instance , beri nama untuk VM nya yag sesuai
4.memilih image dan shape yang dibutuhkan
5. menyimpan private key(wajib) dan public key(optional)
6.gunakan putty untuk mengkoneksikan vm (windows) atau ssh pada terminal UNIX 
7. Masukan Ip Address dan Username yang terdapat di VM yang sudah dibuat pada Website
8.Melakukan instalasi software yang diperlukan 