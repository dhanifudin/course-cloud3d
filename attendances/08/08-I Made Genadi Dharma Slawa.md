# Object Sotrage
Object Storage adalah platform penyimpanan yang
memiliki performa yang tinggi dan scalable, menawarkan ketahanan data yang andal dan hemat
biaya. Layanan Object Storage dapat menyimpan data tidak terstruktur dalam jumlah tak terbatas dari
jenis konten apa pun, termasuk data analitik dan konten (seperti gambar dan video).

## Tipe-tipe Object Storage
- **Buckets** - Adalah logical container untuk menyimpan objek. Pengguna atau sistem membuat
bucket sesuai kebutuhan dalam suatu wilayah. Bucket dikaitkan dengan kompartemen tunggal
(Kumpulan resource yang hanya dapat diakses oleh grup yang telah diberi izin oleh administrator di
organisasi) yang memiliki policies (Dokumen Identity and Access Management (IAM) digunakan
untuk menentukan siapa yang memiliki jenis akses ke resource kita) untuk menentukan tindakan apa
yang dapat dilakukan pengguna pada bucket dan pada semua objek dalam bucket
- **Objects** - Semua tipe data, apa pun tipe kontennya, disimpan sebagai objek. Sebuah objek terdiri dari
objek itu sendiri dan metadata tentang objek tersebut. Setiap objek disimpan dalam bucket.
- **Namespace** - Namespace Object Storage berfungsi sebagai top-level container untuk semua bucket dan
objek. Pada waktu pembuatan akun, setiap penyewa Oracle Cloud Infrastructure diberi satu nama
namespase Object Storage unik yang dibuat oleh sistem dan tidak dapat diubah.
- **Compartment** - Kompartemen adalah primary block building yang digunakan untuk mengatur sumber daya
cloud. Saat sewa, kompartemen root dibuat untuk kemudian membuat kompartemen di bawah
kompartemen root untuk mengatur sumber daya K