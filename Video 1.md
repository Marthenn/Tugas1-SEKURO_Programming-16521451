## [APA ITU GIT & GITHUB?](https://youtu.be/lTMZxWMjXQU)
### Version Control System (VCS):
- Sistem yang menyimpan rekaman/snapshot perubahan di source code
- Membantu dalam berkolaborasi
- Melacak suatu perubahan (oleh siapa dan kapan)
- Memungkinkan untuk kembali ke kondisi sebelum terjadinya perubahan (checkout)

### Contoh Version Control System:
- Git
- Subversion
- Mercurial
- CVS (Concurrent Versions System)

### Git:
- Sebuah VCS terdistribusi untuk mengelola perubahan file di dalam folder (**repository/repo**)
- Riwayat perubahan file disimpan menggunakan serangkaian **commit** (mencatat perubahan yang terjadi ketika disave)
- Akan merekam satu **snapshot** untuk setiap commit<br>
[Wikipedia Git](https://en.wikipedia.org/wiki/git)

### Komponen Commit:
- __Hash__ yaitu penanda bagi setiap commit
- __Author__ yaitu siapa yang melakukan commit
- __Date__ yaitu kapan dilakukan commit
- __Commit Message__ yaitu pesan yang dilampirkan pada suatu commit

### Contoh Commit
commit 42e769bdf4894310333942ffc5a151222a87be<br>
Author: Sandhika Galih (sandhikagalih@wpu.com)<br>
Date: Fri Jan 01 00:00:00<br>
Membuat controller user

### Branch
Digunakan supaya tidak menganggu jalur commit utamanya apabila dibuat suatu perubahan yang masih ragu maupun dalam suatu kolaborasi untuk memudahkan setiap kolaborator

### Merge
Pengabungan beberapa branch menjadi satu

### [GitHub](https://github.com)
- Sebuah layanan cloud untuk menyimpan dan mengelola project / repo git
- Pada prakteknya apabila menggunakan Git dan GitHub dapat dilakukan __push__ (pengiriman commit) dan __pull__ (pengambilan commit) dari lokal ke GitHub apabila GitHub telah dibuat menjadi __remote__ (sumber dari repo) dan telah __diclone__ (pengambilan repo dari cloud) di local device
- Bitbucket dan GitLab adalah contoh layanan cloud VCS lainnya
