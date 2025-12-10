# Cascading Style Sheet (CSS)

Cascading Style Sheets (CSS) is a stylesheet language used to describe the presentation of a document written in HTML. The role of CSS is describe and manipulate visual representation of HTML content.

!!! note "Basic Rules of CSS"

```css
selector {
    properties: value;
}
```

!!! note "Including Style in CSS"

- Inline style (not recommend)

```html
<h1 style="color: purple;">Hello World</h1>
<button style="background-color: palegreen;">I am button</button>
```

- Using &lt;style&gt; tag (not recommend)

```html
<style>
h2 {
  color: palevioletred;
}
</style>
```

- External Style Sheet (Recommend)

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>CSS Intro</title>
    <link rel="stylesheet" href="index-section-6.css" />
  </head>
  <body>
    <h1>Hello World</h1>
    <button>I AM BUTTON</button>
  </body>
</html>
```

!!! note "Styling of CSS Color System"

- Name
  
```css
color: brown;
```  

- RGB Value

```css
color: rgb(255,255,0);
```

- Hexadecimal Value

```css
color: #ffffff;
```

## CSS Properties

### Basic CSS Properties

#### color

!!! note "Key Takeaways"

- Set the foreground color of element text and text decorations

!!! example "Example of use Color Properties"

=== "HTML"

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <link rel="stylesheet" href="style.css" />
        <title>Text Align</title>
    </head>
    <body>
        <h1>Lorem Ipsum</h1>
    </body>
    </html>
    ```

=== "CSS"

    ```css
    h1 {
        color:#ffffff;
        background-color: blue;
        text-align: center;
    }
    ```

#### background-color

!!! note "Key Takeaways"

- Set background color of an element

!!! example "Example of Use background-color Properties"

=== "HTML"

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <link rel="stylesheet" href="style.css" />
        <title>Text Align</title>
    </head>
    <body>
        <h1>Lorem Ipsum</h1>
    </body>
    </html>
    ```

=== "CSS"

    ```css
    h1 {
        color:#ffffff;
        background-color: blue;
        text-align: center;
    }
    ```

#### text-align

!!! note "Key Takeaways"

- Set horizontal aligment of text within element

!!! example "Example of use text-align Properties"

=== "HTML"

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <link rel="stylesheet" href="style.css" />
        <title>Text Align</title>
    </head>
    <body>
        <h1>Lorem Ipsum</h1>
    </body>
    </html>
    ```

=== "CSS"

    ```css
    h1 {
        color:#ffffff;
        background-color: blue;
        text-align: center;
    }
    ```

#### font-weight

!!! note "Key Takeaways"

- Control boldness or lightness of font. The avaliable weight it depends on font type / font family that currently set

!!! example "Example of use font-weight Properties"

=== "HTML"

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <link rel="stylesheet" href="style.css" />
        <title>Text Align</title>
    </head>
    <body>
        <h1>Lorem Ipsum</h1>
        <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero non,
        nostrum reiciendis, cupiditate maxime debitis labore, saepe facilis
        aliquid est quas explicabo ratione nemo possimus odit. Expedita quam autem
        ex! Voluptas dolor, debitis deleniti blanditiis enim magnam, voluptates
        adipisci doloribus soluta illum ipsam maxime qui. Cum modi, eius qui
        sapiente neque dolorem quod, magnam, dignissimos corrupti debitis
        repellat. Error, in. Nobis nesciunt perspiciatis, deserunt libero est,
        itaque explicabo accusamus accusantium officiis voluptate pariatur,
        voluptatibus dolorum architecto voluptatum sequi dignissimos ex error!
        Quos sunt necessitatibus expedita facilis incidunt odit, delectus nam.
        Assumenda, est saepe dolorem, quae pariatur quaerat delectus dolor dolores
        dolore sit et amet expedita rem incidunt aperiam blanditiis illo nobis
        unde temporibus nulla laboriosam dignissimos ad! Sint, pariatur ipsam!
        Dolorum animi praesentium eos ipsam pariatur, eius optio quibusdam
        inventore possimus dolorem nisi eveniet facere aut corrupti enim!
        Perferendis debitis alias sit qui quasi. Accusantium soluta debitis
        dolorem possimus et?
        </p>
    </body>
    </html>
    ```

=== "CSS"

    ```css
    h1 {
        color:#ffffff;
        background-color: blue;
        text-align: center;
    }

    p {
        font-weight: 900;
    }
    ```

#### text-decoration

!!! note "Key Takeaways"

- Adding or removing decorative line on text
- For this properties, they have various value (line, style, color, and thickness)

!!! example "Example of use text-decoration Properties"

=== "HTML"

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <link rel="stylesheet" href="style.css" />
        <title>Text Align</title>
    </head>
    <body>
        <h1>Lorem Ipsum</h1>
    </body>
    </html>
    ```

=== "CSS"

    ```css
    h1 {
        color: #ffffff;
        background-color: blue;
        text-align: justify;
        font-weight: normal;    
        text-decoration: line-through dashed red 3px;
        
    }
    ```

#### line-height

!!! note "Key Takeaways"

