Ada 3 tipe docker network, diantaranya yaitu :
•	Bridge
•	Host 
•	None 

DockerVolumeDriver
Volume juga memiliki beberapa jenis agar mampu terintegrasi dengan jenis penyimpanan yang lain. Berikut beberapa jenis dari Volume diantaranya yaitu :
•	Docker volume driver for Azure file storage yaitu digunakan Azure file storage untuk mount file yang dishare pada cloud ke Docker container sebagai volume.
•	IPFS(InterPlanetary File System) adalah Plugin volume open source yang mengizinkan menggunakan sebuah IPFS filesystem sebagai sebuah volume. IPFS adalah sebuah sistem storage yang memungkinkan dalam mendistribusikan high volume data dengan efisiensi yang tinggi.
•	Keywhiz = Untuk membuat container berkomunikasi secara remote pada server Keywhiz. Keywhiz adalah sistem untuk mengelola dan mendistribusikan data yang bersifat rahasia dengan lebih mudah dan lebih aman, seperti TLS certificate/keys, GPG keys, API tokens, dan database credential.

DOcker Compose
Docker compose adalah sebuah tool untuk mendefiniskan, launching, dan mengelola service yang didefinisikan sebagai satu atau lebih dari sebuah docker container. Service dan sistem service didefinisikan di dalam file YAML dan mengelolanya menggunakan perintah command-line docker-compose. Berikut beberapa kegunaan Docker Compose diantaranya yaitu :
•	Untuk build docker image
•	Menjalankan aplikasi container sebagai service
•	Menjalankan full system dari service
•	Mengelola secara individu service pada sebuah sistem
•	Melakukan scaling up atau down
•	Melihat log dari kumpulan container yang berjalan sebagai service
