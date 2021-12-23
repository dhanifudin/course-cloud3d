# Autoscalling dan Availability

## Availability
Setiap orang pasti menginginkan infrastrukturnya selalu tersedia kapanpun. Akan tetapi infrastruktur tidak dapat menjamin ketersediaan sempurna yang mencapai 100%.

### Calculating Availability
* Availability tidak dapat dihitung atau dijanjikan di awal, akan tetapi availability dapat dilaporkan setelahnya setelah sebuah sistem telah berjalan dalam beberapa tahun.
* Ketersediaan sistem biasanya disajikan dengan persentase dalam jangka waktu tertentu, biasanya dalam setahun atau sebulan.

### MTBF and MTTR
* MTBF (Mean Time Between Failures) yaitu waktu rata-rata yang terjadi di antara tiap kesalahan.
* MTTR (Mean Time To Repair) yaitu waktu yang dibutuhkan untuk melakukan perbaikan dari kesalahan yang terjadi.

### Sumber dari ketidak tersediaan.
* Human Errors, 80% dari kesalahan disebabkan oleh manusia dan isu proses, sebagai contoh melakukan pengujian dalam lingkungan produksi, mematikan sebuah komponen untuk memperbaiki hal lain, menghapus data dalam RAID yang sedang bagus bukannya menghapus data dalam RAID yang sedang bermasalah.
* Software bugs, karena adanya kompleksitas dari sebuah aplikasi maka nantinya hampir tidak mungkin untuk membuat aplikasi yang bebas dari bug. Sebuah bug dapat menghentikan seluruh sistem.
* Perbaikan terencana, terkadangan sistem memerlukan manajemen sistem yang terstruktur, seperti meningkatkan hardware maupun software, migrasi data, dan pembuatan backup.

## Autoscalling
Kemampuan autoscalling merupakan kemampuan yang harus dimiliki sebuah infrastruktur yang memiliki trafik berubah-ubah. Sebagai contoh toko online yang memiliki trafik rendah di saat malam hari, sedangkan ketika memasuki jam kerja yaitu antara pukul 6 sampai 10 pagi maka trafik sedang tinggi. Untuk mengatasi hal tersebut sebaiknya dilakukan autoscalling, dimana infrastruktur yang dijalankan bisa menyesuaikan dengan kebutuhan komputasi pada saat itu