- Set the distance between line of text

!!! example "Example of use line-height Properties"

=== "HTML"

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <link rel="stylesheet" href="style.css" />
        <title>Text Align</title>
    </head>
    <body>
        <h1>Lorem Ipsum</h1>
        <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero non,
        nostrum reiciendis, cupiditate maxime debitis labore, saepe facilis
        aliquid est quas explicabo ratione nemo possimus odit. Expedita quam autem
        ex! Voluptas dolor, debitis deleniti blanditiis enim magnam, voluptates
        adipisci doloribus soluta illum ipsam maxime qui. Cum modi, eius qui
        sapiente neque dolorem quod, magnam, dignissimos corrupti debitis
        repellat. Error, in. Nobis nesciunt perspiciatis, deserunt libero est,
        itaque explicabo accusamus accusantium officiis voluptate pariatur,
        voluptatibus dolorum architecto voluptatum sequi dignissimos ex error!
        Quos sunt necessitatibus expedita facilis incidunt odit, delectus nam.
        Assumenda, est saepe dolorem, quae pariatur quaerat delectus dolor dolores
        dolore sit et amet expedita rem incidunt aperiam blanditiis illo nobis
        unde temporibus nulla laboriosam dignissimos ad! Sint, pariatur ipsam!
        Dolorum animi praesentium eos ipsam pariatur, eius optio quibusdam
        inventore possimus dolorem nisi eveniet facere aut corrupti enim!
        Perferendis debitis alias sit qui quasi. Accusantium soluta debitis
        dolorem possimus et?
        </p>
    </body>
    </html>
    ```

=== "CSS"

    ```css
    p {
        font-weight: 900;
        line-height: 32px;
    }
    ```

#### letter-spacing

!!! note "Key Takeaways"

- Set spacing between text characters.
- Positive value cause text characters future aparts, when negative value cause text characters closer together.

!!! example "Example of use letter-spacing Properties"

=== "HTML"

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <link rel="stylesheet" href="style.css" />
        <title>Text Align</title>
    </head>
    <body>
        <h1>Lorem Ipsum</h1>
        <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero non,
        nostrum reiciendis, cupiditate maxime debitis labore, saepe facilis
        aliquid est quas explicabo ratione nemo possimus odit. Expedita quam autem
        ex! Voluptas dolor, debitis deleniti blanditiis enim magnam, voluptates
        adipisci doloribus soluta illum ipsam maxime qui. Cum modi, eius qui
        sapiente neque dolorem quod, magnam, dignissimos corrupti debitis
        repellat. Error, in. Nobis nesciunt perspiciatis, deserunt libero est,
        itaque explicabo accusamus accusantium officiis voluptate pariatur,
        voluptatibus dolorum architecto voluptatum sequi dignissimos ex error!
        Quos sunt necessitatibus expedita facilis incidunt odit, delectus nam.
        Assumenda, est saepe dolorem, quae pariatur quaerat delectus dolor dolores
        dolore sit et amet expedita rem incidunt aperiam blanditiis illo nobis
        unde temporibus nulla laboriosam dignissimos ad! Sint, pariatur ipsam!
        Dolorum animi praesentium eos ipsam pariatur, eius optio quibusdam
        inventore possimus dolorem nisi eveniet facere aut corrupti enim!
        Perferendis debitis alias sit qui quasi. Accusantium soluta debitis
        dolorem possimus et?
        </p>
    </body>
    </html>
    ```

=== "CSS"

    ```css
    p {
        font-weight: 900;
        line-height: 32px;
        letter-spacing: 0.2rem;
    }
    ```

#### font-size

!!! note "Key Takeaways"

- Set size of the font.

!!! example "Example of use font-size Properties"

=== "HTML"

    ```html
        <!DOCTYPE html>
        <html lang="en">
        <head>
            <meta charset="UTF-8" />
            <meta name="viewport" content="width=device-width, initial-scale=1.0" />
            <link rel="stylesheet" href="style.css" />
            <title>Text Align</title>
        </head>
        <body>
            <h1>Lorem Ipsum</h1>
            <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero non,
            nostrum reiciendis, cupiditate maxime debitis labore, saepe facilis
            aliquid est quas explicabo ratione nemo possimus odit. Expedita quam autem
            ex! Voluptas dolor, debitis deleniti blanditiis enim magnam, voluptates
            adipisci doloribus soluta illum ipsam maxime qui. Cum modi, eius qui
            sapiente neque dolorem quod, magnam, dignissimos corrupti debitis
            repellat. Error, in. Nobis nesciunt perspiciatis, deserunt libero est,
            itaque explicabo accusamus accusantium officiis voluptate pariatur,
            voluptatibus dolorum architecto voluptatum sequi dignissimos ex error!
            Quos sunt necessitatibus expedita facilis incidunt odit, delectus nam.
            Assumenda, est saepe dolorem, quae pariatur quaerat delectus dolor dolores
            dolore sit et amet expedita rem incidunt aperiam blanditiis illo nobis
            unde temporibus nulla laboriosam dignissimos ad! Sint, pariatur ipsam!
            Dolorum animi praesentium eos ipsam pariatur, eius optio quibusdam
            inventore possimus dolorem nisi eveniet facere aut corrupti enim!
            Perferendis debitis alias sit qui quasi. Accusantium soluta debitis
            dolorem possimus et?
            </p>
        </body>
        </html>
    ```

