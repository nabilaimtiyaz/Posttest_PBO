# Praktikum PBO Post Test 1

Nama: Nabila Imtiyaz Agustin | NIM: 2409116011 | Kelas A'2024

# Tema

Sistem Pencatatan Hasil Panen Kebun merupakan tema yang digunakan dengan konsep pengelolaan data hasil pertanian. program ini dirancang untuk menambahkan data panen baru, melihat daftar hasil panen, memperbarui informasi yang sudah ada sebelumnya, serta menghapus data yang tersimpan. setiap item hasil panen memiliki data berupa kategori (sayur/buah), nama, berat dalam jumlah kilogram, dan kualitas. seluruh interaksi dilakukan melalui inputan dari pengguna dengan memilih menu CRUD (Create, Read, Update, Delete).

# <sub>Penjelasan kode</sub>

<img width="494" height="107" alt="image" src="https://github.com/user-attachments/assets/b8dd0067-46e1-4b88-9c7a-e7737ec006ff" />


import library yang digunakan adalah ArrayList dan Scanner. Arraylist digunakan untuk menyimpan daftar hasil panen secara dinamis (bisa ditambah, ubah, dan hapus). Scanner digunakan untuk membaca input dari pengguna, contohnya ketika memilih manu atau memasukkan data.

<img width="1070" height="378" alt="image" src="https://github.com/user-attachments/assets/30d76b69-fc60-48b1-89f6-db8d603cdae4" />


pada kode ini, didefinisikan sebuah kelas utama dengan nama Main. Di dalamnya terdapat kelas statis bernama ItemPanen yang berfungsi sebagai blueprint untuk mempresentasikan data hasil panen. Kelas ItemPanen memiliki empat atribut, yaitu kategori untuk menyimpan jenis panen apakah sayur atau buah, nama untuk menyimpan nama item, beratkg bertipe double untuk menyimpan berat dalam satuan kilogram, dan kualitas untuk menyimpan informasi mutu panen.

(foto)

pada bagian ini akan menampilkan menu utama kepada pengguna, yang diberikan 5 pilihan menu. Perulangan do-while ini terus berjalan sampai pengguna memilih opsi 5 untuk keluar.

(foto)

Pada method tambahItem, program menyiapkan proses untuk menambahkan data hasil panen baru ke dalam daftar. Setelah pengguna memasukkan semua inputan yang diperlukan, semua data kemudian dimasukkan ke dalam sebuah objek baru dari class ItemPanen. Objek tersebut ditmabahkan ke dalam daftarPanen, yaitu ArrayList yang menyimpan semua data hasil panen. sebagai penutup, program menampilkan pesan bahwa data panen berhasil ditambahkan.

(foto)

Pada method tampilkanPanen, program berjalan untuk menampilkan seluruh data hasil panen yang sudah tersimpan dalam daftar. pertama-tama, dilakukan pengecekkan apakah daftarPanen masih kosong menggunakan method isEmpty(). JIka memang belum ada data yang dimasukkan, maka program akan langsung menampilkan pesan "Belum ada data panen". Namun, jika data sudah ada, program akan menngeluarkan output daftar hasil panen.

(foto)

Method editItem ini digunakan untuk mengubah data panen yang sudah ada. Pertama, program akan menampilkan daftar panen. Jika daftar kosong, proses langsung dihentikan. Jika ada data nya, pengguna diminta memilih nomor item yang ingin diedit. Setelah nomor valid, program akan meminta pengguna menginputkan data yang baru.

(foto)

Method hapusItem berfungsi untuk menghapus data panen. Pertama, program menampilkan daftar panen, lalu mengecek apakah ada data. Jika ada, pengguna diminta memilih nomor item yang ingin dihapus. Nomor tersebut dikurangi 1 agar sesuai dengan indeks ArrayList.

# Penjelasan Output

(foto)

ketika program dijalankan, yang pertama ditampilan pengguna adalah menu utama dengan pilihan menu 1 sampai 5. Kemudian, pengguna harus memilih nomor menu yang diinginkan.

(foto)

Pengguna yang memilih nomor 1, maka akan masuk ke menu tambah item. Dimana pengguna dapat menambahkan kategori (sayur/buah), nama, beratkg, dan kualitas hasil panen nya.

(foto)

Selanjutnya jika pengguna memilih nomor 2, maka akan masuk ke menu tampilkanItem. Disini pengguna dapat melihat daftar hasil panen yang sudah diinputkan sebelumnya.

(foto)

Jika pengguna memilih nomor 3, maka akan masuk ke menu edit item. Dimana pengguna harus memilih item nomor berapa yang akan di edit data nya. setelah memilih, selajutnya barulah pengguna bisa mengedit data item panen.

(foto)

Jika pengguna memilih nomor 4, maka akan masuk ke dalam menu hapus item. Sama juga seperti sebelumnya, pengguna harus memilih terlebih dahulu nomor item hasil panen yang ingin dihapus. Apabila nomor valid, akan ada output "Item berhasil dihapus".
