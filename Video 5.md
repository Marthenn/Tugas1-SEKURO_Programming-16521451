## [BEKERJA DENGAN GIT](https://youtu.be/e-6OkXRqWaE)
### Instalasi Git di Windows
1. Download installer git dari [link ini](https://git-scm.com)
2. Jalankan installer git dan install git
   - Pastikan _git bash here_ tercentang

> Command prompt dapat digunakan sebagai pengganti git bash

### Beberapa command git:
- `git`<br>
menampilkan list command git
- `git --version`<br>
menampilkan versi dari git yang terinstall
- `git init`<br>
menginisiasi repo git di local device
- `git add <file(s)>`<br>
menambahkan file(s) ke staging area
- `git status`<br>
mengetahui status repo
- `git commit`<br>
melakukan commit
   - Tambahkan parameter `-m "<message>"` untuk memberikan pesan commit
   - Tambahkan parameter `-a` sebelum parameter `-m` untuk menambahkan file yang telah tertrack untuk dicommit
   - Parameter `-a` dan `-m` dapat digabung menjadi `-am "<message>"`
- `git config`<br>
memasukkan konfigurasi ke dalam git
- `git branch`<br>
membuat branch
- `git help`<br>
menampilkan cara menggunakan suatu command
- `clear`<br>
membersihkan console
- `git log`<br>
menampilkan log pada git
   - Dapat ditambahkan parameter `-<angka>` untuk melihat sekian commit terakhir
   - Dapat ditambahkan parameter `-- <file>` untuk melihat log bagi sebuah file<br>
   ![git log](https://github.com/Marthenn/Tugas1-SEKURO_Programming-16521451/blob/main/Foto/git%20log.jpg)<br>

- `git checkout <lima digit pertama hash> -- <file>`<br>
mengembalikan suatu perubahan
   - Parameter `-- <file>` bersifat opsional dan digunakan apabila ingin mengcheckout suatu file tertentu saja
   - File yang telah dihapus akan tersimpan pada hidden folder `.git`<br>
   ![git checkout](https://github.com/Marthenn/Tugas1-SEKURO_Programming-16521451/blob/main/Foto/git%20checkout.jpg)<br>
   
## Tiga area pada repo:
- __Working tree<br>__
Folder tempat bekerja
- __Staging area<br>__
Memberitahu git bahwa perubahan telah dilakukan
- __History<br>__
Menyimpan commit-commit yang dilakukan

> Staging area dan history akan disimpan dalam hidden folder .git<br>
> Suatu repo git akan dipantau perubahannya<br>
> Perubahan tersebut akan disimpan dalam staging area dengan `git add`<br>
> Apabila perubahan tersebut diterima, digunakanlah `git commit` untuk menyimpan perubahan tersebut dalam history

### Mulai bekerja dengan git:
1. Gunakan `pwd` untuk melihat working directory saat ini
2. Gunakan `ls` untuk melihat files dan folders dalam suatu directory
   - Yang berwarna biru tua dengan `/` di ujungnya adalah folder
3. Gunakan `cd <directory>` untuk berpindah directory<br>

![pwd hingga cd](https://github.com/Marthenn/Tugas1-SEKURO_Programming-16521451/blob/main/Foto/pwd%20hingga%20cd.jpg)<br>
   
4. Gunakan `git init` untuk menginisialisasi working directory saat itu sebagai repo
   - Working directory akan menjadi master branch
   - Akan ada hidden folder `.git` tempat git menyimpan seluruh perubahannya
   
5. Gunakan `git add <file(s)>` untuk menambahkan file(s) tersebut ke dalam staging area
   - Suatu file dapat diunstage dengan command `git rm --cached <file>`
   - `git add .` dapat digunakan untuk menstage semua file sekaligus
7. Gunakan `git config --global user.name "<nama>"` untuk menambahkan identitas nama
8. Gunakan `git config --global user.email "<email>"` untuk menambahkan identitas email
9. Gunakan `git commit -m "<Message>"` untuk mengcommit perubahan
   - Setelah dijalankan, akan masuk ke code editor default pada saat instalasi
   - Pada code editor akan muncul status seperti untracked dan modified di sebelah kanan file
   - Pada percobaan, saya menggunakan vsc sehingga commit message juga dapat dimasukkan pada vsc<br>
![init hingga commit](https://github.com/Marthenn/Tugas1-SEKURO_Programming-16521451/blob/main/Foto/init%20hingga%20commit.jpg)<br>
![commit kedua dan ketiga](https://github.com/Marthenn/Tugas1-SEKURO_Programming-16521451/blob/main/Foto/commit%20dua%20dan%20tiga.jpg)
