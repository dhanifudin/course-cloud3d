# CI/CD

_Continuous Integration_ dan _Continuous Deployment_ atau biasa disingkat CI/CD adalah suatu konsep otomasi yang membantu pekerjaan programmer untuk melakukan suatu hal yang sama tanpa perlu menjalankannya secara manual.

### CI (Continuous Integration)

Mengacu pada integrasi secara berkelanjutan yang dimana mengautomasi suatu proses untuk developer. Ci yang berhasil dijalankan berarti perubahan kode program baru pada aplikasi yang dibentuk secara teratur, teruji, dan tergabung di repositori yang sama.

### CD (Continuous Delivery)

Merupakan suatu proses untuk melakukan deploy aplikasi secara otomatis pada _environment production_.

### CI/CD Ilustration

1. Continuous Integration

   - Build

   - Test

   - Merge

2. Continuous Delivery

   - Automatically release to repository

3. Continuous Deployment

   - Automatically Deploy To Production

### Github Actions

_Github Actions_ merupakan sekumpulan aksi yang terdapat pada _workflow_ repositoy Github.

- **Action** : Bagian blok terkecil dalam sebuah workflow, dapat diidentifikasikan sebagai tugas individu.

- **Artifacts** : File yang digenerate pada saat membangun software.

- **Event** : Sebuah trigger workflow yang terdapat di Github Actions. Trigger dapat disetup pada saat melakukan push code ke Github maupun pull request yang telah dibuat.

- **GitHub-Hosted Runners** : Sebuah mesin yang melakukan hosted agent pada Azure DevOps pipelines. Support pada OS Windows, Linux dan MacOS.

- **Job** : Merupakan langkah yang didefinisikan untuk menjalankan suatu actions.

- **Self-Hosted Runner** : Sangat bermanfaat ketika build sebuah aplikasi yang memiliki spesial hardware yang dikonfigurasi atau beberapa software requirement.

- **Step** : Sebuah tugas yang berisi aksi atau perintah untuk menjalankan job.

- **Workflow** : Proses yang disetup pada file YAML untuk mendefinisikan build, test, package, atau deployment jobs.

- **Workflow File** : File YAML yang disimpan pada github/workflows/ folder di repositori Github.

- **Workflow Run** : Sebuah workflow yang mengeksekusi berdasarkan prekonfigurasi trigger/events.

### Variable

Pada umumnya, kita dapat mendeklarasikan variable pada sistem CI/CD. Berikut ini contoh yang terdapat pada Github Actions :

    env :

    varname1: value1

    varname2: value2

### Secret and Tokens

Digunakan untuk memproteksi informasi yang bersifat sensitif seperti koneksi dan password yang diterapkan pada pengaturan konfigurasi aplikasi.
