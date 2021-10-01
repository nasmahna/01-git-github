# Pengertian
Git merupakan software berbasis Version Control System (VCS) yang bertugas untuk mencatat perubahan seluruh file atau repository suatu project. Developer software biasa menggunakan Git untuk distributed revision (VCS terdistribusi), hal ini bertujuan untuk menyimpan database tidak hanya ke satu tempat. Namun semua orang yang terlibat dalam penyusunan kode dapat menyimpan database ini.

Sementara Github merupakan layanan cloud yang berguna untuk menyimpan dan mengelola sebuah project yang dinamakan repository (repo git). Cara kerja pada Github harus terkoneksi pada internet sehingga tidak perlu menginstall sebuah software ke dalam perangkat keras. Hal ini memberikan keringanan penyimpanan komputer yang kita gunakan karena file project tersimpan oleh cloud Github.


# Langkah-langkah
### Langkah- langkah praktik penggunaan Git- Github, antara lain:
01) Download Git; Git dapat didownload dengan mengakses web https://git-scm.com/
02)	Klik petunjuk download sesuai dengan OS Laptop/ Komputer yang dipakai
03)	Ketiga adalah melakukan penginstallan, berhubung saya menggunakan MAC OS oleh karena itu Git sudah memberikan saya akses utnuk mendownload Git untuk OS saya
04)	Setelah itu, buka package git dan lakukan intalasi
05) Lakukan penginstalan melalui terminal dengan 
```
$ brew install git	
```
06)	Langkah selanjutnya adalah membuat akun di https://github.com 
07)	Setelah selasai, kemudian lakukanlah konfigurasi untuk memberitahu git email dan username yang akan digunakan apabila mengalami perubahan pada repo git. Perintah konfigurasi sebagai berikut: 
```
$ git config --global user.name "Nama Anda di GitHub"
$ git config --global user.email email@domain.tld
```
Setelah sukses kemudian pastikan email dan username yang digunakan sudah sesuai dengan yang ada di GitHub. Untuk melihat konfigurasi gunakan perintah berikut: (Cukup lakukan satu kali, kecuali ingim mengubahnya –unset)
```
$ git config –list
user.email=xxxx@gmail.com
user.name=xxxx
```
08)	Setelah selesai mengecek konfigurasi langkah selanjutnya adalah membuat repository di github, namun, karena mulai bulan Juli 2020 Github memberiahukan tentang penggunaan token-based authenthication pengguna wajib mengaktifkan personal acess token untuk mengaksesnya di terminal nanti, Hal ini ditujukan untuk keamanan data pengguna Github.
Cara mengaktifkan token yaitu:
  > 1. Pertama, pergi ke akun Github 
  > 2. Kedua, klik icon profil akun di kanan atas kemudian klik setting
  > 3. Ketiga, temukanlah developer setting dan klik
  > 4. Keempat, klik personal access tokens lalu generate new token
09)	Kemudian setelah itu membuat repo di akun yang sudah dibuat, dengan langkah- langkah sebagai berikut:






