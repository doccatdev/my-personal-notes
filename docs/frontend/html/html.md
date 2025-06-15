## HTML (Hypertext Markup Language)

Hypertext Markup Language atau HTML adalah sebuah bahasa markup yang digunakan untuk mengatur struktur dari sebuah informasi yang ditampilkan di halaman web.

## Struktur HTML

``` html title="structure.html"
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
```

Berikut ini adalah struktur dari HTML5:

    <!DOCTYPE html> : Menjelaskan bahwa struktur yang digunakan berjenis HTML5.
    <head>  : Berisikan metadata file HTML5.
    <title> : Halaman judul web.
    <body>  : Berisikan semua konten yang akan ditampilkan ke dalam web untuk pengguna.

## Nama Elemen dalam HTML


### <h3>&lt;h1-h6&gt;</h3>
Elemen ini digunakan untuk membuat **judul** dan **subjudul** dalam sebuah halaman web.  
Berikut adalah contoh penggunaannya:

```html title="heading.html"
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen Heading</title>
  </head>
  <body>
    <h1>Heading 1</h1>
    <h2>Heading 2</h2>
    <h3>Heading 3</h3>
    <h4>Heading 4</h4>
    <h5>Heading 5</h5>
    <h6>Heading 6</h6>
  </body>
</html>
```

!!! example "Output elemen <`heading`>"
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen Heading</title>
  </head>
  <body>
    <h1>Heading 1</h1>
    <h2>Heading 2</h2>
    <h3>Heading 3</h3>
    <h4>Heading 4</h4>
    <h5>Heading 5</h5>
    <h6>Heading 6</h6>
  </body>
</html>
    


### <h3>&lt;p&gt;</h3>
Elemen ini digunakan untuk membuat paragraf dalam sebuah halaman web
Berikut adalah contoh penggunaanya:
```html title="paragraph.html"
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen Paragraph</title>
</head>
<body>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut ut est eget mi ultrices luctus. Aenean sed ligula vel sem sodales sodales. 
    Pellentesque consequat velit arcu, sit amet lobortis augue eleifend in. Donec sed porta nunc. Praesent efficitur nulla felis, et fringilla ex auctor commodo. Sed purus libero, dapibus eget dictum at, tempor et arcu. 
    Etiam condimentum ante ac nulla luctus, sed cursus risus rutrum. Sed ac libero tellus. Morbi vel dui vel est tincidunt elementum. 
    Vivamus quis consequat turpis. Vivamus et semper augue, non elementum nulla. Proin gravida imperdiet elit at dictum. Phasellus eget luctus quam. Etiam lacinia sapien fermentum felis euismod, sed porta erat finibus.
</p>
</body>
</html>
```
!!! example "Output elemen <`p`>"
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Element Paragraph</title>
</head>
<body>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut ut est eget mi ultrices luctus. Aenean sed ligula vel sem sodales sodales. 
    Pellentesque consequat velit arcu, sit amet lobortis augue eleifend in. Donec sed porta nunc. Praesent efficitur nulla felis, et fringilla ex auctor commodo. Sed purus libero, dapibus eget dictum at, tempor et arcu. 
    Etiam condimentum ante ac nulla luctus, sed cursus risus rutrum. Sed ac libero tellus. Morbi vel dui vel est tincidunt elementum. 
    Vivamus quis consequat turpis. Vivamus et semper augue, non elementum nulla. Proin gravida imperdiet elit at dictum. Phasellus eget luctus quam. Etiam lacinia sapien fermentum felis euismod, sed porta erat finibus.
</p>
</body>
</html>

### <h3>&lt;ul&gt;</h3>
Elemen ini digunakan untuk membuat list yang tidak memiliki urutan numerik (bullet point) dan menandakan bahwa urutan tidak berarti (meaningless). Berikut adalah contoh penggunaanya:
```html title="ul.html"
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Element ul</title>
</head>
<body>
    <ul>
        <li>Kucing</li>
        <li>Ayam</li>
        <li>Kelinci</li>
    </ul>
</body>
</html>
```

!!! example "Output elemen <`ul`>"
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Element ul</title>
</head>
<body>
    <ul>
        <li>Kucing</li>
        <li>Ayam</li>
        <li>Kelinci</li>
    </ul>
</body>
</html>

### <h3>&lt;ol&gt;</h3>
Elemen ini adalah kebalikan dari elemen ul, elemen ini biasanya digunakan untuk membuat list yang memiliki angka dan menandakan urutan tersebut berarti (meaningful)
```html title="ol.html"
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Element ol</title>
</head>
<body>
    <ol>
      <h4>Tutorial menggoreng telur</h4>
      <li>Pertama siapkan minyak</li>
      <li>Siapkan wajan</li>
      <li>Masukan minyak ke dalam wajan dan tunggu hingga panas</li>
      <li>Pecahkan telur</li>
      <li>Tuangkan telur ke dalam wajan dan tunggu beberapa menit</li>
      <li>Ambil nasi dan sajikan</li>
    </ol>
</body>
</html>
```

!!! example "Output elemen ol"
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Element ol</title>
</head>
<body>
    <ol>
      <h4>Tutorial menggoreng telur</h4>
      <li>Pertama siapkan minyak</li>
      <li>Siapkan wajan</li>
      <li>Masukan minyak ke dalam wajan dan tunggu hingga panas</li>
      <li>Pecahkan telur</li>
      <li>Tuangkan telur ke dalam wajan dan tunggu beberapa menit</li>
      <li>Ambil nasi dan sajikan</li>
    </ol>
