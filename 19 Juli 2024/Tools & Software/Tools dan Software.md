# Merangkum Sofwate Development Tools

### Disusun Oleh

| NAMA 
| ---- 
| [Adam Rasyid Nurmuhammad](https://github.com/adamrasyid01)| 

1. [IDE](#1-ide)
2. [DB Viewer](#2-db-viewer)
3. [PostgreSQL](#3-postgresql)
4. [Docker](#4-docker)
5. [Gitlab](#5-gitlab)
6. [Figma](#6-figma)
7. [Odoo](#7-odoo)
8. [Emulator](#8-emulator)
9. [Postman](#9-postman)
10. [Google Spreadsheet](#10-google-spreadsheet)
11. [Google Doc](#11-google-docs)
12. [Data Modelling](#12-data-modelling)



# 1. IDE

Integrated Development Environment adalah rangkaian software yang menyatukan semua tool pengembangan menjadi satu GUI (Graphical User Interface). Dengannya, proses pengembangan bisa menjadi lebih efisien dan lebih cepat.

- Jenis IDE 

```
Multilanguage

Mendukung banyak program bahasa yang bisa membantu pemula meningkatkan skill. Misalnya, Visual Studio 

Mobile development

secara khusus dibangun untuk mobile development, seperti AppCode dan Android Studio.

Language-specific 

dirancang untuk developer software yang bekerja menggunakan satu bahasa. Contohnya, Jikes dan Jcreator dibuat untuk Java, dan Idle untuk Python

Cloud-based

Menyediakan fitur built-in untuk pair programming real-time dengan feedback langsung yang memungkinkan developer membuat software hanya menggunakan browser

HTML

digunakan untuk mengembangkan aplikasi HTML seperti Notepad++, Atom, dan Adobe DreamWeaver CC. Tool ini mengotomatiskan banyak tugas dalam web development.
```

# 2. DB Viewer
DB Viewer (Database Viewer) adalah perangkat lunak atau alat yang digunakan untuk melihat dan mengelola basis data


| **Fitur/Alat**    | **Navicat**                                      | **DBeaver**                                  | **TablePlus**                                 |
|-------------------|--------------------------------------------------|----------------------------------------------|----------------------------------------------|
| **Dukungan Basis Data** | MySQL, PostgreSQL, Oracle, SQLite, SQL Server, MariaDB, dan lainnya | MySQL, PostgreSQL, SQLite, Oracle, SQL Server, DB2, Sybase, Teradata, MongoDB, Cassandra, Redis, dan lainnya | MySQL, PostgreSQL, SQLite, SQL Server, Redis, Cassandra, CockroachDB, dan lainnya |
| **Antarmuka Pengguna** | Ramah dan mudah digunakan                    | Bersih dan intuitif                          | Modern dan intuitif                          |
| **Pemodelan Basis Data** | Ya                                           | Ya                                           | Tidak                                         |
| **Sinkronisasi Data dan Skema** | Ya                                           | Ya                                           | Tidak                                         |
| **Ekspor dan Impor Data** | Ya                                           | Ya                                           | Ya                                           |
| **Editor SQL**    | Ya                                           | Ya                                           | Ya                                           |
| **Visualisasi Data** | Ya                                           | Ya                                           | Ya                                           |
| **Otomatisasi Tugas** | Ya (dengan penjadwalan)                        | Tidak                                         | Tidak                                         |
| **Plugin dan Ekstensi** | Tidak                                         | Ya                                           | Tidak                                         |
| **Multi-Platform** | Windows, macOS, Linux                          | Windows, macOS, Linux                        | macOS, Windows (beta)                        |
| **Harga**         | Berbayar (dengan uji coba gratis)               | Gratis (open-source) dan versi berbayar (Enterprise) | Berbayar (dengan uji coba gratis)           |
| **Ideal untuk**   | Pengguna yang membutuhkan alat komprehensif dengan banyak fitur manajemen basis data | Pengguna yang membutuhkan fleksibilitas tinggi dan dukungan banyak basis data | Pengguna yang mencari alat cepat dan mudah digunakan untuk manajemen basis data dasar |

# 3. PostgreSQL

| **Kategori**              | **Deskripsi**                                                                                       |
|---------------------------|-----------------------------------------------------------------------------------------------------|
| **Nama**                  | PostgreSQL                                                                                          |
| **Tipe**                  | Sistem Manajemen Basis Data Relasional Objek (ORDBMS)                                               |
| **Lisensi**               | Open Source, di bawah lisensi PostgreSQL                                                            |
| **Situs Resmi**           | [postgresql.org](https://www.postgresql.org)                                                        |
| **Fitur Utama**           | - Kepatuhan SQL<br>- Ekstensi dan Penyesuaian<br>- Tipe Data Beragam<br>- Transaksi ACID<br>- Indeks dan Optimisasi<br>- Replikasi dan Ketersediaan Tinggi<br>- Keamanan |
| **Sejarah Singkat**       | - Awal Mula: Dikembangkan di University of California, Berkeley, pada akhir 1980-an<br>- Rilis Pertama: 1989 sebagai Postgres, berganti nama menjadi PostgreSQL pada pertengahan 1990-an |


# 4. Docker

Docker adalah platform yang dirancang untuk membuat, mengirim, dan menjalankan aplikasi di dalam container. Container adalah lingkungan terisolasi yang mencakup semua yang dibutuhkan untuk menjalankan aplikasi, seperti kode, runtime, alat sistem, pustaka, dan pengaturan.

### 1. **Konsep Dasar Docker**
- **Container**: Unit standar perangkat lunak yang memaketkan kode dan semua dependensinya sehingga aplikasi berjalan secara konsisten di berbagai lingkungan.
- **Image**: Templat hanya-baca yang digunakan untuk membuat container. Images biasanya dibangun dari Dockerfile.
- **Dockerfile**: File teks yang berisi serangkaian instruksi untuk membangun image Docker.
- **Docker Engine**: Runtime yang menjalankan container.


### 2. **Komponen Utama Docker**
- **Docker Hub**: Registry publik yang memungkinkan Anda untuk berbagi, menyimpan, dan mendistribusikan image Docker.
- **Docker Compose**: Alat untuk mendefinisikan dan menjalankan aplikasi multi-container. File `docker-compose.yml` digunakan untuk mengonfigurasi layanan aplikasi.
- **Docker Swarm**: Orkestrator native Docker untuk mengelola cluster dari Docker Engine, memungkinkan deployment dan manajemen container secara terdistribusi.

### 3. **Perintah Dasar Docker**
- **docker run**: Menjalankan container dari sebuah image.
- **docker build**: Membangun image dari Dockerfile.
- **docker pull**: Mengunduh image dari registry seperti Docker Hub.
- **docker push**: Mengunggah image ke registry.
- **docker ps**: Menampilkan daftar container yang sedang berjalan.
- **docker stop**: Menghentikan container yang sedang berjalan.
- **docker rm**: Menghapus container.
- **docker rmi**: Menghapus image.

### 4. **Penggunaan Docker dalam Proyek**
- **Development**: Menyediakan lingkungan pengembangan yang konsisten di berbagai mesin.
- **CI/CD**: Mengotomatisasi build, testing, dan deployment aplikasi.
- **Deployment**: Menyederhanakan deployment aplikasi ke berbagai lingkungan, termasuk cloud dan on-premises.

# 5. Gitlab

| **Aspek**            | **Detail**                                                                                                   |
|----------------------|---------------------------------------------------------------------------------------------------------------|
| **Konsep Dasar**     | Platform DevOps berbasis web yang menyediakan repositori Git dan fitur untuk pengembangan perangkat lunak.     |
| **Komponen Utama**   | - **Repository**: Tempat menyimpan dan mengelola kode sumber.<br>- **Issues**: Alat untuk pelacakan tugas dan bug.<br>- **Merge Requests (MR)**: Proses untuk menggabungkan perubahan kode dengan tinjauan.<br>- **Pipelines**: Rangkaian proses otomatisasi CI/CD.<br>- **Milestones**: Mengelola dan melacak progres proyek.<br>- **Wikis**: Dokumentasi proyek. |
| **Perintah Dasar**   | - `git clone`: Mengunduh salinan repositori.<br>- `git push`: Mengirim perubahan ke repositori remote.<br>- Create Issue: Membuat issue baru.<br>- Create Merge Request: Membuat merge request untuk perubahan kode.<br>- Run Pipeline: Menjalankan pipeline CI/CD secara manual. |
| **Penggunaan**       | - **Version Control**: Mengelola dan melacak kode sumber.<br>- **CI/CD Pipelines**: Mengotomatisasi build, testing, dan deployment.<br>- **Code Review**: Memfasilitasi tinjauan kode.<br>- **Project Management**: Mengelola tugas dan progres proyek.<br>- **Security**: Fitur keamanan seperti vulnerability management dan secret detection. |

# 6. Figma

### Konsep Dasar
Figma adalah alat desain antarmuka pengguna (UI) dan pengalaman pengguna (UX) berbasis web yang memungkinkan kolaborasi real-time antara tim.

### Fitur Utama
- **Design**: Alat untuk membuat dan mendesain antarmuka pengguna dengan berbagai elemen desain seperti frame, shapes, dan text.
- **Prototyping**: Fitur untuk membuat prototipe interaktif, memungkinkan pengguna untuk mendemonstrasikan alur dan interaksi antarmuka.
- **Components**: Memungkinkan penggunaan komponen dan simbol untuk memastikan konsistensi desain di seluruh proyek.
- **Collaboration**: Mendukung kolaborasi langsung dan real-time, sehingga beberapa pengguna bisa bekerja pada desain yang sama secara bersamaan.
- **Feedback**: Memungkinkan tim untuk memberikan komentar dan umpan balik langsung pada elemen desain.
- **Version Control**: Menyediakan riwayat perubahan desain dan opsi untuk mengembalikan versi sebelumnya.

### Penggunaan
- **Desain UI/UX**: Digunakan untuk mendesain antarmuka aplikasi dan website.
- **Prototyping**: Membantu dalam mengembangkan prototipe interaktif untuk pengujian dan demonstrasi.
- **Kolaborasi Tim**: Memfasilitasi kerja sama tim secara real-time dan umpan balik langsung.
- **Dokumentasi Desain**: Menyimpan dan mengelola dokumentasi desain secara terpusat.

# 7. Odoo
# 8. Emulator
# 9. Postman
# 10. Google Spreadsheet
# 11. Google Docs
# 12. Data Modelling 
