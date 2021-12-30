# Cloud computing
## Komputasi Awan dan Sistem Terdistribusi
### Poin 
- Mengetahui Object Storage yang ditawarkan Oracle Cloud Infrastructure (OCI)
- Dapat memanfaatkan layanan Object Storage yang ditawarkan Oracle Cloud Infrastructure (OCI)
### Pendahuluan
#### Object Storage 
Object Storage adalah platform penyimpanan yang memiliki performa yang tinggi dan scalable,  menawarkan ketahanan data yang andal dan hemat biaya. Layanan Object Storage dapat menyimpan data tidak terstruktur dalam jumlah tak terbatas dari jenis konten apa pun, termasuk data analitik dan konten (seperti gambar dan video).
### Object Storage Resource
#### Buckets
- Bucket adalah logical container untuk menyimpan objek. Pengguna atau sistem membuat bucket sesuai kebutuhan dalam suatu wilayah.
- Bucket dikaitkan dengan kompartemen tunggal yang memiliki policies untuk menentukan tindakan apa yang dapat dilakukan pengguna pada bucket dan pada semua objek dalam bucket.
#### Objects
- Semua tipe data, apa pun tipe kontennya, disimpan sebagai objek. Sebuah objek terdiri dari objek itu sendiri dan metadata tentang objek tersebut. Setiap objek disimpan dalam bucket.
#### Namespace
- Namespace Object Storage berfungsi sebagai top-level container untuk semua bucket dan objek. Pada waktu pembuatan akun, setiap penyewa Oracle Cloud Infrastructure diberi satu nama namespase Object Storage unik yang dibuat oleh sistem dan tidak dapat diubah.
- Namespace mencakup semua kompartemen dalam suatu wilayah. Kita dapat mengontrol nama bucket, tetapi nama bucket tersebut harus unik dalam namespace. Meskipun namespace adalah khusus wilayah, nama namespace itu sendiri sama di semua wilayah.
#### Compartment
- Kompartemen adalah primary block building yang digunakan untuk mengatur sumber daya cloud. Saat sewa, kompartemen root dibuat untuk kemudian membuat kompartemen di bawah kompartemen root untuk mengatur sumber daya Kita. 
- Kita dapat mengontrol akses dengan membuat kebijakan yang menentukan tindakan apa yang dapat dilakukan grup pengguna terhadap sumber daya di kompartemen tersebut. Bucket Penyimpanan Objek hanya bisa ada di satu kompartemen.
