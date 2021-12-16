# Pertemuan 15
## High Availability on Cloud Environment

### Menghitung ketersediaan
- Ketersediaan tidak dapat dihitung. Itu hanya dapat dilaporkan setelahnya, ketika sistem telah berjalan selama beberapa tahun
- Selama bertahun-tahun, banyak pengetahuan dan pengalaman diperoleh tentang bagaimana merancang sistem yang tersedia tinggi: kegagalan, Redundansi, Pemrograman terstruktur, Menghindari Satu Poin, Kegagalan (SPOFs), Menerapkan manajemen sistem

### MTBF and MTTR
- Mean Time Between Failures (MTBF): Waktu rata-rata yang berlalu di antara kegagalan
- Mean Time To Repair (MTTR): Waktu yang dibutuhkan untuk pulih dari kegagalan

### Sumber ketidaktersediaan - kesalahan manusia
- 80% pemadaman yang berdampak pada layanan mission-critical disebabkan oleh orang dan masalah proses
- Contoh:
    - Melakukan tes di lingkungan produksi
    - Mematikan komponen yang salah untuk diperbaiki
    - Menukar disk yang berfungsi baik dalam kumpulan RAID alih-alih yang rusak
    - Memulihkan pita cadangan yang salah ke produksi
    - Tidak sengaja menghapus file
    - Folder email, file konfigurasi
    - Tidak sengaja menghapus entri basis data
    - Jatuhkan tabel x alih-alih jatuhkan tabel y

### Sumber ketidaktersediaan - bug perangkat lunak
- Karena kerumitan sebagian besar perangkat lunak, hampir tidak mungkin (dan sangat mahal) untuk membuat perangkat lunak bebas bug
- Bug perangkat lunak aplikasi dapat menghentikan seluruh sistem
- Sistem operasi juga perangkat lunak
    - Sistem operasi yang mengandung bug dapat menyebabkan sistem file rusak, kegagalan jaringan, atau sumber ketidaktersediaan lainnya

### Sumber ketidaktersediaan - pemeliharaan terencana
- Terkadang diperlukan untuk melakukan tugas manajemen sistem:
    - Meningkatkan perangkat keras atau perangkat lunak
    - Menerapkan perubahan perangkat lunak
    - Migrasi data
    - Pembuatan cadangan
- Hanya boleh dilakukan pada bagian infrastruktur di mana bagian lain tetap melayani klien
- Selama pemeliharaan terencana, sistem lebih rentan terhadap waktu henti daripada dalam keadaan normal
    - SPOF sementara dapat diperkenalkan
    - Manajer sistem bisa membuat kesalahan

### Sumber ketidaktersediaan - cacat fisik
- Semuanya rusak pada akhirnya
- Bagian mekanis kemungkinan besar akan rusak terlebih dahulu
- Contoh:
    - Kipas untuk peralatan pendingin biasanya pecah karena debu di bantalan
    - Disk drive berisi bagian yang bergerak
    - Kaset sangat rentan terhadap cacat karena pita diputar dan dimatikan sepanjang waktu
    - Tape drive berisi bagian mekanik yang sangat sensitif yang dapat dengan mudah pecah

### Redudancy
- Redundansi adalah duplikasi komponen kritis dalam satu sistem, untuk menghindari satu titik kegagalan (SPOF)
- Contoh:
    - Sebuah komponen tunggal memiliki dua catu daya; jika satu gagal, yang lain mengambil alih
    - Antarmuka jaringan ganda
    - Kabel redundan

### Failover
- Failover adalah peralihan (semi) otomatis ke sistem atau komponen siaga
- Contoh:
    - Pengelompokan failover Windows Server
    - Ketersediaan Tinggi VMware
    - Database Oracle Real Application Cluster (RAC)

### Fallback
- Fallback adalah peralihan manual ke sistem komputer siaga yang identik di lokasi yang berbeda
- Biasanya digunakan untuk pemulihan bencana
- Tiga bentuk dasar solusi fallback:
    - Situs panas
    - Situs dingin
    - Situs hangat
