## [GITHUB : BRANCH](https://youtu.be/k1QXd-8VbPY)
### Definisi Branch
Percabangan independen dari master / main branch yang dapat jalan dengan commitnya sendiri

### Branching
- Membuat Git Branch
- Membuat snapshot tanpa menganggu master branch
- Umumnya digunakan untuk suatu fitur eksperimental maupun kolaborasi pada suatu repo yang sama

### Cara Branching di GitHub
1. Pada saat commit, pilihlah radio button _"Create a new branch for this commit and start a pull request."_
2. Pilih branch di home page repo

> Checkout = berpindah ke branch / commit yang lain

### Merging
1. Tekan tombol _"Compare & pull request"_
2. Buat sebuah pull request untuk dilakukan pull suatu branch ke base branch
   - Pull request diperlukan untuk meminta pemilik base branch / repo untuk menarik perubahan yang telah dilakukan
   - Hanya dapat dilakukan merging antara dua branch pada satu waktu
3. Pada menu _"Pull requests"_, konfirmasi merging branch
   - Merging dapat dilakukan secara otomatis bila tidak ada conflict
   - Sebelum dimerge, dapat dilakukan pengeditan pada file yang akan dimerge
   - Apabila terdapat merge conflict (baris yang sama diubah oleh dua atau lebih branch yang berbeda), diperlukan pengeditan secara manual sebelum merge
   - Branch yang telah dimerge boleh dihapus maupun tidak