=== "CSS"

    ```css
        p {
            font-weight: 900;
            line-height: 32px;
            letter-spacing: 0.2rem;
            font-size: 50px;
            
        }
    ```

#### font-family

!!! note "Key Takeaways"

- Change font type of selected element in CSS
- You can set many type of font in this properties (as a backup, if the font that selected does not installed in user device)
- The font family that worked it depends on user installed font in there device, maybe this font is work in device user A, but not in device  user B.

!!! example "Example of use font-family Properties"

=== "HTML"

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <link rel="stylesheet" href="style.css" />
        <title>Text Align</title>
    </head>
    <body>
        <h1>Lorem Ipsum</h1>
        <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero non,
        nostrum reiciendis, cupiditate maxime debitis labore, saepe facilis
        aliquid est quas explicabo ratione nemo possimus odit. Expedita quam autem
        ex! Voluptas dolor, debitis deleniti blanditiis enim magnam, voluptates
        adipisci doloribus soluta illum ipsam maxime qui. Cum modi, eius qui
        sapiente neque dolorem quod, magnam, dignissimos corrupti debitis
        repellat. Error, in. Nobis nesciunt perspiciatis, deserunt libero est,
        itaque explicabo accusamus accusantium officiis voluptate pariatur,
        voluptatibus dolorum architecto voluptatum sequi dignissimos ex error!
        Quos sunt necessitatibus expedita facilis incidunt odit, delectus nam.
        Assumenda, est saepe dolorem, quae pariatur quaerat delectus dolor dolores
        dolore sit et amet expedita rem incidunt aperiam blanditiis illo nobis
        unde temporibus nulla laboriosam dignissimos ad! Sint, pariatur ipsam!
        Dolorum animi praesentium eos ipsam pariatur, eius optio quibusdam
        inventore possimus dolorem nisi eveniet facere aut corrupti enim!
        Perferendis debitis alias sit qui quasi. Accusantium soluta debitis
        dolorem possimus et?
        </p>
    </body>
    </html>
    ```

=== "CSS"

    ```css
        p {
            font-weight: 900;
            line-height: 32px;
            letter-spacing: 0.2rem;
            font-size: 50px;
            font-family: Arial;
            
        }
    ```

## CSS Selector

### Universal and Element Selector

!!! note "Key Takeaways"

- Select everything selector
- This method is rarely used, because inefficiency

!!! example "Example of use Universal Selector"

```css
* {
    color: red;
    background-color: green;
}
```

!!! note "Key Takeaways"

- Based on selector element of a given type

!!! example "Example of use Element Selector"

```css
a {
    text-decoration: none;
}
```

!!! note "Key Takeaways"

- Combine multiple / various selector element
- Don't forget to use comma ( , )

!!! example "Example of use Selector List"

```css
h1, button {
    color: green;
}
```

### ID Selector

!!! note "Key Takeways"

- Unique identifier an element
- Can be used in label to associate with input for accesibility
- Also can be use to hook CSS for style single, specific element differently from other
- Use this symbol `#` to style specific id in tag element
  
!!! info "id Selector Syntax"

```css
#id_selector_name {
    properties: value;
}
```

!!! example "Example of use ID Selector"

=== "HTML"

```html

```

=== "CSS"

```css
button {
    color: blue;
    background-color: white;
}

/* in this section, I just wanna to see the different between using id and without using id */

#login {
    color:black;
    background: white;
}
```

### Class Selector

!!! info "Key Takeaways"

- Grouping multiple element to allows for shared styling
- Unlike ID Selector, Class can be used in multiple element of any type
- Class provide flexibility for styling tag element
- Use this symbol `.` to styling specific class in tag element

!!! info "Class Selector Syntax"

```css
.class_name {
    properties: value;
}
```

!!! example "Example of use Class Selector"

=== "HTML"

```html
    
```

=== "CSS"

```css
.posted {
    color: red;
}

.username a {
    text-decoration-line: none;
    font-weight: bold;
}
```

### Descendant Selector

!!! note "Key Takeaways"

- Select all element that nested inside an element
- Nested inside another element
- Combining class selectors with descendant selectors allows for more specific styling without adding classes to every element.
- Descendant selectors apply styles to elements nested at any depth within the ancestor element.

!!! example "Example of Use Descendant Selector"

=== "HTML"

```html
    
```

=== "CSS"

```css
header a {
    text-decoration-color: blue;
    color: black;
    text-decoration: none;
    }
```

- It's mean select all achor tag that are nested inside header

```css
#image-container img {
    border-radius: 25px;
    -webkit-border-radius: 25px;
    -moz-border-radius: 25px;
    -ms-border-radius: 25px;
    -o-border-radius: 25px;
}
```

- It's mean select all image tag that are nested inside image-container id

