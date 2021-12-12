# Konsep CI/CD
Dalam pengembangan perangkat lunak, beberapa anggota tim berkembang kode dan berkontribusi untuk membuat perangkat lunak Kegunaan. Ketika banyak orang berkontribusi pada sebuah kode dasar, penting untuk menjaga integritasnya dan memastikan bahwa setiap anggota tim dapat mengambil versi terbaru dan membangun dan menjalankannya secara lokal. Dua aspek penting harus dipertahankan untuk menjamin stabilitas basis kode. Aspek pertama adalah memastikan bahwa kode dikompilasi tanpa kesalahan. Aspek kedua adalah untuk memastikan bahwa semua pengujian unit yang memvalidasi perilaku kode lulus, termasuk perubahan kode terbaru, dengan harga yang sangat tinggi persentase.

# Github Actions
Github Actions adalah serangkaian tindakan dalam repositori GitHub
## Cara Kerja
- **Action**: Blok bangunan terkecil dari alur kerja adalah action, yang dapat diidentifikasi sebagai tugas individu.
- **Artifacts**: File yang dihasilkan saat Anda membuat perangkat lunak proyek atau uji proyek perangkat lunak Anda adalah actifact.
- **Event**: Event memicu alur kerja di GitHub Actions. Setelah perubahan kode didorong, atau permintaan tarik dibuat, sebuah acara dapat diatur di GitHub Actions untuk memicu alur kerja.

# Secrets and Tokens
Secrets penting dalam setiap saluran CI/CD alat implementasi. Mereka melindungi sensitif informasi, seperti string koneksi dan kata sandi, dan simpan kata sandi atau rahasia lainnya diterapkan dalam pengaturan konfigurasi aplikasi.