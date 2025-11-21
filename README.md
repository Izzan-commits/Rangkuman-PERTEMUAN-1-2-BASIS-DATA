# 📘 Rangkuman BAB 1 — Entity Relationship Diagram (ERD)
<br>
<br>

# 📘 Bab 1 — Entity Relationship Diagram (ERD)

Pada **Bab 1**, kita mempelajari dasar perancangan database menggunakan **Entity Relationship Diagram (ERD)**. ERD membantu kita memvisualisasikan struktur data, objek-objek yang terlibat, serta bagaimana hubungan antar data tersebut terbentuk.  

Diagram ini penting sebagai langkah awal sebelum membuat database sebenarnya, karena memberikan gambaran jelas mengenai apa yang akan disimpan dan bagaimana data saling terhubung.

---

## ✨ Komponen Utama dalam ERD

Di bawah ini adalah komponen yang harus dipahami dalam ERD beserta penjelasan dan simbolnya.

---

## 🔷 1. Entitas
**Entitas** adalah objek utama yang datanya ingin disimpan dalam database. Entitas bisa berupa orang, barang, aktivitas, atau objek lain yang relevan.  
Contoh: `Mahasiswa`, `Produk`, `Pelanggan`, `Transaksi`.

**🖼️ Simbol:**  
Entitas digambarkan sebagai **kotak (rectangle)**.

---

## 🟡 2. Atribut
**Atribut** adalah informasi atau karakteristik yang dimiliki oleh entitas. Misalnya, entitas *Mahasiswa* dapat memiliki atribut seperti `NIM`, `Nama`, `Alamat`, dan `Kelas`.

**🖼️ Simbol:**  
Atribut digambarkan dengan **oval (ellipse)** yang terhubung ke entitas melalui garis.

---

## 🔑 3. Primary Key (PK)
**Primary Key** adalah atribut unik yang digunakan untuk membedakan setiap record dalam entitas. PK tidak boleh kosong dan tidak boleh duplikat.  
Contoh: `ID_Produk`, `NIM`, `ID_Pelanggan`.

**🖼️ Simbol:**  
Masih berupa **oval**, namun diberi **garis bawah (underline)** untuk menandai bahwa atribut tersebut adalah kunci utama.

---

## 🔶 4. Relasi
**Relasi** adalah hubungan antar entitas. Relasi menggambarkan bagaimana dua entitas atau lebih saling terhubung.  
Contoh:  
- Pelanggan **melakukan** Pesanan  
- Guru **mengajar** Mata Pelajaran  

**🖼️ Simbol:**  
Relasi digambarkan menggunakan **belah ketupat (diamond)** yang terhubung ke entitas melalui garis.

---

## 🔗 5. Kardinalitas
**Kardinalitas** menunjukkan tingkat atau jumlah hubungan antar entitas. Kardinalitas menjelaskan berapa banyak satu entitas dapat berhubungan dengan entitas lain.

Contohnya:  
- **1 : 1** → Satu guru memiliki satu ruang kerja  
- **1 : M** → Satu pelanggan dapat membuat banyak pesanan  
- **M : N** → Banyak siswa dapat mengambil banyak mata pelajaran  

**🖼️ Simbol:**  
Ditunjukkan dengan angka **1, M, N** yang ditempatkan pada garis relasi.

---

## 📌 Ringkasan Singkat
- ERD digunakan untuk memodelkan struktur database.  
- Komponen utama: **Entitas**, **Atribut**, **Primary Key**, **Relasi**, dan **Kardinalitas**.  
- Setiap bagian memiliki **simbol khusus** yang memudahkan pemahaman visual.  
- ERD menjadi langkah awal sebelum implementasi ke tabel database.

---

# 📘 Bab 2 — Pengantar Basis Data

Pada **Bab 2**, kita mulai memahami konsep dasar sistem basis data, khususnya menggunakan **MySQL** sebagai DBMS (Database Management System). Bab ini membahas apa itu basis data, mengenal MySQL Server & Client, tipe data, data relasional, serta perintah dasar untuk membuat, melihat, mengakses, dan menghapus database menggunakan perintah DDL.

---

# 🗂️ 1. Pengertian Basis Data

**Basis data (database)** adalah kumpulan data yang dikelola dan disimpan secara terstruktur sehingga mudah digunakan, dirawat, dan diakses.  
Tujuan penggunaan basis data:
- Mempermudah pengelolaan data  
- Menghindari redudansi  
- Mempercepat pencarian data  
- Menjaga keamanan dan konsistensi data  

---

# 🐬 2. MySQL sebagai DBMS

**MySQL** adalah DBMS yang populer, cepat, dan banyak digunakan pada web server atau aplikasi. MySQL menggunakan bahasa **SQL** (Structured Query Language) untuk mengelola data.

Keunggulan MySQL:
- Open-source  
- Stabil dan cepat  
- Mendukung model data relasional  
- Banyak tools pendukung  

MySQL terdiri dari 2 komponen utama:
1. **MySQL Server** → Tempat penyimpanan dan pengolahan data  
2. **MySQL Client** → Media untuk berinteraksi/menjalankan perintah SQL  

---

# 🖥️ 3. Aplikasi Server MySQL

**MySQL Server (mysqld)** adalah layanan yang menjalankan proses penyimpanan, pengolahan, dan manajemen database.  
Jika server tidak berjalan, MySQL tidak bisa digunakan.

Peran MySQL Server:
- Menyimpan database  
- Menjalankan query  
- Mengatur koneksi client  
- Menjaga keamanan data  

---

# 💻 4. Cara Mengakses MySQL (Client)

Untuk masuk ke MySQL, kita dapat menggunakan **command line** atau **GUI**.

### 🔹 1. Command Line (CLI)
Masuk ke MySQL menggunakan username (biasanya `root`):

```bash
mysql -u root -p
```

### 🗃️ 5. Data Relasional

Data disimpan dalam bentuk tabel yang saling terhubung dengan primary key dan foreign key.

Ciri-cirinya:

Data terstruktur dalam tabel

Memiliki PK untuk identitas unik

Tabel bisa saling terhubung

Mudah dikelola dan dianalisis

### 🧩 6. DDL (Data Definition Language)

DDL digunakan untuk membuat, melihat, menggunakan, dan menghapus database atau tabel.

```Membuat 
CREATE DATABASE nama_database;
```

```Mengakses
USE nama_database;
```

```Menghapus
DROP DATABASE nama_database;
```
