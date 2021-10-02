# Pengertian
Git merupakan software berbasis Version Control System (VCS) yang bertugas untuk mencatat perubahan seluruh file atau repository suatu project. Developer software biasa menggunakan Git untuk distributed revision (VCS terdistribusi), hal ini bertujuan untuk menyimpan database tidak hanya ke satu tempat. Namun semua orang yang terlibat dalam penyusunan kode dapat menyimpan database ini.

Sementara Github merupakan layanan cloud yang berguna untuk menyimpan dan mengelola sebuah project yang dinamakan repository (repo git). Cara kerja pada Github harus terkoneksi pada internet sehingga tidak perlu menginstall sebuah software ke dalam perangkat keras. Hal ini memberikan keringanan penyimpanan komputer yang kita gunakan karena file project tersimpan oleh cloud Github.


# Langkah-langkah
### Langkah- langkah praktik penggunaan Git- Github, antara lain:
01) Download Git; Git dapat didownload dengan mengakses web https://git-scm.com/ atau bisa menggunakan terminal dengan perintah sebagai berikut:
```
$ brew install git
```
atau jika pertama kali memakai dan belum pernah menginstal bisa menggunakan perintah sebagai berikut di terminal:
```
$ git --version
```
02)	Klik petunjuk download sesuai dengan OS Laptop/ Komputer yang dipakai
03)	Ketiga adalah melakukan penginstallan, berhubung saya menggunakan MAC OS oleh karena itu Git sudah memberikan saya akses utnuk mendownload Git untuk OS saya
03)	Setelah itu, buka package git dan lakukan intalasi dan tunggu hingga berhasil
04)	Langkah selanjutnya adalah membuat akun di https://github.com 
05)	Setelah selasai, kemudian lakukanlah konfigurasi untuk memberitahu git email dan username yang akan digunakan apabila mengalami perubahan pada repo git. Perintah konfigurasi sebagai berikut: 
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
06)	Setelah selesai mengecek konfigurasi langkah selanjutnya adalah membuat repository di github, namun, karena mulai bulan Juli 2020 Github memberiahukan tentang penggunaan token-based authenthication pengguna wajib mengaktifkan personal acess token untuk mengaksesnya di terminal nanti, Hal ini ditujukan untuk keamanan data pengguna Github.
Cara mengaktifkan token yaitu:
  > 1. Pertama, pergi ke akun Github 
  > 2. Kedua, klik icon profil akun di kanan atas kemudian klik setting
  > 3. Ketiga, temukanlah developer setting dan klik
  > 4. Keempat, klik personal access tokens lalu generate new token
07)	Kemudian setelah itu membuat repo di akun yang sudah dibuat, dengan langkah- langkah sebagai berikut:
  > 1. Pertama, klik icon tambah 
  > 2. Kedua, klik "New Repository"
  > 3. Ketiga, akan dibawa kehalaman baru lalu berilah nama untuk repo yang akan dibuat dan create repo
08) Setelah membuat repo lalu melakukan clone ke local direktori melalui termial yaitu dengan perintah:
```
$ git clone https://github.com/nasmahna/01-git-github
Cloning into '01-git-github'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
Unpacking objects: 100% (3/3), done.
```
**Notes:** sesuaikan nama repo dan akun Github akun. Lalu apabila clone dan repo masih kosong dapat diabaikan.

09) Melakukan perubahan lokal master menjadi main dengan perintah sebagai berikut:
```
$ cd awesome-project
$ git branch -m main
$
```
10) Setelah itu, ubah isi konten dengan perintah dimana setelah mengubah harus melakukan push untuk memberikan update perubahan, yaitu sebagai berikut:
```
$ cat README.md 
$ # 01-git-github%                      
$ git status
$ On branch main
$ Your branch is up to date with 'origin/main'.

$ nothing to commit, working tree clean
$ git add -A
$ git commit -m "Add: README.md"
$ On branch main
$ Your branch is up to date with 'origin/main'.

$ nothing to commit, working tree clean
$ git push origin main
$ Username for 'https://github.com': nasmahna
$ Password for 'https://nasmahna@github.com': 
$ Everything up-to-date
```

## Git Mac Line Command (Most Commonly Used at Git)
- Untuk mengetahui versi mac dan menginstall Git:
```
$ git --version
```
- Untuk meng-clone Git ke lokal direktori:
```
$ git clone git://git.kernel.org/pub/scm/git/git.git
```
- Untuk melihat setting konfigurasi:
```
$ git config --list
```
- Untuk melihat bantuan Git:
```
$ git help <verb>
$ git <verb> --help
$ man git-<verb>
```
ex:
```
$ git help config
```
- Untuk menambahkan file:
```
$ git add -h
usage: git add [<options>] [--] <pathspec>...

    -n, --dry-run               dry run
    -v, --verbose               be verbose

    -i, --interactive           interactive picking
    -p, --patch                 select hunks interactively
    -e, --edit                  edit current diff and apply
    -f, --force                 allow adding otherwise ignored files
    -u, --update                update tracked files
    --renormalize               renormalize EOL of tracked files (implies -u)
    -N, --intent-to-add         record only the fact that the path will be added later
    -A, --all                   add changes from all tracked and untracked files
    --ignore-removal            ignore paths removed in the working tree (same as --no-all)
    --refresh                   don't add, only refresh the index
    --ignore-errors             just skip files which cannot be added because of errors
    --ignore-missing            check if - even missing - files are ignored in dry run
    --chmod (+|-)x              override the executable bit of the listed files
    --pathspec-from-file <file> read pathspec from file
    --pathspec-file-nul         with --pathspec-from-file, pathspec elements are separated with NUL character
  ```
  - Untuk melihat list di dalam direktori:
  ```
  $ ls
  ```
  atau melihat keseluruhan
  ```
  $ ls -a
  ```
  - Untuk membaca isi repo:
  ```
  $ cd [nama repo]
  ```
  - Untuk membuat README.md:
  ```
  $ touch README.md
  ```
  - Untuk mengecek status repository:
  ```
  $ git status
  ```
  - Untuk membuat branch:
  ```
  $ git branch -b [nama_branch]
  ```
  - Untuk mengubah/ mengalihkan ke letak branch [nama_branch]:
  ```
  $ git checkout [nama)branch]
  ```
  - Untuk menambahkan untracked files ke repo:
  ```
  $ git add .
  ```
  - Untuk melihat remote yang digunakan/ remote target:
  ```
  $ git remote -v
  ```
  - Untuk melakukan pengupdatean tebaru:
  ```
  $ git commit -m "Add README.md"
  ```
  -m; switch memungkinkan Anda untuk memasukkan pesan komit pendek dengan tanda kutip ganda.
  - Untuk melakukan sinkronasi perubahan dari Github ke Repo lokal:
   ```
  $ git pull
  ```
  - Untuk melakukan sinkronasi/ pengiriman pembaruan data dari lokal ke Github:
   ```
  $ git push
  ```
  




