# Rangkuman Pertemuan 12
# Serverless with Oracle Functions, Events and API Gateway
1. Oracle Fuction
Oracle Cloud Functions adalah platform tanpa server yang memungkinkan pengembang membuat, menjalankan, dan 
menskalakan aplikasi tanpa mengelola infrastruktur apa pun.  Functions terintegrasi dengan Oracle Cloud 
Infrastructure, layanan platform, dan aplikasi SaaS
* Cara kerjanya 
Push function image to registry => Configure function trigger => Code runs only when triggered => Pay for code execution time only
2. Oracle Events Service
Oracle Cloud Infrastructure Events Service melacak perubahan sumber daya menggunakan 
event yang sesuai dengan standar Cloud Native Computing Foundation (CNCF).  Pengembang 
dapat merespons perubahan secara real-time dengan memicu kode Functions, menulis ke 
Streaming, atau mengirim alert menggunakan Notifikasi.
# Use case
* Real-Time Image Processing.
* Resource Change Notifications.
3. OCI API Gateway
Layanan API Gateway memungkinkan Anda membuat antarmuka HTTP/S yang diatur untuk layanan 
lain, termasuk Oracle Functions, Container Engine for Kubernetes, dan Container 
Registry.  API Gateway juga menyediakan penegakan kebijakan seperti autentikasi dan 
pembatasan kecepatan ke titik akhir HTTP/S.
# Use case
* Serverless Web Backends.