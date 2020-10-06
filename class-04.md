# Class 04

## Links in HTML

Links are the used to navigate between web pages and external resources. With links, you can move one website to another, web pages in the same site, and also, you can also move from one part in the web page to another part in the same page.

To add a link to your website, you can use the tag `<a></a>`. Insie the opening tag of `<a>`, you can add the attribute `href` and inside of it you can add the URL of the website you want to visit, or the path of the web page you want to open, or if you're targeting an element in the same web page you can add the `id` of that element inside the `href` of the link. 

```html
<a href="https://www.imdb.com">IMDB</a>
```

```html
<a href="index.html">Home</a>
```

## Layout

Browsers display pages in normal flow unless you specify relative, absolute, or fixed position. Normal flow means that every block-level element appears on a mew line. Relative positioning moves an element from the position it would be in nomal flow, shifting it to the top, right, bottom, left of where it would have been placed. Absolute poisioning positions the elmement in relation to its containing element and it takes it out of normal flow.
Also, fixed positioning is a form of absolute positioning that positions the element in relation to the browser window. Floating elements in the othe hand allows you to take that element out of normal flow and position it to the far left or right of a containing box.

The table below shows some of CSS positioning properties and values and what they do.

| Property | What it does |
|----|----|
| `position: static;` | Default positiont value |
| `position: relative;` | Relative positioning moves an element in relation to where it would have been in normal flow. |
| `position:absolute;` | box is taken out of normal flow and no longer affects the position of other elements on the page |
| `position:fixed;` | is a type of absolute positioning that requires the position property to have a value of fixed |
| `z-index: value;` | control which element sits on top when elements are covering one another |
| `float: value;` | allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible |

Layout has two type: Fixed Width Layouts and Liquid Layouts. Fixed width layout designs do not change size as the user increases or decreases the size of their browser window Measurements tend to be given in pixels. While liquid layout designs stretch and contract as the user increases or decreases the size of their browser window. They tend to use percentages.
Many designers use a grid structure to help them position items on a page, and the same is true for web designers. Grids set consistent proportions and spaces between items which helps to create a professional looking design. CSS frameworks aim to make your life easier by providing the code for common tasks, such as creating layout grids, styling forms, creating printer-friendly versions of pages and so on. You can include the CSS framework code in your projects rather than writing the CSS from scratch as you can include multiple CSS files in one page. If the same taks needs to be done agian, its better to write it into a function and call the function whenever this task is needed.

## Functions, Methods & Objcets

Functions, methods, and objects are used by programmers to organize their code. A function consists of a set of statements that have been grouped together becase they perform a spicific task. Objects are made up of properties and methods that the user can create, and there is another type of objects called built-in objects that come with the browser.

Example:

```javascript
function sayHi(name){
    console.log('Hi ' + name);
}

sayHi('Husam');
```

Functions could be written to just print a message, or it could do a math operation for example and return the result to the user. Variables that were declared inside a function cannot be used outside of that function, but variables that were declared outside of a function could be called inside any function.

[Back to Home](README.md)
