# Basic HTML (Hypertext Markup Language)

HTML (Hypertext Markup Language) it define the meaning and structure of web content. In simple language, HTML is like skeleton of website.

!!! note "HTML Boilerplate"

``` HTML
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

- Use this `!` to show emmit suggestion for HTML Boilerplate in Visual Studio Code

## Basic HTML Tag

### Paragraph

!!! note "Key Takeaways"

- p tags in HTML not only can use for text, but also can use to grouping of related content
- P tags is block level element

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Coba ulang</title>
  </head>
  <body>
    <h1>Chicken</h1>
    <img src="chicken.jpg" alt="chicken-images" />
    <p>
      The <b>chicken</b><i><b>(Gallus gallus domesticus)</b></i> is a
      domesticated subspecies of the <a href="">red jungleowl</a> (<i
        >Gallus gallus</i
      >), originally native to
      <a href="https://en.wikipedia.org/wiki/Southeast_Asia">Southeast Asia.</a>
    </p>
  </body>
</html>
```

### Heading

!!! note "Key takeaways"

- Heading is used to define title and subtitle in web page
- &lt;h1&gt; is the highest section level and &lt;h6&gt; is the lowest
- Heading is block level element

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Headings</title>
</head>
<body>
    <h1>Hello World</h1>
    <h2>Hello World</h2>
    <h3>Hello World</h3>
    <h4>Hello World</h4>
    <h5>Hello World</h1>
    <h6>Hello World</h6>
</body>
</html>
```

### List

!!! note "Key Takeaways"

- &lt;li&gt;&lt;/li&gt; represent item in list
- &lt;ol&gt;&lt;/ol&gt; ordered list (numbered)
- &lt;ul&gt;&lt;ul&gt; unordered list (bullet points)

#### &lt;ol&gt;&lt;/ol&gt;

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>HTML List</title>
  </head>
  <body>
    <ol>
      <li>Mix flour, baking powder, sugar, and salt.</li>
      <li>In another bowl, mix eggs, milk, and oil.</li>
      <li>Stir both mixtures together.</li>
      <li>Fill muffin tray 3/4 full.</li>
      <li>Bake for 20 minutes.</li>
    </ol>
  </body>
</html>
```

#### &lt;ul&gt;&lt;ul&gt;

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>HTML List</title>
  </head>
  <body>
    <ul>
      <li>Blue cheese</li>
      <li>Feta</li>
    </ul>
  </body>
</html>
```

List can be nested, for example

```html
<ul>
  <li>first item</li>
  <li>
    second item
    <!-- Look, the closing </li> tag is not placed here! -->
    <ul>
      <li>second item first subitem</li>
      <li>
        second item second subitem
        <!-- Same for the second nested unordered list! -->
        <ul>
          <li>second item second subitem first sub-subitem</li>
          <li>second item second subitem second sub-subitem</li>
          <li>second item second subitem third sub-subitem</li>
        </ul>
      </li>
      <!-- Closing </li> tag for the li that
                  contains the third unordered list -->
      <li>second item third subitem</li>
    </ul>
    <!-- Here is the closing </li> tag -->
  </li>
  <li>third item</li>
</ul>
```

### Anchor Element
