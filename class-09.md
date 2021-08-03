# HTML Forms :
An HTML form is used to collect user input. The user input can then be sent to a server for processing.
![](https://i2.wp.com/www.tutorialbrain.com/wp-content/uploads/2019/01/HTML-Form.jpg?fit=1920%2C1080&ssl=1)
## The `<form>` Element

The HTML `<form>` element defines a form that is used to collect user input.

## How does an HTML form work?
A web form has two parts: the HTML ‘front end’ and a back end form processor. The HTML front end part handles the presentation while the back end handles the form submissions (like saving the form submissions, sending emails etc). The back end form processor script is usually written in languages like PHP, ASP or Perl.

The image below illustrates the concept:

![](https://simfatic.com/forms/help/v40/form-working.jpg)

1. A visitor visits a web page that contains a form.
2. The web browser displays the HTML form.
3. The visitor fills in the form and submits
4. The browser sends the submitted form data to the web server
5. A form processor script running on the web server processes the form data
6. A response page is sent back to the browser.

## The `<input>` Element :
The `<input>` element is the most important form element.The `<input>` element is displayed in several ways, depending on the type attribute.

Text Fields “
`<input type="text">` defines a single-line input field for text input.

The `<label>` Element :
Notice the use of the `<label>` element in the example above.

The `<label>` tag defines a label for many form elements.

The `<label>` element is useful for screen-reader users, because the screen-reader will read out loud the label when the user is focused on the input element.

The `<label>` element also help users who have difficulty clicking on very small regions (such as radio buttons or checkboxes) - because when the user clicks the text within the <label> element, it toggles the radio button/checkbox.

The for attribute of the `<label>` tag should be equal to the id attribute of the `<input>` element to bind them together.

The Submit Button :
`<input type="submit">` defines a button for submitting the form data to a form-handler.

The form-handler is typically a page on the server with a script for processing input data.

The form-handler is specified in the form’s action attribute.

## The Action Attribute :
The `action` attribute defines the action to be performed when the form is submitted. Usually, the form data is sent to a page on the server when the user clicks on the submit button. In the example above, the form data is sent to a page on the server called “/action_page.php”. This page contains a server-side script that handles the form data:

`<form action="/action_page.php">`

## The Target Attribute :
The `target` attribute specifies if the submitted result will open in a new browser tab, a frame, or in the current window The default value is `_self` which means the form will be submitted in the current window. To make the form result open in a new browser tab, use the value `_blank`.
  
  ## JavaScript Events
  HTML events are “things” that happen to HTML elements. When JavaScript is used in HTML pages, JavaScript can “react” on these events.
  
  
  
