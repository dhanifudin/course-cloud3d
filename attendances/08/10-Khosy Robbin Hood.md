# PERTEMUAN 8
### Pendahuluan Object Storage 
Layanan Oracle Cloud Infrastructure Object Storage adalah platform penyimpanan yang memiliki performa yang tinggi dan scalable,  menawarkan ketahanan data yang andal dan hemat biaya. Layanan Object Storage dapat menyimpan data tidak terstruktur dalam jumlah tak terbatas dari jenis konten apa pun, termasuk data analitik dan konten (seperti gambar dan video). Dengan Object Storage, Kita dapat menyimpan atau mengambil data langsung dari internet atau dari dalam platform cloud. Object Storage menawarkan beberapa interface yang memungkinkan Kita mengelola penyimpanan dalam skala besar dengan mudah.

### Object Storage Resource
* Buckets, 
Bucket adalah logical container untuk menyimpan objek. Pengguna atau sistem membuat bucket sesuai kebutuhan dalam suatu wilayah.
Bucket dikaitkan dengan kompartemen tunggal yang memiliki policies untuk menentukan tindakan apa yang dapat dilakukan pengguna pada bucket dan pada semua objek dalam bucket.

* Object, 
Semua tipe data, apa pun tipe kontennya, disimpan sebagai objek. Sebuah objek terdiri dari objek itu sendiri dan metadata tentang objek tersebut. Setiap objek disimpan dalam bucket.

* Namespace,
Namespace Object Storage berfungsi sebagai top-level container untuk semua bucket dan objek. Pada waktu pembuatan akun, setiap penyewa Oracle Cloud Infrastructure diberi satu nama namespase Object Storage unik yang dibuat oleh sistem dan tidak dapat diubah.
Namespace mencakup semua kompartemen dalam suatu wilayah. Kita dapat mengontrol nama bucket, tetapi nama bucket tersebut harus unik dalam namespace. Meskipun namespace adalah khusus wilayah, nama namespace itu sendiri sama di semua wilayah.

* Compartment,
Kompartemen adalah primary block building yang digunakan untuk mengatur sumber daya cloud. Saat sewa, kompartemen root dibuat untuk kemudian membuat kompartemen di bawah kompartemen root untuk mengatur sumber daya Kita. 
Kita dapat mengontrol akses dengan membuat kebijakan yang menentukan tindakan apa yang dapat dilakukan grup pengguna terhadap sumber daya di kompartemen tersebut. Bucket Penyimpanan Objek hanya bisa ada di satu kompartemen.

### Object Storage Characteristics
* Strong Consistency
* Durability
* Custom Metadata
* Security

### Cara akses Object Storage :
* Console
* CLI
* REST API
* OCI SDK

### Limits on Object Storage Resources :
* Authentication and Authorization
* Blocking Access to Object Storage Resources
* Object Storage IP Addresses

