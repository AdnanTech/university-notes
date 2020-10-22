# Introduction to CSS

## CSS **Pre Reading Notes**

_Cascading Style Sheets \(CSS\) is a stylesheet language used to define the presentation of a document written in HTML \(less commonly, XML as well\)_

*  A **CSS selector** is the part of a CSS rule that describes what elements in a document the rule will match. The matching elements will have the rule's specified style applied to them, examples would be:
  * Type selectors `elementname`
  * Class selectors `.classname`
  * ID selectors `#idname`
  * Universal selectors `* ns|* *|*`
  * Attribute selectors `[attr=value]`
  * State selectors `a:active, a:visited`
* CSS properties are properties you can apply to an element, examples include
  * font-size
  * background-color
  * display
  * padding
  * margin
  * z-index
  * width
* **CSS values** are values we can apply to css properties, which include
  * Integers
  * real numbers
  * Lengths
  * Percentages
  * URLs \(unfirom resource locators\) and URIs \(uniform resource identifiers\)
  * Counters
  * Colors
* A **query string** is a part of a uniform resource locator \(URL\) that assigns values to specified parameters \(links a href to a link if applied\)
* **Pixel** is a static measurement, 
* while percent and **EM** are relative measurements. The size of an **EM or** percent depends on its parent

| px | em | percent |
| :--- | :--- | :--- |
| 23px |  1.4375**em** | 143.75% |
| 24px | 1.5000em | 150.00% |
| 25px | 1.5625em | 156.25% |

* A core concept in CSS is inheritance, where some CSS properties by default inherit values set on the current element's parent element, depending on how you choose so
* The two CSS attributes you can use to move an element around the page is position
  * this can be absolute 
  * or relative
* CSS can be included in two main ways
  * as an external stylesheet
  * or inline css in the HTML file
* What is the “default stylesheet” or “user agent stylesheet”?
  * Type 1, user agent: 
    * The browser has a basic style sheet that gives a default style to any document, these take precedence over anything when viewing a page. These style sheets are named **user-agent stylesheets**. Some browsers use actual style sheets for this purpose, while others simulate them in code, but the end result is the same.
      * Some browsers let users modify the user-agent stylesheet. Although some constraints on user-agent stylesheets are set by the HTML specification, browsers still have a lot of latitude: that means that significant differences exist from one browser to another. To simplify the development process, Web developers often use a CSS reset style sheet, forcing common properties values to a known state before beginning to make alterations to suit their specific needs.
  * Type 2, default author stylesheets \(style.css\): 
    *  **Author stylesheets** are the most common type of style sheet. These are style sheets that define styles as part of the design of a given web page or site. The author of the page defines the styles for the document using one or more stylesheets, which define the look and feel of the website — its theme.
  * Type 3, default user stylesheets:
    *  The user \(or reader\) of the web site can choose to override styles in many browsers using a custom **user stylesheet** designed to tailor the experience to the user's wishes.
* Why use a CSS reset file?
  * A CSS reset file allows you to clear an elements attributes so that you can stylize them with a clear formatting, this can help reduce ambiguity when stylizing a website
* !important will override any properties, giving the element that specific !important element instead

## Lecture Notes

### CSS has the following uses:

* Keep web page content separate from its formatting \(makes editing easier\)
* Save time by allowing multiple web pages to share the same formatting
* Ensure web pages are consistently formatted, e.g. corporate colours
* Make it easy to set appropriate formats for different output devices
* Make file downloads quicker as formatting instructions are not duplicated

### CSS Implementation and priority

* Browser has the LEAST priority \(how the browser interprets CSS\)
* Then its external style sheets \(style.css file\)
* Embedded or Internal Styles \(in the &lt;head&gt; tag\)
* Inline Styles has the MOST priority

### CSS general form

{% tabs %}
{% tab title="External" %}
```css
<link rel="stylesheet" type="text/css" href=“test.css" />

a {
	text-decoration: none !important;
	color: #65bfdd;
}
```
{% endtab %}

{% tab title="Embedded/Internal" %}
```css
<style type="text/css">
p {
text-align: center;
color: red;
font-family: arial
}
</style>
```
{% endtab %}

{% tab title="Inline" %}
```php
<p style=”text-align: center; color: red; font-family: arial;”>
    HTML basics session
</p>
```
{% endtab %}
{% endtabs %}

* Where color: \#65bfdd; is the declaration
  * where a is the selector
  * color is the property
  * hashtag65bfdd is the value

### General Notes

* The end semi colon is not actually neccessary, only the semi colons to separate the declarations are required
* /\* Short Note \*/ for making notes

### Pseduo Classes

A pseudo-class is used to define a special state of an element.

For example, it can be used to:

* Style an element when a user mouses over it
* Style visited and unvisited links differently
* Style an element when it gets focus

For example, a link may change colour when hovered over or you are on the active link.

```text
a:link {color: #FF0000}
a:visited {color: #00FF00}
a:hover {color: #FF00FF}
a:active {color: #0000FF}
```

### ID Selector

* Used to apply specific instructions to one or more HTML elements \(should be unique to one element\)
* Defined using a \#id
* It uses HTML id attribute as a point of call

### Class Selector

* Used to apply specific instructions to one or more HTML elements
* Defined using a .className
* It uses HTML class attribute as a point of call

## Lecture 2 Notes

### Box model

![](../../../../.gitbook/assets/image%20%2810%29.png)

### Positioning

* Fixed
* Absolute
* Relative

### Properties \(positioning elements\)

* Position property –determines how an element is positioned. Its values are absolute, fixed and relative
* Top property –value that determines the top position of an element’s box
* Bottom property -value that determines the bottom position of an element’s box
* Left property -value that determines the left position of an element’s box
* Right property -value that determines the right position of an element’s box
* Z-index property –a number that is used to determine a stack level of an element

## Notes

### size and space, box model and borders

* Height
* Width
* Float
* Padding
* Margin

### TRBL

Top, Right, Bottom, Left is order of precedence for spacing

