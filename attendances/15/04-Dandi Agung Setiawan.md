# Resume Pertemuan 15 - High Availability on Cloud Environment

## Menghitung ketersediaan
1. Ketersediaan tidak dapat dihitung. Itu hanya dapat dilaporkan setelahnya, ketika sistem telah berjalan selama beberapa tahun
2. Selama bertahun-tahun, banyak pengetahuan dan pengalaman diperoleh tentang bagaimana merancang sistem yang tersedia tinggi: kegagalan, Redundansi, Pemrograman terstruktur, Menghindari Satu Poin, Kegagalan (SPOFs), Menerapkan manajemen sistem

## MTBF and MTTR
1. Mean Time Between Failures (MTBF): Waktu rata-rata yang berlalu di antara kegagalan
2. Mean Time To Repair (MTTR): Waktu yang dibutuhkan untuk pulih dari kegagalan

## Sumber ketidaktersediaan - kesalahan manusia
1. 80% pemadaman yang berdampak pada layanan mission-critical disebabkan oleh orang dan masalah proses
Contoh:
- Melakukan tes di lingkungan produksi
- Mematikan komponen yang salah untuk diperbaiki
- Menukar disk yang berfungsi baik dalam kumpulan RAID alih-alih yang rusak
- Memulihkan pita cadangan yang salah ke produksi
- Tidak sengaja menghapus file
- Folder email, file konfigurasi
- Tidak sengaja menghapus entri basis data
- Jatuhkan tabel x alih-alih jatuhkan tabel y

## Sumber ketidaktersediaan - bug perangkat lunak
1. Karena kerumitan sebagian besar perangkat lunak, hampir tidak mungkin (dan sangat mahal) untuk membuat perangkat lunak bebas bug
2. Bug perangkat lunak aplikasi dapat menghentikan seluruh sistem
3. Sistem operasi juga perangkat lunak. Sistem operasi yang mengandung bug dapat menyebabkan sistem file rusak, kegagalan jaringan, atau sumber ketidaktersediaan lainnya

## Sumber ketidaktersediaan - pemeliharaan terencana
1. Terkadang diperlukan untuk melakukan tugas manajemen sistem:
- Meningkatkan perangkat keras atau perangkat lunak
- Menerapkan perubahan perangkat lunak
- Migrasi data
- Pembuatan cadangan
2. Hanya boleh dilakukan pada bagian infrastruktur di mana bagian lain tetap melayani klien
3. Selama pemeliharaan terencana, sistem lebih rentan terhadap waktu henti daripada dalam keadaan normal
- SPOF sementara dapat diperkenalkan
- Manajer sistem bisa membuat kesalahan

## Sumber ketidaktersediaan - cacat fisik
1. Semuanya rusak pada akhirnya
2. Bagian mekanis kemungkinan besar akan rusak terlebih dahulu
Contoh:
- Kipas untuk peralatan pendingin biasanya pecah karena debu di bantalan
- Disk drive berisi bagian yang bergerak
- Kaset sangat rentan terhadap cacat karena pita diputar dan dimatikan sepanjang waktu
- Tape drive berisi bagian mekanik yang sangat sensitif yang dapat dengan mudah pecah