</body>
</html>

### <h3>&lt;li&gt;</h3>
Elemen ini digunakan untuk membuat list item dalam sebuah webpage.
```html title="li.html"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Element li</title>
</head>

<body>
    <ul>
        <li>Kucing</li>
        <li>Ayam</li>
        <li>Kelinci</li>
    </ul>
</body>

</html>

```

!!! example "Output elemen <`li`>"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Element li</title>
</head>

<body>
    <ul>
        <li>Kucing</li>
        <li>Ayam</li>
        <li>Kelinci</li>
    </ul>
</body>

</html>

### <h3>&lt;dl&gt;</h3>
Elemen ini digunakan untuk membuat description list. Elemen ini biasanya terdiri dari sekumpulan term dan deskripsinya. Di dalam elemen ini, umumnya terdapat elemen lain seperti dt dan dd.
```html title="dl.html"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Element dl</title>
</head>

<body>
    <dl>
        <dt>Sushi</dt>
        <dd>
            adalah makanan Jepang yang terdiri dari nasi yang dibentuk bersama lauk (neta) berupa makanan laut, daging, sayuran bakar atau sudah dimasak.
        </dd>
        <dt>Onigiri</dt>
        <dd>
            adalah nama Jepang untuk makanan berupa nasi yang dipadatkan sewaktu masih hangat sehingga berbentuk segitiga, bulat, atau seperti karung beras
        </dd>
    </dl>
</body>

</html>
```

### <h3>&lt;dt&gt;</h3>
Elemen ini digunakan untuk memuat istilah yang sedang didefinisikan (definition term / istilah definisi)
```html title="dt.html"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Element dt</title>
</head>

<body>
    <dl>
        <dt>Sushi</dt>
        <dd>
            adalah makanan Jepang yang terdiri dari nasi yang dibentuk bersama lauk (neta) berupa makanan laut, daging, sayuran bakar atau sudah dimasak.
        </dd>
        <dt>Onigiri</dt>
        <dd>
            adalah nama Jepang untuk makanan berupa nasi yang dipadatkan sewaktu masih hangat sehingga berbentuk segitiga, bulat, atau seperti karung beras
        </dd>
    </dl>
</body>

</html>
```
### <h3>&lt;dd&gt;</h3>
Elemen ini digunakan untuk memuat sebuah penjelasan dari term / istilah yang sedang didefinisikan
```html title="dt.html"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Element dd</title>
</head>

<body>
    <dl>
        <dt>Sushi</dt>
        <dd>
            adalah makanan Jepang yang terdiri dari nasi yang dibentuk bersama lauk (neta) berupa makanan laut, daging, sayuran bakar atau sudah dimasak.
        </dd>
        <dt>Onigiri</dt>
        <dd>
            adalah nama Jepang untuk makanan berupa nasi yang dipadatkan sewaktu masih hangat sehingga berbentuk segitiga, bulat, atau seperti karung beras
        </dd>
    </dl>
</body>

</html>
```

!!! example "Output elemen <`dl`>, <`dt`> dan <`dd`>"

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Element dd</title>
</head>

<body>
    <dl>
        <dt>Sushi</dt>
        <dd>
            adalah makanan Jepang yang terdiri dari nasi yang dibentuk bersama lauk (neta) berupa makanan laut, daging, sayuran bakar atau sudah dimasak.
        </dd>
        <dt>Onigiri</dt>
        <dd>
            adalah nama Jepang untuk makanan berupa nasi yang dipadatkan sewaktu masih hangat sehingga berbentuk segitiga, bulat, atau seperti karung beras
        </dd>
    </dl>
</body>

</html>

### <h3>&lt;blockquote&gt;</h3>
Elemen ini digunakan untuk kutipan panjang dan biasanya kutipan tersebut diambil dari sumber lain.
```html title="blockquote.html"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Element blockquote</title>
</head>

<body>
<blockquote cite="https://graciousquotes.com/books/">
    <p>"Books are the quietest and most constant of friends;
        they are the most accessible and wisest of counselors, and
        the most patient of teacher."</p> 
        <p>— Charles W. Eliot</p>
    </p>
</blockquote>
</body>

</html>
```

!!! example "Output elemen <`blockquote`>"

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Element blockquote</title>
</head>

<body>
<blockquote cite="https://graciousquotes.com/books/">
    <p>"Books are the quietest and most constant of friends;
        they are the most accessible and wisest of counselors, and
        the most patient of teacher."</p> 
        <p>— Charles W. Eliot</p>
    </p>
</blockquote>
</body>

</html>


### <h3>&lt;figure&gt;</h3>
Elemen ini adalah elemen yang berdiri sendiri. Elemen ini digunakan untuk membungkus konten seperti gambar, ilustrasi, diagram, cuplikan kode, dll.
```html title="figure.html"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Element figure</title>
</head>

<body>
<figure>
    <img src="/frontend/asset/blackgoose.png" alt="Logo produk">
</figure>
</body>

</html>
```
### <h3>&lt;figcaption&gt;</h3>
Elemen ini digunakan untuk menambahkan caption / keterangan dalam sebuah gambar, ilustrasi, diagram, cuplikan kode, dll.
```html title="figcaption.html"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Element figcaption</title>
</head>

<body>
<figure>
    <img src="/frontend/asset/blackgoose.png" alt="Logo produk">
    <figcaption>Gambar 1. Logo Produk</figcaption>
</figure>
</body>

</html>
```
!!! example "Output elemen <`figure`> dan <`figcaption`>"

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Element figure caption</title>
</head>