### Adjacent Selector

!!! note "Key Takeaways"

- Select only the element that are immediately preceded by an element
- The adjacent selector (+) selects elements immediately following a specified element on the same level.

!!! example "Example of Use Adjacent Selector"

```css
input + button {
  background-color: blue;
  color: white;
}

```

- It's mean select only the button that are immediately pereced by input element

### Direct Descendant Selector

- Select only the element tag that are direct children of a element tag
- The direct child selector (>) targets elements that are direct children of a specified parent element.

!!! example "Use of Direct Descendant Selector"

```css
header > a {
    text-decoration-line: none;

}
```

- It's mean select only achor tag that are direct children of a header

### Attribute Selector

!!! note "Key Takeaways"

- Attribute selector allows selection of element based on specific attribute, such as type or href
- Attribute selector use square brackets with syntax like `[attribute=value]`
- Commonly used in input element or achor tag

!!! info "Attribute Selector Syntax"

```css
element_tag[attribute=value]
```

!!! example "Example of Use of Attribute Selector"

```css
input[type=password] {
    color:red;
}
```

### Pseudo Class

!!! note "Key Takeaways"

- Keyword added to a selector that specifies a special state of the selected elements
- Commonly used pseudo-class is `:hover`, `:active`, `:nth-of-type`
  
#### :hover

!!! info "Definition"

- CSS pseudo-class element that matches an element when user interact with it using pointing device

!!! example "Example of Use `:hover` Pseudo Class"

```css
a:hover {
    color: orange;
}
```

#### :active

!!! info "Definition"

- CSS pseudo-class represent an element (such a button) that is being activated by user. "activation" typically starts when the user presses down the primary mouse button
- Commonly used in achor tag or button element tag
- Use this symbol for pseudo class `:`

!!! example "Example of Use `:active` Pseudo Class"

```css
button:active {
    box-shadow: 2px 2px 5px #fc894d;
}
```

#### :nth-of-type

!!! note "Definition"

- CSS pseudo-class matches elements based on their position among siblings of the same type (tag name), counting from the end.

!!! example "Example of Use `:nth-of-type`"

```css
.square:nth-of-type(2n) {
    background-color: black;
}
```

```css
.square:nth-of-type(2n+1) {
    background-color: red;
}
```

### Pseudo Element

!!! note "Key Takeaways"

- Keyword added to a selector that let's you style a particular part of selected element. Common Pseudo element, `::after`, `::before`, ``::first-letter`,`::first-line`,`::selection`
- Use this symbol `::` for pseudo element

#### ::first-letter

!!! info "Definition"

- Applies styles to the first letter of the first line of a block container

!!! example "Example of Use `::first-letter` Pseudo Element"

```css
p::first-letter {
    font-size: 1.5rem;
    font-weight: bold;
    color: black;
}
```

#### ::first-line

!!! info "Definition"

- Applies styles to the first line of a block container.

!!! example "Example of `::first-line` Pseudo Element"

```css
p::first-line {
    font-size: 1.5rem;
    font-weight: bold;
    color: black;
}
```

#### ::selection

!!! info "Definition"

- Applies styles to the part of a document that has been highlighted by the user (such as clicking and dragging the mouse across text).

!!! example "Example of `::selection` Pseudo Element"

```css
p::selection {
    color: blue;
    background-color: green;
}
```

### Cascade

!!! note "Key Takeaways"

- The order your styles are declared in and linked to matters

### Specificity

!!! note "Key Takeaways"

- Specificity is how browser decides which rules to apply when multiples rules could be apply to same element.
- In short, which rules apply when there is conflict when different style is applied to same element.
- It is measure of how specific a given selector is. The more specific selector wins
- Rules order : ID > Class > Element
- Specificity calculator: <https://specificity.keegan.st/>  

### Inline Style and Important

!!! note "Key Takeaways"

- Inline style are more specific than ID and Class and Element selector
- The keyword `!important` is declaration to force style to win regardless of normal specificity rules and should be used sparingly
- Not recommended using this approach

!!! example "Example of Inline Style"

```html
<button style="color: red">Login</button>
```

!!! example "Example of Use `!important` Keywords"

```css
button {
    background-color:red !important;
}
```

### CSS Inheritance

!!! note "Key Takeaways"

- CSS inheritance allows child elements to inherit certain properties from their parents if not explicitly set.
- Not all CSS properties are inheritable. Make sure to check MDN Docs
- Use `inherit` keyword to force inheritance properties that do not inherit by default

!!! example "Example of CSS Inheritance"

=== "HTML"

    ```html
    <!DOCTYPE html>
    <html lang="en">

    <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="style.css" />
    <title>Document</title>
    </head>

    <body>

    <body>
        <h1>Example of CSS Inheritance</h1>
        <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugit velit
        exercitationem, incidunt nesciunt iusto minus quae quisquam pariatur
        nemo similique aut commodi magni, sint modi, voluptates culpa labore
        vitae nam!
        </p>
        <form action="">
        <p>
            <label for="">Text</label>
            <input type="text" name="text" id="text-opton">
            <button type="submit">Submit</button>
            </p>
        </p>
        </form>
    </body>
    </body>

    </html>
    ```

