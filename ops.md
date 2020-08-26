# Inisialisasi Repository

## Apa itu Repository?

Repository dalam git merupakan sebuah tempat di mana kita menyimpan berkas, lalu kita memonitoring nya dengan git. Untuk menginisiasi repository dapat kita lakukan dengan dua cara, yaitu:

* Kalau repository ini baru, maka kita lakukan dengan git init
* Kalau repository ini sudah ada sebelumnya, maka kita bisa lakukan git clone

Oke, mari kita bahas satu per satu:

## Git init

Perintah ini digunakan apabila kita ingin membuat repository baru, mari kita langsung praktik:

* Pertama, siapkan direktori kerja ya
* Kita anggap ini adalah direktori di mana kode sumber kita disimpan, atau pertama kali ketika kita akan memulai sebuah proyek.
* Kemudian kita lakukan git init `git init`
* Setelah menjalankan perintah git init, maka akan terdapat folder `.git` di dalam direktori kerja kita, di dalam folder tersebut lah semua catatan git disimpan nantinya.

## Git clone

Kemudian untuk repository yang sudah ada, lalu kita ingin mengkopi repository tersebut, katakanlah ada sebuah project open source di internet, lalu project nya di-host di github, apabila kita ingin mengkopi source code project tersebut maka kita bisa lakukan dengan clone:

`git clone <alamat-repository>`

Alamat repository bisa menggunakan http, ssh, atau path direktori di mana repository tersebut berada, contoh:

`git clone https://github.com/somat/belajar-git.git`

Maka pada direktori kerja akan tercipta sebuah folder bernama `belajar-git` (sesuai nama repository), dan di dalam folder tersebut berisi salinan repository.

## Melihat status

Perintah git status akan menampilkan status dari direktori kerja kita, sedang berada di branch mana, file mana saja yang dalam kondisi baru, file mana yang dalam kondisi staging, oke jangan khawatir istilah-istilah tersebut akan kita bahas satu-satu.

## Git add

Selanjutnya kita akan belajar bagaimana memasukkan file ke dalam commit, dalam hal ini file tersebut akan masuk ke dalam revisi git:

* Pertama buat file, misalnya README.md dan main.go
* Isi file tersebut, misalnya di file README.md isi dengan "Belajar Git"
* Lalu di main.go isi dengan "package main"
* Selanjutnya kita lihat status dari repository kita dengan `git status`
* Tambahkan file README.md dan main.go ke dalam daftar yang akan kita commit, atau disebut dengan staging, dengan perintah `git add`
* Lihat kembali status dengan perintah `git status`

## Git commit

Setelah memasukkan file ke dalam staging, kita bisa melakukan commit, untuk mencatat revisi yang kita buat ke dalam git, perintahnya adalah:

`git commit -m "pesan"`

Option -m untuk menambahkan pesan yang berkaitan dengan komit, pesan tersebut akan muncul di log.

## Git log

Perintah: `git log`
Digunakan untuk melihat log commit yang sudah dilakukan.
