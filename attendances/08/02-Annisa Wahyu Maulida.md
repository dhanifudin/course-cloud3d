Pertemuan 8 - Object Storage

- Object storage tidak terikat dengan VM / instance komputasi tertentu
- Object storage identik dengan fitur upload
- Web yang membutuhkan object storage merupakan web statis (html, css,js(read js, view js,dll) )
(php termasuk web dinamis krn butuh interpreter untuk mengaksesnya)
- Web dengan object storage membutuhkan penyimpanan data skala besar seperti multimedia(gambar, video, dll) 
- Kelebihan deploy object storage pada web statis hanya melakukan generate url lalu upload data

Object Storage pada layanan Oracle Cloud Infrastucture Object Storage 
- merupakan platform penyimpanan dengan ketahanan data andal, 
performa yang tinggi, scalable serta hemat biaya.
- dapat menyimpan data tidak terstruktur dalam jumlah tak terbatas dari berbagai 
jenis konten termasuk data analitik dan konten(gambar, video, dll)
- dapat mengakses data dari mana saja di dalam atau diluar konteks 
Oracle Cloud Infrastructure selama memiliki konektivitas internet dan 
dapat mengakses salah satu end point object storage.
- Object Storage mendukung private access dari Oracle Cloud 
Infrastructure resource pada VCN melalui gateway layanan (yang memungkinkan 
konektivitas ke end point publik Object Storage dari alamat IP pribadi di subnet pribadi).

Object Storage Resource :
- Buckets
Merupakan logical container untuk menyimpan objek. Pengguna atau sistem membuat bucket 
sesuai kebutuhan. Bucket dikaitkan dengan kompartemen tunggal yang memiliki policies 
untuk menentukan tindakan apa yang dapat dilakukan pengguna pada bucket dan pada objek dalam bucket.
- Objects
Tipe data, apapun kontennya disimpan sebagai objek. Sebuah objek terdiri dari objek itu sendiri 
dan metadata tentang objek tersebut. Setiap objek disimpan dalam bucket.
- Namespace
Namespace Object Storage berfungsi sebagai top-level container untuk semua bucket dan objek. 
Pada waktu pembuatan akun, setiap penyewa Oracle Cloud Infrastructure diberi satu nama 
namespase Object Storage unik yang dibuat oleh sistem dan tidak dapat diubah. 
Namespace mencakup semua kompartemen dalam suatu wilayah. 
- Compartment
Kompartemen adalah primary block building yang digunakan untuk mengatur sumber daya cloud. 
Saat melakukan sewa, kompartemen root dibuat untuk kemudian membuat kompartemen di bawah 
kompartemen root untuk mengatur sumber daya Kita. 

Characteristics :
- Strong Consistency
- Durability
- Custom Metadata
- Security

Cara akses Object Storage :
- Console
- CLI
- REST API
- OCI SDK

Limits on Object Storage Resources :
- Authentication and Authorization
- Blocking Access to Object Storage Resources 
- Object Storage IP Addresses