<body>
<figure>
    <img src="/frontend/asset/blackgoose.png" alt="Logo produk">
    <figcaption>Gambar 1. Logo Produk</figcaption>
</figure>
</body>

</html>

### <h3>&lt;header&gt;</h3>
Elemen ini digunakan untuk mendefinisikan pembuka dari halaman suatu web. Biasanya muncul di bagian atas web atau artikel.
```html title="header.html"
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Header Element</title>
</head>
<body>
    <header>
        <img src="/frontend/asset/blackgoose.png" alt="logo">
        <h1>Web Font</h1>
    </header>
</body>
</html>
```

!!! example "Output elemen <`header`>"

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Header Element</title>
</head>
<body>
    <header>
        <img src="/frontend/asset/blackgoose.png" alt="logo">
        <h1>Web Font</h1>
    </header>
</body>
</html>
### <h3>&lt;footer&gt;</h3>
Elemen ini digunakan untuk mendefinisikan penutup dari halaman suatu web. Biasanya muncul di bagian bawah web atau artikel dan berisi informasi seperti penulis (author), hak cipta (copyright), tautan ke dokumen terkait atau navigasi tambahan. 

```html title="footer.html"
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Elemen Footer</title>
</head>
<body>

  <header>
    <h1>Selamat Datang di Website Saya</h1>
  </header>

  <main>
    <p>Ini adalah konten utama dari halaman web.</p>
  </main>

  <footer>
    <p>Hak Cipta &copy; 2025 - ABCD</p>
    <p>Dibuat oleh <a href="https://github.com/" target="_blank">ABCD</a></p>
  </footer>

</body>
</html>
```

!!! example "Output elemen <`footer`>"

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Elemen Footer</title>
</head>
<body>

  <header>
    <h1>Selamat Datang di Website Saya</h1>
  </header>

  <main>
    <p>Ini adalah konten utama dari halaman web.</p>
  </main>

  <footer>
    <p>Hak Cipta &copy; 2025 - ABCD</p>
    <p>Dibuat oleh <a href="https://github.com/" target="_blank">ABCD</a></p>
  </footer>

</body>
</html>

### <h3>&lt;nav&gt;</h3>
Elemen ini digunakan untuk mendefinisikan bagian navigasi dalam sebuah situs web. Biasanya berisi tautan (link) yang mengarahkan pengguna ke halaman lain di dalam situs tersebut atau ke bagian tertentu dari halaman yang sama.
```html title="nav.html"
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ELemen nav</title>
</head>
<body>
    <nav>
    <ul>
      <li><a href="#beranda">Beranda</a></li>
      <li><a href="#tentang">Tentang</a></li>
      <li><a href="#layanan">Layanan</a></li>
      <li><a href="#kontak">Kontak</a></li>
    </ul>
  </nav>

  <section id="beranda">
    <h2>Beranda</h2>
    <p>Selamat datang di website kami!</p>
  </section>

  <section id="tentang">
    <h2>Tentang Kami</h2>
    <p>Ini adalah catatan pribadi.</p>
  </section>

  <section id="layanan">
    <h2>Layanan</h2>
    <p>Catatan Pribadi.</p>
  </section>

  <section id="kontak">
    <h2>Kontak</h2>
    <p>Email: info@contoh.com</p>
  </section>

</body>
</html>
```

!!! example "Output elemen <`nav`>"

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ELemen nav</title>
</head>
<body>
    <nav>
    <ul>
      <li><a href="#beranda">Beranda</a></li>
      <li><a href="#tentang">Tentang</a></li>
      <li><a href="#layanan">Layanan</a></li>
      <li><a href="#kontak">Kontak</a></li>
    </ul>
  </nav>

  <section id="beranda">
    <h2>Beranda</h2>
    <p>Selamat datang di website kami!</p>
  </section>

  <section id="tentang">
    <h2>Tentang Kami</h2>
    <p>Ini adalah catatan pribadi.</p>
  </section>

  <section id="layanan">
    <h2>Layanan</h2>
    <p>Catatan Pribadi.</p>
  </section>

  <section id="kontak">
    <h2>Kontak</h2>
    <p>Email: info@contoh.com</p>
  </section>

</body>
</html>
### <h3>&lt;section&gt;</h3>
Elemen ini digunakan untuk mengelompokan konten terkait secara bersama-sama, dan biasanya setiap bagian konten memiliki judulnya sendiri.

```html title="section.html"
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen section</title>
</head>
<body>
  <section>
    <h2>Beranda</h2>
    <p>Selamat datang di website kami!</p>
  </section>

  <section>
    <h2>Tentang Kami</h2>
    <p>Ini adalah catatan pribadi.</p>
  </section>

  <section>
    <h2>Layanan</h2>
    <p>Catatan Pribadi.</p>
  </section>

  <section>
    <h2>Kontak</h2>
    <p>Email: info@contoh.com</p>
  </section>

</body>
</html>
```

