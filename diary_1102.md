## Diary 11.02.2020

### About Lists and Tables
* ```<ol> <ul>``` = ordered, unordered lists
* ```<li>``` = list item
* ordered lists can be with numbers, roman numerals, letters; you caan also start with e.g. 9 & be reversed
* undordered lists can also contain special icons with ```list-style-icon```
* definition lists: dl = defined list, dt = defines term, dd = describes terms
* tables starts with head, caption (title of table), thead, tr (=table row),  th (title of row), td (table data), table foot 
* not all CSS rules can be used for all elements.
* pseudo classes, ```a:visited {color: #000;}``` or ```a:hover {color: #777;}``` for links
* ```:nth-child()``` is used to create a striped pattern on a table for example to make it easier to distinguish between lines
* ```colspan``` and ```rowspan``` 

### About Forms
* allows interaction with a user, e.g. login, registration, 
  ```<form action="forms/hallowelt.php" method="post" accept-charset="utf-8">``` 
  
* there are different forms of input a form can get, e.g. text and password. You can also set a maximum length for it.
* php = on the server side
* add buttons with: ```<button type="submit">Send</button>```. There are reset buttons, submit buttons and buttons that need further definiton. 
* placeholder grey text that describes what to do with the field. are not standardized, different code for different websites 
* get- & post- Request: get is visible for the user in the url, post is not. both send data to the server
* radiobuttons are used for example when chosing a gender, if married. with ```checked``` you mark the box that is checked on default. can also anonymous = without id. 
* labels are connected with an id through the ```for```-attribute
* You should always connect labels with the element they belong to. that way, these two are intertwined and it makes it easier for people with disabilities (with a screenreader, for example) to understand the structure of a website
* checkbox basically the same. The difference between radiobuttons and checkboxes is that with radiobuttons you can only choose one, with checkboxes, there are more than one choices possible.
* for short: radiobuttons: single-choice; checkboxes: multiple-choice
* select-box: have different values. there is a single-choice and a multiple-choice. can be styled with CSS
* hidden input elements are used to send technical information to the server, which the user does not need to put in.
* textareas are used for comments or the like. has a defined size on the screen:
```<textarea name="kommentar" cols="50" rows="5">Wert des Textfeldes</textarea>```

### Boxmodel
* inline elements are treated as text: a, b, span, img, label
* block elements use up the whole space (of the container they're in). h1, p, ul,
* ```<span>``` is a contianer for inline elements 
* ```<div>``` is a container for box elements
* inline-block-elements can be created with CSS, by usin ```p {display: block;}```
* with ```p {display: inline-block;}``` you can display two boxes next to each other (if there is enough space)
* negative margin and negative padding does exist. makes sense for collages, etc. 
* overflow: defines if an element reaches over the border of the box. with ```overflow: scroll;``` you can create a scroll option
* header, footer, article, section, aside are not necessary, but useful for people with disabilities or when you create a website for more than one medium (mobile, desktop)