=== "CSS"

    ```css
    body {
        color: purple;
    }

    form {
        color: green;
    }

    button {
        color:inherit
    }
    ```

## CSS Box Model

![CSS-Box-Model](../asset/css_box_model.png)

!!! note "Key Takeaways"

- Everything in CSS is box.
- Each box have different properties (content, border, padding, margin)

### CSS Box Model : Width & Height

!!! note "Key Takeaways"

- Width and height properties is used to control the box size of content area of an element
- Setting width and height explicitly restricts the size of the content box
- Background color only apply to the content area, unless othewise styled

!!! example "CSS Box Model : Width & Height"

=== "HTML"

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>CSS Box Model - Width and Height</title>
        <link rel="stylesheet" href="style.css" />
    </head>
    <body>
        <div>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Atque eius
        aliquam tempore dolor autem ipsam earum ipsum rerum impedit? Harum
        voluptates nihil repudiandae voluptatum unde voluptatem veniam dolore
        reprehenderit vitae? Commodi repellat cupiditate nesciunt reprehenderit
        autem consectetur distinctio, consequatur, mollitia voluptatibus
        asperiores quaerat sint adipisci obcaecati similique alias totam nulla
        corporis laudantium fugiat dolorum eos. Sint repellendus sit nihil
        consequatur.
        </div>
        <div>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Hic blanditiis ab
        alias sit delectus aperiam omnis quis assumenda, repellat nesciunt
        voluptatum voluptatibus cum in, facilis nemo. Minus qui tempora
        cupiditate. Sit voluptas dolorem vitae, sunt odit nam obcaecati. Nisi in
        magni adipisci ea neque molestiae ullam reprehenderit eaque esse ratione
        explicabo a quia impedit perspiciatis, laboriosam porro libero deserunt
        deleniti.
        </div>
        <div>
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Officiis
        accusamus illum non ipsam! Fugiat, nemo voluptatum? Exercitationem est, ab
        nemo architecto placeat necessitatibus, quis, soluta optio doloremque
        officiis sit vel! Temporibus pariatur dolor quasi excepturi esse,
        provident itaque adipisci eos voluptatem vel quidem asperiores nihil totam
        consequuntur aspernatur odit deserunt mollitia sint reprehenderit nam
        nemo. Voluptatem soluta est fugit suscipit.
        </div>
    </body>
    </html>
    ```

=== "CSS"

    ```css
    div {
        width: 300px;
        height: 300px;
        background-color: aqua;
    }
    ```

### CSS Box Model : Border and Border Radius

!!! note "Key Takeaways"

- Set border / visible outline around an element
- `border-width`: Set a thicknes of the border an element
- `border-color`: Set a color of the border an element
- `border-style`: Set a style of the border line an element, such as dotted, solid, dashed
- `border-radius`: Enable to rounds the corner of border an element

!!! example "Example of `border-width`, `border-color`, `border-style` and `border-radius` Properties"

=== "HTML"

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <title>CSS : Border</title>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1" />
        <link rel="stylesheet" href="style.css" />
    </head>
    <body>
        <h1>Lorem Ipsum Text</h1>
        <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis
        ducimus libero, corrupti fugit id beatae quae harum nam voluptatem et
        aliquid! Libero quod non veniam eos rem ut ipsam? Praesentium?
        </p>
    </body>
    </html>
    ```

=== "CSS"

    ```css
        h1 {
            border-width: 3px;
            border-style:solid;
            border-color: blue;
        }

        p {
            border-radius: 5px;
            -webkit-border-radius: 5px;
            -moz-border-radius: 5px;
            -ms-border-radius: 5px;
            -o-border-radius: 5px;
            border-style: solid;
            background-color: green;
            font-weight: bold;
            border-color:brown;
        }

    ```

### CSS Box Model : Padding

!!! note "Key Takeaways"

- Padding is the space between an element's content area and its border, providing internal spacing.
- Padding can be set individually for top, right, bottom, and left, or all at once using the shorthand `padding` property.
- The shorthand padding property accepts one to four values, applying them in specific orders: one value for all sides, two values for vertical and horizontal, three values for top, horizontal, and bottom, and four values for top, right, bottom, and left.
- Padding uses various units such as pixels, ems, rems, and percentages, affecting the size of the spacing accordingly.

!!! example "Example of `padding` Properties"

