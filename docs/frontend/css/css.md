## Cascading Style Sheet (CSS)

Cascading Style Sheet adalah standar W3C untuk mendefinisikan penyajian (_presentation_) dokumen yang ditulis dalam HTML. Penyajian ini mengacu pada cara dokumen disampaikan kepada pengguna, apakah di layar komputer, ditampilkan di ponsel, dll.

### General CSS Syntax 
![css-syntax](../asset/syntax-css.PNG)

### External & Internal Link CSS

Untuk menerapkan rule style CSS bisa menggunakan melalui cara external link CSS dengan syntax berikut.
```
<link rel="stylesheet" href="">
```
Taruh external link tersebut di dalam tag body file HTML. Berikut ini contohnya:
![code-snip](../asset/code-snip-1.png)

Atau bisa juga dengan cara internal link dengan menggunakan elemen tag `<style>`. Berikut ini contohnya:
![code-snip](../asset/code-snip.png)

### Jenis-Jenis CSS Selector

| **Selector**              | **Arti**                                                                 | **Contoh**             | **Penjelasan**                                                                 |
|--------------------------|--------------------------------------------------------------------------|------------------------|---------------------------------------------------------------------------------|
| Universal Selector       | Menerapkan gaya ke semua elemen dalam dokumen                           | `* {}`                 | Menargetkan semua elemen dalam halaman                                         |
| Type Selector            | Menyesuaikan nama elemen                                                 | `h1, h2, h3 {}`        | Menargetkan elemen `<h1>`, `<h2>`, dan `<h3>`                                  |
| Class Selector           | Menargetkan elemen yang memiliki atribut `class` sesuai dengan nama yang diberikan setelah titik (`.`) | `.note {}`             | Menargetkan semua elemen yang memiliki `class="note"`                         |
|                          |                                                                          | `p.note {}`            | Menargetkan hanya elemen `<p>` dengan `class="note"`                          |
| ID Selector              | Menargetkan elemen yang memiliki atribut `id` sesuai dengan nama yang diberikan setelah tanda pagar (`#`) | `#introduction {}`     | Menargetkan elemen dengan `id="introduction"`                                 |
| Child Selector           | Menargetkan elemen yang merupakan _child selector_. Artinya cari elemen `<a>` yang merupakan _child_. dari elemen tag `<li>`     | `li > a {}`            | Menargetkan semua elemen `<a>` yang langsung berada dalam elemen `<li>`   |
| Descendant Selector      | Menargetkan elemen yang merupakan keturunan dari elemen lain (tidak harus anak langsung). Artinya dalam contoh tersebut adalah, semua elemen tag `<a>` adalah keturunan dari elemen tag `<p>` | `p a {}`               | Menargetkan semua elemen `<a>` yang berada di dalam elemen `<p>`              |
| Adjacent Sibling Selector| Menargetkan elemen yang merupakan saudara kandung terdekat setelah elemen lain | `h1 + p {}`            | Menargetkan elemen `<p>` pertama setelah `<h1>`                               |
| General Sibling Selector | Menargetkan elemen yang merupakan saudara kandung umum. | `h1 ~ p {}`            | Menargetkan semua elemen `<p>` yang merupakan saudara dari elemen `<h1>`      |

### Color (Warna)

#### Properties `color`

Properties `color` memungkinkan untuk mengatur warna teks (_foreground color_) dalam sebuah elemen. Hal ini dapat dilakukan dengan 3 cara:

- _RGB Values_
- _Hexadecimal Code_ 
- _Color Names_

!!! Example "_RGB Values_"
  ```
  /* Using RGB values */

  p {
    color: rgb(189, 189, 88);
  }
  ```

!!! Example "_Hexadecimal Code_"
```
  /* Using hexa value */

  h2 {
      color: #f5deb3;
  }
```

!!! Example "_Color Names_"
```
  /* Using color name */

  h1 {
    color: white;
  }
```

#### Properties `background-color`

Properties `background-color` memungkinkan untuk mengatur warna _background_ dalam sebuah elemen. 
Cara pengaturan warna nya sama seperti _properties_ `color`.

!!! Example "_RBG Value_"
```
body {
    background-color: rgb(200, 200, 200);
  }
```

