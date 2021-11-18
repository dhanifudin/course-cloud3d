# CI/CD

### Continuous integration (CI)
CI adalah pengintegrasian kode ke dalam repositori kode kemudian menjalankan pengujian secara otomatis, cepat, dan sering. Biasanya dilakukan menggunakan commit. 
### Continous Delivery atau Continuous Deployment (CD) 
CD adalah praktik yang dilakukan setelah proses CI selesai dan seluruh kode berhasil terintegrasi, sehingga aplikasi bisa dibangun lalu dirilis secara otomatis.

Jadi CI/CD adalah metode untuk mengirimkan aplikasi ke pengguna dengan menggunakan otomatisasi ke dalam tahap pengembangan software. 
Dengan menggunakan CI/CD kita dapat mendeploy suatu aplikasi sesuai dengan code yang telah didefinisikan pada sebuah file dengan format .yml 

### Tools untuk CI/CD
1. Github
2. Gitlab CI/CD
3. Jenkins

## CI/CD Ilustration
1. Continuous Integration
   - Build
   - Test
   - Merge
2. Continuous Delivery
   - Automatically release to repository
3. Continuous Deployment
   - Automatically Deploy To Production

## Github Action
*Github action* adalah serangkaian tindakan dalam alur kerja repository GitHub.
  - Action : Bagian blok terkecil dalam sebuah workflow, dapat diidentifikasikan sebagai tugas individu.

  - Artifacts : File yang digenerate pada saat membangun software.

  - Event : Sebuah trigger workflow yang terdapat di Github Actions. Trigger dapat disetup pada saat melakukan push code ke Github maupun pull request yang telah dibuat.

  - GitHub-Hosted Runners : Sebuah mesin yang melakukan hosted agent pada Azure DevOps pipelines. Support pada OS Windows, Linux dan MacOS.

  - Job : Merupakan langkah yang didefinisikan untuk menjalankan suatu actions.

  - Self-Hosted Runner : Sangat bermanfaat ketika build sebuah aplikasi yang memiliki spesial hardware yang dikonfigurasi atau beberapa software requirement.

  - Step : Sebuah tugas yang berisi aksi atau perintah untuk menjalankan job.

  - Workflow : Proses yang disetup pada file YAML untuk mendefinisikan build, test, package, atau deployment jobs.

  - Workflow File : File YAML yang disimpan pada github/workflows/ folder di repositori Github.

  - Workflow Run : Sebuah workflow yang mengeksekusi berdasarkan prekonfigurasi trigger/events.

## Secret and Tokens
Secret penting dalam tool implementasi pipeline CI/CD apapun. Tujuannya melindungi informasi sensitive, seperti connection strings dan passwords, 
serta menyimpan password atau rahasia lain yang diterapkan dalam pengaturan konfigurasi aplikasi.


