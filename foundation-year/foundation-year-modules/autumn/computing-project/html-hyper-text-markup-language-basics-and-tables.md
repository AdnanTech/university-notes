# HTML  Basics and Tables

**HTML basics**

Hyper Text Markup Language \(HTML\) is a markup language that defines the structure of your content

* HTML consists of a series of elements, which you use to enclose or wrap different parts of the content to make it appear or act a certain way
  * The opening tag defines the way an element is displayed, some examples
    * image
    * url
    * italics
* General form of a HTML element `<opening tag> Content </closing tag>`
* A **html tag i**s a set of characters that sets the way content is displayed on a web page
* An **element** comprises of the opening tag, closing tag, and the content within the tags
* **Attributes** contain extra information about the element that you don't want to appear in the actual content, they tend to be classes or ids.
  *  The **`class`** **global attribute** is a space-separated list of the case-sensitive classes of the element. Classes allow CSS and Javascript to select and **access specific elements via the class selectors** \(multiple\) or functions like the DOM method `document.getElementsByClassName`.
    * `class` is the attribute _name_ and `example-class` is the attribute _value_. The `class` attribute allows you to give the element a **non-unique identifier** that can be used to target it \(and any other elements with the same `class` value\) with style information and other things.
      * `<p class="example-class">Lorem Ipsum</p>`
      *          `<p id="example-class">Lorem Ipsum</p>`
  *  The **`id` global attribute** defines an identifier \(ID\) which must be **unique in the whole document**. Its purpose is to identify the element when linking and styling \(with CSS\)
    * id is the attribute name 
    * An attribute should always have the following:
      * A space between it and the element name \(or the previous attribute, if the element already has one or more attributes\).
      * The attribute name followed by an equal sign
      * The attribute value wrapped by opening and closing quotation marks
* You can crate [web forms using the input tags nested within a block](https://developer.mozilla.org/en-US/docs/Learn/Forms/HTML5_input_types)
* The **HTML Content Division element** \(**`<div>`**\) is the generic container for flow content. it has no styling until applied with CSS. It basically just defines a container for HTML content

**HTML Tables**

The **HTML `<table>` element** represents tabular data — that is, information presented in a two-dimensional table comprised of rows and columns of cells containing data

Examples are in the code base

**Hyper text transfer protocol \(http://\)**