!!! Example "_Hexadecimal Code_"
```
  h2 {
    background-color: #ee3e80;
  }
```

!!! Example "_Color Names_"
```
  p {
    background-color: white;
  }
```

!!! info "HTML and CSS Code"
=== "HTML"

    ``` html
    <!DOCTYPE html>
    <html lang="en">

    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Color in CSS</title>
    </head>

    <body>
        <link rel="stylesheet" href="color.css">
        <h1>Marine Biology</h1>
        <h2>Composition of Sea Water</h2>
        <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Nemo reiciendis molestiae iure repellat! Similique
            assumenda at eligendi pariatur magnam delectus corrupti, veritatis, eveniet quae ab, commodi dolore mollitia cum
            in!
        </p>
    </body>

    </html>
    ```
=== "CSS"

    ``` css
    /* How to add color to html element (selector) */


    /* FOREGROUWND COLOR */

    /* Using color name */

    h1 {
        color: white;
    }

    /* Using hexa value */

    h2 {
        color: #f5deb3;
    }

    /* Using RGB values */

    p {
        color: rgb(189, 189, 88);
    }


    /* BACKGROUND COLOR */

    body {
        background-color: rgb(200, 200, 200);
    }

    h1 {
        background-color: darkcyan;
    }

    h2 {
        background-color: #ee3e80;
    }

    p {
        background-color: white;
    }
    ```

### Text (Teks)

#### Properties `font-family`

Properties ini memungkinkan mengatur tampilan jenis huruf (_font_) dalam sebuah halaman website.

!!! info "HTML and CSS Code"
=== "HTML"

    ``` html
    <!DOCTYPE html>
    <html lang="en">

    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>CSS Text</title>
    </head>

    <body>
        <link rel="stylesheet" href="text.css">
        <h1>Briads</h1>
        <p class="credit">by Ivy Duckets</p>
        <p class="intro">The <a class="breed" href="http://en.wikipedia.org/wiki/
        Briard">briard</a>, or berger de brei, is a large breed of dog traditionally used as
            a header and guardian of sheep
        </p>
    </body>

    </html>
    ```

=== "CSS"

    ``` css
    /* Specify font family / style / typeface */

    body {
        font-family: Georgia, 'Times New Roman', Times, serif;
    }

    h1,
    h2 {
        font-family: Arial, Verdana, Geneva, sans-serif;
    }

    .credit {

        font-family: 'Courier New', Courier, monospace;
    }
    ```

#### Properties `font-size`

Properti ini digunakan untuk mengatur ukuran tulisan (_font_) dalam sebuah halaman website. 
Berikut ini beberapa cara untuk mengatur ukuran tulisan:

  - Pixels
  - Percentages 
  - Ems 

!!! example "Pixels"
```
body {
    font-family: Georgia, 'Times New Roman', Times, serif;
    font-size: 12px;
}
```

!!! example "Percentage"
```
h1,
h2 {
    font-family: Arial, Verdana, Geneva, sans-serif;
    font-size: 200%;
}
```

!!! example "Ems"
```
.credit {

    font-family: 'Courier New', Courier, monospace;
    font-size: 1.5em;
}
```

!!! info "HTML and CSS Code"
=== "HTML"

    ``` html
    <!DOCTYPE html>
    <html lang="en">

    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>CSS Text</title>
    </head>

    <body>
        <link rel="stylesheet" href="text.css">
        <h1>Briads</h1>
        <p class="credit">by Ivy Duckets</p>
        <p class="intro">The <a class="breed" href="http://en.wikipedia.org/wiki/
        Briard">briard</a>, or berger de brei, is a large breed of dog traditionally used as
            a header and guardian of sheep
        </p>
    </body>

    </html>
    ```

=== "CSS"

    ``` css
    /* Specify font family / style / typeface and font size*/

    body {
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-size: 12px;
    }

    h1,
    h2 {
        font-family: Arial, Verdana, Geneva, sans-serif;
        font-size: 200%;
    }

    .credit {

        font-family: 'Courier New', Courier, monospace;
        font-size: 1.5em;
    }
    ```

#### Properties `font-weight`

