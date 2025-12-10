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

!!! example "Example of Use `p` Tag"

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

!!! example "Example of Use `h1-h6` Tag"

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

!!! example "Example of Use `li`, `ol`, `ul` Tag"

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

!!! Key Takeaways

- The anchor (`a` tag) is used to create hyperlinks in HTML
- The `href` attribute specifies the destination of the link and required for the anchor tag function
- Link can point to external website, local file, or specific locations within the same page
- Anchor element are inline element and do not break flow of content

!!! example "Example of Use `a` Tag"

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Anchor Element</title>
  </head>
  <body>
    <!--href attribute-->
    <a href="https://www.google.com">I am a link to Google</a>
    <!--Linking to local file-->
    <a href="about.html">About Page</a>
    <!--Linking to same page-->
    <a href="#about">About</a>
    <!--Linking to external page / resource-->
    <a href="https://en.wikipedia.org/wiki/Fowl">fowl</a>
  </body>
</html>
```

### Image Element

!!! note "Key Takeaways"

- Embeds image into HTML document
- The `<img>` element is unique in HTML as it does not have a closing tag or content between tags
- The `src` attribute specifies the location of the image, which can be a local file path or an external URL
- The `alt` attribute provides alternative text for accessibility and displays when the images cannot be loaded
- Best practice to control image size using CSS rater than using HTML attribute like `width`

!!! example "Example of Use `img` Tag"

```html
<img src="chicken.jpg" alt="chicken-images" />
```

!!! info "Comments"

Use `<!--` to make comments in HTML document

### HTML Next Step

#### Block and Inline Element

!!! note "Key Takeaways"

- Block element: Take up whole of space. E.g, paragraph, heading element
- Inline element: Can fit in alongside with another element. E.g, anchor element

#### Div and Span

!!! note "Key Takeaways"

- `div`: a generic block-level container used to group element for styling or layout
- `span`: a generic inline-container used to target specific text or content for styling

!!! example "Example of Use `div`"

```html
 <div>
      <section>
      <h2>Nomenclature</h2>
      <p>Terms for chickens include</p>
      <ul>
        <li><i>Biddy:</i> a chicken, or a newly hatched chicken</li>
        <li><i>Capon:</i>a castrated or neutered male chicken</li>
      </ul>
</div>
```

!!! example "Example of Use `span`"

```html
<p>
  Add the <span class="ingredient">basil</span>,
  <span class="ingredient">pine nuts</span> and
  <span class="ingredient">garlic</span> to a blender and blend into a paste.
</p>
```

#### Assortment of Element

!!! note "Key Takeaways"

- `hr`: element creates a horizontal rule or thematic break between content sections
- `br`: element insert line break within content, useful for poem or controlled line breaks
- `sup`: element render text as superscript, commonly used for exponent or citation
- `sub`: element render text as subscript, often used in chemical formula or fractions

!!! example "Example of Use `hr`, `br`, `sup`, `sub` Tag"

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>HTML Semantic</title>
  </head>
  <body>
    <h1>hr element</h1>
    <p id="one">
      Lorem ipsum dolor sit, amet consectetur adipisicing elit. Porro saepe
      necessitatibus nesciunt tenetur obcaecati ab similique, dignissimos
      ducimus quo, dolor hic quidem enim, accusantium repellat ea. Aspernatur ut
      vero accusamus!
    </p>
    <hr />
    <p id="two">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestias
      cupiditate suscipit neque, sunt omnis et sint consequatur distinctio ad
      officia ducimus perspiciatis hic a labore harum iste dicta cumque animi!
    </p>
    <h1>br element</h1>
    <div id="container" class="lyrics">
      Twinkle, twinkle, little star <br />
      How I wonder what you are <br />
      Up above the world so high <br />
      Like a diamond in the sky <br />
      Twinkle, twinkle, little star <br />
      How I wonder what you are <br />
      When the blazing sun is gone <br />
      Then you show your little light <br />
      Twinkle, twinkle, all the night <br />
      Twinkle, twinkle, little star <br />
      How I wonder what you are <br />
    </div>
    <h1>sup element</h1>
    E = MC<sup>2</sup>
    <h1>sub element</h1>
    H <sub>2</sub>O
  </body>
</html>
```

#### Entity Code

!!! note "Key Takeaways"

- Entity code is special code or sequence that can be used in HTML to generate different characters
- Entity code start with ampersand and end with semicolon
- Reference: <https://html.spec.whatwg.org/multipage/named-characters.html>

!!! example "Example of Use Entity Code"

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>HTML Semantic</title>
  </head>
  <body>
    <footer>
      <p>&#169; - MYH 2025</p>
    </footer>
  </body>
</html>
```

### Semantic Elementc

!!! note "Key Takeaway"

- Semantic markup add meaningful context to HTML markup, improving clarity
- Semantic markup enhances accessibility for screen reader and improve SEO by helping crawler understanding page structure
- Using semantic element makes code easier to navigate and maintain for developer
- Semantic element: `<main></main>`, `<header></header>`,`<footer></footer>`,`<nav></nav>`,`<section></section>,<article></article>`

!!! example "Example of Use Semantic Element"

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Section 4</title>
  </head>
  <body>
    <!--header of these document. represent intro of document or navigational aids-->
    <header>
    <!--nav: element used to navigate resource in same page or different resource-->
    <nav>
      <ul>
        <li><a href="chicken.html">Chicken</a></li>
        <li><a href="#nomenclature">Nomenclature</a></li>
      </ul>
    </nav>
    </header>
    <!--main: element used to represent semantic main content of in document or pages-->
    <main>
    <h1>Chicken</h1>
    <img src="chicken.jpg" alt="chicken-images" />
    <p>
      The <b>chicken</b><i><b>(Gallus gallus domesticus)</b></i> is a
      domesticated subspecies of the <a href="">red jungleowl</a> (<i
        >Gallus gallus</i
      >), originally native to
      <a href="https://en.wikipedia.org/wiki/Southeast_Asia">Southeast Asia.</a>
    </p>
    <!--hr is element used to create break between section or paragraph-->
    <hr />
    <div>
      <section>
      <h2>Nomenclature</h2>
      <p>Terms for chickens include</p>
      <ul>
        <li><i>Biddy:</i> a chicken, or a newly hatched chicken</li>
        <li><i>Capon:</i>a castrated or neutered male chicken</li>
      </ul>
    </div>
    <ol>
      <li>
        <!--br is element used for break line, useful for poem or address-->
        Joshua (July 27, 2020). <br /><a href=""></a>"Chickens and
        Roosters....As Pets".
      </li>
      <i>IAABC Foundation Journal.</i>
    </ol>
    <h2>Formula phitagoras adalah:</h2>
    <!--sup: element used for create raised baseline (exponent). Usefull for math or STEM equation-->
    <p>a<sup>2</sup> = b<sup>2</sup> + c <sup>2</sup></p>
    <h2>Chemistry formula for Oxygen is:</h2>
    <!--Sub: element used for create lowered baseline. Useful for chemistry equation-->
    <p>O<sub>2</sub></p>
    </section>
    <!--footer element of this document-->
    <footer>
      <p>&#169; - MYH 2025</p>
    </footer>
  </body>
</main>
</html>
```

### HTML Form and Table

#### HTML Table

#### HTML Form
