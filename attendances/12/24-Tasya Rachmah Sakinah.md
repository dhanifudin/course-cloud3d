# Pertemuan 12
## Introduction CI/CD
- CI/CD adalah metode untuk mengirimkan aplikasi ke pelanggan dengan memperkenalkan otomatisasi ke dalam tahapan pengembangan aplikasi.
- "CI" dalam CI/CD selalu mengacu pada integrasi berkelanjutan, yang merupakan proses otomatisasi untuk pengembang. CI yang berhasil berarti perubahan kode baru pada aplikasi secara teratur dibuat, diuji, dan digabungkan ke repositori bersama
- "CD" dalam CI/CD mengacu pada pengiriman berkelanjutan dan/atau penerapan berkelanjutan, yang merupakan konsep terkait yang terkadang digunakan secara bergantian.

## CI/CD Overview
- Dalam pengembangan perangkat lunak, beberapa anggota tim mengembangkan kode dan berkontribusi untuk menciptakan fungsionalitas perangkat lunak. Ketika beberapa orang berkontribusi pada basis kode, penting untuk menjaga integritasnya dan memastikan bahwa setiap anggota tim dapat mengambil versi terbaru dan membangun serta menjalankannya secara lokal.
- Dua aspek penting harus dipertahankan untuk menjamin stabilitas basis kode. Aspek pertama adalah memastikan bahwa kode dikompilasi tanpa kesalahan. Aspek kedua adalah memastikan bahwa semua pengujian unit yang memvalidasi perilaku kode lulus, termasuk perubahan kode terbaru, dengan persentase yang sangat tinggi.

## Introduction to GitHub Actions
- GitHub Actions adalah serangkaian tindakan dalam alur kerja repositori GitHub.
- Action: Blok penyusun terkecil dari alur kerja adalah tindakan, yang dapat diidentifikasi sebagai tugas individu.
- Artifacts: File yang dihasilkan saat Anda membangun proyek perangkat lunak atau menguji proyek perangkat lunak Anda adalah artefak.
- Event: Peristiwa memicu alur kerja di GitHub Actions. Setelah perubahan kode didorong, atau permintaan tarik dibuat, sebuah peristiwa dapat diatur di GitHub Actions untuk memicu alur kerja.

## GitHub Actions
- GitHub-Hosted Runners: Hosted runner adalah mesin yang mirip dengan agen yang dihosting di saluran Azure DevOps. Mereka didukung di Windows, Linux, dan macOS.
- Job: Pekerjaan adalah serangkaian langkah yang disiapkan untuk dijalankan dalam satu pelari.
- Self-Hosted Runner: Pelari yang dihosting sendiri berguna saat memiliki konfigurasi perangkat keras khusus atau persyaratan perangkat lunak untuk membangun aplikasi atau menjalankan pekerjaan Anda.
- Step: Tugas yang merupakan tindakan atau perintah diidentifikasi sebagai langkah. Semua langkah dalam pekerjaan dijalankan di runner yang sama.
- Workflow: Dalam repo GitHub, proses yang disiapkan dalam file YAML yang mendefinisikan tugas build, pengujian, paket, atau penerapan disebut alur kerja.
- Workflow File: File YAML yang disimpan di folder github/alur kerja/ di repositori GitHub Anda adalah file alur kerja.
- Workflow Run: Alur kerja dijalankan berdasarkan pemicu/peristiwa yang telah dikonfigurasi sebelumnya.

## Secrets and Token
Rahasia penting dalam alat implementasi pipa CI/CD apa pun. Mereka melindungi informasi sensitif, seperti string koneksi dan kata sandi, dan menyimpan kata sandi atau rahasia lain yang diterapkan dalam pengaturan konfigurasi aplikasi.
