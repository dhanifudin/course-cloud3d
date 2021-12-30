# Object Storage
Layanan OCI Object Storage adalah platform penyimpanan yang memiliki performa yang tinggi dan scalable,  menawarkan ketahanan data yang andal dan hemat biaya yang tidak terstruktur dan dalam jumlah tak terbatas untuk konten apapun. Dengan Object Storage, kita dapat menyimpan atau mengambil data langsung dari internet, tidak terikat dengan instance tertentu. Object Storage juga mendukung private access menggunakan VCN melalui gateway dari alamat IP Private si subnet Private.

## Beberapa layanan Object Storage Resource
- Bucket, yaitu logical container untuk menyimpan objek yang diatur oleh polies untuk menentukan tindakan apa yang dapat dilakukan pengguna pada bucket tersebut.
- Objects, konten yang berupa tipe data apapun dan disimpan sebagai objek yang disimpan dalam bucket.
- Namespace, berfungsi sebagai top-level container untuk semua bucket dan object, namespace ini hanya akan diberikan satu saja ketika pengguna mendaftar ke OCI dan tidak dapat diubah.
- Compartment, merupakan primary block building yang digunakan untuk mengatur sumber daya pada cloud. Untuk mengakses compartment kita dapat membuat kebijakan yang menentukan tindakan apa yang dapat dilakukan oleh grup pengguna.

## Karakteristik Object Storage
- Strong Consistency, Saat ada read request, Object Storage akan membuat salinan terbaru dari data yang ditulis ke sistem.
- Durability, data disimpan secara redundan sehingga ketika terdapat data yang rusak maka secara otomatis akan terdeteksi dan memperbaiki data tersebut serta memastikan apabila ada kerusakan data maka object storage akan otomatis membuat banyak salinan data.
- Custom Metadata, kita dapat menentukan metadata ekstensif kita sendiri sebagai pasangan nilai kunci untuk tujuan apapun.
- Security, memastikan setiap data terenkripsi.

## Cara mengakses Object Storage
- Console
- CLI
- REST API
- OCI SDK

## Pembatasan dalam Object Storage Resources
- Authentication and Authorization, yaitu layanan di OCI terintegrasi dengan IAM untuk autentikasi dan otorisasi. IAM juga mengelola kredensial API, token autentikasi, serta secret key untuk API Amazon S3.
- Blocking Access to Object Storage Resources, kita dapat meningkatkan kemanan dengan membatasi akses hanya untuk permintaan yang berasal dari alamat IP yang diizinkan.
- Object Storage IP Addresses, OCI Object Storage menggunakan CIDR dengan blok IP range 134.70.0.0/16
