# Class 02

## Text in HTML

HTML has many tags to display text content based on the way the user wants the content to be displayed. For example, there are 6 different tags for headings, from `<h1>` to `<h6>`, and `<p>` is used for paragraphs. Also, those tags are divided into two types:

* Structural markup: the elements that you can use to describe both headings and paragraphs.

* Semantic markup: which provides extra information; such as where emphasis is placed in a sentence, that something you have written is a quotation (and who said it), the
meaning of acronyms, and so on.

The table below shows some of the tags the used in HTML for text.

| Tag | Type | Usage |
| --- | --- | --- |
| `<h?></h?>` | Structural | 6 different levels of tags from h1 to h6 are used to display different headings such main heading, subheadings, etc. |
| `<p></p>` | Structural | p tag is used to wrap paragraphs. |
| `<b></b>` | Semantic | to make characters appears in bold. |
| `<i></i>` | Semantic |  to make characters appears in italic. |
| `<sup></sup>` | Semantic | is used to contain characters that should be superscript. |
| `<sub></sub>` | Semantic | is used to contain characters that should
be subscript. |
| `<br />` | Structural markup | to add a line break inside the middle of a paragraph. |
| `<hr />` | Structural markup | to add a horizontal rule between sections. |


## CSS

CSS is short for Cascading Style Sheet which is used to style to HTML content and beautify it. To apply CSS, we need to specify which element we want to style and call it, that's called selectos. after we choose our selctor, we add the css rules such as color, background color, .etc and those are called properties. Each property needs a value that represents the propery. For example, you can't use the value `10px` to specify the property `background-color`.

CSS can be added inside the HTML document as an inline style for each element, or it could also be added in the head tag inside a style tag. Another option is to write the CSS in an external file with extention CSS and link it inside the HTML document.

## JavaScript

JavaScript is a programing language that is used to make web pages interactive. A script in JS is made of set of statements that specifies what the browser should do based on the user action or other circumstances. Variables are used to store the user inputs temporarily. These values could be strings, numrical values, or even boolean values. To store more than one value that are relatd in a way, there is another type of variables is called Array is used for this purpose.

Comparison operators are used in conditional statements. They are used to determine wehter the condition is true or false and that decides which block of code to execute next. The table below shows a set of comparison operators and the difference between them and how to use each one of them.

|Operator Sign| Operator Name | What it does | Example |
|---|---|---|---|
| `==` | is equal to| compares two valuesto see if they are the same | `'hello == 'hello'` returns true |
| `!=`| is not equal to | compares two values to see if they're not the same | `'hello !== 'hello'` returns false |
| `===` | strict equal to | compares twp values to check that both data type and value are the same | `'3' === 3` returns false |
| `!==` | strict not equal otl | compares twp values to check that both data type and value are not the same | `'3' === 3` returns true |
| `>` | greater than | compares if the number on the left is greater than the number on the right | `4 > 3` returns true |
| `<` | less than | compares if the number on the left is less than the number on the right | `6 < 10` returns false |
| `>=` | greater than or equal to | compares if the number on the left is greater than or equal to the number on the right | `4 >= 4` returns true |
| `<=` | less than or equal to | compares if the number on the left is less than or equal the number on the right | `5 <= 3` returns false |

Logical operaors are used when the need is to compare the results of more than one comparison operator.

|Logical operator | Name | Use|
|---|---|---|
| `&&` | Logial AND | tests more than one condition |
| `!` | Logial NOT | inverts a single boolean value |
| `||` | Logical OR | tests at least one condition |

The operators are used in a statement that decides  whether execute a piece of code or not. This statement is called If statement. If statements has conditions inside them, and based on the result of this condition, it decides whether to ececute the code or not.

Example:

```javascript
if(name !== "Husam"){
    console.log("Only Huam can enter this website");
}
```

A special type of if statements is called switch statement. Switch statement allow you to compare a value against possible outcomes and also provide a default option if none match.

Loops are used when the need is to repeat the execution of block of code couple of times based on a condition. There are 3 types of loops: `For Loop`, `While Loop`, and `Do While Loop`.

For Loop is used when you need to repeat of a piece of code a specific number of times.

Example:

```javascript
for (var i = 0; i <10; i++){
    document.write(i);
}
```

While Loop is used when you don't know the how many times the code should run.

Example:

```javascript
while(i<10){
  document.write(i);
  i++;
}
```

Do While Loop is very similar to the While Loop but has only one difference which is that the code will run at least once.

Example:

```javascript
do{
  document.write(i);
  i++;
}
while(i<10);
```

[Back to Home](README.md)