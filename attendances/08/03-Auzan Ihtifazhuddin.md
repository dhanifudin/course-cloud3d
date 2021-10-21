Object storage pada oracle cloud yang dimana fungsi dari object stroage adalah sebagai platform penyimpanan yang memiliki performa yang tinggi dan scalable, oracle cloud menawarkan object storage ketahanan data yang andal dan hemat biaya tidak hanya itu object storage menyimpan data tidak terstruktur dalam jumlah tak terbatas dari file apapun seperti gambar maupun video, dengan adanya fitur object storage kita langsung dapat menyimpan atau mengambil data melalui internet dari oracle cloud dengan hal ini kita tidak perlu khawatir data akan hilang. oracle cloud mendukung object storage dengan private access melalui ip pribadi tujuan agar data lebih aman, kita dapat mengakses object storage melalui console,cli,rest api dan oci sdk. Object storage memiliki resource diantaranya :

    1. Buckets adalah logical container untuk menyimpan
    2. Objects Yaitu Semua tipe data akan disimpan sebagai objek setiap objek akan disimpan pada buckets
    3. NameSpace Berfungsi sebagai top-level container untuk semua buckets dan object
    4. Compartment adalah Primary block building yang digunakan untuk mengatur sumber daya cloud

Object storage characteristics :

1. Strong Consistency : Saat ada read request, Object Storage akan membuat salinan terbaru dari data yang ditulis ke sistem.
2. Durability : Object Storage adalah layanan regional. Data disimpan secara redundan di beberapa server penyimpanan.
3. Custom Metadata : Kita dapat menentukan metadata ekstensif kita sendiri sebagai pasangan nilai kunci untuk tujuan apa pun.
4. Security : Object Storage memastikan keamanan data yang disimpan menggunakan enkripsi data. 

Kita dapat mengakses Object Storage menggunakan beberapa cara, OCI menyediakan sesuai dengan preferensi kita dan sesuai dengan kebutuhan :
• Console
• CLI
• REST API
• OCI SDK
