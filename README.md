DAFTAR ISI
==========
- [LAPORAN LATIHAN STRING](#laporan-latihan-string)  
    - [CODE PROGRAM STRING](#code-program-string)
    - [KESIMPULAN](#kesimpulan)


# LAPORAN LATIHAN STRING


## CODE PROGRAM STRING

### Step 1 : 
Kode ini mengimpor library re (regular expression) yang digunakan untuk pencocokan pola pada string. Dalam program ini, library ini digunakan untuk memvalidasi nama.

Selain itu, Method _init_ adalah konstruktor yang dijalankan saat objek kelas dibuat. Di sini, atribut data_mahasiswa diinisialisasi sebagai list kosong untuk menyimpan data mahasiswa.

![1 (2)](https://github.com/user-attachments/assets/35b609ed-0072-4bb2-a228-9b63b46a95da)

### Step 2 : 
Fungsi ini digunakan untuk memvalidasi data pendaftaran. Parameter name, phone, dan email adalah input pengguna. Sebuah list kosong bernama errors disiapkan untuk menyimpan pesan kesalahan jika ada.

![2 (1)](https://github.com/user-attachments/assets/07ef8aba-cda8-4cd7-b1f0-d4fe0aba974f)

- Validasi Nama : re.match(r'^[A-Za-z\s]+$', name) memeriksa apakah nama hanya berisi huruf (A-Z atau a-z) dan spasi (\s), Jika nama tidak sesuai dengan pola tersebut,
  pesan kesalahan ditambahkan ke list errors.

![3 (2)](https://github.com/user-attachments/assets/c2cfc669-4334-43ff-aaf4-019028770229)


- Validasi Nomor Telepon : phone.isdigit() memeriksa apakah input nomor telepon hanya terdiri dari angka, Jika ada karakter lain (seperti huruf atau simbol), pesan kesalahan ditambahkan.

![4 (1)](https://github.com/user-attachments/assets/d5eac59e-3dcc-4d07-b784-cc5b44db1819)


- Validasi Email : Memeriksa apakah email mengandung simbol (@) dan (.) Jika tidak, pesan kesalahan ditambahkan.

![5 (3)](https://github.com/user-attachments/assets/6408590f-e251-4c5a-b3ba-2361f1725399)

### Step 3 :
Jika terdapat kesalahan (list errors tidak kosong), setiap pesan kesalahan ditampilkan satu per satu, Jika tidak ada kesalahan, program menampilkan pesan bahwa data pendaftaran valid.

![6 (1)](https://github.com/user-attachments/assets/89ceb7a6-559e-45b3-8e5f-c8752d9ec87a)

### Step 4 :
Program meminta pengguna untuk memasukkan:
- Nama lengkap (name)
- Nomor telepon (phone)
- Email (email)

![7 (1)](https://github.com/user-attachments/assets/2d849c02-6e2c-4a5b-bc3f-5fefebfe8e27)

### Step 5 :
Input dari pengguna dikirim ke fungsi validate_registration untuk diperiksa validitasnya.
 

![8 (1)](https://github.com/user-attachments/assets/d9eb1647-6330-4e2a-ab0d-5739865a9a89)


### Step 6 : 
Tahap akhir adalah uji coba code program yang sudah dibuat dengan mencoba berbagai kemungkinan yang ada.


![Screenshot 2025-01-03 155927](https://github.com/user-attachments/assets/75222870-1b83-402f-8dbe-b277b84d1a63)



## KESIMPULAN
Program ini merupakan aplikasi sederhana untuk memvalidasi data pendaftaran pengguna dengan memeriksa format nama lengkap, nomor telepon, dan email. Validasi dilakukan menggunakan regular expression dan metode bawaan Python untuk memastikan nama hanya berisi huruf dan spasi, nomor telepon hanya terdiri dari angka, serta email mengandung karakter @ dan . sebagai tanda dasar format yang benar. Jika data yang dimasukkan tidak memenuhi kriteria, program akan memberikan pesan kesalahan yang spesifik untuk setiap input. Meskipun efektif untuk validasi dasar, program ini dapat ditingkatkan dengan validasi yang lebih ketat, seperti memeriksa struktur lengkap email, panjang nomor telepon, atau dukungan untuk karakter khusus pada nama. Program ini cocok sebagai pondasi awal untuk aplikasi pendaftaran yang lebih kompleks.
