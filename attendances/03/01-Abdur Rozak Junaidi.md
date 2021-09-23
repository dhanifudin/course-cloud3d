**IaaS (Compute)**

**Jenis-jenis Compute**
- Bare Metal: merupakan instances komputasi bare metal yang memberi Anda akses ke server fisik khusus untuk kinerja tertinggi dan isolasi yang kuat.
- Virtual Machine: (VM) adalah lingkungan komputasi independen secara virtual yang berjalan di atas perangkat keras fisik bare metal. Virtualisasi memungkinkan untuk menjalankan beberapa VM yang terisolasi satu sama lain. 

**Jenis-jenis Instance**
- Jenis shapes : OCI menawarkan berbagai variasi shapes. Shapes adalah sebuah templat yang menentukan kebutuhan jumlah CPU, volume memori, dan sumber daya lainnya yang dialokasikan untuk sebuah compute instance. 
	jenis-jenis shape
	1. Standard shapes
	2. DenseIO shapes
	3. GPU shapes
	4. High performance computing (HPC) shapes
	5. Optimized shapes
- Flexible shapes :sebuah templat yang dapat melakukan kustom sejumlah OCPU dan memori ketika melakukan launching atau mengubah VM.
	Jenis-jenis flexible shapes yang tersedia:
	1. VM.Standard.E3.Flex (AMD)
	2. VM.Standard.E4.Flex (AMD)
	3. VM.Optimized3.Flex (Intel)
	4. VM.Standard.A1.Flex (Arm processor dari Ampere)

**Jenis-jenis Kapasitas**
- On-demand capacity : cukup bayar sesuai dengan kapasitas compute yang kita gunakan saja.
- Preemptible capacity : berguna saat membutuhkan sumber daya ketika beban kerja meningkat (autoscaling) pada periode waktu tertentu, sehingga lebih hemat biaya.
- Reserved capacity : kapasitas cadangan yang berguna untuk masa yang akan datang sesuai dengan kebutuhan. Kapasitas cadangan yang tidak digunakan perhitungan biayanya berbeda dengan sumber daya yang sedang digunakan.
- Dedicated capacity : menjalankan instance VM pada dedicated server, sehingga sumber daya tidak dibagi dengan client/customer lain.

**Komponen ketika membuat VM**
- Availability domain
- Virtual cloud network
- Key pair (untuk Linux)
- Tags
- Password (untuk Windows)
- Image
- Shape
