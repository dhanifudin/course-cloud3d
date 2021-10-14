# Pertemuan 5 PLATFORM AS A SERVICE (PAAS)
## Platform as a Service (PaaS)
Platform as a Service (PaaS) adalah serangkaian layanan untuk membangun dan mengelola
aplikasi modern di era digital²on-premise atau di cloud. PaaS merupakan platform pengembangan
dan penerapan aplikasi yang terstandarisasi, dapat dibagikan (shared), dan dapat diskalakan secara
elastis (elastically scalable) yang dikemas sebagai sebuah layanan. Platform ini biasanya mencakup
database dan middleware, serta kemampuan pengembangan, manajemen, keamanan, dan integrasi,
yang keseluruhannya disampaikan sebagai sebuah layanan. PaaS memberikan infrastruktur dan
komponen middleware yang memungkinkan pengembang (developer), administrator TI, dan
pengguna akhir untuk membangun, mengintegrasikan, bermigrasi, menyebarkan, mengamankan, dan
mengelola aplikasi seluler (mobile) dan web.

## Adapun layanan yang ditawarkan PaaS diantaranya yaitu :
- Kecerdasan buatan (AI)
- Chatbots
- Blockchain -> ledger data terdesentralisasi yang dibagikan dengan aman
- Internet of Things (IoT)

## Pentingnya Platform as a Service (PaaS)
- Penyediaan kapasitas yang cepat (mendekati waktu nyata) terhadap server fisik
- Aplikasi yang sangat dioptimalkan untuk rasio server dan kemampuan untuk mematikan kapasitas cadangan (spare capacity)
- Pemantauan lintas domain dan peringatan yang proaktif (proactive alerting)
- Fasilitas pengukuran untuk menetapkan parameter penggunaan untuk penyewa PaaS

Pada pertemuan ini membahas tentang database virtual machine atau bisa disebut dengan database instance. 
Database instance ini adalah mesin virtual yang mempunyai service penyimpanan database seperti: mysql, oracle no sql, mariadb, 
postgree, dan databse yang lain. Dalam oracle cloud infrasture ada yang namanya database instance yang berfungsi untuk membuat 
atau mendevelop sebuah database instance yang bisa di isi berbagai macam engine database. Pada pertemuan kali ini di jelaskan 
bahwa untuk komunikasi antara virtual machine degan database instance itu dengan ip private yang koneksinya di management di vcn 
atau virtual cloud network oracle cloud infrastucture untuk koneksinya sendiri sebagai jembatan bisa menggunakan engine client.
Contoh nya mysql client dan untuk koneksi dengan assets yang di vitrual machine biasanya diatur dalam .env. 

Untuk awal praktikum, kita bisa langsung coba untuk membuat atau mendevelop database instance di oracle cloud insfrastructure. 
Lalu di coba untuk memanagement koneksi antara database instance dengan vm instance dengan mengatur virtual cloud network dengan 
membuka port database yang disupport.