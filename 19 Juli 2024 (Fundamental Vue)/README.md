Vue 3 Composition API adalah fitur baru yang diperkenalkan di Vue 3 untuk menyediakan cara yang lebih fleksibel dan skalabel dalam mengorganisir logika komponen. Berikut adalah rangkuman tentang Vue 3 Composition API:

### Konsep Dasar

1. **Setup Function**:
   - Fungsi `setup` adalah tempat utama untuk menggunakan Composition API. Ini dijalankan sebelum komponen dibuat dan digunakan untuk mendefinisikan state, methods, dan hooks lain yang diperlukan.
   - Contoh:
     ```javascript
     import { ref } from 'vue';

     export default {
       setup() {
         const count = ref(0);
         const increment = () => {
           count.value++;
         };

         return { count, increment };
       }
     };
     ```

2. **Reaktifitas dengan `ref` dan `reactive`**:
   - `ref` digunakan untuk membuat objek reaktif yang menyimpan nilai primitif.
   - `reactive` digunakan untuk membuat objek reaktif dari objek non-primitif.
   - Contoh:
     ```javascript
     import { ref, reactive } from 'vue';

     export default {
       setup() {
         const count = ref(0);
         const state = reactive({ count: 0 });

         const increment = () => {
           count.value++;
           state.count++;
         };

         return { count, state, increment };
       }
     };
     ```

3. **Komposisi dengan `computed`**:
   - `computed` digunakan untuk membuat nilai terhitung (computed values) yang otomatis di-update ketika dependensinya berubah.
   - Contoh:
     ```javascript
     import { ref, computed } from 'vue';

     export default {
       setup() {
         const count = ref(0);
         const double = computed(() => count.value * 2);

         return { count, double };
       }
     };
     ```

4. **Penggunaan `watch`**:
   - `watch` digunakan untuk memantau perubahan pada data reaktif atau computed properties dan menjalankan efek samping.
   - Contoh:
     ```javascript
     import { ref, watch } from 'vue';

     export default {
       setup() {
         const count = ref(0);

         watch(count, (newCount, oldCount) => {
           console.log(`Count changed from ${oldCount} to ${newCount}`);
         });

         return { count };
       }
     };
     ```

5. **Lifecycle Hooks**:
   - Vue 3 menyediakan berbagai lifecycle hooks yang bisa digunakan dalam `setup` untuk mengelola siklus hidup komponen.
   - Contoh:
     ```javascript
     import { onMounted, onUnmounted } from 'vue';

     export default {
       setup() {
         onMounted(() => {
           console.log('Component is mounted');
         });

         onUnmounted(() => {
           console.log('Component is unmounted');
         });

         return {};
       }
     };
     ```

### Keuntungan Composition API

- **Modularisasi Logika**: Memudahkan untuk memisahkan dan mengorganisir logika komponen dalam unit yang lebih kecil dan reusable.
- **Reusabilitas**: Memungkinkan pembuatan reusable logic (composable functions) yang dapat digunakan kembali di berbagai komponen.
- **Skalabilitas**: Membantu mengelola komponen yang kompleks dengan lebih baik karena logika komponen dapat dipecah menjadi bagian-bagian yang lebih kecil dan mudah dipahami.
- **TypeScript Friendly**: Lebih mudah digunakan dengan TypeScript karena menyediakan tipe yang lebih eksplisit dan dukungan yang lebih baik untuk inferensi tipe.

Dengan Composition API, pengembang Vue memiliki lebih banyak fleksibilitas dan kontrol dalam mengelola state dan logika komponen, membuat kode lebih mudah dibaca, dipelihara, dan digunakan kembali.


### Perbandingan Options API vs Composition API

#### Options API
Options API adalah cara tradisional dalam menulis komponen di Vue 2 dan Vue 3. Komponen didefinisikan menggunakan objek yang terdiri dari beberapa properti seperti `data`, `methods`, `computed`, dan `watch`.

**Contoh**:
```javascript
export default {
  data() {
    return {
      count: 0,
    };
  },
  computed: {
    double() {
      return this.count * 2;
    },
  },
  methods: {
    increment() {
      this.count++;
    },
  },
  watch: {
    count(newVal, oldVal) {
      console.log(`Count changed from ${oldVal} to ${newVal}`);
    },
  },
  mounted() {
    console.log('Component is mounted');
  },
};
```

**Kelebihan**:
- **Struktur yang Jelas**: Memisahkan logika komponen ke dalam properti tertentu (data, methods, computed, dll), sehingga mudah dipahami.
- **Kemudahan Memulai**: Lebih mudah untuk pemula karena pendekatannya yang terstruktur dan terorganisir.

**Kekurangan**:
- **Fragmentasi Logika**: Logika yang berkaitan sering tersebar di berbagai bagian dari objek komponen, sehingga sulit untuk mengelola dan mengikuti alur logika.
- **Reusabilitas Terbatas**: Sulit untuk menggunakan kembali logika komponen tanpa membuat mixin atau menggunakan ekstensi lainnya.

#### Composition API
Composition API memperkenalkan pendekatan yang lebih fleksibel dan modular untuk menulis komponen dengan menggunakan fungsi `setup`. Logika yang berkaitan dapat dikelompokkan bersama, memudahkan untuk digunakan kembali dan dikelola.

**Contoh**:
```javascript
import { ref, computed, watch, onMounted } from 'vue';

export default {
  setup() {
    const count = ref(0);
    const double = computed(() => count.value * 2);

    const increment = () => {
      count.value++;
    };

    watch(count, (newVal, oldVal) => {
      console.log(`Count changed from ${oldVal} to ${newVal}`);
    });

    onMounted(() => {
      console.log('Component is mounted');
    });

    return { count, double, increment };
  },
};
```

**Kelebihan**:
- **Pengelompokan Logika**: Logika yang berkaitan dapat dikelompokkan bersama, membuat kode lebih modular dan mudah dipahami.
- **Reusabilitas yang Lebih Baik**: Memungkinkan pembuatan fungsi komposisi yang dapat digunakan kembali di berbagai komponen.
- **Dukungan TypeScript yang Lebih Baik**: Lebih mudah digunakan dengan TypeScript karena menyediakan tipe yang lebih eksplisit dan dukungan inferensi tipe yang lebih baik.
- **Fleksibilitas**: Memberikan lebih banyak fleksibilitas dalam bagaimana logika komponen diatur dan digunakan.

**Kekurangan**:
- **Kurva Pembelajaran**: Mungkin lebih sulit untuk pemula yang terbiasa dengan Options API karena pendekatan yang lebih fungsional dan kurang terstruktur.
- **Kode yang Lebih Verbose**: Bisa terlihat lebih verbose dan kompleks untuk komponen yang sangat sederhana.

### Kapan Menggunakan Options API atau Composition API

- **Options API**:
  - Cocok untuk komponen sederhana.
  - Baik untuk pemula yang baru belajar Vue karena strukturnya yang lebih terorganisir dan mudah dipahami.
  - Bagus untuk proyek kecil atau tim yang sudah terbiasa dengan Vue 2.

- **Composition API**:
  - Cocok untuk komponen yang kompleks dan besar.
  - Ideal untuk proyek besar atau ketika bekerja dalam tim yang memerlukan modularisasi logika komponen.
  - Direkomendasikan jika menggunakan TypeScript atau membutuhkan reusabilitas logika yang tinggi.

Dalam praktiknya, kedua API ini dapat digunakan bersama dalam satu proyek Vue 3, sehingga Anda dapat memilih pendekatan yang paling sesuai dengan kebutuhan komponen atau proyek tertentu.