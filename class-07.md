# HTML Tables :
**HTML tables allow web authors to arrange data into rows and columns.**

## Defining an HTML Table :

An HTML table is defined with the `<table>` tag.

Each table row is defined with the `<tr>` tag. A table header is defined with the <th> tag. By default, table headings are bold and centered. A table data/cell is defined with the <td> tag.

Example :
  
  `<table style="width:100%">`
  
  `<tr>`
  
    `<th>Firstname</th>`
  
    `<th>Lastname</th>`
  
   ` <th>Age</th>`
  
 ` </tr>`
  
 ` <tr>`
  
    `<td>Jill</td>`
  
   ` <td>Smith</td>`
  
    `<td>50</td>`
  
  `</tr>`
  
  `<tr>`
  

   ` <td>Eve</td>`
  
    `<td>Jackson</td>`
  
   ` <td>94</td>`
  
 ` </tr>`
  
`</table>``
  
    ## HTML Table - Adding a Border :
  If you do not specify a border for the table, it will be displayed without borders.
A border is set using the CSS border property:

Example:
  
  `table, th, td {`
  
  `border: 1px solid black;`
}
  
  ## HTML Table - Collapsed Borders :
If you want the borders to collapse into one border, add the CSS border-collapse property:

Example:
  
 ` table, th, td {`
  
  `border: 1px solid black;`
  
  `border-collapse: collapse;`
}
  
  ## Functions, Methods, and Objects”
Creating a JavaScript Object
  
  ![](https://hsheikhm.files.wordpress.com/2016/02/screen-shot-2016-02-13-at-21-47-35.png?w=584)
  
  ## What is this?
The JavaScript this keyword refers to the object it belongs to.

It has different values depending on where it is used:

1.In a method, this refers to the owner object.
  
2. Alone, this refers to the global object.
  
3. In a function, this refers to the global object.
  
4, In a function, in strict mode, this is undefined.
  
5. In an event, this refers to the element that received the event.
  
6. Methods like call(), and apply() can refer this to any object.
  
  ## Arrays are objects
  Objects are an unordered map from string keys to values, arrays are an ordered list of values (with integer keys). That’s the main difference. They’re both non-primitive, as they’re composed of multiple values, which also implies pass-by-reference in JavaScript.

Arrays are also a kind of object, though, so you can attach extra properties to them, access their prototype and so on.

In your revised example, you’re only taking advantage of the fact that an array is actually an object, i.e. you can set any property on them. You shouldn’t do that. If you don’t need an ordered list of values, use a plain object.

  ## Browser object model
  
  The Browser Object Model (BOM) is used to interact with the browser.

The default object of browser is window means you can call all the functions of window by specifying window or directly.
  
  ![](https://static.javatpoint.com/images/javascript/bom.jpg)
  
  ## Global object
  
  In JavaScript, there’s always a global object defined. In a web browser, when scripts create global variables, they’re created as members of the global object.
  
  ## Strings Object
  
The String object lets you work with a series of characters; it wraps Javascript’s string primitive data type with a number of helper methods.

As JavaScript automatically converts between string primitives and String objects, you can call any of the helper methods of the String object on a string primitive.
  
  
  ## Date Object
  
  The Date object is used to work with dates and times.

Date objects are created with new Date().

There are four ways of instantiating a date
  
  
  
  
  
  
  
  
  
  
  
  