=== "HTML"

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>CSS Pading</title>
        <link rel="stylesheet" href="style.css" />
    </head>
    <body>
        <h1>Hello World</h1>
        <p>
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quos, hic
        sapiente. Officia nam et labore dolorem voluptates magnam iste similique
        libero obcaecati veniam. Sequi voluptatum iusto maxime voluptatibus,
        possimus quaerat! Veniam, placeat ratione tempore maxime blanditiis
        suscipit incidunt repellat porro possimus excepturi, neque laboriosam,
        voluptate vel. Ea nisi vero rerum veritatis voluptas officiis nulla
        architecto suscipit neque officia, a quae. Dolorem eveniet repudiandae
        commodi ducimus voluptates nulla harum similique quaerat voluptatem ab
        perspiciatis doloribus cupiditate voluptatum soluta assumenda ipsam
        cumque, dignissimos id excepturi atque unde iure pariatur! Consequatur,
        quibusdam nobis?
        </p>
    </body>
    </html>
    ```

=== "CSS"

    ```css
    h1 {
        border-width: 5px;
        border-style: dashed;
        border-color: blue;
        padding: 5px;

        /* padding: top, right, bottom, left */
    }
    ```

### CSS Box Model : Margin

!!! note "Key Takeaways"

- Margin is the space outside an element's border, separating it from other elements.
- The margin property can be set individually for top, right, bottom, and left, or using shorthand syntax.
- The shorthand `margin` property accepts one to four values, applying them in specific orders: one value for all sides, two values for vertical and horizontal, three values for top, horizontal, and bottom, and four values for top, right, bottom, and left.
- Margin affects horizontal and vertical spacing, but vertical margin on inline elements may require understanding the display property.
- Default margins exist on some elements like headings and the body, which can be reset to zero.

!!! example "Example of `margin` Properties"

=== "HTML"

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <title>Tes</title>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1" />
        <link href="style.css" rel="stylesheet" />
    </head>
    <body>
        <div id="container">
        <h1>Lorem Ipsum</h1>
        </div>
        <div id="container-1">
        <h1>Lorem Ipsum</h1>
        </div>
    </body>
    </html>
    ```

=== "CSS"

    ```css
    div#container {
        width: 100px;
        height: 100px;
        border-style: dotted;
        border-width: 2px;
        border-color: red;
        margin:5px;
    }

    div#container-1 {
        width: 100px;
        height: 100px;
        border-style:dashed;
        border-width: 2px;
        border-color: green;
        margin:15px;
    }
    ```

### Display Property

!!! note "Key Takeaways"

- The display property in CSS determines how elements are rendered: inline, block, or inline-block.
- `display:inline`: width and height are ignored. margin & padding push elements away horizontally but not vertically
- `display:block`: block elements breaks the flow of a document. width & height, margin, padding, are respected
- `display:inline-block`: behaved like an inline element except width, height, margin, padding are respected
- The display property can also be set to none to hide elements from the page layout

| Display Type   | Width & Height                     | Margin                                | Padding                               | Description                                                                 |
|----------------|------------------------------------|----------------------------------------|----------------------------------------|------------------------------------------------------------------------------|
| `inline`       | **Ignored** — cannot be adjusted   | **Horizontal applies**, vertical ignored | **Horizontal applies**, vertical ignored | Element stays on the same line and does not affect the full line height.    |
| `block`        | **Respected** — can be freely adjusted | **All sides apply**                   | **All sides apply**                   | Element takes up the full line (starts on a new line).                      |
| `inline-block` | **Respected** — can be freely adjusted | **All sides apply**                   | **All sides apply**                   | Behaves like `inline`, but supports size and spacing adjustments.           |

!!! example "Example of `display` Properties"

=== "HTML"

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <link rel="stylesheet" href="style.css" />
        <title>CSS - Display Properties</title>
    </head>
    <body>

        <div></div>
        <div></div>
        <div></div>


        <h1>I am h1</h1>
        <h1>I am also h1</h1>
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quis quam
        voluptates doloremque ad neque, enim repellat fugiat sint voluptate harum
        eaque aliquam eos itaque veniam odio obcaecati dicta autem quidem.
        Voluptatibus dolorem, repudiandae deleniti quo numquam molestiae culpa ipsa
        similique dolores, accusantium quisquam nemo. Aperiam repellendus cum hic
        modi ea? Quae illum fuga sed molestiae tempora doloribus atque vel! Eius. Id
        ex corrupti temporibus itaque, vero eos libero ducimus dicta, quos
        aspernatur minus, non hic quibusdam beatae ad et amet eligendi velit
        consectetur iure? Ipsam alias ullam debitis ratione laboriosam. Cum ad
        aliquid, fugit tenetur pariatur debitis illum sed? Nemo fuga magnam,
        asperiores animi laudantium dolore consectetur perspiciatis cupiditate
        delectus debitis dolorum praesentium ratione minima autem, nulla magni ipsa
        excepturi? Harum nesciunt eius minima quasi. Sunt consequatur veniam vel
        beatae numquam totam? Atque doloremque eveniet in minus voluptatibus, dolore
        quidem porro non error magni accusantium, dolorem quas! Harum, eligendi ut.
        <span>I AM A SPAN</span>
        Nobis soluta nostrum dicta quia perspiciatis tempora modi alias. Modi
        perspiciatis nesciunt neque ipsum facere corrupti ipsam officia qui
        recusandae dolorem amet, sequi beatae, rem, nihil ex voluptatem architecto
        hic! Incidunt iusto praesentium, ipsam doloribus eum voluptatibus eligendi
        laudantium fugit eos dicta excepturi saepe magni ut, ad ducimus? Enim
        pariatur, sed ipsum inventore repudiandae harum dolores tenetur repellat!
        Id, commodi. Atque tempora voluptas doloribus quod ea libero placeat. Eum
        dicta quo dolores quidem deserunt sint explicabo ab sed nobis dolore, quasi
        tenetur vitae unde sit exercitationem culpa! Qui, fuga ullam. Cum, doloribus
        blanditiis. Voluptates, ducimus facilis! Iusto consequuntur nam incidunt eum
        laudantium numquam natus impedit reprehenderit id suscipit dolore eveniet
        deleniti distinctio praesentium, maxime dolores, autem quidem doloribus,
        doloremque laborum! Consequuntur temporibus ipsum ipsam ut mollitia
        praesentium voluptate fugiat eius quae et asperiores, libero necessitatibus
        atque culpa. Iusto itaque alias maxime amet expedita odit, necessitatibus
        laborum vero impedit, nobis sapiente!
    </body>
    </html>
    ```

=== "CSS"

    ```css
    span {
        background-color: palegreen;
        border: 1px solid black;
        width: 500px;
        height: 500px;
        padding:50px;
        margin:50px;
    }


    h1 {
        background-color: palevioletred;
        border: 1px solid black;
        width: 300px;
        height: 200px;
        padding:50px;
        margin:50px;
    }

    div {
        height:200 px;
        width:200px;
        background-color:green;
        border: 5px solid black;
        display: inline-block;
        padding: 20px;
        margin: 20px;
    }
    ```

### CSS Units

#### Percentage (%)

!!! note "Key Takeaways"

- CSS absolute units: pixels (px)
- CSS relative units: percentage (%), em, rem
- Percentage in CSS units is relative value. The value is relative from parents elements. But also it can depends on specific CSS property

!!! example "Example of `%` CSS Units"

=== "HTML"

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <link rel="stylesheet" href="style.css" />
        <title>CSS Units</title>
    </head>
    <body>
        <section>
        <div></div>
        </section>
    </body>
    </html>
    ```