Properties ini digunakan untuk membuat tulisan bold (_text bold_). Properties ini memiliki dua nilai (_value_), yaitu normal dan bold. Untuk value normal maka tampilan teks akan terlihat normal, sedangkan untuk value bold maka tampilan teks akan terlihat tebal.

!!! example "properties font-weight"

```
.credit {

    font-family: 'Courier New', Courier, monospace;
    font-size: 1.5em;
    font-weight: bold;
}
```

!!! info "HTML and CSS Code"
=== "HTML"

    ``` html
    <!DOCTYPE html>
    <html lang="en">

    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>CSS Text</title>
    </head>

    <body>
        <link rel="stylesheet" href="text.css">
        <h1>Briads</h1>
        <p class="credit">by Ivy Duckets</p>
        <p class="intro">The <a class="breed" href="http://en.wikipedia.org/wiki/
        Briard">briard</a>, or berger de brei, is a large breed of dog traditionally used as
            a header and guardian of sheep
        </p>
    </body>

    </html>
    ```

=== "CSS"

    ``` css
    /* Specify font family / style / typeface and font size*/

    body {
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-size: 12px;
    }

    h1,
    h2 {
        font-family: Arial, Verdana, Geneva, sans-serif;
        font-size: 200%;
    }

    .credit {

        font-family: 'Courier New', Courier, monospace;
        font-size: 1.5em;
        font-weight: bold;
    }
    ```

#### Properties `font-style`

Properties ini digunakan untuk membuat huruf / tulisan terlihat _italic_. Terdapat tiga value dalam properties ini, yaitu:

 - normal 
 - italic
 - oblique

!!! example "properties font-style"
```
.credit {

    font-style: italic;
}
```
!!! info "HTML and CSS Code"
=== "HTML"

    ``` html
    <!DOCTYPE html>
    <html lang="en">

    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>CSS Text</title>
    </head>

    <body>
        <link rel="stylesheet" href="text.css">
        <h1>Briads</h1>
        <p class="credit">by Ivy Duckets</p>
        <p class="intro">The <a class="breed" href="http://en.wikipedia.org/wiki/
        Briard">briard</a>, or berger de brei, is a large breed of dog traditionally used as
            a header and guardian of sheep
        </p>
    </body>

    </html>
    ```

=== "CSS"

    ``` css
    /* Specify font family / style / typeface and font size*/

    body {
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-size: 12px;
    }

    h1,
    h2 {
        font-family: Arial, Verdana, Geneva, sans-serif;
        font-size: 200%;
    }

    .credit {

        font-family: 'Courier New', Courier, monospace;
        font-size: 1.5em;
        font-weight: bold;
        font-style: italic;
    }
    ```

#### Properties `text-transform`

Properties ini digunakan untuk mengubah huruf besar/kecil pada sebuah teks / tulisan.

!!! example "text-transform: uppercase"
```
body {
    font-family: Georgia, 'Times New Roman', Times, serif;
    font-size: 12px;
    text-transform: uppercase;
}
```

!!! example "text-transform: lowercase"
```
h1,
h2 {
    font-family: Arial, Verdana, Geneva, sans-serif;
    font-size: 200%;
    text-transform: lowercase;
}

```

!!! example "text-transform: capitalize"
```
.credit {

    font-family: 'Courier New', Courier, monospace;
    font-size: 1.5em;
    text-transform: capitalize;
}
```

!!! info "HTML and CSS Code"
=== "HTML"

    ``` html
    <!DOCTYPE html>
    <html lang="en">

    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>CSS Text</title>
    </head>

    <body>
        <link rel="stylesheet" href="text.css">
        <h1>Briads</h1>
        <p class="credit">by Ivy Duckets</p>
        <p class="intro">The <a class="breed" href="http://en.wikipedia.org/wiki/
        Briard">briard</a>, or berger de brei, is a large breed of dog traditionally used as
            a header and guardian of sheep
        </p>
        <h2>Breed History</h2>
        <p class="description">
            The briad, which is believed to have originated in France, has been bred for centuries to herd and protect the
            sheep.
        </p>
    </body>

    </html>
    ```

