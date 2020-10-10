# Class 06

## Objects

Objects has a set of properties and methods to create a model of something you wld recognize from the real world. A property in an object is basically a variable that tells something about the object such as its name, and a method is represents a task that is associated with an object or more.

An example on an object:

```javascript

var hotel = {
    name: 'Quay'. //name property and its value
    rooms: 40, //rooms property and its value
    booked: 25, //booked property and its value
    gym: true, //gym property and its value
    roomTypes:['twins','double', 'suite'], //roomTypes property and its array of values
    checkAvailabilty: function(){
        return this.rooms - this.booked;
    } //checkAvailabilty method that checks if the hotel is fully booked or not
    };

```

Properties and methods of an object can be accessed using dot notation, or square brackets to access properties.

Example:

```javascript

var hotelName = hotel.name;  // accessing hotel's propery name
var hotelName = hotel[name]; // anotehr way of accessing hotel's property name
var roomsFree = hotel.checkAvailabilty(); // accessing hotel's method checkAvailabilty()

```

## DOM

DOM is short for Document Object Model, it specifies how browesers should create a model of an HTML page and how JS can access and update the content of web page while its in the browser window. DOM tree is the model of a web page when the browser loads it.

Example:
The image below shows a DOM tree.

![DOM Model](images/DOM-model.svg)

As shown in the image above, a DOM tree consits of a set of nodes. There are 4 types of nodes:

1. Document Node: is the first node in the DOM tree and its the root of the DOM tree.
2. Element Node: element nodes are basically the HTML elements.
3. Attribute Node: attribute nodes are basically a part of a element node.
4. Text Node: its where the element node text is stored.

Accessing and updating the DOM tree involves two steps:

1. Locate the node that represents the element you want to work with.
2. Use its text content, child elements, and attributes.

You can select an individual ekement node, multiple elements, or traversing between element nodes.

To select an individual element you can use the following methods:

* getElementById(): As ids are unique, you can select an element using this method by adding its id value to the method.
* querySelector(): By using CSS selector, and returns the first matching element.

To select multiole elements you can use the following methods:

* getElementsByClassName(): Unlike id, class could be given to many elements, and this method can be helpful when the need is to select multiple elements that have the same class.
* getElementsByTagName(): this method select all the element with the specified tag name.
* querySelectorAll(): Use CSS selectors to select all matching elements.

To traverse between nodes, you can use the following methods:

* parentNode: Selects the parent oof the current element.
* previousSibling / nextSibling: To select the previous or the next sibling of the current element.
* firstChild / lastChild: the select the first or the last child of the current element.

There are many reasons to access an node. For example, you may want to access an element to get it text value, and that could be done using `nodeValue` property, or you may want to access a node to create children element or remove them, or you maybe want to add or remove an attribute to that element.

Web browsers offer tools for viewing the DOM tree.

[Back to Home](README.md)
