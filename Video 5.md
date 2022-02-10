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
- `git config`<br>
memasukkan konfigurasi ke dalam git
- `git branch`<br>
membuat branch
- `git help`<br>
menampilkan cara menggunakan suatu command

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