=== "CSS"

    ``` css
    body {
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-size: 12px;
        text-transform: uppercase;
    }

    h1,
    h2 {
        font-family: Arial, Verdana, Geneva, sans-serif;
        font-size: 200%;
        text-transform: lowercase;
    }

    .credit {

        font-family: 'Courier New', Courier, monospace;
        font-size: 1.5em;
        text-transform: capitalize;
    }
    ```

#### Properties `text-decoration`

Properties ini digunakan untuk menambahkan dekorasi pada teks. Properties ini memiliki empat _value_ (_overline_, _underline_, _line through_ dan _blink_).

!!! info "HTML and CSS Code"
=== "HTML"

    ``` html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>CSS Text Properties</title>
        <link rel="stylesheet" href="text.css">
    </head>
    <body>
        <h1>This is Heading 1</h1>
        <h2>This is Heading 2</h2>
        <h3>This is Heading 3</h3>
        <h4>This is Heading 4</h4>
    </body>
    </html>
    ```

=== "CSS"

    ``` css
    h1 {
    text-decoration: overline;
    }

    h2 {
    text-decoration: line-through;
    }

    h3 {
    text-decoration: underline;
    }

    h4 {
    text-decoration: blink;
    }
    ```

#### Properties `line-height`

Properties ini digunakan untuk mengatur jarak antar teks.

!!! info "HTML and CSS Code"
=== "HTML"

    ```html
    <!DOCTYPE html>
    <html lang="en">

    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>CSS Text Properties</title>
        <link rel="stylesheet" href="text.css">
    </head>

    <body>
        <h1>The Breed History</h1>
        <p>
            The briard, which is believed to have originated in France, has been bred for centuries to herd<br>
            and to protect sheep. The breed was used by French Army as sentries, messengers and to<br> 
            search for wounded soldiers because of its fine sense of hearing.
        </p>
    </body>

    </html>
    ```

=== "CSS"

    ```css
    p {
        line-height: 1.6;
    }
    ```

#### Properties `letter-spacing`

Properties ini digunakan untuk mengatur jarak (_space_) antar huruf dalam teks atau tulisan. 

!!! info "HTML dan CSS Code"
=== "HTML"

    ```html
    <!DOCTYPE html>
    <html lang="en">

    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>CSS Text Properties</title>
        <link rel="stylesheet" href="text.css">
    </head>

    <body>  
        <h1>Briads</h1>
        <p class="credit">by Ivy Duckets</p>
        <h2>The Breed History</h2>
        <p>
            The briard, which is believed to have originated in France, has been bred for centuries to herd<br>
            and to protect sheep. The breed was used by French Army as sentries, messengers and to<br> 
            search for wounded soldiers because of its fine sense of hearing.
        </p>
    </body>

    </html>
    ```

=== "CSS"

    ```css
    h1,h2 { 
        letter-spacing: 0.3em;
    }

    p {
        line-height: 1.6;
    }
    ```

#### Properties `word-spacing`

Properties ini digunakan untuk mengatur jarak (_space_) antar huruf dalam teks atau tulisan.

!!! info "HTML dan CSS Code"
=== "HTML"

    ```html
    <!DOCTYPE html>
    <html lang="en">

    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>CSS Text Properties</title>
        <link rel="stylesheet" href="text.css">
    </head>

    <body>  
        <h1>Briads</h1>
        <p class="credit">by Ivy Duckets</p>
        <h2>The Breed History</h2>
        <p>
            The briard, which is believed to have originated in France, has been bred for centuries to herd<br>
            and to protect sheep. The breed was used by French Army as sentries, messengers and to<br> 
            search for wounded soldiers because of its fine sense of hearing.
        </p>
    </body>

    </html>
    ```

=== "CSS"

    ```css
    h1,h2 { 
        letter-spacing: 0.3em;
    }

    p {
        line-height: 1.6;
        word-spacing: 1em;
    }
    ```

#### Properties `text-align`

Properties ini digunakan untuk mengatur _alignment_ sebuah teks. Terdapat empat _value_ dalam pengaturan _alignment_.
- left
- right
- center
- justify

!!! info "HTML dan CSS Code"

