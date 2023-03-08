# PHP BASIC
##### Sumber Youtube : [Laracast](https://www.youtube.com/playlist?list=PL3VM-unCzF8ipG50KDjnzhugceoSG3RTC)

## 1. How to Choose A First Programming Language
##### Dalam Memilih bahasa pemrograman, kita harus mempertimbangkan tujuan apa yang kita miliki saat ingin belajar bahasa tersebut. Jadi dalam memilih bahasa pemrograman harus sesuai dengan tujuan kita. Contohnya apabila kita ingin membuat situs web, kita bisa belajar bahasa pemrograman seperti HTML, CSS, dan JS. Jika kita ingin membuat aplikasi desktop, kita mungkin bisa memilih bahasa seperti Python, C++, atau Java. Jika kita benar benar baru dalam pemrograman, cobalah memilih bahasa yang lebih mudah seperti Python atau Ruby. Setelah itu kita bisa mempertimbangkan jenis proyek yang kita ingin kerjakan di masa depan, jika kita ingin menjadi seorang pengembang Game, kita bisa memilih bahasa C++ atau C#, dan apa bila kita ingin fokus pada pengembangan Web, kita bisa memilih bahasa JavaScript atau PHP.
#### Kali ini Kita akan belajar tentang Bahasa Pemrograman PHP
##### PHP adalah bahasa pemrograman server-side yang dirancang untuk pengembangan web. PHP singkatan dari "PHP: Hypertext Preprocessor". PHP digunakan untuk menghasilkan konten dinamis pada website, seperti halaman web yang mengambil data dari database, membuat dan mengirim email, mengolah formulir, dan masih banyak lagi. PHP juga dapat digunakan untuk membuat aplikasi web yang lebih besar dan kompleks. PHP umumnya digunakan dengan teknologi web seperti Apache, MySQL, dan HTML. Saat ini, PHP terus berkembang dan ditingkatkan oleh komunitas pengembang web, dan menjadi salah satu bahasa pemrograman web yang paling populer dan mudah digunakan.

## 2. PHP For Beginners, Ep 2 - Tools of the Trade
##### Ada beberapa Tools yang diperlukan untuk menjalankan PHP Seperti :
1. Text Editor: Dalam pengembangan web, text editor digunakan untuk menulis kode program. Ada banyak pilihan text editor gratis dan berbayar yang tersedia, seperti Visual Studio Code dan Sublime Text.
2. Terminal: Terminal adalah alat yang digunakan untuk mengeksekusi perintah pada sistem operasi. Dalam pengembangan web dengan PHP, terminal digunakan untuk menjalankan perintah seperti menjalankan server web lokal atau menginstal paket PHP.
3. PHP: PHP harus diinstal di server untuk dapat menjalankan aplikasi web PHP. PHP menyediakan banyak fungsi dan fitur untuk memproses data dan menghasilkan konten dinamis pada website.
4. Local Development Environment: Saat membangun situs web, seringkali lebih mudah untuk membangun dan menguji di lingkungan lokal. Ada beberapa alat yang tersedia untuk membuat lingkungan pengembangan lokal, seperti XAMPP, MAMP, atau WAMP.
5. Browser: Browser digunakan untuk menampilkan halaman web yang dihasilkan oleh aplikasi web PHP. Beberapa pilihan browser yang populer antara lain Google Chrome, Mozilla Firefox, dan Microsoft Edge.Browser: Browser digunakan untuk menampilkan halaman web yang dihasilkan oleh aplikasi web PHP. Beberapa pilihan browser yang populer antara lain Google Chrome, Mozilla Firefox, dan Microsoft Edge.
6. Version Control: Version control digunakan untuk melacak perubahan pada kode program dan bekerja sama dengan tim. Salah satu platform version control yang populer adalah Git dan tersedia beberapa hosting Git seperti GitHub, GitLab, Bitbucket.

## 3. PHP For Beginners, Ep 3 - Your First PHP Tag
##### Tag PHP digunakan untuk menandai kode PHP pada halaman web. Tag PHP dimulai dengan ``<?php`` dan diakhiri dengan ``?>``. Semua kode PHP harus ditempatkan di antara tag PHP. Contoh :
```
<?php
  // Baris kode Anda
?>
```
##### Fungsi ``echo`` digunakan untuk menampilkan teks atau variabel pada halaman web. Fungsi ``echo`` ditulis dengan format ``echo 'teks';``. Contoh :
```
  echo 'Hello World';
```
##### Contoh kode pada video menunjukkan cara menampilkan teks dengan fungsi ``echo``. Kode tersebut adalah sebagai berikut:
```
<?php
  echo "Hello, world!";
?>
```
##### Penjelasan kode program:
1. ``<?php`` dan ``?>`` adalah tag PHP yang digunakan untuk menandai awal dan akhir kode PHP.
2. Fungsi ``echo`` digunakan untuk menampilkan teks ``"Hello, world!"`` pada halaman web.
3. Teks ``"Hello, world!"`` harus diapit dengan tanda kutip (" ") untuk menandakan bahwa itu adalah string.
4. Tanda titik koma (;) digunakan untuk menandakan akhir dari setiap perintah.

