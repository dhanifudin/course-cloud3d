# PERTEMUAN 3
## Jenis-jenis Komputasi
Oracle Cloud Infrastructure menawarkan 2 jenis instances yaitu bare metal dan virtual machine (VM).
- Bare Metal: memberi akses ke server fisik khusus untuk kinerja tertinggi dan isolasi yang kuat.
- Virtual Machine: (VM) yang berjalan di atas perangkat keras fisik bare metal. Ideal untuk menjalankan 
aplikasi yang tidak memerlukan kinerja dan sumber daya.

## Jenis-jenis Instance
Ketika membuat sebuah compute instance, kita dapat memilih jenis instance yang sesuai kebutuhan berdasarkan 
karakteristik sumber daya misalnya jumlah core CPU yang dibutuhkan, jumlah memori, dan sumber daya jaringan.

## Jenis shapes
OCI menawarkan berbagai variasi shapes. Shapes adalah sebuah templat yang menentukan kebutuhan jumlah CPU, 
volume memori, dan sumber daya lainnya yang dialokasikan untuk sebuah compute instance. Berikut ini 
jenis-jenis shape yang tersedia:
• Standard shapes
dirancang untuk kebutuhan umum yang digunakan pada aplikasi-aplikasi dan use case.
• DenseIO shapes
digunakan untuk basis data yang besar seperti big data dan yang lain sekiranya membutuhkan perform storage tinggi
• GPU shapes
dirancang untuk akselerasi pada hardware terutama kebutuhan GPU termasuk Inter, AMD CPU dan prosesor grafis NVIDIA.
• High performance computing (HPC) shapes
dirancang untuk komputasi performa tinggi yang membutuhkan frekuensi prosesor core yang tinggi dan HPC dalam klaster jaringan yang diakses secara paralel.
• Optimized shapes
dirancang untuk komputasi tingkat tinggi pada frekuensi core prosesor. Shape ini juga cocok untuk kebutuhan HPC dengan low latency. Shape ini juga mendukung cluster networking.

## Flexible shapes
Flexible shapes adalah sebuah templat yang dapat melakukan kustom sejumlah OCPU dan memori ketika melakukan 
launching atau mengubah VM.

## Flexible shapes
Jenis-jenis flexible shapes yang tersedia:
VM.Standard.E3.Flex (AMD)
VM.Standard.E4.Flex (AMD)
VM.Optimized3.Flex (Intel)
VM.Standard.A1.Flex (Arm processor dari Ampere)

Kita dapat memilih kapasitas tiap jenis host yang digunakan untuk VM. Secara default kapasitas jenis on-demand sudah terpilih, 
tetapi juga memungkinkan memilih jenis kapasitas lainnya.