=== "CSS"

    ```css
    section {
        background-color:darkgray;
        width: 500px;
        height: 500px;
    }

    div {
        background-color: red;
        width:50%;
        height:50%;
    }

    h2 {
        font-size: 2em;
    }

    section {
        font-size: 10px;
    }
    ```

#### em

!!! note "Key Takeaways"

- `em` units are relative units in CSS based on font sizes in parent elements, with their value depending on the context.
- If the `font-size` is `12px` then `2em` is equal to `24px`
- For properties like margin and padding, 1em equals the font size of the element itself.
- Using `em` units allows elements like buttons to scale proportionally with font size changes, maintaining consistent shapes and spacing.
  
!!! example "Example of Use `em` CSS Unit"

=== "HTML"

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <link rel="stylesheet" href="style.css" />
        <title>CSS Units</title>
    </head>
    <body>
        <button>Click Me</button>
        <article>
        <button>Click Me</button>
        <h2>I am h2</h2>
        <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Natus
            blanditiis odio vitae suscipit, eius, quos assumenda ducimus aliquid
            impedit debitis nisi dolores vero quam adipisci fuga cum consequatur a
            fugit. Qui rem ipsam unde necessitatibus, obcaecati quibusdam, at iste
            officia consequuntur ab distinctio exercitationem voluptates perferendis
            nemo totam ea, non aliquam! Iste suscipit maiores odit omnis tenetur
            culpa! Tenetur, similique.
        </p>
        </article>
    </body>
    </html>
    ```

=== "CSS"

    ```css

    h2 {
        font-size: 2em;
    }

    article {
        font-size: 20px;
    }

    button {
    font-size: 1em;
    padding: 0 1em;
    border-radius:0.5em;
    background-color: #3498db;
    color: white;
    -webkit-border-radius:0.5em;
    -moz-border-radius:0.5em;
    -ms-border-radius:0.5em;
    -o-border-radius:0.5em;
    }
    ```

#### rem

!!! note "Key Takeaways"

- Rems are relative to the root html element's font size, providing consistent sizing throughout the document
- If the root `font-size` is `20px`, 1 rem always `20px`, 2 rem always `40px`,etc.
- Using rems avoids the compounding scaling issue seen with ems in nested elements.
- Mixing ems and rems can be useful for components that need to scale based on their own font size while maintaining overall document consistency.

!!! example "Example of `rem` CSS Unit"

=== "HTML"

    ```html
    <!DOCTYPE html>
    <!--HTML root elements-->
    <html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <link rel="stylesheet" href="style.css" />
        <title>CSS Units</title>
    </head>
    <body>
        <h1>Lorem Ipsum</h1>
        <article id="rems">
        <h2>Using rems instead of ems</h2>
        <h3>I am h3</h3>
        <button>Click Me</button>
        <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Enim modi
            dolores provident eos, recusandae consequatur laboriosam, ut beatae
            molestias autem minus distinctio error, quisquam maxime vero officiis
            architecto! Amet, doloremque!
        </p>
        <ul>
            <li>Pasta</li>
            <ul>
            <li>Ravioli</li>
            <ul>
                <li>Spinach Ricotta</li>
            </ul>
            <li>Penne</li>
            </ul>
            <li>Salad</li>
            <li>Gelato</li>
        </ul>
        </article>
    </body>
    </html>
    ```

=== "CCS"

    ```css
    html {
        font-size: 10px;
    }

    #rems h2 {
        font-size: 3rem;
    }

    #rems h3 {
        font-size: 2rem;
    }

    #rems ul {
        font-size: 0.8rem;
    }

    #rems button {
        font-size: 1.5rem;
    }
    ```

### Assorted CSS Properties

- **Skip from now and bootstrap too. Right now, I am going to learn CSS Responsive, and then go to Javascript**

### Responsive CSS & Flexbox

#### Flexbox

!!! note "Key Takeaways"

- Flexbox is one-dimentional layout method for laying out item in row or coloumn.
- It allows us to distribute space dynamically across elements
- `display:flex` make element to become `flex` or active `flexbox` on container
- Flexbox model:  
  ![alt text](Untitled.png)

- `flex-direction:__;`: control directon of main axis
    - `row`: default. order stack horizontally
    - `row-reverse`: row direction. left-right to right-left
    - `coloumn`: change coloumn. top-bottom. order stack vertically
    - `coloumn-reverse`: coloumn. bottom-top

- `justify-content__:`: control the distribution of content along the main axis in a flex container. it depends on `flex-direction` properties and set of main axis of flex container
    - `flex-start`: default;
    - `flex-end`: go to end of main axis
    - `center`: center along main axis
    - `space-between`: distributed space between an element
    - `space-around`: give same amount of space between an element
    - `space-evenly`: space is even between an element

- `flex-warp__`: Set flex item are forced onto one line or wrap onto multiple line
    - `nowarp`: default
    - `warp`: warp onto multiple line
    - `warp-reverse`: warp onto multiple line and reverse order stack

- `align-items__`: property distributes items along the cross axis, which varies depending on the flex direction
    - `center`: center between cross axis
    - `flex-start`: top-bottom (default)
    - `flex-end`: bottom-top
    - `baseline`: row along their text's baseline

- `align-content__`: property to control or distribute space along cross axis, but only when there are multiple rows and coloumns. This depends on whether the layout is row-based or column-based (`flex-direction` properties)
    - `space-between`
    - `flex-start`
    - `flex-end`
    - `space-around`
    - `center`

- `align-self__`: property to control or distribute space along cross axis, but only when there are multiple rows and coloumns, This depends on whether the layout is row-based or column-based (`flex-direction` properties). But, this properties is only applies to individual flex items / elements
    - `flex-start`
    - `flex-end`
    - `auto`
    - `center`

- `flex-basis`: defines initial size of an element before additional space distributed
- `flex-grow`: control amount of avaliable space an element should take up. accept a unit-less number value
- `flex-shrink`: if items are larger than the container, they shrink according to flex-shrink
- `flex`: shorthand properties for `flex-grow` | `flex-shrink` | `flex-basis`

=== "HTML"

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <link rel="stylesheet" href="style.css" />
        <title>CSS Responsive and Flexbox</title>
    </head>
    <body>
        <h1>Let's Plat with Flexbox</h1>
        <section id="container">
        <div style="background-color: #80ffdb"></div>
        <div style="background-color: #64dfdf"></div>
        <div style="background-color: #48bfe3"></div>
        <div style="background-color: #5390d9"></div>
        <div style="background-color: #6930c3"></div>
        </section>

        <h2>Another Example</h2>
        <main>
        <section class="sidebar"></section>
        <section class="maincontent"></section>
        <section class="sidebar"></section>
        </main>
    </body>
    </html>
    ```

