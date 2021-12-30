# CI/CD

## Continuous Integration (CI)
Yaitu integrasi yang terjadi secara berkelanjutan. CI yang berhasil berarti adanya perubahan kode pada aplikasi dibuat, diuji, dan digabungkan ke repositori bersama.

## Continuous Delivery (CD)
Yaitu penerapan yang terjadi secara otomatis setelah adanya perubahan kode pada aplikasi.

## Github Actions
Github action merupakan sekumpulan aksi yang terjadi dalam aliran kerja repository github.
* Action : bagian terkecil dari sebuah aliran kerja, yang diidentifikasi sebagai tugas individual.
* Artifacts : berkas yang diciptakan ketika membangun project aplikasi.
* Event : sebuah event yang memicu terjadinya aliran kerja Github Actions.
* Github-Hosted Runners: Hosted Runners adalah sebuah mesin untuk menjalankan pipeline dari CI/CD yang terdapat dalam github actions.
* Job : job merupakan langkah untuk mengerjakan sebuah perintah, sebuah job dapat terdiri dari satu atau lebih actions.
* Self hosted runner : mesin ini berguna ketika memiliki konfigurasi khusus untuk hardware yang diperlukan.
* Step : sebuah tugas yang dijalankan sebagai action diidentifikasi sebagai step.
* Workflow : dalam repository github, proses dimasukkan ke dalam file yaml yang mendefinisikan pembuatan, pemeriksaan, pembuatan package maupun pengaplikasian jobs.
* Workflow file : file yml disimpan di dalam folder github/workflows
* Workflow run : sebuah workflow mengeksekusi perintah berdasarkan event yang telah ditentukan.

## Variabel
Dalam sistem CI/CD kita dapat menambahkan variabel yang diinginkan, seperti
```
varname1: value1
varname2: value2
```

## Secrets and Token
Secrets sangat penting untuk alat pengimplementasi dalam CI/CD. Secret melindungi informasi-informasi penting yang nantinya akan digunakan untuk deployment aplikasi seperti password, kunci autentikasi, username, dll.