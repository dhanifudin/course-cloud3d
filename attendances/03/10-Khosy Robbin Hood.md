# Pertemuan 3
### Jenis-jenis compute 
Oracle Cloud Infrastructure menawarkan 2 jenis instances yaitu bare metal dan virtual machine (VM):
* merupakan instances komputasi yang memberi Anda akses ke server fisik dengan kinerja tinggi dan isolasi kuat.
* Virtual Machine: (VM) adalah lingkungan komputasi independen secara virtual yang berjalan di atas perangkat keras fisik bare metal. 
### Jenis-jenis Instance
1. OCI menawarkan berbagai variasi shapes. Shapes adalah sebuah templat yang menentukan kebutuhan jumlah CPU, volume memori, dan sumber daya lainnya Berikut ini jenis-jenis shape yang tersedia:
  * Standard shapes: Standard shapes menyediakan sumber daya yang seimbang pada core, memori, dan jaringan. Standard shapes tersedia dengan prosesor Intel, AMD, dan Arm-based.
  * DenseIO shapes: dirancang untuk basis data yang besar, seperti big data dan aplikasi-aplikasi yang membutuhkan performa storage yang tinggi. Shapes ini mendapat fitur NVMe berbasis SSD.
  * GPU shapes: dirancang untuk akselerasi pada hardware.
  * High performance computing (HPC) shapes: dirancang untuk komputasi performa tinggi yang membutuhkan frekuensi prosesor core yang tinggi.
  * Optimized shapes: dirancang untuk komputasi tingkat tinggi pada frekuensi core prosesor. Shape ini juga cocok untuk kebutuhan HPC dengan low latency.
2. Flexible shapes Flexible shapes adalah sebuah templat yang dapat melakukan kustom sejumlah OCPU dan memori ketika melakukan launching atau mengubah VM. Jenis-jenis flexible shapes yang tersedia:
  * VM.Standard.E3.Flex (AMD)
  * VM.Standard.E4.Flex (AMD)
  * VM.Optimized3.Flex (Intel)
  * VM.Standard.A1.Flex (Arm processor dari Ampere)
### Jenis-jenis kapasitas
Secara default kapasitas jenis on-demand sudah terpilih, tetapi juga memungkinkan memilih jenis kapasitas lainnya.
* On-demand capacity: cukup bayar sesuai dengan kapasitas compute yang kita gunakan saja.
* Preemptible capacity: berguna saat membutuhkan sumber daya ketika beban kerja meningkat (autoscaling) pada periode waktu tertentu, sehingga lebih hemat biaya.
* Reserved capacity: kapasitas cadangan yang berguna untuk masa yang akan datang sesuai dengan kebutuhan. Kapasitas cadangan yang tidak digunakan perhitungan biayanya berbeda dengan sumber daya yang sedang digunakan.
* Dedicated capacity: menjalankan instance VM pada dedicated server, sehingga sumber daya tidak dibagi dengan client/customer lain.
### Komponen membuat VM
* Availability domain
* Virtual cloud network
* Key pair (untuk Linux)
* Tags
* Password (untuk Windows)
* Image
* Shape
