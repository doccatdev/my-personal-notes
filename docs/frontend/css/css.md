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

#### background-color

!!! note "Key Takeaways"

#### text-align

!!! note "Key Takeaways"

- Set horizontal aligment of text within element

```css
h1 {
    color: #ffffff;
    background-color: blue;
    text-align: justify;
  
}
```

#### font-weight

!!! note "Key Takeaways"

- Control boldness or lightness of font. The avaliable weight it depends on font type / font family that currently set

```css
p {
    font-weight: 900;
}
```

#### text-decoration

!!! note "Key Takeaways"

- Adding or removing decorative line on text
- For this properties, they have various value (line, style, color, and thickness)

```css
h1 {
    color: #ffffff;
    background-color: blue;
    text-align: justify;
    font-weight: normal;    
    text-decoration: line-through dashed red 3px;
    
}
```

#### line height

!!! note "Key Takeaways"

- Set the distance between line of text

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

```css
p {
    font-weight: 900;
    line-height: 32px;
    letter-spacing: 0.2rem;
    font-size: 50px;
    font-family: Arial;
}
```

## CSS Box Model
