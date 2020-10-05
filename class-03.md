# Class 03

## Lists in HTML

Lists in HTML have 32 types: ordered lists, unordered lists, and definition lists. Ordered lists are used when the order is important, so it numbers the items inside the list. Unordered lists are used when the order isn't important but the items should be listed, so it adds bullets or dashes to the items inside the list. Finally, definition lists are made up of a set of terms along with the
definitions for each of those terms.

The `<ol></ol` tag is used to define an ordered list, the `<ul></ul>` is used to define an unordered list, and the tag `<dl></dl>` to define a definition list.

Lists can be listed inside one another. For example, you can start with an unordered list, and inside it add another ordered list.

Examples:

Ordered List:

``` html
<h6>How to open a word document:</h6>
<ol>
<li>Click on start.<li>
<li>In the search bar, type "Microsoft Word"</li>
<li>you will find it in the search results</li>
</ol>


```

Unordered List:

``` html
<h6>Shopping list:</h6>
<ol>
<li>Potate<li>
<li>Tomato</li>
<li>Yogurt</li>
</ol>

```

Definition List:

``` html
<dl>
<dt>Sashimi</dt>
<dd>Sliced raw fish that is served with
condiments such as shredded daikon radish or
ginger root, wasabi and soy sauce</dd>
<dt>Scale</dt>
<dd>A device used to accurately measure the
weight of ingredients</dd>
<dd>A technique by which the scales are removed
from the skin of a fish</dd>
<dt>Scamorze</dt>
<dt>Scamorzo</dt>
<dd>An Italian cheese usually made from whole
cow's milk (although it was traditionally made
from buffalo milk)</dd>
</dl>

```

## Boxes

In CSS, elements are treaded as they're inside boxes. These boxes could have borders, background color, margin from one another, padding inside the box. Also these boxes could be hidden or visible. Block-level boxes could be changed to inline-block, and viseversa.

The table below has some CSS properties and what they do:

| Propery | Job |
|----|----|
| `margin` | Adds margin to the element from the outside. |
| `padding` | Adds padding to the element from the inside. |
| `visibility` | Controls the visibility of the element |
| `display` | Contorls the way of how the element is displayed and also its visibility |
| `width:` | controls the width of the element |

## IF Statement

If statement evaluates the a condition, and if the condition is true; the code between subsequent code block gets executed, and if not; it doesn't.

If..else statement is very similar to the if statement. The only difference is that if the condition evaluates is false, it executes another block of code instead of not executing at all.

Switch statement is another way of writing if...else statement. A switch statement starts with a variable called the switch value. Each case indicates a possible value for this variable and the code that should run if the variable matches that value.

Examples:

If statement:

```javascript
if(condition){
    block of code;
}
```

If...else statement:

```javascript
if(condition){
    block of code;
} else{
    another block of code;
}
```

Switch statement:

```javascript
switch(value){
    case '1':
        block of code;
        break;
    case '2':
        block of code;
        break;
    case '3':
        block of code;
        break;
    default:
        anothe code
        break;
}
```

## Loops

Loops are used to repeat the same instructions couple of times based on a condtion. It evaluates the condition and if its true, it executes the code, and if it not it stops executing that block of code.

For loops are used when the number of iterations is known. While loop is used when the number of iteration is not known, and do while loop which is similar to while loop but it does at least 1 iteration before it checks the condition.

```javascript
for(var i=0; condition; i++){
    block of code;
}
```

```javascript
while(condition){
    block of code;
}
```

```javascript
do{
    block of code;
}while(condition);
```
