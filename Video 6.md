## [GIT BRANCH & MERGE](https://youtu.be/EGl7KxVOyNs)
### Implementasi Branching
1. Terdapat pointer `head` yang akan menandakan kita sedang berada di branch yang mana
2. Pointer `master` dan `head` akan mengikuti commit terbaru sebelum terjadinya branching
3. Gunakan command `git branch <nama branch>` untuk membuat branch baru
   - Pengunaan `git branch <nama branch>` akan membuat pointer baru yang mengarah ke branch yang sama
   - Pengunaan `git branch` tanpa parameter `<nama branch>` akan menampilkan ada branch apa saja
      - Branch yang berwarna hijau dan diberi tanda `*` di awalnya berarti branch itu adalah branch yang sedang aktif
   - Pengunaan `git log --all --decorate --oneline --graph` akan memvisualisasikan branches dan commit yang telah terjadi
      - Pengunaan `alias <nama alias>=<command>` dapat digunakan untuk menyingkat pemanggilan suatu command 
      ![contoh graph](https://github.com/Marthenn/Tugas1-SEKURO_Programming-16521451/blob/main/Foto/contoh%20graph.jpg)
   - Pengunaan `git checkout <nama branch>` dilakukan untuk memindahkan pointer `head` ke branch tertentu (branch aktif berubah)
      - Perubahan branch akan memberlakukan perubahan file secara dinamis pada repo

![buat branch hingga pindah](https://github.com/Marthenn/Tugas1-SEKURO_Programming-16521451/blob/main/Foto/buat%20branch%20hingga%20pindah.jpg)
![commit branch dosen hingga commit branch staff](https://github.com/Marthenn/Tugas1-SEKURO_Programming-16521451/blob/main/Foto/commit%20branch%20dosen%20hingga%20commit%20staff.jpg)

### Jenis-Jenis Merge:
- __Fast Forward__
   - Terjadi ketika branch yang ingin digabungkan berada dalam direct path
   - Tahapannya:
      1. Pindahkan head ke branch yang akan menjadi tujuan merging
      2. Tentukan branch yang memiliki direct path (langsung bercabang ke branch tujuan)
      3. Gunakan command `git merge <nama branch>` untuk melakukan merge branch tersebut dengan branch yang sedang aktif sekarang
      4. Branch yang telah dimerge dapat dihapus dengan command `git branch -d <nama branch>`
         - Dapat digunakan `git branch --merged` untuk melihat branch(es) yang telah dimerge
         - Branch yang belum dimerge dapat dihapus tetapi yang digunakan adalah `git branch -D <nama branch>` (dengan D kapital)

![fast forward merge](https://github.com/Marthenn/Tugas1-SEKURO_Programming-16521451/blob/main/Foto/fast%20forward%20merge.jpg)

- __Three-way Merge__
   - Terjadi ketika branch yang ingin digabungkan tidak berada dalam direct path
   - Disebut juga merge commit karena selain merge dilakukan pula commit
   - Tahapannya (kurang lebih sama seperti fast forward merge):
      1. Pindahkan head ke branch yang akan menjadi tujuan merging
      2. Gunakan command `git merge <nama branch>`
      3. Masukkan commit message
  
![three-way merge](https://github.com/Marthenn/Tugas1-SEKURO_Programming-16521451/blob/main/Foto/threeway%20merge.jpg)