!!! example "Output elemen <`section`>"

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen section</title>
</head>
<body>
  <section>
    <h2>Beranda</h2>
    <p>Selamat datang di website kami!</p>
  </section>

  <section>
    <h2>Tentang Kami</h2>
    <p>Ini adalah catatan pribadi.</p>
  </section>

  <section>
    <h2>Layanan</h2>
    <p>Catatan Pribadi.</p>
  </section>

  <section>
    <h2>Kontak</h2>
    <p>Email: info@contoh.com</p>
  </section>

</body>
</html>
### <h3>&lt;article&gt;</h3>
Elemen ini digunakan untuk konten mandiri yang dapat berdiri sendiri atau digunakan kembali dalam konteks yang berbeda. Biasanya elemen ini digunakan untuk artikel majalah, atau surat kabar, postingan blog, komentar atau item lain.

```html title="article.html"
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen artikel</title>
</head>
<body>
    <article>
        <h2>Ini adalah contoh penggunaan elemen artikel</h2>
        <p>
        Belajar pemrograman membantu meningkatkan logika dan kemampuan problem solving. Ini juga membuka peluang karir yang luas di bidang teknologi
        </p>
    </article>
</body>
</html>
```
!!! example "Output elemen <`article`>"

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen artikel</title>
</head>
<body>
    <article>
        <h2>Ini adalah contoh penggunaan elemen artikel</h2>
        <p>
        Belajar pemrograman membantu meningkatkan logika dan kemampuan problem solving. Ini juga membuka peluang karir yang luas di bidang teknologi
        </p>
    </article>
</body>
</html>

### <h3>&lt;aside&gt;</h3>
Elemen ini digunakan untuk memberikan informasi tambahan. Contohnya, dalam sebuah elemen artikel aside biasanya akan menampung informasi yang berhubungan dengan artikel tetapi tidak essential untuk artikel secara keseluruhan. Sebagai contoh, menambahkan pullquote atau glosarium. Elemen ini juga dapat digunakan diluar elemen artikel untuk menampung informasi yang terakit dalam suatu halaman di dalam webpage.

Aside dalam elemen artikel (pullquote):
```html title="aside.html"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen aside sebagai pullquote</title>
</head>

<body>
    <article>
        <h2>Mengapa Python Cocok untuk Pemula?</h2>
        <p>Python adalah bahasa pemrograman yang sangat populer karena sintaksnya yang sederhana dan mudah dipahami,
            terutama bagi pemula.</p>

        <aside>
            <blockquote>
                "Python dirancang agar bisa dibaca seperti bahasa manusia — itulah kekuatan utamanya."
            </blockquote>
        </aside>

        <p>Selain itu, Python juga didukung oleh komunitas besar dan pustaka (library) yang lengkap, mulai dari
            pengolahan data hingga pengembangan web dan kecerdasan buatan.</p>
    </article>


</body>

</html>
```
!!! example "Output elemen <`aside`> sebagai pullquote"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen aside sebagai pullquote</title>
</head>

<body>
    <article>
        <h2>Mengapa Python Cocok untuk Pemula?</h2>
        <p>Python adalah bahasa pemrograman yang sangat populer karena sintaksnya yang sederhana dan mudah dipahami,
            terutama bagi pemula.</p>

        <aside>
            <blockquote>
                "Python dirancang agar bisa dibaca seperti bahasa manusia — itulah kekuatan utamanya."
            </blockquote>
        </aside>

        <p>Selain itu, Python juga didukung oleh komunitas besar dan pustaka (library) yang lengkap, mulai dari
            pengolahan data hingga pengembangan web dan kecerdasan buatan.</p>
    </article>


</body>

</html>


Aside sebagai glosarium:
```html title="aside_glosarium.html"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen aside sebagai glosarium</title>
</head>

<body>
    <article>
        <h2>Dasar-Dasar Fungsi di Python</h2>
        <p>Fungsi di Python digunakan untuk mengelompokkan kode agar dapat digunakan kembali dan membuat program lebih
            rapi.</p>

        <aside>
            <h3>Glosarium</h3>
            <ul>
                <li><strong>Fungsi:</strong> Blok kode yang hanya dijalankan saat dipanggil.</li>
                <li><strong>Parameter:</strong> Variabel yang diteruskan ke dalam fungsi.</li>
                <li><strong>Return:</strong> Nilai yang dikembalikan oleh fungsi setelah dieksekusi.</li>
            </ul>
        </aside>

        <p>Kita bisa membuat fungsi sendiri menggunakan kata kunci <code>def</code> dan memanggilnya sesuai kebutuhan.
        </p>
    </article>



</body>

</html>
```
!!! example "Output elemen <`aside`> sebagai glosarium"

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen aside sebagai glosarium</title>
</head>

<body>
    <article>
        <h2>Dasar-Dasar Fungsi di Python</h2>
        <p>Fungsi di Python digunakan untuk mengelompokkan kode agar dapat digunakan kembali dan membuat program lebih
            rapi.</p>

        <aside>
            <h3>Glosarium</h3>
            <ul>
                <li><strong>Fungsi:</strong> Blok kode yang hanya dijalankan saat dipanggil.</li>
                <li><strong>Parameter:</strong> Variabel yang diteruskan ke dalam fungsi.</li>
                <li><strong>Return:</strong> Nilai yang dikembalikan oleh fungsi setelah dieksekusi.</li>
            </ul>
        </aside>

        <p>Kita bisa membuat fungsi sendiri menggunakan kata kunci <code>def</code> dan memanggilnya sesuai kebutuhan.
        </p>
    </article>



