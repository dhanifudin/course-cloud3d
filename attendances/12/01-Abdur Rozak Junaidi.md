<h1>CI/CD</h1>

**Pengenalan CI/CD**
- CI/CD adalah metode untuk sering mengirimkan aplikasi ke pelanggan dengan memperkenalkan otomatisasi ke dalam tahapan pengembangan aplikasi.
- "CI" dalam CI/CD selalu mengacu pada integrasi berkelanjutan, yang merupakan proses otomatisasi untuk pengembang. CI yang berhasil berarti perubahan kode baru pada aplikasi secara teratur dibuat, diuji, dan digabungkan ke repositori bersama.
- "CD" dalam CI/CD mengacu pada pengiriman berkelanjutan dan/atau penerapan berkelanjutan, yang merupakan konsep terkait yang terkadang digunakan secara bergantian.

**CI/CD Overview**
- Dalam pengembangan perangkat lunak, beberapa anggota tim mengembangkan kode dan berkontribusi untuk menciptakan fungsionalitas perangkat lunak. 
- Dua aspek penting harus dipertahankan untuk menjamin stabilitas basis kode :
	- memastikan bahwa kode dikompilasi tanpa kesalahan. 
	- memastikan bahwa semua pengujian unit yang memvalidasi perilaku kode lulus, termasuk perubahan kode terbaru, dengan persentase yang sangat tinggi.

**Introduction to GitHub Actions**.
GitHub adalah serangkaian tindakan dalam alur kerja repositori GitHub. 
- Action : Blok bangunan terkecil dari alur kerja yaitu tindakan yang dapat diidentifikasi sebagai tugas individu.
- Artifacts : File yang dihasilkan saat Anda membangun proyek perangkat lunak atau menguji proyek perangkat lunak Anda adalah artefak.
- Event : Peristiwa memicu alur kerja di GitHub Actions. 

**GitHub Actions**
- GitHub-Hosted Runners: Hosted runner yaitu mesin yang mirip dengan agen yang dihosting di saluran Azure DevOps yang didukung di Windows, Linux, dan macOS. 
- Job : langkah yang disiapkan untuk indivdu yang terdiri dari satu atau lebih tindakan.
- Self-Hosted Runner: berguna saat Anda memiliki konfigurasi perangkat keras khususuntuk membangun aplikasi suatu pekerjaan.

- Step : Tugas yang merupakan perintah diidentifikasi sebagai langkah. 
- Work : Dalam repo GitHub, proses yang disiapkan dalam file YAML yang mendefinisikan tugas build, pengujian, paket, atau penerapan disebut alur kerja.
- Workflow File: File YAML yang disimpan di folder github/alur kerja/ di repositori GitHub.

**Secrets dan Token**
penting dalam alat implementasi pipa CI/CD apa pun. Dapat melindungi informasi sensitif, seperti string koneksi dan kata sandi, dan menyimpan kata sandi atau rahasia lain yang diterapkan dalam pengaturan konfigurasi aplikasi.

