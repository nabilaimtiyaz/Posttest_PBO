# Praktikum PBO Post Test 1

Nama: Nabila Imtiyaz Agustin | NIM: 2409116011 | Kelas A'2024

# Tema

Sistem Pencatatan Hasil Panen Kebun merupakan tema yang digunakan dengan konsep pengelolaan data hasil pertanian. program ini dirancang untuk menambahkan data panen baru, melihat daftar hasil panen, memperbarui informasi yang sudah ada sebelumnya, serta menghapus data yang tersimpan. setiap item hasil panen memiliki data berupa kategori (sayur/buah), nama, berat dalam jumlah kilogram, dan kualitas. seluruh interaksi dilakukan melalui inputan dari pengguna dengan memilih menu CRUD (Create, Read, Update, Delete).

# <sub>Penjelasan kode</sub>

<img width="494" height="107" alt="image" src="https://github.com/user-attachments/assets/b8dd0067-46e1-4b88-9c7a-e7737ec006ff" />


Import library yang digunakan adalah ArrayList dan Scanner. Arraylist digunakan untuk menyimpan daftar hasil panen secara dinamis (bisa ditambah, ubah, dan hapus). Scanner digunakan untuk membaca input dari pengguna, contohnya ketika memilih manu atau memasukkan data.

<img width="1070" height="378" alt="image" src="https://github.com/user-attachments/assets/30d76b69-fc60-48b1-89f6-db8d603cdae4" />


Pada kode ini, didefinisikan sebuah kelas utama dengan nama Main. Di dalamnya terdapat kelas statis bernama ItemPanen yang berfungsi sebagai blueprint untuk mempresentasikan data hasil panen. Kelas ItemPanen memiliki empat atribut, yaitu kategori untuk menyimpan jenis panen apakah sayur atau buah, nama untuk menyimpan nama item, beratkg bertipe double untuk menyimpan berat dalam satuan kilogram, dan kualitas untuk menyimpan informasi mutu panen.

<img width="932" height="616" alt="image" src="https://github.com/user-attachments/assets/b0bdf66e-2bae-4a7d-a680-4a394d83fe83" />


Pada bagian ini akan menampilkan menu utama kepada pengguna, yang diberikan 5 pilihan menu. Perulangan do-while ini terus berjalan sampai pengguna memilih opsi 5 untuk keluar.

<img width="1055" height="377" alt="image" src="https://github.com/user-attachments/assets/5b4a77b6-2104-4035-8dcc-99229c1e17ad" />


Pada method tambahItem, program menyiapkan proses untuk menambahkan data hasil panen baru ke dalam daftar. Setelah pengguna memasukkan semua inputan yang diperlukan, semua data kemudian dimasukkan ke dalam sebuah objek baru dari class ItemPanen. Objek tersebut ditmabahkan ke dalam daftarPanen, yaitu ArrayList yang menyimpan semua data hasil panen. sebagai penutup, program menampilkan pesan bahwa data panen berhasil ditambahkan.

<img width="1583" height="291" alt="image" src="https://github.com/user-attachments/assets/f74bb615-65f5-4247-8abf-bccd15bbb4ba" />


Pada method tampilkanItem, program berjalan untuk menampilkan seluruh data hasil panen yang sudah tersimpan dalam daftar. pertama-tama, dilakukan pengecekkan apakah daftarPanen masih kosong menggunakan method isEmpty(). JIka memang belum ada data yang dimasukkan, maka program akan langsung menampilkan pesan "Belum ada data panen". Namun, jika data sudah ada, program akan menngeluarkan output daftar hasil panen.

<img width="1123" height="669" alt="image" src="https://github.com/user-attachments/assets/96977ba3-6214-4e44-a9dd-f6cb981a679d" />


Method editItem ini digunakan untuk mengubah data panen yang sudah ada. Pertama, program akan menampilkan daftar panen. Jika daftar kosong, proses langsung dihentikan. Jika ada data nya, pengguna diminta memilih nomor item yang ingin diedit. Setelah nomor valid, program akan meminta pengguna menginputkan data yang baru.

<img width="910" height="431" alt="image" src="https://github.com/user-attachments/assets/75069249-32ca-43da-be1d-67a94024b8eb" />


