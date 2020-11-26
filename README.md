# praktikum-pertemuan-9
[![Screenshot-2020-11-26-103325.png](https://i.postimg.cc/Pf4b6ymV/Screenshot-2020-11-26-103325.png)](https://postimg.cc/JtsB0bYj)
[![Screenshot-2020-11-26-103443.png](https://i.postimg.cc/7ZvR3DSr/Screenshot-2020-11-26-103443.png)](https://postimg.cc/dLBnFbW5)
[![Screenshot-2020-11-26-103527.png](https://i.postimg.cc/Hnq694c9/Screenshot-2020-11-26-103527.png)](https://postimg.cc/SYGLy9Gn)
[![Screenshot-2020-11-26-103616.png](https://i.postimg.cc/cJLPHhQv/Screenshot-2020-11-26-103616.png)](https://postimg.cc/PC0SVmVH)
[![Screenshot-2020-11-26-103729.png](https://i.postimg.cc/7YLzKTMg/Screenshot-2020-11-26-103729.png)](https://postimg.cc/hhHhjvYj)
Penjelasan:

Header

data={} untuk menampung list dengan format dictionary
Gunakanlah perulangan While untuk menampilkan data sebanyak banyaknya
menu = input("(T)ambah, (U)bah, (H)apus, (L)ihat, (C)ari, (K)eluar: ") kita tambahkan input Tambah, Ubah, Hapus, Lihat, Cari, Keluar dalam variabel menu
else: print("Upss ada yang salah, silahkan cek kembali.") jika kita salah dalam input maka akan tercetak 'Upss ada yang salah, silahkan cek kembali.'
masukan nama, nim, nilai_tugas, nilai_uts, nilai_uas, dan nilai_akhir yang nanti akan di masukkan kedalam data={}
Nilai akhir didapat dari = (nilai_tugas)*30/100 + (nilai_uts)*35/100 + (nilai_uas)*35/100
Keluar

if menu.lower() == 'k': Ambil data 'k' dari menu
lalu break untuk menghentikan seluruh proses
Lihat data

elif menu.lower() == 'l': Kita menggunakan kondisi percabangan if, ambil data dari menu lalu kita akan mengubah perintah 'l' yang kita input menjadi huruf kecil dengan fungsi lower()
lalu cetak print()
Tambah data

elif menu.lower() == 't': Ambil data 't' dari menu
nama = input("Masukan nama: ") lalu tambahkan input nama, nim, nilai tugas, uts, uas
nilai_akhir = (nilai_tugas)*30/100 + (nilai_uts)*35/100 + (nilai_uas)*35/100 untuk nilai akhir diambil dari perhitungan 3 komponen nilai (nilai_tugas: 30%, nilai_uts: 35%, nilai_uas: 35%)
data[nama] = [nama, nim, nilai_tugas, nilai_uts, nilai_uas, nilai_akhir] kita akan masukkan data yang tadi kita input ke dalam `data[nama]'
lalu cetak print()
Ubah data

elif menu.lower() == 'u': Ambil data 'u' dari menu
nama = input("Masukan nama untuk mengubah data: ") kita akan menginput data yang nanti akan di ubah
if nama in data.keys(): print("Mau mengubah apa?") jika 'nama' dari di dalam 'data' maka akan mengembalikan daftar menggunakan fungsi 'keys()' lalu di cetak lah 'print()'
sub_data = input("(Semua), (Nama), (NIM), (Tugas), (UTS), (UAS) : ") membuat menu ubah di dalam sub_data
if sub_data.lower() == "semua": ambil kata kunci 'semua' di dalam sub_data jika 'semua' maka input data[nama][1] = input("Ubah NIM:") data[nama][2] = int(input("Ubah Nilai Tugas: ")) data[nama][3] = int(input("Ubah Nilai UTS: ")) data[nama][4] = int(input("Ubah Nilai UAS: "))
data[nama][5] = data[nama][2] *30/100 + data[nama][3]*35/100 + data[nama][4] *35/100 kita dapatkan nilai akhir dengan diambil dari perhitungan 3 komponen nilai (tugas: 30%, uts: 35%, uas: 35%),
ket: [5] = nilai_akhir, dimana [0] = nama

lalu cetak print("\nBerhasil ubah data!")
Jika kita ingin mengubah data tertentu maka elif sub_data.lower() == "nim": data[nama][1] = input("NIM:") dan berlaku juga untuk nilai tugas, UTS dan UAS
lalu cetak print("\nBerhasil ubah data!")
else: print("'{}' tidak ditemukan.".format(nama)) jika kita salah dalam memasukkan nama untuk mengubah data maka akan muncul 'nama tidak di temukan'
Cari data

elif menu.lower() == 'c': Ambil data 'c' dari menu
nama = input("Masukan nama untuk mencari data: ") kita akan menginput data yang nanti akan di cari
if nama in data.keys(): kita mengambil list 'nama' di dalam 'data' menggunakan pengkondisian
maka cetak print("Nama: {0}\nNIM : {1}\nNilai Tugas: {2}\nUTS: {3}\nUAS: {4}\nNilai akhir: {5}" untuk menampilkan data yang tersedia
else: print("'{}' tidak ditemukan.".format(nama)) jika data yang kita input salah/tidak ditemukan maka akan tercetak 'nama tidak di temukan'
Hapudata

elif menu.lower() == 'h': Ambil data 'h' dari menu
nama = input("Masukan nama untuk menghapus data : ") kita akan menginput data yang nanti akan di hapus
if nama in data.keys(): kita mengambil list 'nama' di dalam 'data' menggunakan pengkondisian
del data[nama] hapus semua 'nama' yang ada di dalam 'data'
jika sudah maka cetak print("sub_data '{}' berhasil dihapus.".format(nama))
else: print("'{}' tidak ditemukan.".format(nama)) jika data yang kita input salah/tidak ditemukan maka akan tercetak 'nama tidak di temukan'
OUTPUT :

TAMBAH DATA

[![Screenshot-2020-11-26-121146.png](https://i.postimg.cc/gjLxP3M5/Screenshot-2020-11-26-121146.png)](https://postimg.cc/kR9JQRPF)

UBAH DATA

[![Screenshot-2020-11-26-121254.png](https://i.postimg.cc/Hkg9BLnH/Screenshot-2020-11-26-121254.png)](https://postimg.cc/kBTS5qWh)

LIHAT DATA

[![Screenshot-2020-11-26-121348.png](https://i.postimg.cc/4ycp1CTm/Screenshot-2020-11-26-121348.png)](https://postimg.cc/9wW4Wn0h)

CARI DATA

[![Screenshot-2020-11-26-121449.png](https://i.postimg.cc/1zz6jVQx/Screenshot-2020-11-26-121449.png)](https://postimg.cc/G4ZHB2tz)

HAPUS DATA

[![Screenshot-2020-11-26-121607.png](https://i.postimg.cc/FFSS8Q2K/Screenshot-2020-11-26-121607.png)](https://postimg.cc/fkwkS1W4)

FLOWCHART :

[![flowchart.png](https://i.postimg.cc/gJ80SGnF/flowchart.png)](https://postimg.cc/sQfy1dYw)