</body>

</html>
### <h3>&lt;address&gt;</h3>
Elemen ini digunakan untuk kebutuhan yang spesifik, yaitu untuk membuat detail kontak penulis halaman dalam situs web. 

```html title="address.html"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen address</title>
</head>

<body>
    <footer>
        <p>Hak Cipta &copy; 2025 - ABCD</p>
        <p>Dibuat oleh <a href="https://github.com/" target="_blank">ABCD</a></p>
        <address>
            <p>
                Jl. Contoh. No. 12356.<br> 
                Indonesia. Jawa Barat
            </p>
        </address>
    </footer>



</body>

</html>
```

!!! example "Output elemen <`address`>"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen address</title>
</head>

<body>
    <footer>
        <p>Hak Cipta &copy; 2025 - ABCD</p>
        <p>Dibuat oleh <a href="https://github.com/" target="_blank">ABCD</a></p>
        <address>
            <p>
                Jl. Contoh. No. 12356.<br> 
                Indonesia. Jawa Barat
            </p>
        </address>
    </footer>



</body>

</html>

### <h3>&lt;em&gt;</h3>
Elemen ini gunakan untuk melakukan penekanan secara halus dalam suatu teks. Elemen ini biasanya ditampilkan secara italic oleh browser.

```html title="em.html"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen em</title>
</head>

<body>

    <p>I <em>think</em> Ivy was the first</p>
    <p>I think <em>Ivy</em> was the first</p>

</body>

</html>
```
!!! Example "Output elemen <`em`>"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen em</title>
</head>

<body>

    <p>I <em>think</em> Ivy was the first</p>
    <p>I think <em>Ivy</em> was the first</p>

</body>

</html>

### <h3>&lt;strong&gt;</h3>
Elemen ini digunakan untuk menunjukan penekanan yang kuat, menunjukan bahwa isinya sangat penting, serius atau mendesak.

```html title="strong.html"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen strong</title>
</head>

<body>

    <p>
        <strong>This text is important!</strong>
    </p>

</body>

</html>
```
!!! Example "Output elemen <`strong`>"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen strong</title>
</head>

<body>

    <p>
        <strong>This text is important!</strong>
    </p>

</body>

</html>

### <h3>&lt;b&gt; (bold)</h3>
Elemen ini digunakan untuk membuat karakter dalam teks atau tulisan tampak tebal.

```html title="elemenbold.html"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen bold</title>
</head>

<body>

    <p>
        Hello <b>World</b>
    </p>

</body>

</html>
```
!!! Example "Output elemen <`b`> (bold)"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen bold</title>
</head>

<body>

    <p>
        Hello <b>World</b>
    </p>

</body>

</html>

### <h3>&lt;i&gt; (italic)</h3>
Elemen ini digunakan untuk membuat karakter dalam teks atau tulisan tampak miring. Elemen ini biasanya digunakan untuk istilah teknis atau istilah asing.

```html title="elemenitalic.html"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen italic</title>
</head>

<body>

    <p>
        <p>The <i>RMS Titanic</i>, a luxury steamship, sank on April 15, 1912 after striking an iceberg.</p>
    </p>

</body>

</html>
```
!!! Example "Output elemen <`i`> (italic)"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen italic</title>
</head>

<body>

    <p>
        <p>The <i>RMS Titanic</i>, a luxury steamship, sank on April 15, 1912 after striking an iceberg.</p>
    </p>

</body>

</html>

### <h3>&lt;s&gt; (strike throught text)</h3>
Elemen ini digunakan untuk mengindikasikan bahwa suatu informasi sudah tidak akurat atau relevan lagi, tetapi informasi tidak boleh dihapus dalam webpage. Secara visual, elemen ini ditampilkan dengan garis melintang di tengah kata.

```html title="elmen_s.html"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen strike throught line</title>
</head>

<body>

    <p>Laptop computer:</p>
    <p><s>Was $995</s></p>
    <p>Now only $375</p>

</body>

</html>
```
!!! Example "Output elemen `<s>`"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen strike throught line</title>
</head>

<body>

    <p>Laptop computer:</p>
    <p><s>Was $995</s></p>
    <p>Now only $375</p>

</body>

</html>

### <h3>&lt;u&gt; (underline)</h3>
Elemen ini digunakan untuk teks atau tulisan yang ditata atau diartikulasikan berbeda dari teks yang normal / pada umumnya, seperti kata yang salah pengejaan atau nama seseorang dalam bahasa Mandarin (Chinese Text).

```html title="elemen_u"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen underline</title>
</head>

<body>

    <p>This is some <u>mispeled</u> text.</p>

</body>

</html>
```

!!!Example "Output elemen `<u>` (underline)"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen underline</title>
</head>

<body>

    <p>This is some <u>mispeled</u> text.</p>

</body>

</html>

### <h3>&lt;small&gt;</h3>
Elemen ini digunakan untuk menampilkan teks dengan ukuran yang lebih kecil dari teks yang ada disekitarnya. Biasanya teks ini digunakan untuk kebutuhan hak cipta atau _side comment_.

