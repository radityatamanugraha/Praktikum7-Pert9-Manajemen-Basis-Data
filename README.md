# Tugas Praktikum 7 (Pertemuan ke 9) <img src=https://qph.fs.quoracdn.net/main-qimg-648763cc041459725b62108f4fdf5b91 width="110px">

|Nama|NIM|Kelas|Mata Kuliah|
|----|---|-----|------|
|**Radityatama Nugraha**|**312310644**|**TI.23.A3**|**Manajemen Basis Data**|

# Soal 1:
![gambar](Ss_Manajemen_Basis_Data_Pertemuan9/ss1_pertemuan9.jpg)

## - Untuk Memulai Codingan Database di XAMPP dan ke Shell
![gambar](Ss_Manajemen_Basis_Data_Pertemuan9/ss2_pertemuan9.png)

## - Membuat dan memilih database perpustakaan dengan perintah CREATE DATABASE perpustakaan; dan USE perpustakaan;.
![gambar](Ss_Manajemen_Basis_Data_Pertemuan9/ss3_pertemuan9.png)

## - Membuat tabel buku dalam database perpustakaan dengan perintah CREATE TABLE buku; yang berisi kolom id_buku, judul, penulis, penerbit, tahun_terbit, dan isbn untuk menyimpan data buku secara terstruktur.
![gambar](Ss_Manajemen_Basis_Data_Pertemuan9/ss4_pertemuan9.png)

## - Membuat tabel anggota dalam database perpustakaan dengan perintah CREATE TABLE anggota; yang berisi kolom id_anggota, nama, alamat, dan no_hp untuk menyimpan data anggota perpustakaan.
![gambar](Ss_Manajemen_Basis_Data_Pertemuan9/ss5_pertemuan9.png)

## - Membuat tabel peminjaman dalam database perpustakaan dengan perintah CREATE TABLE peminjaman; yang berisi kolom id_pinjam, id_buku, id_anggota, tanggal_pinjam, dan tanggal_kembali, serta relasi ke tabel buku dan anggota menggunakan foreign key.
![gambar](Ss_Manajemen_Basis_Data_Pertemuan9/ss6_pertemuan9.png)

## - Menampilkan daftar tabel dalam database perpustakaan dengan perintah SHOW TABLES; yang menghasilkan tiga tabel yaitu anggota, buku, dan peminjaman.
![gambar](Ss_Manajemen_Basis_Data_Pertemuan9/ss7_pertemuan9.png)

## - Menambahkan data ke dalam tabel buku dengan perintah INSERT INTO buku; untuk menyimpan informasi dua buku yaitu Belajar Manajemen Basis Data dan Belajar Kriptografi beserta detail penulis, penerbit, tahun terbit, dan ISBN.
![gambar](Ss_Manajemen_Basis_Data_Pertemuan9/ss8_pertemuan9.png)

## - Menampilkan seluruh data dari tabel buku dengan perintah SELECT * FROM buku; yang menghasilkan dua baris data berisi informasi judul, penulis, penerbit, tahun terbit, dan ISBN buku.
![gambar](Ss_Manajemen_Basis_Data_Pertemuan9/ss11_pertemuan9.png)

## - Menambahkan data ke dalam tabel anggota dengan perintah INSERT INTO anggota; untuk menyimpan informasi dua anggota yaitu Radit dan Rifqi beserta alamat dan nomor HP masing-masing.
![gambar](Ss_Manajemen_Basis_Data_Pertemuan9/ss9_pertemuan9.png)

## - Menampilkan seluruh data dari tabel anggota dengan perintah SELECT * FROM anggota; yang menghasilkan dua baris data berisi informasi nama, alamat, dan nomor HP anggota perpustakaan.
![gambar](Ss_Manajemen_Basis_Data_Pertemuan9/ss12_pertemuan9.png)

## - Menambahkan data ke dalam tabel peminjaman dengan perintah INSERT INTO peminjaman; untuk mencatat dua transaksi peminjaman buku oleh anggota pada tanggal 15 dan 16 November 2025.
![gambar](Ss_Manajemen_Basis_Data_Pertemuan9/ss10_pertemuan9.png)

## - Menampilkan seluruh data dari tabel peminjaman dengan perintah SELECT * FROM peminjaman; yang menghasilkan dua baris data berisi informasi peminjaman buku oleh anggota, termasuk tanggal pinjam dan tanggal kembali.
![gambar](Ss_Manajemen_Basis_Data_Pertemuan9/ss13_pertemuan9.png)

# Soal 2:
## - Pengertian Super Key 
### - Super Key adalah kombinasi atribut yang dapat mengidentifikasi satu baris secara unik di dalam tabel.
## - Contoh Super Key (tabel Buku)
### - Tabel Buku(id_buku, judul, penulis, isbn)
### - {id_buku}
### - {isbn}
### - {id_buku, judul} → tetap unik karena ada id_buku
### - {isbn, penulis}

# Soal 3:
## - Pengertian Candidate Key 
### - Candidate Key adalah super key yang paling minimal (atributnya tidak bisa dikurangi lagi tapi tetap unik).
## - Contoh Candidate Key (tabel Buku)
### - {id_buku}
### - {isbn}

# Soal 4:
## - Pengertian Primary Key 
### - Primary Key adalah candidate key yang dipilih sebagai identitas unik utama dari tabel.
## - Contoh Primary Key (tabel Buku)
### - {id_buku}

# Soal 5:
## - Pengertian Alternatif Key 
### - Alternate Key adalah candidate key yang tidak dipilih menjadi primary key.
## - Contoh Alternatif Key (tabel Buku)
### - {isbn} Karena isbn tetap unik tapi tidak dipilih sebagai primary key.

# Soal 6:
## - Pengertian Foreign Key 
### - Foreign Key adalah atribut yang menghubungkan satu tabel dengan tabel lain, mengacu pada primary key tabel lain.
## - Contoh Foreign Key (tabel Peminjaman)
### Tabel Peminjaman(id_pinjam, id_buku, id_anggota, tanggal_pinjam)
### - id_buku → foreign key ke Buku(id_buku)
### - id_anggota → foreign key ke Anggota(id_anggota)

