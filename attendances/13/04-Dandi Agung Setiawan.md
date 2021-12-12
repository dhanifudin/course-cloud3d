# Resume Pertemuan 14 - Serverless with Oracle Functions, Events and API Gateway
## 1. Oracle Fuction
Oracle Cloud Functions adalah platform tanpa server yang memungkinkan pengembang membuat, menjalankan, dan menskalakan aplikasi tanpa
 mengelola infrastruktur apa pun. Fungsi terintegrasi dengan Oracle Cloud Infrastructure, layanan platform, dan aplikasi SaaS. 
Karena Functions didasarkan pada Fn Project open source, pengembang dapat membuat aplikasi yang dapat dengan mudah di-porting ke lingkungan 
cloud dan lokal lainnya. Kode berdasarkan Fungsi biasanya berjalan untuk jangka waktu pendek, dan pelanggan hanya membayar untuk sumber daya yang mereka gunakan.

Cloud Functions memungkinkan developer mengakses peristiwa Firebase dan Google Cloud, beserta daya komputasi yang skalabel untuk menjalankan kode sebagai respons 
terhadap peristiwa tersebut. Meskipun Cloud Functions pada aplikasi Firebase diharapkan bekerja secara unik untuk memenuhi kebutuhan developer yang juga unik, 
kasus penggunaan yang umum terjadi adalah sebagai berikut:
- Memberi tahu pengguna jika ada sesuatu yang menarik.
- Melakukan pembersihan dan pemeliharaan database.
- Menjalankan tugas intensif di cloud, bukan di aplikasi Anda.
- Melakukan integrasi dengan API dan layanan pihak ketiga.
### Cara kerjanya 
Push function image to registry => Configure function trigger => Code runs only when triggered => Pay for code execution time only.

## 2. Oracle Events Service
Oracle Cloud Infrastructure Events Service melacak perubahan sumber daya menggunakan 
event yang sesuai dengan standar Cloud Native Computing Foundation (CNCF).  Pengembang 
dapat merespons perubahan secara real-time dengan memicu kode Functions, menulis ke 
Streaming, atau mengirim alert menggunakan Notifikasi.
### Use case
- Real-Time Image Processing.
- Resource Change Notifications.

## 3. OCI API Gateway
Layanan API Gateway memungkinkan Anda membuat antarmuka HTTP/S yang diatur untuk layanan 
lain, termasuk Oracle Functions, Container Engine for Kubernetes, dan Container 
Registry.  API Gateway juga menyediakan penegakan kebijakan seperti autentikasi dan 
pembatasan kecepatan ke titik akhir HTTP/S.
### Use case
- Serverless Web Backends.