=== "HTML"

    ```html
    <!DOCTYPE html>
    <html lang="en">

    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>CSS Text Properties</title>
        <link rel="stylesheet" href="text.css">
    </head>

    <body>
        <h1>Briads</h1>
        <p class="credit">by Ivy Duckets</p>
        <p>
            The briad or berger de brie, is a large 
        </p>
        <h2>The Breed History</h2>
        <p>
            The briard, which is believed to have originated in France, has been bred for centuries to herd<br>
            and to protect sheep. The breed was used by French Army as sentries, messengers and to<br> 
            search for wounded soldiers because of its fine sense of hearing.
        </p>
    </body>

    </html>
    ```

=== "CSS"

    ```css
    h1,h2 {
        text-align: center;
    }

    .credit {
        text-align:right
    }
    p {
        line-height: 1.6;
        text-align: justify;
    }
    ```

#### Properties `vertical-align`
#### Properties `text-indent`

Properties ini digunakan untuk membuat indent di baris pertama sebuah teks.

!!! info "HTML dan CSS Code"

=== "HTML"

    ```html
    <!DOCTYPE html>
    <html lang="en">

    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>CSS Text Properties</title>
        <link rel="stylesheet" href="text.css">
    </head>

    <body>
        <h1>Briads</h1>
        <p class="credit">by Ivy Duckets</p>
        <p>
            The briad or berger de brie, is a large 
        </p>
        <h2>The Breed History</h2>
        <p>
            The briard, which is believed to have originated in France, has been bred for centuries to herd<br>
            and to protect sheep. The breed was used by French Army as sentries, messengers and to<br> 
            search for wounded soldiers because of its fine sense of hearing.
        </p>
    </body>

    </html>
    ```

=== "CSS"

    ```css
    h1,h2 {
        text-align: center;
    }

    .credit {
        text-indent:20px;
    }
    p {
        line-height: 1.6;
        text-align: justify;
    }
    ```

#### Properties `text-shadow`

#### Properties `first-letter`

Properties ini digunakan untuk membuat **drop capital** dimana huruf pertama dari awal tulisan ukuranya lebih besar daripada yang lain

!!! info "HTML dan CSS Code"

=== "HTML"

    ```html
    <!DOCTYPE html>
    <html lang="en">

    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>CSS Text Properties</title>
        <link rel="stylesheet" href="text.css">
    </head>

    <body>
        <h1>Briads</h1>
        <p class="credit">by Ivy Duckets</p>
        <p>
            The briad or berger de brie, is a large 
        </p>
        <h2>The Breed History</h2>
        <p class="intro">
            The briard, which is believed to have originated in France, has been bred for centuries to herd<br>
            and to protect sheep. The breed was used by French Army as sentries, messengers and to<br> 
            search for wounded soldiers because of its fine sense of hearing.
        </p>
    </body>

    </html>
    ```

=== "CSS"

    ```css
    h1,h2 {
        text-align: center;
    }

    .credit {
        text-indent:20px;
    }
    p {
        line-height: 1.6;
        text-align: justify;
    }

    p.intro:first-letter {
        font-size: 200%;
    }
    ```

#### Properties `first-line`

Properties ini digunakan untuk membuat efek tulisan (_typography effect_), misalnya untuk membuat tulisan bercetak tebal di baris pertama dalam sebuah teks.

!!! info "HTML dan CSS Code"

=== "HTML"

    ```html
    <!DOCTYPE html>
    <html lang="en">

    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>CSS Text Properties</title>
        <link rel="stylesheet" href="text.css">
    </head>

    <body>
        <h1>Briads</h1>
        <p class="credit">by Ivy Duckets</p>
        <p>
            The briad or berger de brie, is a large 
        </p>
        <h2>The Breed History</h2>
        <p class="intro">
            The briard, which is believed to have originated in France, has been bred for centuries to herd<br>
            and to protect sheep. The breed was used by French Army as sentries, messengers and to<br> 
            search for wounded soldiers because of its fine sense of hearing.
        </p>
    </body>

    </html>
    ```

=== "CSS"

    ```css
    h1,h2 {
        text-align: center;
    }

    .credit {
        text-indent:20px;
    }
    p {
        line-height: 1.6;
        text-align: justify;
    }

    p.intro:first-letter {
        font-size: 200%;
    }

    p.intro::first-line {
        font-weight: bold;
    }
    ```