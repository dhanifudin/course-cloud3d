<h1>Object Storage</h1>

**Layanan Oracle Cloud Infrastructure Object Storage** adalah platform penyimpanan yang memiliki performa yang tinggi dan scalable,  menawarkan ketahanan data yang andal dan hemat biaya. Layanan Object Storage dapat menyimpan data tidak terstruktur dalam jumlah tak terbatas dari jenis konten apa pun, termasuk data analitik dan konten (seperti gambar dan video).

**Object Storage Resource**
- Buckets : logical container untuk menyimpan objek. Pengguna atau sistem membuat bucket sesuai kebutuhan dalam suatu wilayah.
- Objects : Semua tipe data, apa pun tipe kontennya, disimpan sebagai objek. 
- Namespace : Namespace Object Storage berfungsi sebagai top-level container untuk semua bucket dan objek. 
- Compartment : primary block building yang digunakan untuk mengatur sumber daya cloud. 

**Object Storage Characteristics**
- Strong Consistency : Saat ada read request, Object Storage akan membuat salinan terbaru dari data yang ditulis ke sistem.
- Durability : Object Storage adalah layanan regional. Data disimpan secara redundan di beberapa server penyimpanan. Object Storage secara aktif memantau integritas data menggunakan checksum dan secara otomatis mendeteksi dan memperbaiki data yang rusak.
- Custom Metadata : dapat menentukan metadata ekstensif sendiri sebagai pasangan nilai kunci untuk tujuan apa pun juga dapat menetapkan metadata khusus ke objek dan bucket menggunakan Oracle Cloud Infrastructure CLI atau SDK.
- Security : Object Storage memastikan keamanan data yang disimpan menggunakan enkripsi data. Data dapat diakses menggunakan kunci dekripsi yang dibuat saat mengunggah objek ke bucket. Ini digunakan bersama dengan kebijakan IAM yang mengautentikasi pengguna yang melakukan tugas.

**Limits on Object Storage Resources**
- Authentication and Authorization : Setiap layanan di Oracle Cloud Infrastructure terintegrasi dengan IAM untuk otentikasi dan otorisasi, untuk semua interface (Konsol, SDK atau CLI, dan REST API).
- Blocking Access to Object Storage Resources : dapat meningkatkan keamanan Object Storage policies dengan membatasi akses hanya untuk permintaan yang berasal dari alamat IP yang diizinkan. 
- Object Storage IP Addresses : Oracle Cloud Infrastructure Object Storage service menggunakan CIDR dengan blok IP range 134.70.0.0/16 untuk semua region.