Method hapusItem berfungsi untuk menghapus data panen. Pertama, program menampilkan daftar panen, lalu mengecek apakah ada data. Jika ada, pengguna diminta memilih nomor item yang ingin dihapus. Nomor tersebut dikurangi 1 agar sesuai dengan indeks ArrayList.

# Penjelasan Output

<img width="612" height="210" alt="image" src="https://github.com/user-attachments/assets/0f9d4463-8c9e-4a10-871a-14a65a742519" />


Ketika program dijalankan, yang pertama ditampilan pengguna adalah menu utama dengan pilihan menu 1 sampai 5. Kemudian, pengguna harus memilih nomor menu yang diinginkan.

<img width="569" height="153" alt="image" src="https://github.com/user-attachments/assets/e0b814d5-cc3c-4c95-9228-0004645ee3c2" />


Pengguna yang memilih nomor 1, maka akan masuk ke menu tambah item. Dimana pengguna dapat menambahkan kategori (sayur/buah), nama, beratkg, dan kualitas hasil panen nya.

<img width="372" height="225" alt="image" src="https://github.com/user-attachments/assets/6f00da0e-f139-4c05-ad71-e0fce6a650a9" />


Selanjutnya jika pengguna memilih nomor 2, maka akan masuk ke menu tampilkanItem. Disini pengguna dapat melihat daftar hasil panen yang sudah diinputkan sebelumnya.

<img width="411" height="379" alt="image" src="https://github.com/user-attachments/assets/3c831731-a594-40ec-b6aa-af7c23261c1d" />


Jika pengguna memilih nomor 3, maka akan masuk ke menu edit item. Dimana pengguna harus memilih item nomor berapa yang akan di edit data nya. setelah memilih, selajutnya barulah pengguna bisa mengedit data item panen.

<img width="415" height="276" alt="image" src="https://github.com/user-attachments/assets/2aefdc3d-8fc1-47a6-8a33-deef62ef6d6f" />


Jika pengguna memilih nomor 4, maka akan masuk ke dalam menu hapus item. Sama juga seperti sebelumnya, pengguna harus memilih terlebih dahulu nomor item hasil panen yang ingin dihapus. Apabila nomor valid, akan ada output "Item berhasil dihapus".

<img width="328" height="200" alt="image" src="https://github.com/user-attachments/assets/867bdac7-fb90-4740-b938-5f38929b68f5" />


Nomor terakhir, yaitu apabila pengguna memilih menu nomor 5 maka program berhenti dan menampilkan output "Terima Kasih yaa" kepada pengguna.

# Post test 2

# Tema

Tema yang digunakan masih sama, yaitu Sistem Pencatatan Hasil Panen Kebun. Perbedaan mendasar dari Posttest 1 adalah struktur program yang telah ditingkatkan dengan penerapan tiga kelas yang masing-masing memiliki properti, constructor, serta access modifier untuk menjaga enkapsulasi data. Program ini juga dikelola menggunakan packages yang dipisahkan berdasarkan fungsinya sesuai pola MVC (Model-View-Controller) sehingga kode menjadi lebih rapi, terorganisir, dan mudah dikembangkan.

Selain itu, pada Posttest 2 ini ditambahkan fitur pencarian (search) yang memudahkan pengguna untuk menemukan data hasil panen tertentu secara cepat. Interaksi dengan program dilakukan melalui input berbasis indeks yang dimasukkan oleh pengguna. Jika terdapat kesalahan dalam input, sistem akan menampilkan validasi berupa peringatan sehingga dapat meminimalisasi kesalahan penggunaan. Penjelasan dalam dokumentasi ini akan difokuskan pada aspek-aspek baru yang membedakan implementasi program dari Posttest sebelumnya.


# Post test 3

# Tema

Sistem Pencatatan Hasil Panen Kebun, dirancang untuk membantu pencatatan, pengelolaan, serta pencarian data hasil panen petani. Program ini menggunakan encapsulation, inheritance, dan polymorphism/overriding untuk memudahkan pengembangan serta pemeliharaan kode.

