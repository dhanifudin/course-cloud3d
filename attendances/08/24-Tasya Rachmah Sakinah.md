# Pertemuan 8
## Pendahuluan Object Storage (Overview)
Layanan Oracle Cloud Infrastructure Object Storage adalah platform penyimpanan yang memiliki performa yang tinggi dan scalable. Layanan Object Storage dapat menyimpan data tidak terstruktur dalam jumlah tak terbatas dari jenis konten apa pun, termasuk data analitik dan konten (seperti gambar dan video).

## Object Storage Resource-Buckets
Bucket adalah logical container untuk menyimpan objek. Bucket dikaitkan dengan kompartemen tunggal yang memiliki policies untuk menentukan tindakan apa yang dapat dilakukan pengguna pada bucket dan pada semua objek dalam bucket.

## Object Storage Resource-Objects
Semua tipe data, apa pun tipe kontennya, disimpan sebagai objek. Sebuah objek terdiri dari objek itu sendiri dan metadata tentang objek tersebut. Setiap objek disimpan dalam bucket.

## Object Storage Resource-Namespace
Namespace Object Storage berfungsi sebagai top-level container untuk semua bucket dan objek. Pada waktu pembuatan akun, setiap penyewa Oracle Cloud Infrastructure diberi satu nama namespase Object Storage unik yang dibuat oleh sistem dan tidak dapat diubah.
Namespace mencakup semua kompartemen dalam suatu wilayah. Kita dapat mengontrol nama bucket, tetapi nama bucket tersebut harus unik dalam namespace.

## Object Storage Resource-Compartment
Kompartemen adalah primary block building yang digunakan untuk mengatur sumber daya cloud. Saat sewa, kompartemen root dibuat untuk kemudian membuat kompartemen di bawah kompartemen root untuk mengatur sumber daya Kita. Bucket Penyimpanan Objek hanya bisa ada di satu kompartemen.

## Object Storage Characteristics-Strong Consistency
Saat ada read request, Object Storage akan membuat salinan terbaru dari data yang ditulis ke sistem.

## Object Storage Characteristics-Durability
Object Storage adalah layanan regional. Data disimpan secara redundan di beberapa server penyimpanan. 

## Object Storage Characteristics-Custom Metadata
- Dapat menentukan metadata ekstensif kita sendiri sebagai pasangan nilai kunci untuk tujuan apa pun.
- Dapat menetapkan metadata khusus ke objek dan bucket menggunakan Oracle Cloud Infrastructure CLI atau SDK.

## Object Storage Characteristics-Security
- Object Storage memastikan keamanan data yang disimpan menggunakan enkripsi data. 
- Data dapat diakses menggunakan kunci dekripsi yang dibuat saat mengunggah objek ke bucket.

## Cara akses Object Storage
Dapat mengakses Object Storage menggunakan beberapa cara, OCI menyediakan sesuai dengan preferensi kita dan sesuai dengan kebutuhan.
- Console
- CLI
- REST API
- OCI SDK

## Limits on Object Storage Resources Authentication and Authorization
Setiap layanan di Oracle Cloud Infrastructure terintegrasi dengan IAM untuk otentikasi dan otorisasi, untuk semua interface (Konsol, SDK atau CLI, dan REST API). IAM juga mengelola kredensial pengguna API signing keys, token autentikasi, dan secret key untuk kompatibilitas API Amazon S3. 

## Limits on Object Storage Resources Blocking Access to Object Storage Resources 
Dapat meningkatkan keamanan Object Storage policies dengan membatasi akses hanya untuk permintaan yang berasal dari alamat IP yang diizinkan.

## Limits on Object Storage Resources-Object Storage IP Addresses
Oracle Cloud Infrastructure Object Storage service menggunakan CIDR dengan blok IP range 134.70.0.0/16 untuk semua region.

## Limits on Object Storage Resources-Object Storage IP Addresses
- Number of Object Storage namespaces per root compartment: 1
- Maximum object size: 10 TiB
- Maximum object part size in a multipart upload: 50 GiB
- Maximum number of parts in a multipart upload: 10,000
- Maximum object size allowed by PutObject API: 50 GiB
- Maximum size of object metadata: 2 K
