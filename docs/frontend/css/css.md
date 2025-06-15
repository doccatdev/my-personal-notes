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