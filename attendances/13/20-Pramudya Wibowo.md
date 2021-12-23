# Serverless

## Oracle Functions
Pada praktikum-praktikum sebelumnya kita diajarkan bahwa virtualisasi komputer pada saat ini berkembang dari Bare Metal, kemudian ke Virtual Machines, dan Containers. Akan tetapi saat ini telah dikembangkan juga sebuah layanan yang lebih kecil dan lebih spesifik lagi untuk digunakan. Yaitu Functions as a service (FaaS). Fungsi dibentuk menjadi sebuah containers.

# Functions as a Service (FaaS)
FaaS menjalankan sebuah code saja dalam sebuah layanan sehingga kebutuhan akan sumber dayanya akan semakin kecil. Berikut model programming untuk fungsi :
* Short Execution
* Stateless
* Trigerred from user code or cloud events
* Self contained

# Function Development Kits (FDKs)
* FDKs mempermudah untuk membuat fungsi
* Mudah untuk membuat fungsi 'handler' pada FDK yang diinginkan kemudian FDK akan menyediakan masukan ke fungsi sesuai dengan output yang anda inginkan.
* FDK antara lain : Python, Java, Node.js

# FaaS Example
Contoh sederhana dari penggunaan FaaS :
1. Pengguna berinteraksi dengan web
2. Web memiliki fungsi untuk mengambil data dari oracle object storage
3. Permintaan yang dikirimkan dari web dan masuk ke Oracle akan dieksekusi oleh fungsi yang berkaitan.
4. Hasil dari permintaan akan dikirim kembali ke web dan ditampilkan.