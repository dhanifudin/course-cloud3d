# Rangkuman Pertemuan 12
# CI/CD
CI/CD adalah metode untuk mengirimkan aplikasi ke pengguna dengan menggunakan otomatisasi ke dalam tahap pengembangan software.
"CI" dalam CI/CD selalu mengacu pada integrasi berkelanjutan, yang merupakan proses otomatisasi untuk pengembang. 
CI yang berhasil berarti perubahan kode baru pada aplikasi secara teratur dibuat, diuji, dan digabungkan ke repositori bersama.
Dengan menggunakan CI/CD kita dapat mendeploy suatu aplikasi sesuai dengan code yang telah didefinisikan pada sebuah file dengan format .yml
Contoh CI/CD
1. Github
2. Gitlab
3. Jenkins

# Ilustrasi CI/CD
CI(Continuous Integartion)          Continuous Delivery            Continuous Deployment
Build => Test => Merge => secara otomatis merilis ke repositori => secara otomastis deploy ke produksi

# Github Action
Github action adalah serangkaian tindakan dalam alur kerja repositori GitHub.
* Action: Blok bangunan terkecil dari alur kerja yang dapat diidentifikasi sebagai tugas individu.
* Artifacts: File yang dihasilkan saat membangun proyek perangkat lunak atau menguji proyek perangkat lunak.
* Event: Suatu peristiwa memicu alur kerja di GitHub Actions. Setelah perubahan kode 
dipush, atau pull request, sebuah event dapat diatur di GitHub Actions untuk memicu alur kerja.
* Github Host: Runner yang dihosting adalah mesin yang mirip dengan agen yang dihosting di pipeline Azure DevOps. Mereka didukung di Windows, Linux, dan macOS.
* Job: Adalah serangkaian langkah yang disiapkan untuk dijalankan dalam single runner. Sebuah job dapat terdiri dari satu atau lebih action.
* Self-Hosted: Berguna saat kita memiliki konfigurasi perangkat keras khusus atau persyaratan perangkat lunak untuk membangun aplikasi atau menjalankan pekerjaan.
* Step: merupakan tindakan atau perintah. Semua step dalam pekerjaan dijalankan di runner yang sama.
* Workflow: Dalam repo GitHub, proses yang disiapkan dalam file YAML yang mendefinisikan pekerjaan build, test, package, atau deployment.
* Workflow file: File YAML yang disimpan di folder github/workflow/ di repositori GitHub 
* Workflow run: Workflow executes dijalankan berdasarkan trigger/events yang telah dikonfigurasi sebelumnya.

# Secrets and Token
Secrets penting dalam alat implementasi CI/CD pipeline. Konfigurasi tersebut melindungi
informasi sensitif, seperti string koneksi dan kata sandi, dan menyimpan kata sandi atau 
rahasia lain yang diterapkan dalam pengaturan konfigurasi aplikasi.