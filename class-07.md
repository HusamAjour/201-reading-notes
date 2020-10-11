# Class 07

## Tables

Tables in HTML are a way to displyay the data as a grid. There are many reasons to use it such as a report, user informatio, etc.
In HTML, data in tables are filled row by row. The main tag for tables is `<table></table>` and inside of it comes the other tags such as `<tr></tr>` for a table row, and `<td></td>` for table data. Another tag is used which is `<th></th>` which is used to add a table header. Another thing about tables in HTML is that you can make cells of a table span more than one row or column using the `rowspan` and `colspan` attributes. If the table we're bulidng is too long, it is preferable to use `<thead></thead>`, `<tbody></tbody>`, and `<tfoot></tfoot>` to split the table into sections.

Example:
The code below represents how to write a table in HTML:

```html
<table>
<thead>
<tr>
<th>Date</th>
<th>Income</th>
<th>Expenditure</th>
</tr>
</thead>
<tbody>
<tr>
<th>1st January</th>
<td>250</td>
<td>36</td>
</tr>
<tr>
<th>2nd January</th>
<td>285</td>
<td>48</td>
</tr>
<!-- additional rows as above -->
<tr>
<th>31st January</th>
<td>129</td>
<td>64</td>
</tr>
</tbody>
<tfoot>
<tr>
<td></td>
<td>7824</td>
<td>1241</td>
</tr>
</tfoot>
</table>

```

## Object Constructor

Object constructor is used when the need is to create several objects represent similar things, it uses a function as a template for creating objects with properties and methods that already added in the template.

Example:
The example below shows how to create objects using constructor notation and how to call these objects.

```javascript

function Hotel (name, rooms, booked) {
    this .name = name;
    this.rooms = rooms;
    this.booked = booked;
    this.checkAvailability = function(){
        return this.rooms - this.booked;
    };
}

var quayHotel = new Hotel('Quay', 40, 25);
var parkHotel = new Hotel( ' Park', 120, 77);

```

Browsers come with a set of built-in objects that represent things like the browser window and the current web page shown in that window. These built-in objects act like a toolkit for creating interactive web pages.

### BROWSER OBJECT MODEL

The Browser Object Model contains objects that represent the current browser window or tab. It contains objects that model things like browser history and the device's screen.

A set of global JavaScript objects:

* window.innerHeight
* window.innerWidth
* window.pageXOffset
* window. pageYOffset
* window.document
* window.history
* window.location
* window.a1ert()
* window.open()
* window.print()

### DOCUMENT OBJECT MODEL

The Document Object Model uses objects to create a representation of the current page. It creates a new object for each element (and each individual section of text) within the page.

### GLOBAL JAVASCRIPT OBJECTS

The global JavaScript objects represent things that the JavaScript language needs to create a model of. For example, there is an object that deals only with dates and times.

A set of global JavaScript objects:

* String
* Number
* Boolean
* Date
* Math
* Regex

[Back to Home](README.md)
