# Rangkuman Pertemuan 8
# Layanan Oracle Cloud Infrastructure Object Storage
Layanan Object Storage dapat menyimpan data tidak terstruktur dalam jumlah tak terbatas dari
jenis konten apa pun, termasuk data analitik dan konten (seperti gambar dan video). Layanan ini
digunakan ketika aplikasi yang kita deploy menggunakan fitur upload data. Elastisitas platform memungkinkan
Kita melakukan skala untuk menggunakan kapasitas yang kecil (minimum) hingga paling maksimal,
tanpa mengalami penurunan kinerja atau service reability.
# Object Storage
Adalah layanan regional dan tidak terikat dengan instance komputasi tertentu.
Kita dapat mengakses data dari mana saja di dalam atau di luar konteks Oracle Cloud Infrastructure,
selama Kita memiliki konektivitas internet dan dapat mengakses salah satu end point Object Storage.
Object Storage mendukung private access dari Oracle Cloud Infrastructure resource yang ada
di VCN melalui gateway layanan.
# Object Storage Resource 
Oracle Cloud Infrastructure memili memiliki berbagai tipe Object Storage untuk mengelola
dan menyimpan data, antara lain yaitu:
1. Bucket adalah logical container untuk menyimpan objek. Pengguna atau sistem membuat bucket sesuai kebutuhan dalam suatu wilayah.
2. Objects, semua tipe data, apa pun tipe kontennya, disimpan sebagai objek.
3. Namespace, berfungsi sebagai top-level container untuk semua bucket dan objek. Kita dapat mengontrol nama bucket, tetapi
nama bucket tersebut harus unik dalam namespace. Meskipun namespace adalah khusus wilayah,
nama namespace itu sendiri sama di semua wilayah. 
4. Compartment adalah primary block building yang digunakan untuk mengatur sumber daya cloud.
Kita dapat mengontrol akses dengan membuat kebijakan yang menentukan tindakan apa yang dapat 
dilakukan grup pengguna terhadap sumber daya di kompartemen tersebut. 
Bucket Penyimpanan Objek hanya bisa ada di satu kompartemen.
# Object Storage Characteristics
1. Strong Consistency, Saat ada read request, Object Storage akan membuat salinan terbaru dari data yang ditulis ke sistem.
2. Durability, Object Storage adalah layanan regional. Data disimpan secara redundan di beberapa server
penyimpanan. Object Storage secara aktif memantau dan memastikan redundansi data. Jika kehilangan redundansi terdeteksi,
Object Storage secara otomatis membuat lebih banyak salinan data.
3. Custom Metadata, kita dapat menentukan metadata ekstensif kita sendiri sebagai pasangan nilai kunci untuk
tujuan apa pun. Misalnya, kita dapat membuat tag deskriptif untuk objek, mengambil tag tersebut, dan
menyortir data.
4. Security, Object Storage memastikan keamanan data yang disimpan menggunakan enkripsi data.
# Cara akses Object Storage
Kita dapat mengakses Object Storage menggunakan beberapa cara, OCI menyediakan sesuai
dengan preferensi kita dan sesuai dengan kebutuhan : 
1. Console
2. CLI
3. REST API
4. OCI SDK
# Authentication and Authorization
Setiap layanan di Oracle Cloud Infrastructure terintegrasi dengan IAM untuk otentikasi dan
otorisasi, untuk semua interface (Konsol, SDK atau CLI, dan REST API). IAM juga mengelola
kredensial pengguna API signing keys , token autentikasi, dan secret key untuk kompatibilitas API
Amazon S3. Kita perlu menyiapkan atau membuat grup, kompartemen dan policies  yang mengontrol
pengguna mana yang dapat mengakses layanan, resource dan jenis akses. Misalnya, kebijakan
mengontrol siapa yang dapat membuat pengguna dan grup, membuat bucket, mengunduh objek dan
mengelola kebijakan dan aturan terkait Object Storage.
# Blocking Access to Object Storage Resources from Unauthorized IP Addresses.
Kita dapat meningkatkan keamanan Object Storage policies dengan membatasi akses hanya
untuk permintaan yang berasal dari alamat IP yang diizinkan. Pertama, kita membuat network source
(grup alamat IP dapat digunakan dalam policies untuk membatasi akses) untuk menentukan alamat IP
yang diizinkan, lalu kita menambahkan ketentuan ke kebijakan untuk membatasi akses ke alamat IP di
sumber jaringan.
# Object Storage IP Addresses 
Oracle Cloud Infrastructure Object Storage service menggunakan CIDR dengan blok IP range
134.70.0.0/16 untuk semua region.