=== "CSS"

    ```css
    @import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300..800;1,300..800&display=swap');

    body {
        font-family: 'Open-Sans', sans-serif;
    }

    h1 {
        text-align: center;
    }

    h2 {
        text-align: center;
    }
    #container {
        background-color: #003049;
        width: 90%;
        /* height: 500px; */
        margin: 0 auto;
        border: 5px solid #003049;
        display: flex;
        flex-direction: wrap;
        justify-content: center;
        /* flex-wrap: wrap; */
            
            
    }

    #container div {
        width: 200px;
        height: 200px;
        text-align: center;
        flex-basis: 600px;
        /* flex-grow: 1; */
            
    }

    div:nth-of-type(3) {
    /* align-self: flex-end; */
        flex-grow: 1;
        flex-shrink: 5;
    } 


    div:nth-of-type(5) {
        flex-grow: 2;
    }

    main {
        width: 80%;
        margin: 0 auto;
        border: 5px solid black;
        height: 500px;
        display: flex;
    }

    main .sidebar {
        background-color: #6930c3;
        flex: 1 2 300px;
    }

    main .maincontent {
        background-color: #80ffdb;
        flex: 2 1 600px;
    }
    ```

#### Media Queries

!!! note "Key Takeaways"

- Media Queries : Allows us to modify our style depending on particular parameter like device type or  or device orientation or screen width

### Responsive Web Design 101
### Bootstrap (Framework)

- **Skip from now**
