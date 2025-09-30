# Sistem Pendaftaran Konser Post-test-4
Nama: Nur Aliyya

Kelas: C

Nim: 2409116094
# Deskeripsi Program
Program ini merupakan sistem pendaftaran konser sederhana yang dibuat menggunakan bahasa pemrograman Java. Aplikasi ini memungkinkan pengguna untuk menambahkan peserta baru, menampilkan daftar peserta, memperbarui data peserta, menghapus peserta, serta mencari peserta berdasarkan nama. Terdapat dua jenis peserta yang dapat dipilih oleh pengguna, yaitu Peserta VIP dengan fasilitas khusus dan Peserta Reguler dengan nomor kursi. Program ini juga sudah menerapkan konsep OOP (Object-Oriented Programming) seperti inheritance dan method overriding pada class PesertaVIP dan PesertaReguler.

Alur Program Sistem Pendaftaran Konser

Program dijalankan tampil menu utama.
Program akan menampilkan daftar pilihan:

- Tambah Peserta
- Tampilkan Peserta
- Update Peserta
- Hapus Peserta

Cari Peserta

Keluar

=== Sistem Pendaftaran Konser ===
1. Tambah Peserta
2. Tampilkan Peserta
3. Update Peserta
4. Hapus Peserta
5. Cari Peserta
0. Keluar
Pilih menu: 


User memilih menu “Tambah Peserta” (1).
Program akan meminta data peserta:

Nama

Email

Jenis Peserta (VIP atau Reguler)

Misalnya user isi:

Nama → Jihan

Email → jihanalya@gmail.com

Jenis Peserta → pilih 1 (VIP)

Fasilitas VIP → Backstage Pass

Maka program menyimpan data ke daftar.

Masukkan Nama: Jihan
Masukkan Email: jihanalya@gmail.com
Jenis Peserta (1 = VIP, 2 = Reguler): 1
Masukkan Fasilitas VIP: Backstage Pass
Peserta berhasil ditambahkan!


User memilih menu “Tampilkan Peserta” (2).
Program menampilkan semua peserta yang sudah tersimpan dalam ArrayList.

=== Daftar Peserta ===
ID: 1 | Nama: Jihan | Email: jihanalya@gmail.com | Fasilitas: Backstage Pass


User memilih menu “Cari Peserta” (5).
Program akan minta input nama yang dicari.
Misalnya user ketik Jihan, maka program menampilkan hasilnya:

Masukkan Nama yang dicari: Jihan
Hasil Pencarian:
ID: 1 | Nama: Jihan | Email: jihanalya@gmail.com | Fasilitas: Backstage Pass


User memilih menu “Keluar” (0).
Program berhenti.
- Keluar dari program...

  # Penerapan Abstraction
Pada program ini, abstraction diterapkan dengan membuat abstract class Peserta yang menjadi induk bagi class PesertaVIP dan PesertaReguler. Peserta memiliki method abstract tampilkanInfo() yang wajib di-override oleh setiap subclass. Dengan abstraction, kita hanya mendefinisikan struktur umum peserta tanpa detail implementasi, dan detailnya diberikan pada subclass sesuai jenis peserta.

# Penerapan Polymorphism

Polymorphism diterapkan dalam dua bentuk:

Overriding

Method tampilkanInfo() di-override pada PesertaVIP dan PesertaReguler. Masing-masing class memberikan implementasi berbeda sesuai data tambahan yang dimiliki (fasilitas untuk VIP, nomor kursi untuk Reguler).

Overloading

Method cariPeserta() pada PesertaService dibuat dalam dua versi:

cariPeserta(int id) mencari peserta berdasarkan ID. Dan cariPeserta(String nama) mencari peserta berdasarkan Nama.

Ini contoh method overloading karena nama method sama, tetapi parameter berbeda.


<img width="1408" height="845" alt="image" src="https://github.com/user-attachments/assets/4ae2204f-2250-4c83-85ab-dc36a2f84d12" />

<img width="1474" height="847" alt="image" src="https://github.com/user-attachments/assets/e2046e02-3ac8-4d59-8e3a-f905e6b0daf7" />

<img width="1458" height="885" alt="image" src="https://github.com/user-attachments/assets/a164d85e-0ece-4c95-b245-3d30283ed351" />

<img width="1521" height="887" alt="image" src="https://github.com/user-attachments/assets/e23c0e69-aa79-49d6-bb97-a88162539cf9" />
