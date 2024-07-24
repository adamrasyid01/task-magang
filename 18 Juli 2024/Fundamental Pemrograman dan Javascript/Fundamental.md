
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

1. [Tipe Data](#tipe-data-dalam-javascript)
2. [Operator](#2-operator)
3. [Function](#3-fungsi)
4. [Looping](#4-looping)
5. [Percabangan](#5-percabangan)
6. [TypeCasting](#6-typecasting)
7. [Variabel](#7-variabel)



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

Berikut adalah rangkuman berbagai cara membuat fungsi dalam JavaScript dalam bentuk tabel:

| Metode | Sintaks | Keterangan |
|---|---|---|
| **Function Declaration** | `function myFunction() { // kode }` | Metode tradisional untuk mendefinisikan fungsi dengan nama tertentu. |
| **Function Expression** | `const myFunction = function() { // kode };` | Membuat fungsi yang dapat disimpan dalam variabel. |
| **Arrow Function** | `const myFunction = () => { // kode };` | Sintaks yang lebih ringkas, sering digunakan untuk callback. |
| **Anonymous Function** | `setTimeout(function() { // kode }, 1000);` | Fungsi tanpa nama, biasanya digunakan dalam callback. |
| **IIFE (Immediately Invoked Function Expression)** | `(function() { // kode })();` | Fungsi yang dijalankan segera setelah didefinisikan. |
| **Generator Function** | `function* myGeneratorFunction() { yield 'nilai'; }` | Membuat iterasi yang dapat dihentikan sementara dan dilanjutkan. |
| **Async Function** | `async function myAsyncFunction() { // kode }` | Menangani operasi asinkron dengan cara yang lebih mudah. |
| **Constructor Function** | `function MyConstructor() { this.property = 'nilai'; } const obj = new MyConstructor();` | Membuat objek baru dengan properti dan metode tertentu. |

# 4. Looping

Berikut adalah tabel yang berisi macam-macam looping di JavaScript:

| Tipe Looping   | Sintaks                                               | Deskripsi                                                                                                         |
|----------------|-------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|
| `for`          | `for (initialization; condition; increment) { //code }` | Loop ini digunakan untuk mengulangi blok kode sejumlah yang ditentukan.                                          |
| `while`        | `while (condition) { //code }`                         | Loop ini digunakan untuk mengulangi blok kode selama kondisi yang diberikan bernilai `true`.                      |
| `do...while`   | `do { //code } while (condition);`                     | Loop ini mirip dengan `while` loop, namun blok kode akan dieksekusi setidaknya sekali, sebelum kondisi diuji.     |
| `for...in`     | `for (variable in object) { //code }`                  | Loop ini digunakan untuk mengulangi properti-properti yang enumerable dari suatu objek.                           |
| `for...of`     | `for (variable of iterable) { //code }`                | Loop ini digunakan untuk mengulangi nilai-nilai dari iterable objects seperti array, string, Map, Set, dll.      |
| `forEach`      | `array.forEach(function(currentValue, index, arr) { //code })` | Metode ini memanggil fungsi untuk setiap elemen array.                                                             |

# 5. Percabangan

Berikut adalah tabel yang berisi macam-macam percabangan dalam JavaScript beserta sintaks dan deskripsinya:

| Tipe Percabangan          | Sintaks                                                                                 | Deskripsi                                                                                               |
|---------------------------|------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------|
| `if`                      | `if (condition) { // code }`                                                             | Menjalankan blok kode jika kondisi yang diberikan bernilai `true`.                                     |
| `if...else`               | `if (condition) { // code } else { // code }`                                            | Menjalankan blok kode pertama jika kondisi bernilai `true`, jika tidak maka menjalankan blok kode kedua.|
| `if...else if...else`     | `if (condition1) { // code } else if (condition2) { // code } else { // code }`          | Memeriksa beberapa kondisi dan menjalankan blok kode yang sesuai dengan kondisi yang bernilai `true`.  |
| `switch`                  | `switch (expression) { case value1: // code break; case value2: // code break; default: // code }` | Memilih salah satu dari banyak blok kode yang akan dijalankan berdasarkan nilai dari ekspresi.        |

# 6. Typecasting
Dalam JavaScript, typecasting (konversi tipe data) adalah proses mengubah satu tipe data menjadi tipe data lain. Ini bisa dilakukan secara eksplisit (disebut **typecasting eksplisit**) atau secara implisit (disebut **type coercion**). Berikut adalah beberapa cara umum untuk melakukan typecasting di JavaScript:

### Typecasting Eksplisit

1. **Mengubah ke String**:
    - Menggunakan `String()`:
      ```javascript
      let num = 123;
      let str = String(num); // "123"
      ```
    - Menggunakan `toString()`:
      ```javascript
      let num = 123;
      let str = num.toString(); // "123"
      ```

2. **Mengubah ke Number**:
    - Menggunakan `Number()`:
      ```javascript
      let str = "123";
      let num = Number(str); // 123
      ```
    - Menggunakan unary plus (`+`):
      ```javascript
      let str = "123";
      let num = +str; // 123
      ```

3. **Mengubah ke Boolean**:
    - Menggunakan `Boolean()`:
      ```javascript
      let str = "hello";
      let bool = Boolean(str); // true
      ```
    - Menggunakan double negation (`!!`):
      ```javascript
      let str = "hello";
      let bool = !!str; // true
      ```

### Type Coercion (Konversi Implicit)

JavaScript juga melakukan konversi tipe secara otomatis dalam konteks tertentu, seperti saat melakukan operasi dengan tipe data berbeda.

1. **String Coercion**:
    - Saat menggunakan operator `+` dengan string:
      ```javascript
      let num = 123;
      let str = "Hello";
      let result = str + num; // "Hello123"
      ```

2. **Number Coercion**:
    - Saat menggunakan operator aritmatika lain selain `+`:
      ```javascript
      let str = "123";
      let result = str * 1; // 123
      ```

3. **Boolean Coercion**:
    - Dalam konteks logika, seperti pernyataan `if`:
      ```javascript
      let str = "hello";
      if (str) {
          // true, karena str bukan nilai falsy
      }
      ```

### Nilai Falsy dan Truthy

Beberapa nilai di JavaScript akan dievaluasi sebagai `false` saat dikonversi ke boolean, dikenal sebagai nilai **falsy**. Contohnya adalah:

- `false`
- `0`
- `""` (string kosong)
- `null`
- `undefined`
- `NaN`

Nilai lainnya akan dievaluasi sebagai `true`, dikenal sebagai nilai **truthy**.

# 7 Variabel
Dalam JavaScript, ada tiga cara utama untuk mendeklarasikan variabel: `var`, `let`, dan `const`. Masing-masing memiliki karakteristik dan aturan penggunaannya sendiri.

### `var`
- **Scope:** Fungsi atau global. Variabel yang dideklarasikan dengan `var` memiliki cakupan fungsi, artinya mereka hanya dapat diakses dalam fungsi di mana mereka dideklarasikan. Jika dideklarasikan di luar fungsi, mereka menjadi variabel global.
- **Hoisting:** `var` dihoist ke atas cakupan fungsi atau global, artinya deklarasi variabel dipindahkan ke atas saat runtime. Namun, nilai tidak akan dihoist.
- **Redeklarasi:** Variabel yang dideklarasikan dengan `var` dapat dideklarasikan ulang dalam cakupan yang sama.
- **Contoh:**
  ```javascript
  function example() {
      console.log(x); // undefined
      var x = 5;
      console.log(x); // 5
  }
  example();
  ```

### `let`
- **Scope:** Blok. Variabel yang dideklarasikan dengan `let` memiliki cakupan blok, artinya mereka hanya dapat diakses di dalam blok (dalam `{}`) di mana mereka dideklarasikan.
- **Hoisting:** `let` juga dihoist, tetapi tidak diinisialisasi. Mengakses variabel `let` sebelum deklarasi akan menghasilkan ReferenceError.
- **Redeklarasi:** Tidak bisa dideklarasikan ulang dalam cakupan yang sama.
- **Contoh:**
  ```javascript
  function example() {
      console.log(x); // ReferenceError
      let x = 5;
      console.log(x); // 5
  }
  example();
  ```

### `const`
- **Scope:** Blok. Sama seperti `let`, variabel `const` memiliki cakupan blok.
- **Hoisting:** `const` dihoist tetapi tidak diinisialisasi. Mengakses variabel `const` sebelum deklarasi akan menghasilkan ReferenceError.
- **Redeklarasi:** Tidak bisa dideklarasikan ulang dalam cakupan yang sama.
- **Mutasi:** Nilai variabel `const` tidak dapat diubah (immutable). Namun, jika variabel `const` adalah objek atau array, properti atau elemen di dalamnya bisa diubah.
- **Contoh:**
  ```javascript
  function example() {
      const x = 5;
      console.log(x); // 5
      x = 10; // TypeError: Assignment to constant variable.
  }
  example();
  
  const arr = [1, 2, 3];
  arr.push(4); // Tidak menghasilkan error
  console.log(arr); // [1, 2, 3, 4]
  ```

### Ringkasan
- Gunakan `var` jika membutuhkan cakupan fungsi, meskipun ini jarang disarankan dalam kode modern.
- Gunakan `let` untuk variabel yang nilainya akan berubah dan hanya butuh cakupan blok.
- Gunakan `const` untuk variabel yang tidak akan berubah nilainya, memberikan jaminan bahwa variabel tidak akan di-reassign.
### Contoh Lengkap

```javascript
// Mengubah ke String
let num = 123;
console.log(String(num)); // "123"
console.log(num.toString()); // "123"

// Mengubah ke Number
let str = "123";
console.log(Number(str)); // 123
console.log(+str); // 123

// Mengubah ke Boolean
let str2 = "hello";
console.log(Boolean(str2)); // true
console.log(!!str2); // true

// Konversi implisit
let num2 = 123;
let str3 = "Hello";
console.log(str3 + num2); // "Hello123"

let str4 = "123";
console.log(str4 * 1); // 123

if (str2) {
    console.log("This is truthy"); // "This is truthy"
}
```
