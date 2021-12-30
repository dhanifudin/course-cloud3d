# PERTEMUAN 12
## CI/CD
CI/CD adalah metode untuk sering mengirimkan aplikasi ke pelanggan dengan memperkenalkan otomatisasi ke dalam tahap pengembangan aplikasi "CI" dalam CI/CD selalu mengacu pada integrasi berkelanjutan, yang merupakan proses otomatisasi untuk pengembang. CI yang berhasil berarti perubahan kode baru pada aplikasi secara teratur dibuat, diuji, dan digabungkan ke repositori bersama "CD" dalam CI/CD mengacu pada pengiriman berkelanjutan dan/atau penerapan berkelanjutan, yang merupakan konsep terkait yang terkadang digunakan secara bergantian.
### Manfaat dari CI/CD
* Mendapat feedback lebih cepat
* Dapat mendeteksi bug lebih cepat
* Dapat mempercepat proses rilis
## GitHub Actions
GitHub Actions adalah serangkaian tindakan dalam alur kerja repositori GitHub. Berikut beberapa istilah dalam Github Action yang perlu diketahui :
* Action : Block building terkecil dari workflow yang dapat diidentifikasi sebagai tugas individu.
* Artifacts : File yang dihasilkan saat membangun proyek software atau menguji proyek software.
* Event : Peristiwa yang memicu workflow di GitHub Actions. Setelah perubahan kode di-push, atau pull request dibuat, sebuah peristiwa dapat diatur di GitHub Actions untuk memicu workflow.
* GitHub-Hosted Runners : Mesin yang mirip dengan agen yang dihosting di saluran Azure DevOps.
* Job : Serangkaian langkah yang disiapkan untuk dijalankan dalam single runner. Sebuah job dapat terdiri dari satu atau lebih action.
* Self-Hosted Runner : Berguna saat memiliki konfigurasi hardware khusus atau persyaratan software untuk membangun aplikasi atau menjalankan job.
* Step : Tugas yang merupakan action atau command yang diidentifikasi sebagai langkah. Semua step dalam job dijalankan di runner yang sama.
* Workflow : Dalam repo GitHub, proses yang disiapkan dalam file YAML yang mendefinisikan tugas/job build, build, test, package, atau deployment
* Workflow File : File YAML yang disimpan di folder github/workflows/ di repositori GitHub.
* Workflow Run : Workflow dijalankan berdasarkan pemicu/peristiwa yang telah dikonfigurasi sebelumnya.
## Secrets and Token
Secrets penting dalam alat implementasi CI/CD pipeline apa pun. Mereka melindungi informasi sensitif, seperti string koneksi dan kata sandi, dan menyimpan password atau rahasia lain yang diterapkan dalam pengaturan konfigurasi aplikasi.
