# Komputasi Awan dan Sistem Terdistribusi
## Layanan Oracle Cloud
Terdapat 2 jenis instance pada Oracle Cloud :
* **Bare Metal**, merupakan instances komputasi yang berjalan secara fisik sehingga kinerjanya lebih tinggi.
* **Virtual Machine (VM)**, merupakan instance yang bekerja secara virtual yang memungkinkan beberapa komputer
dalam satu sumber daya bekerja secara bersamaan.

## Jenis Instance
### Shapes
Yaitu sebuah templat yang telah ditentukan spesifikasi untuk instance yang akan dibuat, antara lain :
* Standard shapes : dirancang untuk kebutuh umum yang standar dan menyediakan spesifikasi yang optimal untuk aplikasi
yang sering digunakan.
* DenseIO shapes : dirancang untuk basis data yang besar, seperti big data dan aplikasi yang membutuhkan performa storage tinggi.
* High Performance Computing (HPC): dirancang untuk komputasi berperforma tinggi yang membutuhkan spesifikasi tinggi.
* Optimized shapes : dirancang untuk komputasi tingkat tinggi pada frekuensi core prosesor untuk menyediakan HPC dengan low latency.

### Flexible Shapes
Flexible shapes adalah sebuah templat yang dapat melakukan kustom terhadap spesifikasi ketika melakukan launching atau mengubah VM.
Jenis-jenis flexibe shapes yang tersedia :
* VM.Standard.E3.Flex (AMD), 64GB per OCPU, 1024 GB Memory
* VM.Standard.E4.Flex (AMD), 64GB per OCPU, 1024 GB Memory
* VM.Optimized3.Flex (Intel), 64GB per OCPU, 256 GB Memory
* VM.Standard.A1.Flex (ARM processor dari Ampere), 64GB per OCPU, 512 GB Memory

## Kapasitas
Ketika membuat VM, kita dapat memilih jenis kapastias dari instance, yaitu :
* On-Demand Capacity : cukup bayar sesuai dengan kapasitas yang digunakan.
* Preemptible capacity : ketika ada beban kerja yang meningkat, sistem ini akan diaktifkan.
* Reserved capacity : kapasitas yang sedang tidak digunakan akan berbeda biayanya dengan kapasitas yang sedang digunakan.
* Dedicated capacity : kapasitas yang tersedia untuk instance itu saja.
