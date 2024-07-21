
# TUGAS Kamis 18 / 07 / 2024

# Disusun Oleh

| NAMA 
| ---- 
| [Adam Rasyid Nurmuhammad](https://github.com/adamrasyid01)| 

**DAFTAR ISI**

Fundamental Pemrograman

1. [Konsep Dasar Pemrograman](#1-konsep-dasar-pemrograman)
2. [Jenis Bahasa Pemrograman](#2-jenis-bahasa-pemrograman)
3. [Logika Bahasa Pemrograman](#3-logika-bahasa-pemrograman)
4. [Paradigma Pemrograman](#4-paradigma-pemrograman)


Fundamental Javascript

1. [Tipe Data](#4-paradigma-pemrograman)
2. [Operator](#4-paradigma-pemrograman)
3. [Function](#4-paradigma-pemrograman)
4. [Looping](#4-paradigma-pemrograman)
5. [Percabangan](#4-paradigma-pemrograman)
6. [TypeCasting](#4-paradigma-pemrograman)
7. [Variabel](#4-paradigma-pemrograman)



Fundamental Pemrograman
# 1. Konsep Dasar Pemrograman

Pemrograman adalah aktivitas memberikan perintah terhadap komputer untuk melakukan tugas-tugas tertentu menggunakan bahasa pemrograman. Bahasa pemrograman sendiri merupakan instruksi-instruksi yang dimengerti oleh komputer untuk melakukan tugas tertentu. Kumpulan tugas-tugas yang dapat dilakukan oleh komputer tersebut kemudian akan menjadi program atau perangkat lunak.

# 2. Jenis Bahasa Pemrograman

Bahasa pemrograman yang dapat dimengerti oleh manusia dapat dikelompokkan menjadi dua, yaitu:

* 2.1 Bahasa pemrograman  tingkat  rendah.

* 2.2 Bahasa pemrograman tingkat  tinggi.

# 3. Logika Bahasa Pemrograman

* Sekuensial

  Instruksi dalam bahasa pemrograman tersusun secara berurutan. Sebuah instruksi akan dijalankan apabila instruksi sebelumnya telah dilakukan.

* Percabangan/bersyarat (conditional)

  Sebuah instruksi bisa juga tidak akan dijalankan apabila suatu syarat tidak terpenuhi. Demikian pula sebaliknya, sebuah instruksi akan dijalankan ketika suatu syarat terpenuhi. 

* Perulangan (loop).

  Memungkinkan eksekusi suatu blok kode berulang kali hingga suatu kondisi tertentu terpenuhi. Ini sangat berguna untuk mengotomatisasi tugas-tugas yang berulang


# 4. Paradigma Pemrograman
Paradigma pemrograman adalah pendekatan atau gaya dalam menulis dan mengorganisir kode dalam pengembangan perangkat lunak. Ada beberapa paradigma pemrograman yang umum digunakan, masing-masing dengan karakteristik dan prinsip yang berbeda. Berikut beberapa paradigma pemrograman yang populer:

1. **Pemrograman Prosedural**: Berfokus pada urutan langkah-langkah atau instruksi yang harus diikuti untuk menyelesaikan tugas. Contoh bahasa: C, Pascal.

2. **Pemrograman Berorientasi Objek (OOP)**: Mengorganisir kode ke dalam objek yang memiliki atribut (data) dan metode (fungsi). Contoh bahasa: Java, C++, Python.

3. **Pemrograman Fungsional**: Berdasarkan pada fungsi matematika dan penghindaran perubahan status (immutable). Contoh bahasa: Haskell, Lisp, Scala.

4. **Pemrograman Logika**: Menggunakan aturan logika untuk mendeskripsikan hubungan dan inferensi dari fakta-fakta. Contoh bahasa: Prolog.

5. **Pemrograman Deklaratif**: Menyatakan apa yang harus dilakukan tanpa mendefinisikan bagaimana caranya. Contoh: SQL untuk query database, HTML untuk markup web.

6. **Pemrograman Berbasis Acara (Event-Driven)**: Tergantung pada peristiwa atau aksi yang terjadi (seperti klik tombol). Contoh bahasa: JavaScript, C# dengan WinForms atau WPF.

7. **Pemrograman Konkurensi (Concurrency)**: Berfokus pada pengelolaan eksekusi simultan dari beberapa proses atau thread. Contoh bahasa: Go, Erlang.

8. **Pemrograman Reaktif**: Menangani aliran data dan perubahan status secara asynchronous. Contoh: RxJS (Reactive Extensions for JavaScript), React.

# Fundamental Javascript

## Tipe Data dalam JavaScript

1. **String (teks)**:
   - Tipe data yang digunakan untuk menyimpan teks. String adalah urutan karakter yang diapit oleh tanda kutip tunggal (`'`) atau ganda (`"`).
   - Contoh: `"Hello, World!"`, `'Adam Rasyid'`

2. **Integer atau Number (bilangan bulat)**:
   - Dalam JavaScript, tipe data untuk angka termasuk bilangan bulat dan pecahan, semuanya menggunakan tipe `Number`.
   - Bilangan bulat adalah angka tanpa komponen desimal.
   - Contoh: `42`, `-7`, `1000`

3. **Float (bilangan Pecahan)**:
   - Float juga merupakan tipe data `Number` dalam JavaScript yang mewakili angka dengan komponen desimal.
   - Contoh: `3.14`, `-0.001`, `2.718`

4. **Boolean**:
   - Tipe data yang hanya memiliki dua nilai: `true` atau `false`. Tipe data ini sering digunakan dalam kondisi logika dan pernyataan kontrol.
   - Contoh: `true`, `false`

5. **Object**:
   - Tipe data yang digunakan untuk menyimpan koleksi data yang lebih kompleks. Object berisi pasangan kunci-nilai (key-value pairs), di mana kuncinya adalah string (atau simbol) dan nilainya bisa berupa tipe data apa pun.
   - Contoh:
     ```javascript
     let person = {
       name: "Adam",
       age: 30,
       isDeveloper: true
     };
     ```

# 2. Operator
Operator adalah simbol yang digunakan untuk melakukan operasi pada suatu nilai dan variabel.


Terdapat berbagai jenis operator dalam JavaScript:

`Operator Aritmatika`

| Operator | Deskripsi                   | 
|----------|-----------------------------|
| +        | Penjumlahan                 |
| -        | Pengurangan                 |
| *        | Perkalian                   |
| **       | Pemangkatan (ES2016)        |
| /        | Pembagian                   |
| %        | Modulus (Sisa Pembagian)    |
| ++       | Increment (Penambahan)      |
| --       | Decrement (Pengurangan)     |


`Operator Penugasan`

| Operator | Deskripsi | Sama seperti
|----------|-----------| ----------------
| =        | x = y     | x = y
| +=       | x += y    | x = x + y
| -=       | x -= y    | x = x - y
| *=       | x *= y    | x = x * y
| /=       | x /= y    | x = x / y
| %=       | x %= y    | x = x % y
| **=      | x **= y   | x = x ** y


`Operator Perbandingan`
| Operator | Deskripsi                   | 
|----------|-----------------------------|
| ==       | sama dengan                 |
| ===      | sama nilainya dan tipenya   |
| !=       | tidak sama dengan           |
| !==      | tak sama nilai dan tipenya  |
| >        | lebih dari                  |
| <        | kurang dari                 |
| >=       | lebih dari sama dengan      |
| <=       | kurang dari sama dengan     |
| ?        | operator ternary            |

`Operator String`


`Operator Logika`
| Operator | Deskripsi                 | 
|----------|---------------------------|
| &&       | logika AND                |
| I         | logika or                |
| !        | tidak sama dengan         |


`Operator Bitwise`

| Operator | Description | 
| :------: | :--------: |
| &   | AND     | 
| I    | OR      |
| ~    | NOT     | 
| ^    | XOR     | 
| <<    | left shift      | 
| >>    | right shift    | 
| >>>    | unsigned right shift     |

`Operator Ternary`


`Operator Tipe`

| Operator          | Deskripsi                              | 
|-------------------|----------------------------------------|
| typeof            | Mengembalikan tipe dari variabel       |
| instanceof        | Mengembalikan true jika merupakan objek|

# 3. Fungsi
