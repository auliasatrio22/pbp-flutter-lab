# counter_7

A new Flutter project.

## Jelaskan apa yang dimaksud dengan stateless widget dan stateful widget dan jelaskan perbedaan dari keduanya.
-> Stateless widget merupakan widget yang sifatnya tetap dan tidak akan berubah ketika aplikasi sedang dijalankan. Perubahan yang dimaksud adalah variabel, ikon, tombol, serta pengambilan data.

-> Stateful widget merupakan widget yang dapat berubah-ubah atau dinamis. Widget ini nantinya akan merubah tampilan dari aplikasi yang ada. Tampilan yang berubah dapat berupa warna, ikon, tombol, variabel, dan hal-hal lain yang nantinya dimasukan ke dalam widget ini. Ketika aplikasi berjalan, widget ini akan terus mengubah tampilannya. Contoh method dari stateful widget yang saya gunakan adalah setState()

-> Perbedaan dari stateless widget dan stateful widget yaitu sifat dari masing-masing yang sangat kontras, dimana stateless widget tidak akan melakukan perubahaan pada aplikasi ketika aplikasi sedang dijalankan dan stateful widget akan melakukan perubahan tampilan pada aplikasi ketika aplikasi dijalankan. Jadi dapat diambil kesimpulan bahwa penggunaan dari widget ini akan bergantung pada aplikasi itu sendiri, apakah membutuhkan perubahan atau tidak.

## Sebutkan widget apa saja yang kamu pakai di proyek kali ini dan jelaskan fungsinya.
-> TextStyle: memiliki fungsi untuk memberikan styling pada text yang ada

-> Text: untuk menampilkan text pada aplikasi yang dibuat

-> Column: berfungsi untuk mengatur posisi letak widget

-> MaterialApp: merupakan parent yang akan menerapkan style material design pada sesuatu yang diapitnya

-> Scaffold: untuk mengatur struktur visual layout yang diimplementasikan melalui material design

-> Center: untuk meletakkan widget ke bagian tengah

-> FloatingActionButton: untuk membuat suatu tombol

## Apa fungsi dari setState()? Jelaskan variabel apa saja yang dapat terdampak dengan fungsi tersebut.
-> setState() berfungsi untuk memberitahu suatu framework bahwa terdapat perubahan object pada State yang kemudian akan melakukan build ulang pada widget tersebut. Variabel yang terdapat pada setState() ialah variabel yang memiliki sifat dapat berubah atau dinamis dan juga variabel yang terdeklarasi secara global pada sebuah class.

## Jelaskan perbedaan antara const dengan final.
-> Perbedaan antara const dengan final terletak pada saat pemberian nilai pada suatu variabel. const akan mengharuskan suatu variabel diinisiasi pada saat kompilasi, sehingga nilainya bersifat konstan dan secara langsung sudah memiliki nilai ketika dikompilasi. Sebaliknya, final tidak mengharuskan suatu variabel memiliki nilai secara langsung ketika dikompilasi. Jadi pada final, deklarasi variabel yang nilainya sudah ataupun belum diketahui pada saat waktu kompilasi berjalan.

## Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas.
-> Hal yang pertama saya lakukan dengan adalah dengan membuat aplikasi counter_7 dengan menggunakan perintah flutter create counter_7. Lalu saya membuat variabel counter pada class _MyHomePageState untuk menginisiasi angka 0 yang nantinya akan berubah seiring aplikasi berjalan. Selanjutnya, saya membuat method _decrementCounter(), dalam method ini akan melakukan pengurangan counter dan method ini saya menambahkan kondisi apabila counter = 0 maka method ini tidak akan tampil. Pada proses ini dilakukan dalam fungsi setState(). Kemudian, saya membuat program yang akan melakukan pengecekan pada angka. Program ini akan melihat apakah angka tersebut berupa ganjil atau genap, dilihat melalui counter yang berubah-ubah nilainya. Ketika counter tersebut menunjukkan angka genap, maka text yang akan terlihat berupa tulisan genap yang berwarna merah, begitupun sebaliknya tetapi text ganjil yang tampil akan berwarna biru. Setelah itu saya menambahkan widget floatingActionButton lalu memasukkan fungsi atau method yang sudah kita buat sebelumnya pada onPressed yang pada tugas ini bernama _decrementCounter dan _incrementCounter. Jadi ketika diklik maka akan menjalankan method tersebut.

# Tugas 8
## Jelaskan perbedaan Navigator.push dan Navigator.pushReplacement.
-> Navigator.push bekerja dengan cara menambahkan sebuah rute ke stack navigator, sedangkan Navigator.pushReplacement bekerja dengan cara mengganti rute yang sedang ditampilkan dengan push route datau halaman baru ke stack navigator.

## Sebutkan widget apa saja yang kamu pakai di proyek kali ini dan jelaskan fungsinya.
-> Drawer : Sebagai hamburger menu untuk navigasi ke halaman berbeda.

-> TextFormField : Untuk menerima input dari user.

-> DropdownButton: Untuk menentukan input yang diberikan adalah pemasukan atau pengeluaran.

-> FloatingActionButton : Button yang di-bind untuk menambahkan data ke dalam list

## Sebutkan jenis-jenis event yang ada pada Flutter (contoh: onPressed).
->  onPressed()

-> onTap()

-> onChanged()

-> onSaved()

## Jelaskan bagaimana cara kerja Navigator dalam “mengganti halaman dari aplikasi Flutter.
-> Navigator bekerja dengan konsep Last In First Out, seperti struktur data stack. Setiap tampilan akan di push ke stack navigator untuk ditampilkan, sehingga yang tampil adalah halaman yang paling terakhir di push yang berarti berada di posisi paling atas stack.

## Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas.
-> Hal yang dilakukan terlebih dahulu adalah membuat widget drawer untuk navigasi ke halaman lain. Lalu membuat file baru pada folder lib yang bernama tambah.dart untuk menerima input dari user dan data.dart untuk menampilkan input dari user yang sudah ditambahkan. Kemudian membuat FloatingActionButton untuk menyimpan input dan melakukan validasi terhadap input sudah terisi atau belum. Mengimport file tambah.dart dan main.dart agar list input data dapat diakses pada data.dart. Menampilkan data pada list dengan menggunakan builder ListView.builder().
