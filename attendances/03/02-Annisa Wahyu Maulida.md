Komputasi Awan dan Sistem Terdistribusi

Jenis Compute :
- Bare Metal
- VM, yang akan kita gunakan dalam pembelajaran

Jenis Instance :

- Shapes, mendefinisikan spek (sesuai kebutuhan),
 1. Standard shapes, untuk kebutuhan umum. Seperti Intel & AMD.
 2. DenseIO, untuk kebutuhan basis data besar. Seperti NVMe berbasis SSD.
 3. GPU, untuk akselerasi pada hardware terutama kebutuhan GPU. Termasuk Inter, AMD CPU, NVIDIA.
 4. HPC, untuk komputasi performa tinggi. Dalam klaster jaringan dapat diakses secara paralel.
 5. Optimized, untuk komputasi tingkat tinggi pada frekuensi core prosesor. Cocok untuk kebutuhan HPC low latency, serta mendukung cluster networking.

- Flexible shape, dapat di kostumisasi sesuai pemakaian kita (dimulai ketika launching maupun mengubah VM),
 1. VM.Standard.E3.Flex (AMD), 64 GB per OCPU max 1024 GB
 2. VM.Standard.E4.Flex (AMD), 64 GB per OCPU max 1024 GB
 3. VM.Optimized3.Flex (Intel), 64 GB per OCPU max 256 GB
 4. VM.Standard.A1.Flex (Arm processor dari Ampere), 64 GB per OCPU max 512 GB

Jenis Host untuk VM,
1. On-demand capacity: bayar sesuai dengan kapasitas compute yang digunakan.
2. Preemptible capacity: saat membutuhkan sumber daya lebih / beban kerja meningkat pada periode tertentu.
3. Reserved capacity: kapasitas cadangan untuk masa akan datang sesuai dengan kebutuhan (dilihat mana yang digunakan dan tidak).
4. Dedicated capacity: menjalankan pada dedicated server, sehingga sumber daya tidak dibagi dengan client/customer lain.

Komponen VM :
- Komponen VM
- Availability domain
- Virtual cloud network
- Key pair (untuk Linux), sangat direkomendasi.
- Tags, aplikasikan firewall tergantung dengan apa yang dipakai.
- Password (untuk Windows)
- Image
- Shape, sesuai dengan penjelasan sebelumnya (E3, E4)