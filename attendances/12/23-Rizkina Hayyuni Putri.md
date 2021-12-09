## CI/CD
CI/CD adalah adalah proses pengintegrasian kode ke dalam repositori kode lalu akan dijalankan pengujian secara otomatis, cepat, dan sering, 
setelah itu aplikasi bisa dibangun lalu dirilis secara otomatis. 
Automated test memastikan fungsi aplikasi tersebut dapat sesuai dengan yang diharapkan ketika didorong ke lingkungan produksi hingga ke tangan 
pengguna yang sebenarnya (real users).


## Aspek Stabilitas Basis Kode
Terdapat 2 aspek yang perlu diperhatikan untuk menjamin stabilitas basis kode, yaitu seperti berikut ini:
1. Aspek untuk memastikan bahwa kode dikompilasi tanpa kesalahan.
2. Aspek untuk memastikan bahwa semua unit test yang memvalidasi perilaku kode lulus, termasuk perubahan kode terbaru dengan persentase yang sangat tinggi.

## Github Actions
Ada beberapa istilah dalam Github Action yitu :
1. Action : Block building terkecil dari workflow yang dapat diidentifikasi sebagai tugas individu.
2. Artifacts : File yang dihasilkan saat membangun proyek software atau menguji proyek software.
3. Event : Peristiwa yang memicu workflow di GitHub Actions. Setelah perubahan kode di-push, atau pull request dibuat, sebuah peristiwa dapat diatur di GitHub Actions untuk memicu workflow.
4. GitHub-Hosted Runners : Mesin yang mirip dengan agen yang dihosting di saluran Azure DevOps.
5. Job : Serangkaian langkah yang disiapkan untuk dijalankan dalam single runner. Sebuah job dapat terdiri dari satu atau lebih action.
6. Self-Hosted Runner : Berguna saat memiliki konfigurasi hardware khusus atau persyaratan software untuk membangun aplikasi atau menjalankan job.
7. Step : Tugas yang merupakan action atau command yang diidentifikasi sebagai langkah. Semua step dalam job dijalankan di runner yang sama.
8. Workflow : Dalam repo GitHub, proses yang disiapkan dalam file YAML yang mendefinisikan tugas/job build, build, test, package, atau deployment
9. Workflow File : File YAML yang disimpan di folder github/workflows/ di repositori GitHub.
10. Workflow Run : Workflow dijalankan berdasarkan pemicu/peristiwa yang telah dikonfigurasi sebelumnya.
