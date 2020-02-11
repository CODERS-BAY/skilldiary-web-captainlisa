## Skilldiary 7.2.2020

### CSS Stylesheet
* with 
```<link href="stylesheet.css" rel="stylesheet"/>``` 
you can import a stylesheet <br>
* \# means in the stylesheet tells you that something is an id<br>
* . in the stylesheet tells you that something is a class<br>
* List of CSS tags:
  * color
  * background-color
  * background-image
  * background-size: **cover** cuts the image to the size of the window and **contain** shows picture in full with white borders
  * background-repeat
  * height
  * width
  * background-attachment
  * font-size
  * font-style
  * font-family
  * @font-face
  * font-weight (changes text to bold, etc.; same does  ```<strong></strong>``` and ```<b></b>```)
  * text-transform (changes fonts to uppercase, lowercase, capitalize)
  * font-variant (e,g, small caps, annotation,)
  * textfield-decoration (underline, overline, line-through)
  * text-indent
  * text-align (right, left, center, justify (blocksatz))

### html
* ```<br>``` is a break
*  ```<span>...</span>``` & ```<div>...</div>``` have no semantic meaning
*  span is for inline elements; div is for block elements geht über die gesamte zeile = zeilenumbruch
* block elements = headline, paragraph,
* inline element = image, span, links

### Classes in CSS

* classes belong in the **opening tag**! 
```
<p class="classname">...</P>
```

* Here is a list of examples what classes can look like:
```
.img-size {
    width: 100%;
}
```
 
```
.bg-img {
    background-image: url(...);
    background-repeat; no-repeat;
    background-attachment: fixed;
    background-size: cover;
    background-position: center;
}
```
```
.bg-light {
    background-color: rgba(255,255,255,.75);
}
```
```
.m-a {
    margin: 20px;
}
```
```
.p-a {
    padding: 20px;
}
```
```
body{
    font-family: 'Raleway', sans-serif
}
```
```
.title {
    font-family: 'Sacramento', 'cursive'
    font-size: 3em;
    color: #fff;
}
```
```
span {
    color: red;
}
```

### Miscellaneous

* **Always** open the "examine element" function in the browser.

* all parts of a website with the box model
* there is a margin, a border, a padding and it shows you how big the actual element is
* @font-face: font implementieren mit link oder mit fontface
* if you reuse a font it's smart to put them into the head
* google fonts for getting fonts there you get the link to embed/import the font or the code you need to put it in the css file


