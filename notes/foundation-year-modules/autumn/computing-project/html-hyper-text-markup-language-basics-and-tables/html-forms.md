# HTML Forms

## Basics

An HTML form is used to collect user input. The user input is most often sent to a server for processing. A good website to reference is [W3Schools](https://www.w3schools.com/html/html_forms.asp)

### The &lt;form&gt; Element

The HTML `<form>` element is used to create an HTML form for user input.  The `<form>` element is a container for different types of input elements, such as: text fields, checkboxes, radio buttons, submit buttons, etc.

### The &lt;input&gt; Element

The HTML `<input>` element is the most used form element.

An `<input>` element can be displayed in many ways, depending on the `type` attribute.

### Text Fields

The `<input type="text">` defines a single-line input field for text input.

## Attributes

### The Action Attribute

The `action` attribute defines the action to be performed when the form is submitted.

Usually, the form data is sent to a file on the server when the user clicks on the submit button.

### The Method Attribute

The `method` attribute specifies the HTTP method to be used when submitting the form data.

The form-data can be sent as URL variables \(with `method="get"`\) or as HTTP post transaction \(with `method="post"`\).

The default HTTP method when submitting form data is GET.

### **Notes on GET:**

* Appends the form data to the URL, in name/value pairs
* NEVER use GET to send sensitive data! \(the submitted form data is visible in the URL!\)
* The length of a URL is limited \(2048 characters\)
* Useful for form submissions where a user wants to bookmark the result
* GET is good for non-secure data, like query strings in Google

### **Notes on POST:**

* Appends the form data inside the body of the HTTP request \(the submitted form data is not shown in the URL\)
* POST has no size limitations, and can be used to send large amounts of data.
* Form submissions with POST cannot be bookmarked

## Elements



### The HTML &lt;form&gt; Elements

The HTML `<form>` element can contain one or more of the following form elements:

*  `<input>`
*  `<label>`
*  `<select>`
*  `<textarea>`
*  `<button>`
*  `<fieldset>`
*  `<legend>`
*  `<datalist>`
*  `<output>`
*  `<option>`
*  `<optgroup>`

## Types



### HTML Input Types

Here are the different input types you can use in HTML:

* `<input type="button">`
* `<input type="checkbox">`
* `<input type="color">`
* `<input type="date">`
* `<input type="datetime-local">`
* `<input type="email">`
* `<input type="file">`
* `<input type="hidden">`
* `<input type="image">`
* `<input type="month">`
* `<input type="number">`
* `<input type="password">`
* `<input type="radio">`
* `<input type="range">`
* `<input type="reset">`
* `<input type="search">`
* `<input type="submit">`
* `<input type="tel">`
* `<input type="text">`
* `<input type="time">`
* `<input type="url">`
* `<input type="week">`

