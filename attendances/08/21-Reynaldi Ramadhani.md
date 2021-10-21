## Object Storage
Object Storage adalah Platform Penyimpanan dari OCI yang memiliki performa tinggi dan scalable yang dapat menyimpan data tidak terstruktur dalam jumlah tidak terbatas seperi gambar,video dll . Dengan Object Storage juga bisa mengambil data dari Internet atau pun dari platfrom cloud .
    Object Storage mendukung private access dari Oracle Cloud Infrastructure resource yang ada
di VCN melalui gateway layanan. Sebuah gateway layanan memungkinkan konektivitas ke end point
publik Object Storage dari alamat IP pribadi di subnet pribadi.

## Penggunaan Object Storage
Biasanya Digunakan saat kita membutuhkan upload dan membutuhkan penyimpanan yang besar

## Object Storage Resource 
Oracle Cloud Infrastructure memili memiliki berbagai tipe Object Storage untuk mengelola 
dan menyimpan data, antara lain yaitu:
    -   Bucket
                Bucket adalah logical container untuk menyimpan objek. Pengguna atau sistem membuat 
        bucket sesuai kebutuhan dalam suatu wilayah. Bucket dikaitkan dengan kompartemen tunggal
        (Kumpulan resource yang hanya dapat diakses oleh grup yang telah diberi izin oleh administrator di 
        organisasi) yang memiliki policies (Dokumen Identity and Access Management (IAM) digunakan 
        untuk menentukan siapa yang memiliki jenis akses ke resource kita) untuk menentukan tindakan apa 
        yang dapat dilakukan pengguna pada bucket dan pada semua objek dalam bucket.
    -   Object
            Semua tipe data, apa pun tipe kontennya, disimpan sebagai objek. Sebuah objek terdiri dari 
        objek itu sendiri dan metadata tentang objek tersebut. Setiap objek disimpan dalam bucket.
    -   Namespace
            Namespace Object Storage berfungsi sebagai top-level container untuk semua bucket dan 
        objek. Namespace mencakup semua kompartemen dalam suatu wilayah. Kita dapat mengontrol nama bucket, tetapi 
        nama bucket tersebut harus unik dalam namespace. Meskipun namespace adalah khusus wilayah, 
        nama namespace itu sendiri sama di semua wilayah.
    -   Compartment
            Kompartemen adalah primary block building yang digunakan untuk mengatur sumber daya 
        cloud. Saat sewa, kompartemen root dibuat untuk kemudian membuat kompartemen di bawah 
        kompartemen root untuk mengatur sumber daya Kita

## Object Storage Karakteristik
    - Strong Konsistensi : Akan membuat salinan jika ada read request
    - Durability : Object Storage secara aktif memantau integritas data menggunakan checksum dan secara otomatis mendeteksi dan memperbaiki data yang rusak.
    - Custom MetaData: Kita dapat menentukan metadata ekstensif kita sendiri sebagai pasangan nilai kunci untuk tujuan apa pun
    - Security : Object Storage memastikan keamanan data yang disimpan menggunakan enkripsi data. Enkripsi data adalah metode yang digunakan untuk melindungi   kerahasiaan data

## Cara Akses Object Storage
    - Console
    - CLI
    - Rest API
    - OCI SDK 

## Praktikum JS
    Dalam Praktikum kita mendeploy sebuah web statis lalu kita dapat mengakses nya melalui link atau path url yang sudah digenerate