Dalam sistem ini, hasil panen dikelompokkan menjadi dua kategori utama, yaitu sayur dan buah. Masing-masing kategori memiliki atribut umum seperti nama, berat, dan kualitas, serta atribut khusus (misalnya cara penyimpanan untuk sayur dan lama simpan untuk buah). Pengguna dapat melakukan berbagai operasi melalui menu.

# <sub>Penjelasan kode</sub>

<img width="1091" height="624" alt="image" src="https://github.com/user-attachments/assets/dfd8f90b-b9f1-4d0f-a6e6-4a79630fb3a7" />

<img width="1041" height="380" alt="image" src="https://github.com/user-attachments/assets/83b101f9-f80a-46de-9ca8-2b20e6d449a8" />

Class itemPanen berperan sebagai superclass yang mempresentasikan data umum dari sebuah hasil panen. Didalamnya terdapat properti utama seperti 'nama', 'beratkg', dan 'kualitas'. Menerapkan encapsulation dengan menjadikan atribut private lalu menyediakan getter dan setter agar data hanya bisa diakses melalui method yang sudah disediakan. Memiliki constructor untuk memudahkan pembuatan objek hasil panen baru. Ada juga method tampilkanInfo() yang nantinya bisa di-override oleh subclass untuk menampilkan detail khusus.

<img width="1028" height="623" alt="image" src="https://github.com/user-attachments/assets/632a6adc-384b-4d08-b89b-a549fd0db69f" />

Class buah adalah subclass dari itemPanen yang mempresentasikan hasil panen khusus katefori buah. Menambahkan atribut khusus seperti lamaSimpan untuk menyimpan informasi ketahanan buah. Menggunakan constructor untuk mengisi data buah sekaligus memanggil constructor superclass. Melakukan overriding pada method tampilkanInfo() agar selain menampilkan atribut umum juga menampilkan informasi lama simpan.

<img width="1080" height="628" alt="image" src="https://github.com/user-attachments/assets/8c831c71-4b92-4b51-81c4-f06157ecc8aa" />

Class sayur merupakan subclass dari itemPanen, tapi khusus untuk kategori sayur. Menambahkan atribut tambahan seperti caraSimpan. Constructor dibuat untuk menginisialisasi data sayur dan tetap memanggil constructor superclass. Method tampilkanInfo() juga di-override sehingga informasi khusus sayur ikut tampil selain atribut umum.

<img width="1035" height="673" alt="image" src="https://github.com/user-attachments/assets/07f9b6d3-37ea-4f20-a9fb-cc4b63a91952" />

<img width="1147" height="775" alt="image" src="https://github.com/user-attachments/assets/0a6baf50-9c55-4a6e-b86a-77af40538fe4" />

<img width="1147" height="782" alt="image" src="https://github.com/user-attachments/assets/78aefc21-8d67-47a7-b61b-1a79ab9b0a01" />

<img width="865" height="779" alt="image" src="https://github.com/user-attachments/assets/2bbfe549-54de-4952-8455-682bff60293b" />

<img width="1202" height="324" alt="image" src="https://github.com/user-attachments/assets/65fca370-97af-4244-ab30-4fe09d8bb569" />

Class panenService berguna untuk mengatur logika CRUD  dan pengelolaan data panen. Menyimpan data hasil panen dalam sebuah ArrayList<itemPanen>. Memiliki method untuk melakukan operasi: 
1. tambahItem(), menambahkan data baru (baik buah maupun sayur).
2. tampilkanItem(), menampilkan seluruh data panen, memanggil method.
3. tampilkanInfor(), hasil overriding dari subclass.
4. editItem(), mengubah data berdasarkan index pilihan pengguna.
5. hapusItem(), menghapus item dari daftar panen.
6. cariItem(), fitur tambahan untuk encari panen berdasarkan nama.
Class ini menjadi penghubung utama antara input pengguna dan data yang dikelola.

Class mainProgram adalah entry point atau titik awal eksekusi program. Class ini menyediakan menu interaktif berupa pilihan angka agar pengguna dapat melakukan operasi CRUD, menggunakan objek dari panenService untuk menjalankan logika pengelolaan data. Alur programnya berupa perulangan menu, sehingga program terus berjalan hingga pengguna memilih opsi keluar. Juga menangani validasi input, misalnya jika pengguna memasukkan perintah yang salah, maka sistem menampilkan pesan peringatan.
