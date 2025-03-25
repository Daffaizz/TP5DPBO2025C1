# TP 5 DPBO 2025 C1
# Janji
Saya Daffa Faiz Restu Oktavian dengan NIM 2309013 mengerjakan Tugas Praktikum 2 dalam mata kuliah Desain dan Pemrograman Berorientasi Objek untuk keberkahanNya maka saya tidak melakukan kecurangan seperti yang telah dispesifikasikan. Aamiin.
# Desain Program
1. Struktur Program
- Menu (JFrame - GUI Utama):
    - Menampilkan form input dan tabel mahasiswa.
    - Memproses tambah, edit, hapus, dan reset data.
- DataBase:
    - Menghubungkan aplikasi dengan MySQL.
    - Menjalankan query SELECT, INSERT, UPDATE, DELETE.
- Mahasiswa (Opsional - Model Data):
    - Menyimpan data mahasiswa dalam objek untuk manipulasi lebih mudah.
2. Antarmuka Pengguna (GUI Design)
- Form Input:
    - NIM, Nama, Program Studi (TextField).
    - Jenis Kelamin (ComboBox).
- Tombol Aksi:
    - Add/Update: Menyimpan atau memperbarui data.
    - Delete: Menghapus data (muncul saat baris dipilih).
    - Cancel: Mengosongkan form input.
- Tabel Data Mahasiswa:
    - Menampilkan data dari database.
    - Klik baris untuk edit atau hapus.
# Penjelasan Kelas
1. Kelas Menu (Tampilan GUI dan Logika Aplikasi)
- Kelas utama yang mengelola tampilan pengguna dan interaksi dengan database.
- Menampilkan tabel mahasiswa yang diambil dari database.
- Menyediakan input form untuk memasukkan atau mengubah data mahasiswa.
- Mengelola aksi tombol untuk menambah, mengupdate, menghapus, dan mereset form.
- Menghubungkan ke database menggunakan objek DataBase untuk menjalankan perintah SQL.
2. Kelas Mahasiswa (Model Data)
- Kelas ini merepresentasikan objek Mahasiswa dalam program.
    - Menyimpan informasi NIM, Nama, Jenis Kelamin, dan Program Studi.
    - Digunakan dalam ArrayList untuk menyimpan daftar mahasiswa sementara sebelum ditampilkan dalam tabel GUI.
3. Kelas DataBase (Koneksi dan Akses Database)
- Kelas yang menangani koneksi ke MySQL dan menjalankan perintah SQL.
    - Membuka koneksi ke database saat program dijalankan.
    - Menjalankan query SQL, seperti SELECT, INSERT, UPDATE, DELETE.
    - Mengembalikan hasil query untuk ditampilkan di tabel GUI.
# Alur Program
Aplikasi ini adalah program berbasis GUI (Graphical User Interface) menggunakan Java Swing yang berfungsi untuk mengelola data mahasiswa dengan fitur tambah, ubah, hapus, dan melihat data yang tersimpan dalam database MySQL.
1. Program Dimulai
- Jendela utama (window) ditampilkan dengan ukuran yang telah ditentukan.
- Tabel mahasiswa diisi dengan data dari database MySQL.
- Form input dan tombol aksi ditampilkan (tombol "Delete" disembunyikan).
2. Pengguna Mengelola Data Mahasiswa
- Menambah Data: Pengguna mengisi form dan menekan "Add", sistem menyimpan data ke database jika NIM belum ada.
- Mengedit Data: Pengguna memilih baris tabel, data ditampilkan di form, lalu diperbarui dengan menekan "Update".
- Menghapus Data: Pengguna memilih baris tabel, menekan "Delete", lalu mengonfirmasi penghapusan.
- Membatalkan Input: Menekan "Cancel" untuk mengosongkan form.
3. Interaksi dengan Database
- Data ditampilkan di tabel dengan mengambil informasi dari database menggunakan query SELECT.
- Penambahan, pengeditan, dan penghapusan data dilakukan dengan query INSERT, UPDATE, dan DELETE.
- Setiap perubahan langsung diperbarui di database dan tabel GUI.
4. Respons Sistem
- Jika form tidak lengkap, muncul peringatan agar pengguna melengkapi input.
- Jika NIM sudah ada, muncul notifikasi bahwa data tidak dapat disimpan.
- Jika penghapusan dikonfirmasi, data dihapus dan tabel diperbarui.
- Setelah setiap aksi, form dikosongkan dan tombol kembali ke kondisi awal.
5. Program Berjalan hingga Ditutup
- Pengguna dapat terus mengelola data mahasiswa.
- Saat jendela ditutup, program berhenti dan koneksi ke database dihentikan
# Dokumentasi
### Dialog/prompt error jika masih ada input yang kosong saat insert/update.
<img src = "Dokumentasi/Screenshot 2025-03-25 153143.png">

### Dialog/prompt error jika sudah ada NIM yang sama saat insert.
<img src = "Dokumentasi/Screenshot 2025-03-25 153217.png">

### Insert data dan perubahannya di database.
<img src = "Dokumentasi/Screenshot 2025-03-25 153359.png">
<img src = "Dokumentasi/Screenshot 2025-03-25 153504.png">

### Update data dan perubahannya di database.
<img src = "Dokumentasi/Screenshot 2025-03-25 153611.png">
<img src = "Dokumentasi/Screenshot 2025-03-25 153715.png">

### Delete data dan perubahannya di database.
<img src = "Dokumentasi/Screenshot 2025-03-25 153652.png">
<img src = "Dokumentasi/Screenshot 2025-03-25 153715.png">