## 4. PHP For Beginners, Ep 4 - Variables
##### Variabel digunakan untuk menyimpan data yang dapat digunakan dalam kode PHP. Variabel dapat menyimpan berbagai jenis data, termasuk teks, angka, dan boolean. Variabel diawali dengan tanda ``$`` diikuti dengan nama variabel. Nama variabel harus dimulai dengan huruf atau garis bawah, dan dapat mengandung huruf, angka, dan garis bawah. Contohnya :
```
// Variabel dengan nama $greeting dan value "Hello"
$greeting = "Hello";

// Pemanggilan dalam echo, dipisahkan oleh ' . ' jika terdapat tambahan argumen, 
// misalnya string atau variabel lain (concate)
echo $greeting . "Everybody!";

// untuk menambahkan spasi, bisa dilakukan sebelum "Everybody!"
echo $greeting . " Everybody!";
// atau
echo $greeting . " " . "Everybody!";

// selain cara di atas, kita juga bisa dengan cara Variabel dipanggil di didalam string. 
// agar terlihat lebih rapih dan lebih efision
echo "$greeting Everybody!";
```
##### berikut adalah hasil dari kode program di atas :
![hello](https://github.com/FaisAkbar/PHP/blob/main/img/hello.png)

## 5. PHP For Beginners, Ep 5 - Conditionals and Booleans
##### Conditional adalah pernyataan yang mengevaluasi suatu kondisi dan menjalankan kode tertentu berdasarkan hasil evaluasi. Jika kondisi tersebut bernilai *true* maka sistem menjalankan statement di dalam if statement namun jika kondisi tersebut bernilai *false* maka sistem tidak menjalankan statement tersebut. Sedangkan boolean adalah tipe data yang hanya memiliki dua nilai, yaitu *true* dan *false*. Nilai default dari Boolean adalah *false*. Contoh : 
```
<?php
//Membuat variabel
$name = "Dark Matter";
$read = true;

//Operasi if-else
if ($read) {
    $message = "You have read $name"; // jika bernilai true, maka akan mengembalikan nilai true
} else {
    $message = "You have NOT read $name"; // jika bernilai false, maka akan mengembalikan nilai false
}
<?
<h1>
    // cara menampilkan variabel
    <?php 
    echo $message;
    ?>
    // atau
    <?= $message ?> // membuka php sekaligus memanggil echo
</h1>
```
##### karena variabel $read bernilai true, maka akan mengembalikan nilai true dan akan menampilkan "You have read Dark Matter"
![true](https://github.com/FaisAkbar/PHP/blob/main/img/true.png)
##### namun jika kita mengubah nilai variabel $read menjadi false, maka akan mengembalikan nilai false dan akan menampilkan "You have NOT read Dark Matter"
![false](https://github.com/FaisAkbar/PHP/blob/main/img/false.png)

## 6. PHP For Beginners, Ep 6 - Arrays
##### Array adalah kumpulan data yang disimpan dalam satu variabel. Array dapat menyimpan satu atau lebih nilai. Array dapat menyimpan berbagai jenis data, termasuk teks, angka, dan boolean. Array diawali dengan tanda ``$`` diikuti dengan nama variabel. Nama variabel harus dimulai dengan huruf atau garis bawah, dan dapat mengandung huruf, angka, dan garis bawah. Contoh :
```
<?php
$books = [
  "Do Androids Dream of Electric Sheep",
  "The Langoliers",
  "Hail Mary"
];
```
##### Array di atas memiliki tiga buah data, yaitu "Do Androids Dream of Electric Sheep", "The Langoliers", dan "Hail Mary". Untuk mengakses data pada array dapat digunakan ekspresi perulangan(*loop*) di dalam tag html, misalnya *for, foreach, while,* atau *do-while*. Contoh menggunakan *foreach* :
```
 <ul>
        <?php foreach ($books as $book) : ?>
            <li><?= $book ?></li>
        <?php endforeach ?>
 </ul>
```
##### berikut adalah hasil dari kode program di atas :
![array](https://github.com/FaisAkbar/PHP/blob/main/img/array.png)

## 7. PHP For Beginners, Ep 7 - Associative Arrays
#### Associative array merupakan array yang berisi satu atau lebih array, dimana terdapat key dan value pada setiap data, contoh :

## 8. PHP For Beginners, Ep 8 - Functions and Filtering
#### Function adalah sebuah blok kode yang dapat digunakan berulang kali untuk melakukan suatu tugas tertentu. Function dapat menerima parameter dan mengembalikan nilai. Function dapat digunakan untuk memecah kode menjadi bagian-bagian yang lebih kecil dan mudah dipahami. Contoh :

## 9. PHP For Beginners, Ep 9 - Lambda Functions
#### Lambda function adalah function yang tidak memiliki nama. Lambda function dapat digunakan untuk membuat function yang sederhana dan hanya digunakan sekali. Contoh :

## 10. PHP For Beginners, Ep 10 - Separate PHP Logic From the Template
#### Dalam pembuatan website, biasanya terdapat beberapa halaman yang memiliki tampilan yang sama, namun konten yang berbeda. Untuk menghindari duplikasi kode, kita dapat memisahkan kode PHP dari kode HTML. Contoh :