```html title="elemen_small.html"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen small</title>
</head>

<body>

    <p>
        Ini adalah elemen paragraf
    </p>

    <p>
        <p><small>&copy; 2025 ABCD. Semua hak cipta dilindungi.</small></p>
    </p>


</body>

</html>
```
!!! Example "Output elemen `<small>`"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen small</title>
</head>

<body>

    <p>
        Ini adalah elemen paragraf
    </p>

    <p>
        <p><small>&copy; 2025 ABCD. Semua hak cipta dilindungi.</small></p>
    </p>


</body>

</html>

### <h3>&lt;q&gt; (qoute)</h3>
Elemen ini digunakan untuk kutipan pendek yang berada dalam paragraf. 

```html title="elementq.html"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen q</title>
</head>

<body>

    <p>As A.A. Milne said, <q>Some people talk to
            animals. Not many listen though. That's the
            problem.</q></p>


</body>

</html>
```
!!! Example "Output elemen <`q`> (quote)"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen q</title>
</head>

<body>

    <p>As A.A. Milne said, <q>Some people talk to
            animals. Not many listen though. That's the
            problem.</q></p>


</body>

</html>

### <h3>&lt;abbr&gt; (abbreviations)</h3>
Elemen ini digunakan untuk menandai singkatan atau akronim dalam sebuah teks.

```html title="elemenabbr.html"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen abbr</title>
</head>

<body>
<p>
    The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.
</p>
</body>

</html>
```

!!!Example "Output elemen `<abbr>`"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen abbr</title>
</head>

<body>
<p>
    The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.
</p>
</body>

</html>

### <h3>&lt;cite&gt; (citation)</h3>
Elemen ini digunakan untuk memberikan referensi ketika mengambil sumber dari buku, tulisan orang lain atau referensi ilmiah (paper penelitian / riset).

```html title="elemencite.html"
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen  cite</title>
</head>
<body>
    <p>
        <cite>The Scream</cite>by Edward Munch. Painted in 1893.
    </p>
</body>
</html>
```

!!! Example "Output elemen `<cite>`"
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen  cite</title>
</head>
<body>
    <p>
        <cite>The Scream</cite>by Edward Munch. Painted in 1893.
    </p>
</body>
</html>

### <h3>&lt;dfn&gt; (define terms)</h3>
Elemen ini digunakan untuk menjelaskan beberapa terminologi baru (seperti konsep akademis atau jargon) dalam sebuah dokumen.

```html title="elemendfn.html"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen cite</title>
</head>

<body>
    <p>
        <dfn>HTML</dfn>is standard markup language for creating web pages
    </p>
</body>

</html>
```
!!! Example "Output elemen `<dfn>`"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen cite</title>
</head>

<body>
    <p>
        <dfn>HTML</dfn> is standard markup language for creating web pages
    </p>
</body>

</html>

### <h3>&lt;sup&gt; (supscript)</h3>
Elemen ini digunakan untuk memunculkan teks kecil di atas garis normal teks. Umumnya digunakan untuk Notasi matematika (contoh: pangkat) atau catatan kaki (footnote).

```html title="elemensup.html"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen supscript</title>
</head>

<body>
    <p>
        This is supscript
    </p>
    E = MC<sup>2</sup>
</body>

</html>
```

!!! Example "Output elemen `<sup>`"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen supscript</title>
</head>

<body>
    <p>
        This is supscript
    </p>
    E = MC<sup>2</sup>
</body>

</html>

### <h3>&lt;sub&gt; (subscript)</h3>
Elemen ini digunakan untuk memunculkan teks kecil di bawah garis normal teks. Umumnya digunakan untuk rumus kimia.

```html title="elemensup.html"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen supscript</title>
</head>

<body>
    <p>
        This is subscript
    </p>
    H<sub>2</sub>O
</body>

</html>
```

!!! Example "Output elemen `<sub>`"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen subscript</title>
</head>

<body>
    <p>
        This is subscript
    </p>
    H<sub>2</sub>O
</body>

</html>

### <h3>&lt;mark&gt;</h3>
### <h3>&lt;time&gt;</h3>
### <h3>&lt;data&gt;</h3>
### <h3>&lt;ins&gt; (inserted)</h3>
Elemen ini digunakan untuk menunjukan bahwa sebuah konten telah dimasukan ke dalam sebuah dokumen.
```html title="elemen_ins.html"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen ins dan del</title>
</head>

<body>
    <p>It was the <del>worst</del> <ins>best</ins> idea
        she had ever had.</p>
</body>

</html>
```
!!! Example "Output elemen `<ins>`"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen ins dan del</title>
</head>

<body>
    <p>It was the <del>worst</del> <ins>best</ins> idea
        she had ever had.</p>
</body>

</html>

### <h3>&lt;del&gt; (deleted)</h3>
Elemen ini adalah kebalikan dari elemen ins. Elemen ini digunakan untuk menunjukan bahwa sebuah konten telah dihilangkan dari dalam dokumen.

```html title="elemen_del.html"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen ins dan del</title>
</head>

<body>
    <p>It was the <del>worst</del> <ins>best</ins> idea
        she had ever had.</p>
</body>

</html>
```

