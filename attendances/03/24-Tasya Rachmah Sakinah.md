# Pertemuan 03

## Jenis-jenis Compute
- Oracle Cloud Infrastructure menawarkan 2 jenis instances yaitu bare metal dan virtual machine (VM):
- Bare Metal: merupakan instances komputasi bare metal yang memberi Anda akses ke server fisik khusus untuk kinerja tertinggi dan isolasi yang kuat.
- Virtual Machine: (VM) adalah lingkungan komputasi independen secara virtual yang berjalan di atas perangkat keras fisik bare metal. 

## Jenis-jenis Instance
1. Jenis shapes

    - Standard shapes
    - DenseIO shapes
    - GPU shapes
    - High performance computing (HPC) shapes
    - Optimized shapes

2. Flexible shapes
    - Flexible shapes
    - OCPU ekuivalen dengan satu core fisik dengan multithreading simultan (hyper-threading)
    - Ketika Anda membuat VM menggunakan flexible shape, pilihan jumlah OCPU dan volume memori yang dibutuhkan dapat disesuaikan.

## Jenis-jenis Kapasitas
- On-demand capacity : cukup bayar sesuai dengan kapasitas compute yang kita gunakan saja.
- Preemptible capacity : berguna saat membutuhkan sumber daya ketika beban kerja meningkat (autoscaling) pada periode waktu tertentu, sehingga lebih hemat biaya
- Reserved capacity : kapasitas cadangan yang berguna untuk masa yang akan datang sesuai dengan kebutuhan. 
- Dedicated capacity : menjalankan instance VM pada dedicated server, sehingga sumber daya tidak dibagi dengan client/customer lain.

## Komponen ketika membuat VM
- Availability domain
- Virtual cloud network
- Key pair (untuk Linux)
- Tags
- Password (untuk Windows)
- Image
- Shape
