## Read 02:

### Javascript Templating:
 **Javascript templating** is a helpfull technique to obtain the client-side view templates with Javascript by using a JSON data source. The template is HTML markup, by adding templating tags that will either insert variables or run programming logic.

 ### What is "Mustache":
 **Mustache** is a logic-less template syntax. It can be used for HTML.
 
 **How it is work?**
 It works by expanding tags in a template using values provided in a hash or object.

>>
**mustache.js** is an implementation of the mustache template system in JavaScript.
>>

### Mustache-Express:
 we can use **mustache-express.If** we intend you use **mustache** with Node and Express, Mustache Express lets you use Mustache and Express together easily.

 we can install it by:
 - With Yarn:`` $ yarn add mustache-express``

 - with NPM: $``npm install mustache --save``

 -------------------------------------------------------
 ## Flexbox:
  The **Flexbox**  module  used to providing a more efficient way to lay out, align and distribute space among items in a container, even when their size is unknown and dynamic. in other words to give the container the ability to alter its items’ width/height and order to best fill the available space.

  ### How using Flexbox:
  the first thing is in ``display`` property:

```  
.container {
  display: flex; /* or inline-flex */
} 
```

  This defines a flex container; inline or block depending on the given value. It enables a flex context for all its direct children.

  ### flex-direction:
  This establishes the main-axis, thus defining the direction flex items are placed in the flex container.

  **ex:**

  ```
  .container {
  flex-direction: row | row-reverse | column | column-reverse;
}
```
``row ``(default): left to right in ltr; right to left in rtl
``row-reverse``: right to left in ltr; left to right in rtl
``column``: same as row but top to bottom
``column-reverse``: same as row-reverse but bottom to top

### flex-basis:
This defines the default size of an element before the remaining space is distributed.

**EX:**

```
.item {
  flex-basis: <length> | auto; /* default auto */
}

```

### justify-content:
**justify-content** defines the alignment along the main axis. It helps distribute extra free space leftover when either all the flex items on a line are inflexible, or are flexible but have reached their maximum size.

- ``flex-start (default)``: items are packed toward the start of the flex-direction.
- ``flex-end``: items are packed toward the end of the flex-direction.
- ``start``: items are packed toward the start of the writing-mode direction.
- ``space-between``: items are evenly distributed in the line; first item is on the start line, last item on the end line
- ``space-around``: items are evenly distributed in the line with equal space around them
and moch more.

### align-items:
**align-items**: defines the default behavior for how flex items are laid out along the cross axis on the current line.

### align-content: 
**align-content** aligns a flex container’s lines within when there is extra space in the cross-axis, similar to how justify-content aligns individual items within the main-axis.