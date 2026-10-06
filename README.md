# TUGAS PWEB LATIHAN CSS

5025251095_Alessandro Almaz Filemon

# LINK WEBSITE
Link Website: https://5025251095latihancss.netlify.app

# Pendahuluan
Tugas ini bertujuan membangun Academic Portal yang memperlihatkan keterkaitan antar HTML sebagai strukturnya, CSS sebagai pengatur layout dan tampilannya, dan JavaScript sebagai interaction. Terdapat beberapa bagian dimana ada bagian Form untuk mengisi NRP, Nama, Major, dan Email yang juga ketika tidak sesuai pengisiannya akan ada warning berwarna merah bahwa isi tidak sesuai. Lalu ada bagian Directory berisi nama semua Mahasiswa/Student yang sudah ditambahkan dari form. Untuk data awal saya sudah memasukkan data Aren Gentong dan Mango The Cat. Pada bagian DIrectory ini juga terdapat Search Bar untuk mencari data mahasiswa sesuai dengan data yang sudah tertera. Terdapat juga pembagian list mahasiswa yang ditampilkan yaitu max 5 orang per pagesnya.

# Struktur
index.html sebagai struktur utama
style.css	sebagai keseluruhan layouting dan tampilan
app.js sebagai data, validasi, tambah, ubah, hapus, pencarian, dan pagination

# HTML
Terdapat elemen header berisi berupa Academic Portal di kiri, navigation bar berupa Home Student Information, dan Profil Admin di kanan. 

Main element terdapat judul halaman dan dua section berbentuk card, yaitu Form untuk menginput NRP, Full name, Major, Email dan Directory untuk menginput data mahasiswa/student lengkap dengan kolom pencarian, badge jumlah data, serta pagination. 

Elemen footer berisi keterangan portal.

# CSS
Navbar - Flexbox dengan justify-content: space-between, bg Dark Cyan, dan underline Tea Green
Layout Utama - CSS Grid dua kolom: 380px untuk formulir dan minmax(0, 1fr) untuk tabel, lebar maksimum 1320px
Card dan Form - Padding, border, radius, dan box-shadow. Jika salah input akan muncul warning kesalahan berwarna merah
Button - Tombol-tombol yang berfungsi sesuai kegunaanya masing masing
Tabel - Berisi data student/mahasiswa
Search, Action, Pagination - Flexbox untuk kolom pencarian, tombol Edit/Delete, dan nomor halaman
Responsive

# JavaScript
Data mahasiswa disimpan pada array objek dengan dua data awal. Fungsi render() menampilkan baris tabel berdasarkan hasil pencarian dan halaman aktif, kemudian memperbarui badge jumlah, teks informasi, dan tombol pagination. Beberapa function:
- Tambah data (Submit Form): Input divalidasi lalu ditambahkan ke array; NRP harus berupa angka (4–12 digit) dan tidak boleh sama dengan data lain, nama minimal 3 karakter, jurusan wajib dipilih, dan format email diperiksa.
- Edit dan Delete: Tombol Edit mengisi formulir dengan data terpilih dan mengubah tombol menjadi Save changes dan tombol Delete meminta konfirmasi sebelum data dihapus.
- Search: pencarian berdasarkan nama atau NRP yang berjalan saat pengguna mengetik.
- Pagination: lima data per page. Badge pada judul daftar menampilkan total seluruh mahasiswa.

# Dokumentasi Tampilan
Laptop:

<img width="1280" height="698" alt="image" src="https://github.com/user-attachments/assets/427f5ad5-2b09-407b-aaad-47ff44f4bbb7" />
<img width="1280" height="697" alt="image" src="https://github.com/user-attachments/assets/1743513c-b1c8-4e5f-b674-34c968e856f7" />


HP:

<img width="720" height="1600" alt="WhatsApp Image 2026-10-07 at 03 20 32" src="https://github.com/user-attachments/assets/152ebba7-1cbe-4075-bd3e-dce380d21356" />
<img width="720" height="1600" alt="WhatsApp Image 2026-10-07 at 03 20 32 (1)" src="https://github.com/user-attachments/assets/215a1c63-588d-43b4-86ae-a3a263ee4253" />
<img width="720" height="1600" alt="WhatsApp Image 2026-10-07 at 03 20 32 (2)" src="https://github.com/user-attachments/assets/fa01c9e5-a436-42b0-b67d-af0b0336ddde" />

# Kesimpulan
Tampilan Portal Academic berhasil dibangun dengan jelas dimana HTML untuk struktur, CSS untuk tampilan dan responsif, dan JavaScript untuk fungsi tambah, ubah, hapus, pencarian, dan pagination. Data masih disimpan di memori browser sehingga hilang saat halaman dimuat ulang.
