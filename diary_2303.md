# Diary 23.03.2020

# Responsive Layout CSS

* ```overflow: hidden;``` usually ensures that, overflowing text in a box with fixed dimensions gets cut off. 
* with ```overflow: hidden;``` you also create a new Block Formatting Context, which means that all elements must be completely enclose by the outer element, even floated elements. 
* another way to clear floats is with the so-called Clearfix Hack
  * first you create a pseudo-element with ```::after``` so it creates an empty space after the element you want to clear.
  * this pseudo-element gets assigned ```clear: both;``` 
  * for example:
  ```css
  .clearfix::after {
      content: "";
      display: block; 
      clear: both;
  }
  ```
  * you can also use ```display: table;```, but it must be a block element, since you can't clear inline elements
* There is another way to create a Block Formatting Context. the rule  ```display: flow-root;```, technically does the same thing as overflow:hidden, but it was invented to do just that. it is a rather new rule though, and not a lot of browsers support it yet.
* let's sum that up:
  * floated elements always create a block-box.
  * floated elements are quasi in the flow, but not entirely.
  * floated elements are not enclosed by the surrounding element 
  * you can enclose floating elements with either ```overflow: hidden;```, with the Clearfix Hack, or with ```display: flow-root;``` 
* CSS-shapes are used together with float. ```shape-outside; circle(50%);``` arranges text in a circle. only works with floated elements.