!!! Example "Output elemen `<del>`"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen ins dan del</title>
</head>

<body>
    <p>It was the <del>worst</del> <ins>best</ins> idea
        she had ever had.</p>
</body>

</html>

### <h3>&lt;br&gt;</h3>
Elemen ini digunakan untuk membuat baris baru / jeda baris di tengah paragraf.

```html title="elemenbr.html"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen br</title>
</head>

<body>
    <p>
        Jl. Contoh. No. 12356.<br>
        Indonesia. Jawa Barat
    </p>
</body>

</html>
```

!!! Example "Output elemen br"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elemen br</title>
</head>

<body>
    <p>
        Jl. Contoh. No. 12356.<br>
        Indonesia. Jawa Barat
    </p>
</body>

</html>

### <h3>&lt;wbr&gt;</h3>

### <h3>&lt;div&gt;</h3>
Elemen ini digunakan untuk mengelompokan konten yang bertipe blok (_block element_). Tag ini dapat menggunakan atribut id dan class agar dapat dimanipulasi oleh CSS atau JavaScript.

```html title="div.html"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Div and Span Element in HTML</title>
</head>

<body>
    <!--Div element: Tag element to grouping block of content (block element)-->
    <div class="listing">
        <img src="/frontend/asset/blackgoose.png" alt="blackgoose-logo">
        <p><cite>The Complete Manual of Typography</cite>, James Felici</p>
        <p>A Combination of type history and example of good or bad type design</p>
    </div>

    <div id="news">
        <h1>New Thid Week</h1>
        <p>We've been working on</p>
        <p>And last but not least, ....</p>
    </div>
```

!!! example "Output elemen `<div>`"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Div and Span Element in HTML</title>
</head>

<body>
    <!--Div element: Tag element to grouping block of content (block element)-->
    <div class="listing">
        <img src="/frontend/asset/blackgoose.png" alt="">
        <p><cite>The Complete Manual of Typography</cite>, James Felici</p>
        <p>A Combination of type history and example of good or bad type design</p>
    </div>

    <div id="news">
        <h1>New Thid Week</h1>
        <p>We've been working on</p>
        <p>And last but not least, ....</p>
    </div>
    
</body>

</html>

### <h3>&lt;span&gt;</h3>
Elemen ini digunakan untuk mengelompokan konten inline (_inline element_). Tag ini dapat menggunakan atribut id dan class agar dapat dimanipulasi oleh CSS atau JavaScript.

```html title="elemen span"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Div and Span Element in HTML</title>
</head>

<body>
<!--Span element: Tag element to group inline content (inline element)-->
    <li>John: <span class="tel">999.8282</span></li>
    <li>Paul: <span class="tel">888.4889</span></li>
    <li>George: <span class="tel">888.1628</span></li>
    <li>Ringo: <span class="tel">999.3220</span></li>
</body>

</html>
```

!!! example "Output elemen `<span>`"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Div and Span Element in HTML</title>
</head>

<body>
<!--Span element: Tag element to group inline content (inline element)-->
    <li>John: <span class="tel">999.8282</span></li>
    <li>Paul: <span class="tel">888.4889</span></li>
    <li>George: <span class="tel">888.1628</span></li>
    <li>Ringo: <span class="tel">999.3220</span></li>
</body>

</html>


#### Notes
!!! info "Tabel perbedaan elemen div dan span"
    
    | Perbedaan            | `<div>`          | `<span>`              |
    |----------------------|------------------|------------------------|
    | Jenis Elemen         | Block Level      | Inline Level           |
    | Tampilan Dalam Website | Mulai Baris Baru | Dalam Baris            |
    | Kegunaan             | Layout, Container| Penyorotan teks        |

!!! info "Atribut id dan class"

    - `id` digunakan untuk identifikasi **unik** pada satu elemen HTML.
    - `class` digunakan untuk **mengelompokkan beberapa elemen** yang memiliki gaya atau fungsi yang sama.
    - Baik `id` maupun `class` adalah **atribut global** dalam HTML, yang berarti bisa digunakan di hampir semua elemen.


### <h3>&lt;a&gt;</h3>
Elemen ini biasanya digunakan untuk menambahkan hyperlink ke dalam sebuah website. Fungsinya biasanya untuk membuat tautan ke situs lain, ke halaman di dalam situs sendiri atau ke bagian tertentu dalam halaman yang sama. Tujannya adalah agar dapat memudahkan navigasi konten di dalam maupun di luar website. 

#### Notes

!!! note "Absolute URL"
Absolute URL (_Uniform Resource Locator_) adalah alamat lengkap dari sebuah resource di internet. Umumnya absolute url menyertakan protokol web yang digunakan, domain situs dan _pathname_. Biasanya hal ini dipergunakan untuk mengarahkan resource yang berada di luar website atau server.

```html title="absolute.html"
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>URL</title>
</head>
<body>
    <a href="https://www.allrecipes.com/recipe/12345/fried-rice/">Lihat Resep Fried Rice</a>
</body>
</html>
```

!!! example "Contoh output Absolute URL"
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>URL</title>
</head>
<body>
    <a href="https://www.allrecipes.com/recipe/36875/indonesian-satay/">Lihat Resep Indonesian Satay</a>
</body>
</html>


