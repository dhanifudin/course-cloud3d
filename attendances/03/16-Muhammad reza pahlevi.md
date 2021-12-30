# Cloud computing
## IaaS(Compute)
### Poin penting
- Mengetahui layanan Oracle Cloud Infrastructure Compute
- Mampu membuat Virtual Machine (VM) di layanan compute Oracle Cloud
### Jenis-jenis Compute
- Bare Metal : Meripakan instaces komputasi yang memberikan akses ke server fisik khusus untuk kinerja tertinggi
- Virtual Machine (VM) : Lingkungan independen virtual yang berjalan secara virtual diatas perangkat keras bare metal
### Jenis-jenis instance
#### Shape 
Jenis ini merupakan sebat template yang menentukan kebutuhan jumlah CPU,memoru, dan sumber data yang dialokasikan untuk sebuah compute instace
- Standart Shapes : dirancang untuk kebutuhan umum yang banyak digunakan pada aplikasi-aplikasi dan use cases pada umumnya
- DenseIO shapes: dirancang untuk basis data yang besar, seperti big data dan aplikasi-aplikasi yang membutuhkan performa storage yang tinggi
- DenseIO shapes: dirancang untuk basis data yang besar, seperti big data dan aplikasi-aplikasi yang membutuhkan performa storage yang tinggi
- High performance computing (HPC) shapes: dirancang untuk komputasi performa tinggi yang membutuhkan frekuensi prosesor core yang tinggi dan HPC dalam klaster jaringan yang diakses secara paralel.
- Optimized shapes: dirancang untuk komputasi tingkat tinggi pada frekuensi core prosesor. Shape ini juga cocok untuk kebutuhan HPC dengan low latency. Shape ini juga mendukung cluster networking.
#### Flexible Shapes
- Flexible shapes adalah sebuah templat yang dapat melakukan kustom sejumlah OCPU dan memori ketika melakukan launching atau mengubah VM.
- OCPU ekuivalen dengan satu core fisik dengan multithreading simultan (hyper-threading), di mana setiap OCPU merujuk pada dua hardware yang mengeksekusi threads (juga dikenal sebagai virtual CPUs atau vCPUs).
- Ketika Anda membuat VM menggunakan flexible shape, pilihan jumlah OCPU dan volume memori yang dibutuhkan dapat disesuaikan.
