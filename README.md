# Lab8Web.


**Dibuat oleh:** 

    Nama: Burhan Isnain Nur Huda
    NIM: 312410226
    Kelas: TI.24.A.2
    Mata Kuliah: Pemograman Web1

# Praktikum 8: PHP dan Database MySQL

## Tujuan
1. Mahasiswa mampu memahami konsep dasar Database
2. Mahasiswa mampu memahami konsep dasar CRUD menggunakan PHP  
3. Mahasiswa mampu membuat program CRUD sederhana menggunakan PHP

## Penjelasan Program
Program ini adalah aplikasi **CRUD (Create, Read, Update, Delete)** sederhana untuk mengelola data barang menggunakan **PHP dan MySQL**. Aplikasi ini memungkinkan pengguna untuk menambah, melihat, mengedit, dan menghapus data barang dengan fitur upload gambar.

### Struktur Database
- **Database**: `latihan1`
- **Tabel**: `data_barang`
- **Field**: id_barang, kategori, nama, gambar, harga_beli, harga_jual, stok

### Arsitektur Aplikasi
- **Frontend**: HTML dengan CSS styling (theme coklat muda)
- **Backend**: PHP native dengan MySQLi
- **Database**: MySQL
- **Server**: XAMPP (Apache + MySQL)

## Langkah-langkah Praktikum

### 1. Persiapan Database
- Membuat database `latihan1`
- Membuat tabel `data_barang` dengan struktur yang sesuai
- Insert data sample untuk testing

### 2. Implementasi CRUD
- **Create** (`tambah.php`) - Menambah data barang baru dengan form input dan upload gambar
- **Read** (`index.php`) - Menampilkan semua data barang dalam tabel responsive  
- **Update** (`ubah.php`) - Mengedit data barang existing dengan form pre-filled
- **Delete** (`hapus.php`) - Menghapus data barang dengan konfirmasi

### 3. Fitur Tambahan
- **Upload dan management gambar** - Support upload image dengan validasi
- **Design responsive** dengan CSS theme coklat muda yang aesthetic
- **Form validation** - Validasi input form untuk data yang benar
- **Konfirmasi hapus data** - Popup konfirmasi sebelum menghapus data
- **Error handling** - Penanganan error koneksi database dan query

## File Structure
lab8_php_database/
├── index.php # Halaman utama (Read)
├── tambah.php # Form tambah data (Create)
├── ubah.php # Form edit data (Update)
├── hapus.php # Proses hapus data (Delete)
├── koneksi.php # Koneksi database
├── style.css # Styling theme coklat muda
└── gambar/ # Folder penyimpanan gambar
├── hp_samsung.jpg
├── hp_xiaomi.jpg
└── hp_oppo.jpg

## Screenshot Hasil
- **Halaman Utama:** <img width="1913" height="953" alt="image" src="https://github.com/user-attachments/assets/4ea96e6b-b93a-441e-a8f9-25874934d93a" />
 
- **Form Tambah Data:** <img width="1912" height="947" alt="image" src="https://github.com/user-attachments/assets/a8ef23a8-663f-4c97-9798-a84eb4b25443" />
<img width="1914" height="948" alt="image" src="https://github.com/user-attachments/assets/b5740854-6dd7-4090-b370-37cc51a7e252" />
- **Hasil Setelah Tambah Data** <img width="1916" height="948" alt="image" src="https://github.com/user-attachments/assets/a1f144ca-8d29-4f9b-a06a-1bf066876fbe" />



- **Form Edit Data:** <img width="1916" height="948" alt="image" src="https://github.com/user-attachments/assets/9a621384-8aec-499f-92df-a06969fe98d8" />
<img width="1914" height="953" alt="image" src="https://github.com/user-attachments/assets/9d5da0db-193c-4160-b640-b02c187c8a94" />
- **Hasil Setelah Edit Data** <img width="1919" height="951" alt="image" src="https://github.com/user-attachments/assets/dab2ac00-d981-4b9a-acfc-2a238293b492" />



## Teknologi Used
- **PHP** - Bahasa pemrograman server-side
- **MySQL** - Database management system
- **HTML/CSS** - Struktur dan styling tampilan
- **XAMPP** - Web server solution stack
- **MySQLi** - PHP extension untuk koneksi MySQL

## Cara Menjalankan
1. Start Apache dan MySQL di XAMPP Control Panel
2. Import database `latihan1` (file SQL tersedia di folder database)
3. Letakkan folder `lab8_php_database` di dalam `htdocs`
4. Akses melalui browser: `http://localhost/lab8_php_database/`

## Cara Penggunaan
1. **Lihat Data**: Buka halaman utama untuk melihat semua data barang
2. **Tambah Data**: Klik "Tambah Barang Baru" → isi form → Simpan
3. **Edit Data**: Klik tombol "Edit" pada data → ubah form → Update
4. **Hapus Data**: Klik tombol "Hapus" → konfirmasi → Data terhapus

## Catatan
- Pastikan folder `gambar` memiliki permission write untuk upload file
- Database configuration dapat diubah di file `koneksi.php`
- Aplikasi sudah responsive dan dapat diakses dari mobile device

