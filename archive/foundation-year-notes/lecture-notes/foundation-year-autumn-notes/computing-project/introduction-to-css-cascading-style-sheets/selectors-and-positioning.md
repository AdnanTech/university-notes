# Selectors and Positioning

## CSS Selectors and Positioning

A tag can have multiple classes, having properties from any that are called (seperated via spaces)

### Selectors

* Type/Tag
  * p
  * h1
* Class
  * .center
  * .title
  * .red
* ID
  * \#main
  * \#wrapper
  * \#specialText
* All Elements
  * \*

### Group Selectors

* Selecting **multiple **selectors, (elements (tags)) to apply a style to
  * h1, p (changes all h1 and p elements)
* Selecting **nested **elements
  * h1 p (changes all p tags that are inside h1)
* Class **within **an element
  * ul.niceList

### Relational Selectors

* Selecting all **child **elements
  * h1 > p (selects all p where parent is h1)
* Selecting all elements **after **the next
  * h1 + p (selects all p tags that are placed after a h1 tag)
* Selecting all elements **before **the next
  * h1 \~ p (selects all p tags that are placed before a h1 tag)

You can combine these together to be very specific about the lement you want to change

### Attribute Selectors

* All elements with href attributes
  * \*\[href]
* all a tags with href attribute
  * a \[href]
* All input elements with type attribute where value is "submit"
  * input \[type="submit"]

### Pesudo class selectors

These have default values, but you can change the,

* a:link - hasn't been visited
* a:visited - has been visited
* a:hover - changes when hovered
* a:active - mouse button down is clicked on element
* a:focus - form control (for tab to move to next tab)







