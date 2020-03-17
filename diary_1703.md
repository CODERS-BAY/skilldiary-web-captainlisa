# Diary 17.03.2020

## Web 

* create gradients with ```background-image: linear-gradient(direction, color1, color2)```
* direction can be: to bottom (default),  to top, to right, to left, to right bottom (diagonal)
* with ```box-sizing: border-box;``` the height and width of an element includes the padding and the border, unlike the original box model. bootstrap uses this as well. (original would be content-box)
* best practice: 
```css
html {
    box-sizing: border-box;
}
*, *:before, *:after {
    box-sizing: inherit;
}
```
* you can avoid collapsing margins by using this CSS rule: 
```css
h1, h2, h3, h4, h5, h6, p, ul, ol, blockquote {
    margin-top: 0;
    margin-bottom: 1em;
}
```
* sometimes there are elements that you want to hide/are not necessary on your website, but are very necessary for screenreaders/accessibilty. with ```display: none;``` you hide an element completely, so not even screenreaders know that it's there. there are some ways to hide elements (like headlines) in a way that they are invisible on the screen, but are still available for a screenreader
```css
.visually-hidden {
    position: absolute;
    width: 1px;
    height: 1px;
    padding: 0;
    border: 0;
    margin: -1px;
    clip: rect (0 0 0 0);
    overflow: hidden;
    white-space: nowrap;
}