Abraham Javier Sebastian Situmorang

2106704364 -- PBP Kelas D

# Tugas 7: Elemen Dasar Flutter
##  Jelaskan apa yang dimaksud dengan stateless widget dan stateful widget dan jelaskan perbedaan dari keduanya.
```Stateless Widget``` merupakan widget yang tidak dapat diubah dan tidak akan berubah, contohnya adalah Icon, IconButton, dan Text yang statis. widget ini di-build hanya dengan konfigurasi yang telah diinisiasi sejak awal. Sementara itu, ```Stateful Widget``` merupakan widget yang dapat berubah secara dinamis ketika user berinteraksi dengan widget tersebut. 

## Sebutkan widget apa saja yang kamu pakai di proyek kali ini dan jelaskan fungsinya.
```FloatingActionButton``` widget--dalam kasus ini berupa tombol icon--yang 'mengambang' (floating) dan digunakan untuk mempromosikan tindakan atau menambahkan sesuatu pada halaman aplikasi

```Padding``` untuk membuat padding/space kosong antara widget

```Row``` untuk alignment agar sejajar secara horizontal

```Text``` untuk menampikan teks

```Visibility``` untuk mengeset terlihat atau tidaknya widget

## Apa fungsi dari ```setState()```? Jelaskan variabel apa saja yang dapat terdampak dengan fungsi tersebut.
```SetState``` berfungsi untuk memberitahu bahwa terdapat internal state yang berubah dan akibatnya akan terjadi build ulang, sehingga jika state yang berubah merupakan state yang ditampilkan, state tersebut akan berubah juga pada tampilannya. Contohnya adalah variabel ```_counter``` (dalam tugas 7 ini) yang nilainya dapat berubah saat terjadi pemanggilan fungsi increment dan decrement

## Jelaskan perbedaan antara const dengan final.
Perbedaan keduanya adalah ```const``` digunakan untuk mendeklarasi variabel yang harus sudah diketahui valuenya saat compile time.
Sementara itu, ```final``` digunakan untuk mendeklarasi variabel yang sudah atau belum diketahui saat compile time. Persamaannya adalah keduanya digunakan untuk mendeklarasi variabel yang bersifat immutable

## Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas.
1. Buka terminal lalu menjalankan command ```flutter create counter_7```
2. Buka file ```main.dart``` yang terdapat pada direktori ```counter_7/lib/main.dart```

Mengedit file ```main.dart```

3. Menambahkan widget row pada ```floatingActionButton```
4. menambahkan ```floatingActionButton``` widget lagi di row, sehingga terdapat 2 ```floatingActionButton```
5. membuat fungsi ```_decrementCounter()```
6. menambahkan logic pada teks Ganjil dan Genap (mengubah warna)
7. melakukan handling hanya ketika ```_counter > 0``` baru bisa melakukan decrement
8. melakukan binding fungsi increment dan decrement pada ```onPressed``` di button increment dan decrement

# Tugas 8: Flutter Form

##  Jelaskan perbedaan ```Navigator.push``` dan ```Navigator.pushReplacement```.
```Navigator.push``` = digunakan untuk berpindah dari activity pertama ke activity kedua, dan ketika saat activity kedua kita menekan tombol back maka akan dialihkan ke activity pertama (tidak menghilangkan screen sebelumnya). 
```Navigator.pushReplacement``` = ketika tombol kembali di-tap maka activity sebelumnya dihilangkan.

## Sebutkan widget apa saja yang kamu pakai di proyek kali ini dan jelaskan fungsinya.
```FloatingActionButton``` widget--dalam kasus ini berupa tombol icon--yang 'mengambang' (floating) dan digunakan untuk mempromosikan tindakan atau menambahkan sesuatu pada halaman aplikasi

```Padding``` untuk membuat padding/space kosong antara widget

```Row``` untuk alignment agar sejajar secara horizontal

```Text``` untuk menampikan teks

```Visibility``` untuk mengeset terlihat atau tidaknya widget

```TextButton``` untuk membuat button berbentuk teks

```DropdownButton``` Untuk membuat dropdown

```ListView.builder``` untuk membuat children

```List Tile``` untuk membentuk sebuah list dan terdapat juga widget widget didalamnya.

## Sebutkan jenis-jenis event yang ada pada Flutter (contoh: onPressed.
```onPressed``` -> terjadi ketika user telah selesai menekan objek (secara khusus button)
```onTap``` -> terjadi ketika sesaat setelah menekan objek
```onChanged``` -> terjadi ketika terdapat perubahan

## Jelaskan bagaimana cara kerja Navigator dalam "mengganti" halaman dari aplikasi Flutter.
```Navigator```metode push yang digunakan untuk menambahkan rute lain ke atas tumpukan layar (secara stack / last in first out) saat ini sehingga halaman baru akan ditampilkan di atas halaman sebelumnya.

## Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas.
1. Mengedit file ```main.dart``` (menambahkan ```drawer: const DrawerApp()```)
2. Membuat file ```drawer.dart``` yang berisi DrawerApp 
3. Membuat file ```add_budget.dart``` yang berisi form
4. Membuat file ```globals.dart``` yang berisi global variabel
5. Membuat file ```showdata_budget.dart``` untuk menampilkan data
