# HTML  Basics and Tables

**HTML basics**

Hyper Text Markup Language \(HTML\) is a markup language that defines the structure of your content

* HTML consists of a series of elements, which you use to enclose or wrap different parts of the content to make it appear or act a certain way
  * The opening tag defines the way an element is displayed \(image, url, italics\)
* General form of a HTML element `<opening tag> Content </closing tag>`
* A **html tag i**s a set of characters that sets the way content is displayed on a web page
* An **element** comprises of the opening tag, closing tag, and the content within the tags
* **Attributes** contain extra information about the element that you don't want to appear in the actual content. 
  * Here, `class` is the attribute _name_ and `editor-note` is the attribute _value_. The `class` attribute allows you to give the element a non-unique identifier that can be used to target it \(and any other elements with the same `class` value\) with style information and other things.
  * A_**n id is x y z, its different to a class because it can only be applied to one element**_
    * An attribute should always have the following:
      * A space between it and the element name \(or the previous attribute, if the element already has one or more attributes\).
      * The attribute name followed by an equal sign
      * The attribute value wrapped by opening and closing quotation marks.
        * example: `<p class="example-class">Lorem Ipsum</p>`
        *          `<p id="example-class">Lorem Ipsum</p>`
* Why do we separate HTML and CSS?
* You can crate [web forms using the input tags nested within a block](https://developer.mozilla.org/en-US/docs/Learn/Forms/HTML5_input_types)
* The **HTML Content Division element** \(**`<div>`**\) is the generic container for flow content. it has no styling until applied with CSS. It basically just defines a container for HTML content
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
* CSS values are values we can apply to css properties, which include
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

**HTML Tables**



**Hyper text transfer protocol \(http://\)**

