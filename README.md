# Mohammad-Farrel-Firzatullah-Tugas-Asistensi-P2
# Deskripsi Tugas
Buatlah mesin generator gambar. Mesin ini akan menerima input gambar yang diinginkan dan mengeluarkan output gambar sesuai input yang dimasukkan. 

Kriteria Wajib : 
Dapat menampilkan output gambar yang minimal tersusun dari simbol asterisk “*” dan space “ “.
Dapat menampilkan satu jenis gambar berukuran panjang dan lebar sesuai input dengan minimal panjang 10 karakter dan lebar 5 karakter serta maksimal panjang 100 karakter dan lebar 75 karakter. 
Apabila melebihi atau kurang dari batas maksimal dan minimal maka gambar tidak akan ditampilkan dan akan menampilkan pesan sesuai pelanggaran
Dapat menjelaskan kode yang diberikan melalui file  dokumentasi README.md

Kriteria Tambahan : 
Dapat menampilkan lebih dari satu jenis gambar, tergantung demand dari input
Dapat menampilkan gambar yang bergerak 
Program dapat menerima input dan menampilkan output secara terus menerus sampai dihentikan secara paksa 
# Penjelasan
#include <stdio.h>: Digunakan untuk fungsi input/output standar seperti printf() dan scanf().
#include <stdlib.h>: Digunakan untuk fungsi sistem standar seperti system() yang digunakan untuk membersihkan layar.
Fungsi ini digunakan untuk mencetak persegi panjang dengan ukuran panjang dan lebar yang diinput oleh pengguna.
Ada dua loop:
Loop luar (for (int i = 0; i < lebar; i++)) yang menjalankan lebar kali untuk mencetak baris.
Loop dalam (for (int j = 0; j < panjang; j++)) yang menjalankan panjang kali untuk mencetak simbol bintang (*).
Fungsi gambar_bergerak():
Fungsi ini mencetak persegi panjang dengan animasi bergerak ke bawah sebanyak steps langkah.
Setiap kali layar dibersihkan menggunakan clear_screen(), fungsi ini menambahkan baris kosong (\n) sebanyak nilai step untuk menciptakan ilusi bahwa gambar "bergerak" ke bawah.
Fungsi sleep(1) membuat jeda 1 detik pada setiap langkah agar pergerakan terlihat lebih lambat.
Program memulai dengan menampilkan menu pilihan gambar.
Pengguna memilih jenis gambar:
Jika memilih persegi panjang, pengguna diminta memasukkan panjang dan lebar, kemudian gambar persegi panjang dicetak.
Jika memilih segitiga, pengguna memasukkan tinggi, dan gambar segitiga dicetak.
Jika memilih gambar bergerak, pengguna memasukkan panjang, lebar, dan jumlah langkah, lalu gambar persegi panjang akan "bergerak" ke bawah di layar.
Program terus berjalan dalam loop hingga pengguna memilih opsi untuk keluar (pilihan == 0).