!!! note "Relative URL"
Relative URL (_Uniform Resource Locator_) adalah alamat yang mendeskripsikan _pathname_ berdasarkan posisi relatif dokumen saat ini. Biasanya hal ini digunakan untuk mengarahkan resource yang masih berada dalam satu website atau server.
```html title="relativeurl.html"
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>URL</title>
</head>
<body>
    <a href="frontend/pages/about.html">Tentang Kami</a>
</body>
</html>
```

!!! example "Contoh output Relative URL"

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>URL</title>
</head>
<body>
    <a href="/frontend/pages/about.html">Tentang Kami</a>
</body>
</html>

!!! info "Anchor tag atribut blank"
Atribute _blank digunakan untuk membuka suatu halaman web di window atau tab baru.

```html title="blankatrribute.html"
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>URL</title>
</head>
<body>
    <a href="www.google.com" target="_blank"></a>
</body>
</html>
```

!!! example "Atribut target_ blank"


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>URL</title>
</head>
<body>
    <a href="https://www.google.com" target="_blank">Kunjungi Google</a>
</body>
</html>


!!! note "mailto dalam anchor tag"
mailto digunakan untuk membuka program email pengguna dan mengarahkan email ke alamat tertentu.

```html title="mailto.html"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>URL</title>
</head>

<body>
    <a href="mailto:coba@example.com">Email contoh</a>
</body>

</html>
```

!!! example "Contoh output `<mailto>`"
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>URL</title>
</head>

<body>
    <a href="mailto:coba@example.com">Email contoh</a>
</body>

</html>


#### Tabel Perbedaan Relative Linking Path dengan Anchor Tag

| Deskripsi                                | Contoh Path                         | Contoh Penggunaan `<a href="">`                                  | Penjelasan                                                                 |
|------------------------------------------|-------------------------------------|------------------------------------------------------------------|----------------------------------------------------------------------------|
| File berada di folder yang sama          | `file.html`                         | `<a href="file.html">Buka File</a>`                              | Mengarah ke file di direktori yang sama dengan file HTML saat ini.        |
| Masuk ke subfolder                       | `folder/file.html`                  | `<a href="folder/file.html">Masuk Folder</a>`                    | Masuk ke dalam subfolder dari direktori saat ini.                         |
| Masuk lebih dalam (nested folder)        | `folder1/folder2/file.html`         | `<a href="folder1/folder2/file.html">Buka File Nested</a>`       | Masuk ke subfolder di dalam subfolder.                                    |
| Naik satu level ke parent folder         | `../file.html`                      | `<a href="../file.html">Kembali Satu Level</a>`                  | Kembali satu folder ke atas dari direktori saat ini.                      |
| Naik satu level lalu masuk subfolder     | `../images/logo.png`                | `<a href="../images/logo.png">Lihat Gambar</a>`                  | Naik satu level, lalu masuk ke folder `images`.                           |
| Naik dua level                           | `../../file.html`                   | `<a href="../../file.html">Naik Dua Level</a>`                   | Kembali dua folder ke atas dari direktori saat ini.                       |
| Naik dua level lalu masuk subfolder      | `../../assets/img.png`              | `<a href="../../assets/img.png">Lihat Logo</a>`                  | Naik dua level, lalu masuk ke folder `assets`.                            |
| Link ke bagian spesifik di dalam halaman yang sama   | `#section1`                         | `<a href="#section1">Lompat ke Section 1</a>`                    | Mengarah ke elemen dengan `id="section1"` di halaman yang sama.           |
| Link ke bagian spesifik di halaman lain  | `page.html#section1`               | `<a href="page.html#section1">Lompat ke Section 1 di Halaman Lain</a>` | Mengarahkan ke elemen dengan `id="section1"` di halaman lain bernama `page.html`. Berguna untuk langsung menuju bagian tertentu pada halaman lain. |

### <h3>&lt;img&gt;</h3>
Elemen ini digunakan untuk menambahkan / menyisipkan gambar ke dalam sebuah _webpage_.

```html title="img.html"

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image Element</title>
</head>

<body>
    <!--Img element. To Insert element in webpage. There are several atribute like width and heigt to adjust width and height and align to adjust position in web. Lebih baik atur di CSS saja-->
    <img src="images/blackgoose.png" alt="Blackgoose-logo" width="120" height="120" align="middle">

    <!--fig or figcaption: same as img element, but fig and figcaption can add caption to an image-->
    <!-- <figure>
        <img src="images/blackgoose.png" alt="blackgoose.png">
        <figcaption>
            BlackGoose Merk Logo
        </figcaption>
    </figure> -->
</body>

</html>
```

!!! example "Output Elemen `<img>`"

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image Element</title>
</head>
<body>
    <!-- Elemen img digunakan untuk menyisipkan gambar ke halaman web. -->
    <!-- Atribut seperti width, height, dan align dapat digunakan, namun lebih baik mengatur gaya melalui CSS. -->
    <img src="/frontend/asset/blackgoose.png" alt="Logo BlackGoose" width="120" height="120" align="left">

    <!-- Alternatif: Gunakan <figure> dan <figcaption> untuk menambahkan keterangan gambar -->
    <!--
    <figure>
        <img src="/frontend/asset/blackgoose.png" alt="Logo BlackGoose">
    <figcaption>BlackGoose Merk Logo</figcaption>
    </figure>
        -->
</body>
</html>



