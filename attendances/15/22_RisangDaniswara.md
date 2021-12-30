# High Availability on Cloud Environment

- AVAILABILITY
 - Semua orang ingin infrastruktur mereka selalu aktif 
 - 100% avaibilitas dari infrastruktur adalah tidak mungkin 

- Calculating availability
 - Ketersediaan tidak dapat dihitung, atau dijamin 
 - Selama bertahun-tahun, banyak pengetahuan dan pengalaman diperoleh tentang bagaimana merancang sistem yang tersedia terus menerus
 - Ketersediaan sistem biasanya dinyatakan sebagai persentase waktu aktif dalam periode waktu tertentu selama satu tahun atau satu bulan
 - Persyaratan umum yang digunakan dalam perjanjian tingkat layanan saat ini adalah ketersediaan 99,8% atau 99,9% per bulan untuk sistem TI lengkap
 - Amazon, Google, dan Microsoft menetapkan SLA cloud mereka pada 99,9% 
 - Ketersediaan infrastruktur harus jauh lebih tinggi Biasanya di kisaran 99,99% atau lebih tinggi
 - Waktu aktif 99,999% juga dikenal sebagai ketersediaan tingkat Carrier Grade
 
# Sources of unavailability - human errors 

 - 80% pemadaman yang berdampak pada layanan mission-critical disebabkan oleh Person Error dan masalah proses
 Contohnya : 
 - Melakukan tes di proses produksi
 - Mematikan komponen yang salah untuk diperbaiki 
 - Menukar disk yang berfungsi baik dalam kumpulan RAID alih-alih yang rusak
 - Memulihkan pita cadangan yang salah ke produksi 
 - Tidak sengaja menghapus file

# Sources of unavailability - software bugs
 - Karena kerumitan sebagian besar perangkat lunak, hampir tidak mungkin (dan sangat mahal) untuk membuat perangkat lunak bebas bug
 - Bug perangkat lunak aplikasi dapat menghentikan seluruh sistem
 - Sistem operasi juga perangkat lunak

# Sources of unavailability - planned maintenance
 - Terkadang diperlukan untuk melakukan tasks manajemen sistem, sperti : upgrade software, implementasi perubahan, migrasi data, pembuatan dan backups
 - Hanya boleh dilakukan pada bagian infrastruktur di mana bagian lain tetap melayani klien
 - Selama pemeliharaan terencana, sistem lebih rentan terhadap waktu henti daripada dalam keadaan normal

# Sources of unavailability - physical defects
 - Semuanya rusak pada akhirnya
 - Bagian mekanis kemungkinan besar akan rusak terlebih dahulu

# Sources of unavailability - environmental issues
 - Bencana Alam
 - Fasilitas rusak

# Sources of unavailability - complexity of the infrastructure
 - Menambahkan lebih banyak komponen ke desain sistem secara keseluruhan dapat merusak ketersediaan tinggi
 - Complex systems
 - Terkadang lebih baik memiliki sistem cadangan ekstra di Storage daripada menggunakan sistem redundan yang rumit 

# Redundancy 
 - Redundansi adalah duplikasi komponen kritis dalam satu sistem, untuk menghindari satu titik kegagalan (SPOF)

# Failover
 - Failover adalah peralihan (semi) otomatis ke sistem atau komponen siaga

# Fallback
 - Fallback adalah peralihan manual ke sistem komputer siaga yang identik di lokasi yang berbeda