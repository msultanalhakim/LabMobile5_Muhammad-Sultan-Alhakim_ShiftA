# Tugas Praktikum Pemrograman Mobile 5
Nama       : Muhammad Sultan Alhakim

NIM        : H1D022105

Shift Baru : A

1. Proses Login

a. Tahapan Login Pertama

Pada tahap ini, pengguna diminta untuk memasukkan username dan password pada halaman login aplikasi. Kedua data tersebut akan dikirimkan melalui metode POST ke server untuk proses autentikasi. Jika data yang dimasukkan benar dan telah teregister di dalam database, pengguna akan dialihkan ke halaman utama aplikasi.

![image](https://github.com/user-attachments/assets/f4a5ca0d-223e-497b-b504-96cd4553e8ce)

b. Gagal Login

Gambar di bawah menunjukkan notifikasi kesalahan ketika login gagal. Hal ini biasanya terjadi jika username atau password tidak cocok dengan data yang ada di database. Aplikasi menampilkan pesan error yang mengindikasikan bahwa pengguna belum teregister atau data yang dimasukkan salah. Pada tahap ini, pengguna bisa memilih untuk coba login lagi atau menuju halaman register jika belum memiliki akun.

![image](https://github.com/user-attachments/assets/f14854a7-35b1-4b99-9248-88ba0a56dc60)

![image](https://github.com/user-attachments/assets/d9771695-c348-4464-b460-c096103ad49a)

2. Proses Register

Pada proses ini, pengguna mengisi formulir pendaftaran yang berisi data seperti nama, email, password, dan informasi lain yang diperlukan untuk membuat akun baru. Setelah form diisi dengan lengkap dan benar, data tersebut akan dikirimkan ke server melalui metode POST untuk dilakukan validasi dan penyimpanan. Jika validasi berhasil, akun pengguna akan tersimpan di database, dan pengguna dapat melakukan login.

![image](https://github.com/user-attachments/assets/5011cb9c-23e9-43fa-9859-50b855d401e5)

![image](https://github.com/user-attachments/assets/ecb26692-9df1-4fc5-b240-bb424034f0b3)

3. Proses Tampil Produk
   
Setelah berhasil login, pengguna dapat melihat daftar produk yang tersedia. Proses ini melibatkan pengambilan data produk dari server yang ditampilkan dalam bentuk list di aplikasi. Data ini ditarik dari API dengan metode GET, yang kemudian diolah untuk ditampilkan dalam UI aplikasi.

![Screenshot 2024-10-07 204521](https://github.com/user-attachments/assets/727cea4e-5dda-4a66-8904-c34a3609c900)

4. Proses Tambah Produk
   
Pengguna dapat menambahkan produk baru melalui formulir tambah produk. Setelah data produk diisi seperti nama produk, deskripsi, dan harga, data tersebut dikirimkan ke server menggunakan metode POST. Jika data berhasil diterima oleh server, produk baru akan disimpan di database dan dapat dilihat di halaman daftar produk.

![image](https://github.com/user-attachments/assets/4bc01b10-8bd0-438e-8c5c-feda150b0864)

![image](https://github.com/user-attachments/assets/165c4e5c-a3e5-4b4e-aebd-cdd360f31858)

5. Proses Detail Produk
   
Pengguna dapat melihat detail dari produk tertentu dengan memilih produk yang ingin dilihat dari daftar. Proses ini memerlukan permintaan GET dari API yang akan mengembalikan data lengkap dari produk tersebut, termasuk gambar produk, harga, deskripsi, dan informasi lainnya.

![image](https://github.com/user-attachments/assets/f0cd981a-8ff0-4354-87ef-bdc2cea168cb)

6. Proses Ubah Produk
   
Jika pengguna memiliki izin untuk mengedit produk, mereka dapat melakukan perubahan terhadap data produk yang ada. Setelah melakukan perubahan, data yang telah diubah dikirimkan ke server melalui metode PUT atau PATCH. Server kemudian memperbarui data produk di database. Jika berhasil, perubahan akan langsung terlihat di daftar produk.

![image](https://github.com/user-attachments/assets/cd0e24fc-6d9c-4b19-a311-c07e3e27a5b0)

![image](https://github.com/user-attachments/assets/ca048d84-8a85-4477-a38e-0ee66077e7e6)

7. Proses Hapus Produk
   
Untuk menghapus produk, pengguna dapat memilih produk yang ingin dihapus dan mengonfirmasi tindakan tersebut. Data produk akan dikirim ke server menggunakan metode DELETE, dan jika berhasil, produk akan dihapus dari database. Daftar produk akan diperbarui, dan produk yang telah dihapus tidak akan lagi muncul.

![image](https://github.com/user-attachments/assets/ca89e684-66e6-4864-a2e1-7bd2cfc20570)

![image](https://github.com/user-attachments/assets/588fea36-5c20-488e-a5e2-7f4b93d92f9e)

![image](https://github.com/user-attachments/assets/3916d0b1-ff27-4c89-89d5-5fbeb2fc5bb0)

8. Proses Logout
   
Pengguna dapat melakukan logout setelah selesai menggunakan aplikasi. Proses ini akan menghapus session token dari aplikasi, mengakhiri sesi login saat ini, dan mengarahkan pengguna kembali ke halaman login. Dengan demikian, pengguna harus melakukan login kembali jika ingin mengakses fitur aplikasi.

![image](https://github.com/user-attachments/assets/e2bd9904-9592-4830-b9a4-51e8aa5905af)

Proses-proses tersebut adalah bagian dari implementasi mobile programming berbasis Flutter yang terhubung dengan API untuk melakukan CRUD (Create, Read, Update, Delete).
