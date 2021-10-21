# Object Storage

Layanan Oracle Cloud Infrastructure Object Storage adalah platform penyimpanan yang memiliki performa yang tinggi dan scalable, 
menawarkan ketahanan data yang andal dan hemat biaya. 
Layanan Object Storage dapat menyimpan data tidak terstruktur dalam jumlah tak terbatas dari jenis konten apa pun, 
termasuk data analitik dan konten (seperti gambar dan video).

Object storage sendiri digunakan saat kita ingin melakukan upload file seperti upload website statis contohnya menggunakan react js, vue js, angular js, atau bisa juga digunakan saat membutuhkan upload multimedia

## Tipe Object Storage
<ul>
   <li>Buckets, adalah logical container untuk menyimpan objek. Pengguna atau sistem membuat bucket sesuai kebutuhan dalam suatu wilayah. Bucket dikaitkan dengan kompartemen tunggal 
     (Kumpulan resource yang hanya dapat diakses oleh grup yang telah diberi izin oleh administrator di organisasi) 
     yang memiliki policies (Dokumen Identity and Access Management (IAM) digunakan untuk menentukan siapa yang memiliki jenis akses ke resource kita)
     untuk menentukan tindakan apa yang dapat dilakukan pengguna pada bucket dan pada semua objek dalam bucket </li>
  <li>Objects, semua tipe data, apa pun tipe kontennya, disimpan sebagai objek. Sebuah objek terdiri dari objek itu 
    sendiri dan metadata tentang objek tersebut. Setiap objek disimpan dalam bucket.</li>
  <li>Namespace, Namespace Object Storage berfungsi sebagai top-level container untuk semua bucket dan objek. 
    Pada waktu pembuatan akun, setiap penyewa Oracle Cloud Infrastructure diberi satu nama namespase Object 
    Storage unik yang dibuat oleh sistem dan tidak dapat diubah. </li>
  <li>Compartment, Kompartemen adalah primary block building yang digunakan untuk mengatur sumber daya cloud. 
    Saat sewa, kompartemen root dibuat untuk kemudian membuat kompartemen di bawah kompartemen root untuk mengatur sumber daya </li>
</ul>
  
## Object Storage Characteristics
Object Storage Characteristics menyediakan beberapa fitur-fitur, antara lain
<ul>
  <li>Strong Consistency, di sini artinya yaitu membuat salinan terbaru dari data yang ditulis ke sistem.</li>
  <li>Durability, mendeteksi dan memperbaiki data yang rusak.</li>
  <li>Custom Metadata, menetapkan metadata khusus ke objek dan bucket.</li>
  <li>Security</li>
</ul>


