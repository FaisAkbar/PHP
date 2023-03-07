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
### Di dalam file php, tag php dimulai dengan :
```
<?php
  // Baris kode Anda
?>
```
#### Untuk menampilkan baris kode ke web browser, di dalam tag php, digunakan perintah ``` echo ```, contoh :
```
  echo 'Hello World';
```
## 4. PHP For Beginners, Ep 4 - Variables
#### Di dalam PHP, penamaan variabel dimulai dengan simbol ```$```. Contohnya adalah :
```
// Variabel bernama $greeting dengan value "Hello"
$greeting = "Hello";

// Pemanggilan dalam echo, dipisahkan oleh ' . ' jika terdapat tambahan argumen, misalnya string atau variabel lain (concate)
echo $greeting . " Everybody!";

// Variabel juga dapat dipanggil di didalam string, NAMUN HARUS DI DALAM PETIK DUA " "
echo "$greeting Everybody!"; // Output sama dengan di atas
```
## 5. PHP For Beginners, Ep 5 - Conditionals and Booleans
#### Conditional merupakan salah satu ekspresi dalam pemrograman yang menghasilkan nilai *true / false*. Jika kondisi tersebut bernilai *true* maka sistem menjalankan statement di dalam if statement namun jika kondisi tersebut bernilai *false* maka sistem tidak menjalankan statement tersebut. Terdapat sebuah tipe data yang hanya mengembalikan nilai *true / false*, yaitu boolean. Nilai boolean memiliki default *false*. Contohnya :
#### Di dalam tag php :
```
<?php
$name = "Dark Matter";
$read = true;

//Operasi if-else
if ($read) {
    $message = "You have read $name"; // Mengembalikan nilai true
} else {
    $message = "You have NOT read $name"; // Mengembalikan nilai false
}
<?
```
#### Di dalam body tag html
```
 <!-- Print variabel $message ke web browser di dalam tag html
    Menggunakan <?php echo $message ?> atau <= $message ?> -->
<h1><?= $message ?></h1>
```
#### Maka akan tampil "You have read Dark Matter" pada web browser, karena bernilai true :
![if-else](https://github.com/HanifAjiPrasetyo/PHP/blob/main/if-else.png?raw=true)
## 6. PHP For Beginners, Ep 6 - Arrays
#### Array dalam pemgrograman termasuk PHP, merupakan suatu tipe data terstruktur yang dapat menyimpan banyak data dengan suatu nama yang sama dan menempati tempat di memori yang berurutan serta bertipe data sama pula. Dalam PHP, array adalah struktur data yang memungkinkan untuk menyimpan beberapa elemen dalam satu variabel. Elemen-elemen ini disimpan sebagai pasangan nilai-kunci. Contoh deklarasi array :
```
<?php
$books = [
  "Do Androids Dream of Electric Sheep",
  "The Langoliers",
  "Hail Mary
];
```
#### Untuk memperoleh isi dari array tersebut, dapat digunakan ekspresi perulangan(*loop*) di dalam tag html, misalnya *for, foreach, while,* atau *do-while*. Contoh menggunakan *foreach* :
```
 <ul>
        <?php foreach ($books as $book) : ?>
            <li><?= $book ?></li>
        <?php endforeach ?>
 </ul>
```
#### Maka akan tampil di web browser :
![if-else](https://github.com/HanifAjiPrasetyo/PHP/blob/main/foreach-array.png?raw=true)
## 7. PHP For Beginners, Ep 7 - Associative Arrays
#### Associative array merupakan array yang berisi satu atau lebih array, dimana terdapat key dan value pada setiap data, contoh :
```
<?php
$books = [
  [
    'name' => "Do Androids Dream of Electric Sheep",
    'author' => "Philip K. Dick",
    'purchaseUrl' => "http://example.com"
  ],
  [
    'name' => "Project Hail Mary",
    'author' => "Andy Weir",
    'purchaseUrl' => "http://example.com"
  ]
]
```
#### Setiap item dalam array di atas memiliki identifier atau key dengan value masing-masing, contohnya *key : name, value : Project Hail Mary*.
